# Comparing `tmp/ecs_session-24.4.6.tar.gz` & `tmp/ecs_session-24.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_session-24.4.6.tar", max compression
+gzip compressed data, was "ecs_session-24.4.7.tar", max compression
```

## Comparing `ecs_session-24.4.6.tar` & `ecs_session-24.4.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1428 2024-04-23 08:14:37.442380 ecs_session-24.4.6/README.md
--rw-r--r--   0        0        0     3859 2024-04-23 12:01:42.084232 ecs_session-24.4.6/ecs_session/__init__.py
--rw-r--r--   0        0        0     6174 2024-04-23 12:10:20.120283 ecs_session-24.4.6/ecs_session/cli.py
--rw-r--r--   0        0        0      477 2024-04-23 12:10:51.978972 ecs_session-24.4.6/pyproject.toml
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 ecs_session-24.4.6/setup.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 ecs_session-24.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1428 2024-04-23 08:14:37.442380 ecs_session-24.4.7/README.md
+-rw-r--r--   0        0        0     3859 2024-04-23 12:01:42.084232 ecs_session-24.4.7/ecs_session/__init__.py
+-rw-r--r--   0        0        0     7038 2024-04-25 13:00:17.901007 ecs_session-24.4.7/ecs_session/cli.py
+-rw-r--r--   0        0        0      640 2024-04-25 13:00:05.940577 ecs_session-24.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 ecs_session-24.4.7/setup.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 ecs_session-24.4.7/PKG-INFO
```

### Comparing `ecs_session-24.4.6/README.md` & `ecs_session-24.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ecs_session-24.4.6/ecs_session/__init__.py` & `ecs_session-24.4.7/ecs_session/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_session-24.4.6/ecs_session/cli.py` & `ecs_session-24.4.7/ecs_session/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,19 +73,21 @@
 def show_menu(items: list, title: str, source: list = None):
     """
     menu function
     """
     index = None
     source = source or items
     menu = TerminalMenu(
-        items,
-        title=f"? {title}:\n",
+        items + ["Back"],
+        title=f'? {title} (Press "q"/"ESC" to quit):\n',
         show_search_hint=True,
     )
     index = menu.show()
+    if index == len(items):
+        return None, index
     if index is None:
         exit(0)
     return source[index], index
 
 
 def ecs_paginator(ecs: session.Session.client, paginator: str, leaf: str, **kwargs):
     """
@@ -117,96 +119,108 @@
     )
 
 
 def get_service(ecs: session.Session.client, service: str, cluster: str):
     """
     get service
     """
+    if not cluster:
+        return cluster, None, None
     if service:
-        return service, None
+        return cluster, service, None
     arns = ecs_paginator(
         ecs=ecs,
         paginator="list_services",
         leaf="serviceArns",
         cluster=cluster,
     )
     services = [service.split("/")[-1] for service in arns]
-    return show_menu(
+    ret = show_menu(
         items=services,
-        title="Select service",
+        title=f"[{cluster}] Select service",
     )
+    if ret[0] is None:
+        return (None, *ret)
+    return (cluster, *ret)
 
 
 def get_task(ecs: session.Session.client, task: str, cluster: str, service: str):
     """
     get services
     """
+    if not service:
+        return cluster, service, None, None
     if task:
-        return task, None
+        return cluster, service, task, None
     arns = ecs_paginator(
         ecs=ecs,
         paginator="list_tasks",
         leaf="taskArns",
         cluster=cluster,
         serviceName=service,
     )
     tasks = [task.split("/")[-1] for task in arns]
-    return show_menu(
+    ret = show_menu(
         items=tasks,
-        title="Select task",
+        title=f"[{cluster}|{service}] Select task",
     )
+    if ret[0] is None:
+        return (cluster, None, *ret)
+    return (cluster, service, *ret)
 
 
-def get_container(containers: list, container: str):
+def get_container(cluster: str, service: str, task: str, containers: list, container: str):
     """
     get container
     """
     if container:
         return container, containers.index(container)
-    return show_menu(
+    ret = show_menu(
         items=containers,
-        title="Select container",
+        title=f"[{cluster}|{service}|{task}] Select container",
     )
+    if ret[0] is None:
+        return (None, *ret)
+    return (task, *ret)
 
 
 def run():
     """main cli function"""
     parser = get_parser()
     arguments = parser.parse_args()
     boto3_session_args = {
         "region_name": arguments.region,
     }
     if arguments.profile != "default":
         boto3_session_args.update({"profile_name": arguments.profile})
     boto3_session = session.Session(**boto3_session_args)
     ecs = boto3_session.client("ecs")
     ssm = boto3_session.client("ssm")
-    cluster, _ = get_cluster(ecs=ecs, cluster=arguments.cluster)
-    service, _ = get_service(ecs=ecs, service=arguments.service, cluster=cluster)
-    task, _ = get_task(ecs=ecs, task=arguments.task, cluster=cluster, service=service)
-    task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
-    containers = [
-        container.get("name")
-        for container in task_details.get("tasks")[0].get("containers")
-    ]
-    container, container_index = get_container(
-        containers=containers,
-        container=arguments.container,
-    )
+    cluster, service, task, container = (arguments.cluster, arguments.service, arguments.task, arguments.container)
+    while not (cluster and service and task and container):
+        cluster, _ = get_cluster(ecs=ecs, cluster=cluster)
+        cluster, service, _ = get_service(ecs=ecs, cluster=cluster, service=service)
+        cluster, service, task, _ = get_task(ecs=ecs, cluster=cluster, service=service, task=task)
+        if cluster and task:
+            task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
+            containers = [container.get("name") for container in task_details.get("tasks")[0].get("containers")]
+            task, container, container_index = get_container(
+                cluster=cluster,
+                service=service,
+                task=task,
+                containers=containers,
+                container=container,
+            )
     remote_port = arguments.remote_port
     if arguments.action == "forward" and not remote_port:
         task_definition_arn = task_details.get("tasks")[0].get("taskDefinitionArn")
-        task_definition = ecs.describe_task_definition(
-            taskDefinition=task_definition_arn
-        ).get("taskDefinition")
+        task_definition = ecs.describe_task_definition(taskDefinition=task_definition_arn).get("taskDefinition")
         ports = [
             str(container.get("containerPort"))
-            for container in task_definition.get("containerDefinitions")[
-                container_index
-            ].get("portMappings")
+            for container in task_definition.get("containerDefinitions")[container_index].get("portMappings")
         ]
         remote_port, _ = show_menu(items=ports, title="Select port")
     ecs_session = ECSSession(
         cluster=cluster,
         command=arguments.command,
         container=container,
         container_index=container_index,
@@ -219,14 +233,14 @@
         task=task,
         task_details=task_details,
     )
     function = {
         "forward": ecs_session.port_forward,
         "command": ecs_session.execute_command,
     }
-    print(f"---")
+    print("---")
     print(f"cluster: {cluster}")
     print(f"service: {service}")
     print(f"task: {task}")
     print(f"container: {container}")
-    print(f"---")
+    print("---")
     function.get(arguments.action)()
```

### Comparing `ecs_session-24.4.6/setup.py` & `ecs_session-24.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['boto3', 'configargparse', 'shtab', 'simple_term_menu']
 
 entry_points = \
 {'console_scripts': ['ecs-session = ecs_session.cli:run']}
 
 setup_kwargs = {
     'name': 'ecs-session',
-    'version': '24.4.6',
+    'version': '24.4.7',
     'description': 'ECS SSM tool',
     'long_description': '# ecs-session\n\nInspired by [ecsgo](https://github.com/tedsmitt/ecsgo) (`ecspy` is in use already).\n\nProvides a tool to interact with AWS ECS tasks.\n\nCurrently provides:\n\n* interactive execute-command (e.g. shell)\n* port-forwarding\n\nYou can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.\n\n## Installation\n\n```\npip install ecs-session\n```\n\n## Pre-requisites\n\n### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)\n\n#### Linux\n\n```bash\ncurl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"\nmkdir -p ~/bin\ndpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin\n```\n\n#### MacOS\n\n`brew install --cask session-manager-plugin`\n\n### Infrastructure\n\nUse [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.\n\n\n## Usage\n\nSee `ecs-session --help` for all features.\n\n### Execute command\n\nSelect all from menu:\n\n```bash\necs-session command\n```\n\n### Port forwarding\n\nSelect all from menu:\n\n```bash\necs-session forward\n```\n\nSpecify port and select the rest from menu:\n\n```bash\necs-session --remote-port 8080 forward\n```\n',
     'author': 'Stefan Heitmüller',
     'author_email': 'stefan.heitmueller@gmx.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/morph027/ecs-session',
```

### Comparing `ecs_session-24.4.6/PKG-INFO` & `ecs_session-24.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-session
-Version: 24.4.6
+Version: 24.4.7
 Summary: ECS SSM tool
 Home-page: https://github.com/morph027/ecs-session
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```


# Comparing `tmp/py_infraflow_cdk-0.1.9.8.9.7.tar.gz` & `tmp/py_infraflow_cdk-0.1.9.8.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_infraflow_cdk-0.1.9.8.9.7.tar", max compression
+gzip compressed data, was "py_infraflow_cdk-0.1.9.8.9.8.tar", max compression
```

## Comparing `py_infraflow_cdk-0.1.9.8.9.7.tar` & `py_infraflow_cdk-0.1.9.8.9.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.8.9.7/README.md
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.8.9.7/infraflow/__init__.py
--rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/_step_functions/__init__.py
--rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/_step_functions/core.py
--rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/_step_functions/patterns.py
--rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/api_gateway.py
--rw-r--r--   0        0        0     7248 2024-04-11 23:31:09.971668 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/app_patterns/express_default_dlq_processor.py
--rw-r--r--   0        0        0    12703 2024-04-24 21:30:34.435023 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/app_patterns/standard.py
--rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/arns.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/__init__.py
--rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/component_service.py
--rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/construct.py
--rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/environment.py
--rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/service_stage.py
--rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/utils.py
--rw-r--r--   0        0        0    10283 2024-04-25 18:12:48.845869 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/docker.py
--rw-r--r--   0        0        0     8184 2024-02-19 16:53:56.961586 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/events.py
--rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/__init__.py
--rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/_actions.py
--rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/action_groups.py
--rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/actions
--rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/base.py
--rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/alarms.py
--rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/docker.py
--rw-r--r--   0        0        0     7304 2024-04-11 23:31:09.974549 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/lambdas.py
--rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/metrics.py
--rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/queues.py
--rw-r--r--   0        0        0     6208 2024-04-11 23:31:09.976357 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/lambdas.py
--rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/queue.py
--rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/__init__.py
--rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/patterns.py
--rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/ports.py
--rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/tier_maps.py
--rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.8.9.7/infraflow/priv_utils/__init__.py
--rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.8.9.7/infraflow/util.py
--rw-r--r--   0        0        0      687 2024-04-25 18:13:34.472896 py_infraflow_cdk-0.1.9.8.9.7/pyproject.toml
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.8.9.7/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-01-24 18:03:42.816211 py_infraflow_cdk-0.1.9.8.9.8/README.md
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856613 py_infraflow_cdk-0.1.9.8.9.8/infraflow/__init__.py
+-rw-r--r--   0        0        0      240 2024-01-22 17:24:55.856719 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.856794 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/_step_functions/__init__.py
+-rw-r--r--   0        0        0     1329 2024-01-22 17:24:55.856883 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/_step_functions/core.py
+-rw-r--r--   0        0        0     1261 2024-01-22 17:24:55.856942 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/_step_functions/patterns.py
+-rw-r--r--   0        0        0      280 2024-01-22 17:24:55.857004 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/api_gateway.py
+-rw-r--r--   0        0        0     7248 2024-04-11 23:31:09.971668 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/app_patterns/express_default_dlq_processor.py
+-rw-r--r--   0        0        0    12703 2024-04-24 21:30:34.435023 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/app_patterns/standard.py
+-rw-r--r--   0        0        0      156 2024-01-22 17:24:55.857163 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/arns.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.857224 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/__init__.py
+-rw-r--r--   0        0        0      364 2024-01-22 17:24:55.857292 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/component_service.py
+-rw-r--r--   0        0        0      316 2024-01-22 17:24:55.857349 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/construct.py
+-rw-r--r--   0        0        0     5168 2024-03-20 16:31:56.831033 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/environment.py
+-rw-r--r--   0        0        0     1020 2024-01-24 18:03:42.816662 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/service_stage.py
+-rw-r--r--   0        0        0      367 2024-02-19 16:57:57.498391 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/utils.py
+-rw-r--r--   0        0        0    10349 2024-04-25 18:37:44.510733 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/docker.py
+-rw-r--r--   0        0        0     8184 2024-02-19 16:53:56.961586 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/events.py
+-rw-r--r--   0        0        0      139 2024-01-22 17:24:55.857712 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/__init__.py
+-rw-r--r--   0        0        0   533095 2024-01-24 18:03:42.817968 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/_actions.py
+-rw-r--r--   0        0        0   249582 2024-01-22 17:24:55.859417 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/action_groups.py
+-rw-r--r--   0        0        0   108710 2024-01-22 17:24:55.859750 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/actions
+-rw-r--r--   0        0        0     4943 2024-01-22 17:24:55.859832 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/base.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:31:56.831151 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-11 23:31:09.973506 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/alarms.py
+-rw-r--r--   0        0        0     5976 2024-04-24 21:59:03.929389 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/docker.py
+-rw-r--r--   0        0        0     7304 2024-04-11 23:31:09.974549 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/lambdas.py
+-rw-r--r--   0        0        0     1704 2024-04-11 23:31:09.974803 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/metrics.py
+-rw-r--r--   0        0        0     4435 2024-04-11 23:31:09.975272 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/queues.py
+-rw-r--r--   0        0        0     6208 2024-04-11 23:31:09.976357 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/lambdas.py
+-rw-r--r--   0        0        0      349 2024-02-28 20:32:26.259456 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/queue.py
+-rw-r--r--   0        0        0        0 2024-01-22 17:24:55.859986 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/__init__.py
+-rw-r--r--   0        0        0     3481 2024-01-24 18:03:42.818220 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/patterns.py
+-rw-r--r--   0        0        0      715 2024-01-24 18:03:42.818283 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/ports.py
+-rw-r--r--   0        0        0      629 2024-01-22 17:24:55.860118 py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/tier_maps.py
+-rw-r--r--   0        0        0      141 2024-01-24 18:03:42.818392 py_infraflow_cdk-0.1.9.8.9.8/infraflow/priv_utils/__init__.py
+-rw-r--r--   0        0        0      154 2024-01-22 17:24:55.860264 py_infraflow_cdk-0.1.9.8.9.8/infraflow/util.py
+-rw-r--r--   0        0        0      687 2024-04-25 18:38:19.480062 py_infraflow_cdk-0.1.9.8.9.8/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 py_infraflow_cdk-0.1.9.8.9.8/PKG-INFO
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/_step_functions/core.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/_step_functions/core.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/_step_functions/patterns.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/_step_functions/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/app_patterns/express_default_dlq_processor.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/app_patterns/express_default_dlq_processor.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/app_patterns/standard.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/app_patterns/standard.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/environment.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/core/service_stage.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/core/service_stage.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/docker.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             security_groups=[self.get_security_group(name)],
             task_subnets=self.subnets(),
             assign_public_ip=False,
             public_load_balancer=False,
             memory_limit_mib=container.size.memory_limit_mib,  # Default is 512
         )  # Default is True
         # subnet workaround, since assigning above didnt work [https://github.com/aws/aws-cdk/issues/5892]
-        self.service_instrumentation[alb_fargate_service.service] = EcsServiceInstrumentation(alb_fargate_service.service)
+        self.service_instrumentation[alb_fargate_service.service] = EcsServiceInstrumentation(ecs_service=alb_fargate_service.service, log_group=log_group)
         cfn_lb = alb_fargate_service.load_balancer.node.default_child
         cfn_lb.subnets = [subnet.subnet_id for subnet in self.scope.env.service_subnets(self.subnet_type)]
         return alb_fargate_service
 
     def queued_service_with_queue(
             self,
             name,
@@ -202,15 +202,15 @@
             task_definition=task,
             propagate_tags=PropagatedTagSource.SERVICE,
             security_groups=[self.get_security_group(name)],
             task_subnets=self.subnets(),
             assign_public_ip=False,
         )  # Default is True
 
-        self.service_instrumentation[service.service] = EcsServiceInstrumentation(service.service)
+        self.service_instrumentation[service.service] = EcsServiceInstrumentation(ecs_service=service.service, log_group=log_group)
         return service
 
     def scheduled_service(
             self,
             name,
             container: ContainerInstanceInfo,
             schedule: Union[Duration, timedelta, int]
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/events.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/events.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/_actions.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/_actions.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/action_groups.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/action_groups.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/actions` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/actions`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/iam/base.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/iam/base.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/alarms.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/alarms.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/docker.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/docker.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/lambdas.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/lambdas.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/metrics.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/metrics.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/instrumentation/queues.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/instrumentation/queues.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/lambdas.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/lambdas.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/patterns.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/patterns.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/ports.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/ports.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/infraflow/cdk/sg/tier_maps.py` & `py_infraflow_cdk-0.1.9.8.9.8/infraflow/cdk/sg/tier_maps.py`

 * *Files identical despite different names*

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/pyproject.toml` & `py_infraflow_cdk-0.1.9.8.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-infraflow-cdk"
-version = "0.1.9.8.9.7"
+version = "0.1.9.8.9.8"
 description = "Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns"
 authors = ["Matthew Beatty <infraflow@upcontent.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "infraflow"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_infraflow_cdk-0.1.9.8.9.7/PKG-INFO` & `py_infraflow_cdk-0.1.9.8.9.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-infraflow-cdk
-Version: 0.1.9.8.9.7
+Version: 0.1.9.8.9.8
 Summary: Build Event Based and Microservice infrastructure and connections using these reusable AWS CDK patterns
 License: MIT
 Author: Matthew Beatty
 Author-email: infraflow@upcontent.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


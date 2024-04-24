# Comparing `tmp/pve_cli-0.5.0.tar.gz` & `tmp/pve_cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pve_cli-0.5.0.tar", last modified: Sun Apr 14 20:43:10 2024, max compression
+gzip compressed data, was "pve_cli-0.5.1.tar", last modified: Wed Apr 24 22:01:13 2024, max compression
```

## Comparing `pve_cli-0.5.0.tar` & `pve_cli-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    16725 2023-12-25 02:44:02.838927 pve_cli-0.5.0/LICENSE
--rw-r--r--   0        0        0      757 2024-04-14 20:34:42.634837 pve_cli-0.5.0/README.md
--rw-r--r--   0        0        0      198 2023-12-25 02:44:02.838927 pve_cli-0.5.0/pve_cli/__init__.py
--rw-r--r--   0        0        0     3727 2024-02-05 19:02:35.874529 pve_cli-0.5.0/pve_cli/guest_cmd.py
--rw-r--r--   0        0        0     1880 2024-01-21 23:14:01.404696 pve_cli-0.5.0/pve_cli/main.py
--rw-r--r--   0        0        0     6808 2024-04-14 20:34:42.638837 pve_cli-0.5.0/pve_cli/nodes_cmd.py
--rw-r--r--   0        0        0      233 2023-12-25 02:44:02.842927 pve_cli-0.5.0/pve_cli/proxmox/__init__.py
--rw-r--r--   0        0        0     3849 2024-02-22 15:55:23.490925 pve_cli-0.5.0/pve_cli/proxmox/api.py
--rw-r--r--   0        0        0      449 2023-12-25 02:44:02.842927 pve_cli-0.5.0/pve_cli/proxmox/exceptions.py
--rw-r--r--   0        0        0       96 2023-12-25 02:44:02.842927 pve_cli-0.5.0/pve_cli/proxmox/types.py
--rw-r--r--   0        0        0        0 2024-04-14 20:42:52.680254 pve_cli-0.5.0/pve_cli/util/__init__.py
--rw-r--r--   0        0        0      910 2024-01-21 23:14:01.408696 pve_cli-0.5.0/pve_cli/util/callbacks.py
--rw-r--r--   0        0        0      129 2023-12-25 02:44:02.846927 pve_cli-0.5.0/pve_cli/util/exceptions.py
--rw-r--r--   0        0        0     1574 2023-12-26 03:06:31.021608 pve_cli-0.5.0/pve_cli/util/validators.py
--rw-r--r--   0        0        0     2298 2024-04-14 20:43:10.176358 pve_cli-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 20:42:52.684254 pve_cli-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1159 2023-12-26 03:06:31.021608 pve_cli-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      974 2023-12-26 03:06:31.025608 pve_cli-0.5.0/tests/test_main.py
--rw-r--r--   0        0        0     2505 2023-12-25 02:44:02.850927 pve_cli-0.5.0/tests/test_validators.py
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 pve_cli-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-12-25 02:44:02.838927 pve_cli-0.5.1/LICENSE
+-rw-r--r--   0        0        0      757 2024-04-14 20:34:42.634837 pve_cli-0.5.1/README.md
+-rw-r--r--   0        0        0      198 2023-12-25 02:44:02.838927 pve_cli-0.5.1/pve_cli/__init__.py
+-rw-r--r--   0        0        0     3727 2024-02-05 19:02:35.874529 pve_cli-0.5.1/pve_cli/guest_cmd.py
+-rw-r--r--   0        0        0     1880 2024-01-21 23:14:01.404696 pve_cli-0.5.1/pve_cli/main.py
+-rw-r--r--   0        0        0     6940 2024-04-24 21:54:12.403998 pve_cli-0.5.1/pve_cli/nodes_cmd.py
+-rw-r--r--   0        0        0      233 2023-12-25 02:44:02.842927 pve_cli-0.5.1/pve_cli/proxmox/__init__.py
+-rw-r--r--   0        0        0     3849 2024-02-22 15:55:23.490925 pve_cli-0.5.1/pve_cli/proxmox/api.py
+-rw-r--r--   0        0        0      449 2023-12-25 02:44:02.842927 pve_cli-0.5.1/pve_cli/proxmox/exceptions.py
+-rw-r--r--   0        0        0       96 2023-12-25 02:44:02.842927 pve_cli-0.5.1/pve_cli/proxmox/types.py
+-rw-r--r--   0        0        0        0 2024-04-24 22:01:01.380246 pve_cli-0.5.1/pve_cli/util/__init__.py
+-rw-r--r--   0        0        0      910 2024-01-21 23:14:01.408696 pve_cli-0.5.1/pve_cli/util/callbacks.py
+-rw-r--r--   0        0        0      129 2023-12-25 02:44:02.846927 pve_cli-0.5.1/pve_cli/util/exceptions.py
+-rw-r--r--   0        0        0     1574 2023-12-26 03:06:31.021608 pve_cli-0.5.1/pve_cli/util/validators.py
+-rw-r--r--   0        0        0     2298 2024-04-24 22:01:13.584568 pve_cli-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 22:01:01.384247 pve_cli-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     1159 2023-12-26 03:06:31.021608 pve_cli-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0      974 2023-12-26 03:06:31.025608 pve_cli-0.5.1/tests/test_main.py
+-rw-r--r--   0        0        0     2505 2023-12-25 02:44:02.850927 pve_cli-0.5.1/tests/test_validators.py
+-rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 pve_cli-0.5.1/PKG-INFO
```

### Comparing `pve_cli-0.5.0/LICENSE` & `pve_cli-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/README.md` & `pve_cli-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/pve_cli/guest_cmd.py` & `pve_cli-0.5.1/pve_cli/guest_cmd.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/pve_cli/main.py` & `pve_cli-0.5.1/pve_cli/main.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/pve_cli/nodes_cmd.py` & `pve_cli-0.5.1/pve_cli/nodes_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,21 +153,22 @@
                             description=f'[blue]✅ Migrated {vm["name"]} ({vm["vmid"]}) from {source_node} to {dest_node}')
             running_tasks_list.remove(upid)
 
 
 def migrate_vms(api: Proxmox, dest_node: str, vm_list: list, parallel_migrations: int = 4):
     running_tasks = {}
     running_tasks_list: list[str] = []
+    vm_list_working_copy = vm_list[:]  # copy list to not empty the actual list
     if parallel_migrations == 0:
-        parallel_migrations = len(vm_list)
+        parallel_migrations = len(vm_list_working_copy)
 
     with Progress(spinner_col, text_col) as progress:
-        while vm_list:
-            while len(running_tasks_list) < parallel_migrations and vm_list:
-                vm = vm_list.pop()
+        while vm_list_working_copy:
+            while len(running_tasks_list) < parallel_migrations and vm_list_working_copy:
+                vm = vm_list_working_copy.pop()
                 source_node, upid = api.migrate_vm(vm['vmid'], dest_node)
                 task_id = progress.add_task(
                     description=f'[white]🚚 Migrating {vm["name"]} ({vm["vmid"]}) from {source_node} to {dest_node}...',
                     total=1
                 )
                 running_tasks[upid] = (vm, source_node, task_id)
                 running_tasks_list.append(upid)
```

### Comparing `pve_cli-0.5.0/pve_cli/proxmox/api.py` & `pve_cli-0.5.1/pve_cli/proxmox/api.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/pve_cli/util/callbacks.py` & `pve_cli-0.5.1/pve_cli/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/pve_cli/util/validators.py` & `pve_cli-0.5.1/pve_cli/util/validators.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/pyproject.toml` & `pve_cli-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pve-cli"
-version = "0.5.0"
+version = "0.5.1"
 description = "CLI Tool to manage VMs and more on proxmox clusters"
 authors = [
     { name = "Dominik Rimpf", email = "dev@drimpf.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `pve_cli-0.5.0/tests/conftest.py` & `pve_cli-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/tests/test_main.py` & `pve_cli-0.5.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/tests/test_validators.py` & `pve_cli-0.5.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.5.0/PKG-INFO` & `pve_cli-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pve-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: CLI Tool to manage VMs and more on proxmox clusters
 Author-Email: Dominik Rimpf <dev@drimpf.de>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/beacontower_btpy-0.1.5.tar.gz` & `tmp/beacontower_btpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beacontower_btpy-0.1.5.tar", max compression
+gzip compressed data, was "beacontower_btpy-0.1.6.tar", max compression
```

## Comparing `beacontower_btpy-0.1.5.tar` & `beacontower_btpy-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,33 @@
--rw-r--r--   0        0        0        7 2023-12-26 12:21:25.959856 beacontower_btpy-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.5/btpy/__init__.py
--rw-r--r--   0        0        0     1113 2023-12-26 12:47:59.614828 beacontower_btpy-0.1.5/btpy/application.py
--rw-r--r--   0        0        0      997 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.5/btpy/cosmosdb.py
--rw-r--r--   0        0        0      304 2023-12-26 12:47:59.614828 beacontower_btpy-0.1.5/btpy/environment.py
--rw-r--r--   0        0        0      322 2023-12-26 12:06:09.115318 beacontower_btpy-0.1.5/btpy/main.py
--rw-r--r--   0        0        0     4808 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.5/btpy/misc.py
--rw-r--r--   0        0        0      577 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.5/btpy/scripts.py
--rw-r--r--   0        0        0     1601 2024-03-14 20:38:11.198694 beacontower_btpy-0.1.5/btpy/ssh.py
--rw-r--r--   0        0        0      304 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.5/btpy/stamp.py
--rw-r--r--   0        0        0     1892 2024-03-14 20:38:11.198694 beacontower_btpy-0.1.5/btpy/subscription.py
--rw-r--r--   0        0        0     2061 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.5/btpy/suffix.py
--rw-r--r--   0        0        0      287 2023-12-26 12:49:20.112579 beacontower_btpy-0.1.5/btpy/terraform.py
--rw-r--r--   0        0        0     3258 2023-12-26 12:47:59.614828 beacontower_btpy-0.1.5/btpy/tfvars.py
--rw-r--r--   0        0        0      404 2023-12-26 12:47:59.622829 beacontower_btpy-0.1.5/btpy/variables.py
--rw-r--r--   0        0        0      655 2024-03-14 20:37:29.145843 beacontower_btpy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 beacontower_btpy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-03-25 20:45:38.735946 beacontower_btpy-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.6/btpy/__init__.py
+-rw-r--r--   0        0        0     1113 2023-12-26 12:47:59.614828 beacontower_btpy-0.1.6/btpy/application.py
+-rw-r--r--   0        0        0     1907 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/commands/env_commands.py
+-rw-r--r--   0        0        0      930 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/configuration/config.py
+-rw-r--r--   0        0        0      382 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/azure_utility.py
+-rw-r--r--   0        0        0     6349 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/envs/desc_templates/bt_3_0_0.json
+-rw-r--r--   0        0        0     2406 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/envs/env_client.py
+-rw-r--r--   0        0        0     4179 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/envs/env_desc.py
+-rw-r--r--   0        0        0     6427 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/envs/env_desc_loader.py
+-rw-r--r--   0        0        0      113 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/envs/env_utility.py
+-rw-r--r--   0        0        0      328 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/file_utility.py
+-rw-r--r--   0        0        0     1839 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/resource_clients/azure/azure_appservice_client.py
+-rw-r--r--   0        0        0     1456 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/resource_clients/azure/azure_function_client.py
+-rw-r--r--   0        0        0     1127 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/resource_clients/azure/azure_storage_web_client.py
+-rw-r--r--   0        0        0     1127 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/resource_clients/azure/azure_vm_client.py
+-rw-r--r--   0        0        0     1099 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/resource_clients/resource_client.py
+-rw-r--r--   0        0        0      984 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/core/resource_clients/resource_client_factory.py
+-rw-r--r--   0        0        0      997 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.6/btpy/cosmosdb.py
+-rw-r--r--   0        0        0      304 2023-12-26 12:47:59.614828 beacontower_btpy-0.1.6/btpy/environment.py
+-rw-r--r--   0        0        0      157 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/main.py
+-rw-r--r--   0        0        0     4808 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.6/btpy/misc.py
+-rw-r--r--   0        0        0      491 2024-04-25 12:32:24.654248 beacontower_btpy-0.1.6/btpy/print_utility.py
+-rw-r--r--   0        0        0      577 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.6/btpy/scripts.py
+-rw-r--r--   0        0        0     1601 2024-03-14 20:38:11.198694 beacontower_btpy-0.1.6/btpy/ssh.py
+-rw-r--r--   0        0        0      304 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.6/btpy/stamp.py
+-rw-r--r--   0        0        0     1892 2024-03-14 20:38:11.198694 beacontower_btpy-0.1.6/btpy/subscription.py
+-rw-r--r--   0        0        0     2061 2023-12-25 12:56:58.479687 beacontower_btpy-0.1.6/btpy/suffix.py
+-rw-r--r--   0        0        0      287 2023-12-26 12:49:20.112579 beacontower_btpy-0.1.6/btpy/terraform.py
+-rw-r--r--   0        0        0     3258 2023-12-26 12:47:59.614828 beacontower_btpy-0.1.6/btpy/tfvars.py
+-rw-r--r--   0        0        0      404 2023-12-26 12:47:59.622829 beacontower_btpy-0.1.6/btpy/variables.py
+-rw-r--r--   0        0        0      849 2024-04-25 12:35:32.414738 beacontower_btpy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 beacontower_btpy-0.1.6/PKG-INFO
```

### Comparing `beacontower_btpy-0.1.5/btpy/application.py` & `beacontower_btpy-0.1.6/btpy/application.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/cosmosdb.py` & `beacontower_btpy-0.1.6/btpy/cosmosdb.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/misc.py` & `beacontower_btpy-0.1.6/btpy/misc.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/scripts.py` & `beacontower_btpy-0.1.6/btpy/scripts.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/ssh.py` & `beacontower_btpy-0.1.6/btpy/ssh.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/subscription.py` & `beacontower_btpy-0.1.6/btpy/subscription.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/suffix.py` & `beacontower_btpy-0.1.6/btpy/suffix.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/btpy/tfvars.py` & `beacontower_btpy-0.1.6/btpy/tfvars.py`

 * *Files identical despite different names*

### Comparing `beacontower_btpy-0.1.5/PKG-INFO` & `beacontower_btpy-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: beacontower-btpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Fredrik Svensson
 Author-email: fredrik@glaze.se
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: ansible (>=9.1.0,<10.0.0)
 Requires-Dist: az-cli (>=0.5,<0.6)
+Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
+Requires-Dist: azure-mgmt-appconfiguration (>=3.0.0,<4.0.0)
+Requires-Dist: azure-mgmt-compute (>=30.6.0,<31.0.0)
+Requires-Dist: azure-mgmt-web (>=7.2.0,<8.0.0)
+Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dda-python-terraform (>=2.1.1,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sshkey-tools (>=0.10.3,<0.11.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # btpy
 
+https://github.com/frier-sam/pypi_multi_versions
+
```


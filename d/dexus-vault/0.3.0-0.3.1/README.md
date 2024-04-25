# Comparing `tmp/dexus_vault-0.3.0.tar.gz` & `tmp/dexus_vault-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexus_vault-0.3.0.tar", last modified: Wed Apr 24 12:04:52 2024, max compression
+gzip compressed data, was "dexus_vault-0.3.1.tar", last modified: Thu Apr 25 16:33:39 2024, max compression
```

## Comparing `dexus_vault-0.3.0.tar` & `dexus_vault-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.477134 dexus_vault-0.3.0/dexus_vault/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/src/dex_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/src/vault_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/syncer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.401476 dexus_vault-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-25 16:33:39.401476 dexus_vault-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.397476 dexus_vault-0.3.1/dexus_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.397476 dexus_vault-0.3.1/dexus_vault/grpc_dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/grpc_dexidp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.397476 dexus_vault-0.3.1/dexus_vault/grpc_dexidp/dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/grpc_dexidp/dexidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.397476 dexus_vault-0.3.1/dexus_vault/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/src/dex_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/src/vault_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.397476 dexus_vault-0.3.1/dexus_vault/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/dexus_vault/utils/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:33:39.401476 dexus_vault-0.3.1/dexus_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-25 16:33:39.000000 dexus_vault-0.3.1/dexus_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-25 16:33:39.000000 dexus_vault-0.3.1/dexus_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:33:39.000000 dexus_vault-0.3.1/dexus_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 16:33:39.000000 dexus_vault-0.3.1/dexus_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 16:33:39.000000 dexus_vault-0.3.1/dexus_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 16:33:39.000000 dexus_vault-0.3.1/dexus_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:33:39.401476 dexus_vault-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-25 16:33:33.000000 dexus_vault-0.3.1/setup.py
```

### Comparing `dexus_vault-0.3.0/LICENSE` & `dexus_vault-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/PKG-INFO` & `dexus_vault-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.3.0
+Version: 0.3.1
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `dexus_vault-0.3.0/README.md` & `dexus_vault-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/__main__.py` & `dexus_vault-0.3.1/dexus_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py` & `dexus_vault-0.3.1/dexus_vault/grpc_dexidp/dexidp/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py` & `dexus_vault-0.3.1/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/src/dex_processor.py` & `dexus_vault-0.3.1/dexus_vault/src/dex_processor.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/src/vault_processor.py` & `dexus_vault-0.3.1/dexus_vault/src/vault_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     return True
                 else:
                     logger.warning(
                         f"Vault {self.config.vault_addr} is not initialized {status}"
                     )
             except requests.exceptions.ConnectionError:
                 logger.warning(f"Vault {self.config.vault_addr} connection failed")
-            time.sleep(self.config.vault_addr)
+            time.sleep(self.config.vault_retry_wait)
         logger.error(f"Vault {self.config.vault_addr} unreachable, exiting...")
         sys.exit(1)
 
     def _check_if_vault_auth(self, client: object, auth_method: str) -> None:
         """
         Function validates if we successfully authenticated to Vault
         """
```

### Comparing `dexus_vault-0.3.0/dexus_vault/syncer.py` & `dexus_vault-0.3.1/dexus_vault/syncer.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/utils/config.py` & `dexus_vault-0.3.1/dexus_vault/utils/config.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/utils/logger.py` & `dexus_vault-0.3.1/dexus_vault/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault/utils/metrics.py` & `dexus_vault-0.3.1/dexus_vault/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/dexus_vault.egg-info/PKG-INFO` & `dexus_vault-0.3.1/dexus_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.3.0
+Version: 0.3.1
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `dexus_vault-0.3.0/dexus_vault.egg-info/SOURCES.txt` & `dexus_vault-0.3.1/dexus_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.3.0/setup.py` & `dexus_vault-0.3.1/setup.py`

 * *Files identical despite different names*


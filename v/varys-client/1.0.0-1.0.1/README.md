# Comparing `tmp/varys-client-1.0.0.tar.gz` & `tmp/varys_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varys-client-1.0.0.tar", last modified: Thu Feb 15 15:42:18 2024, max compression
+gzip compressed data, was "varys_client-1.0.1.tar", last modified: Thu Apr 25 10:09:10 2024, max compression
```

## Comparing `varys-client-1.0.0.tar` & `varys_client-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:42:18.562998 varys-client-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-15 15:42:10.000000 varys-client-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-02-15 15:42:18.562998 varys-client-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-02-15 15:42:10.000000 varys-client-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-15 15:42:18.562998 varys-client-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 15:42:10.000000 varys-client-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:42:18.558998 varys-client-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 15:42:10.000000 varys-client-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-02-15 15:42:10.000000 varys-client-1.0.0/tests/test_varys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:42:18.558998 varys-client-1.0.0/varys/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-15 15:42:10.000000 varys-client-1.0.0/varys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-15 15:42:10.000000 varys-client-1.0.0/varys/consumer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8018 2024-02-15 15:42:10.000000 varys-client-1.0.0/varys/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-02-15 15:42:10.000000 varys-client-1.0.0/varys/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-02-15 15:42:10.000000 varys-client-1.0.0/varys/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-15 15:42:10.000000 varys-client-1.0.0/varys/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:42:18.562998 varys-client-1.0.0/varys_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-02-15 15:42:18.000000 varys-client-1.0.0/varys_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-15 15:42:18.000000 varys-client-1.0.0/varys_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 15:42:18.000000 varys-client-1.0.0/varys_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 15:42:18.000000 varys-client-1.0.0/varys_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-15 15:42:18.000000 varys-client-1.0.0/varys_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-15 15:42:18.000000 varys-client-1.0.0/varys_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-15 15:42:10.000000 varys-client-1.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:09:10.866993 varys_client-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 10:09:04.000000 varys_client-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-25 10:09:10.866993 varys_client-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-25 10:09:04.000000 varys_client-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-25 10:09:10.870993 varys_client-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:09:04.000000 varys_client-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:09:10.866993 varys_client-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:09:04.000000 varys_client-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-25 10:09:04.000000 varys_client-1.0.1/tests/test_varys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:09:10.866993 varys_client-1.0.1/varys/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 10:09:04.000000 varys_client-1.0.1/varys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-25 10:09:04.000000 varys_client-1.0.1/varys/consumer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8018 2024-04-25 10:09:04.000000 varys_client-1.0.1/varys/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-25 10:09:04.000000 varys_client-1.0.1/varys/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-25 10:09:04.000000 varys_client-1.0.1/varys/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-25 10:09:04.000000 varys_client-1.0.1/varys/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:09:10.866993 varys_client-1.0.1/varys_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-25 10:09:10.000000 varys_client-1.0.1/varys_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-25 10:09:10.000000 varys_client-1.0.1/varys_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:09:10.000000 varys_client-1.0.1/varys_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:09:10.000000 varys_client-1.0.1/varys_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 10:09:10.000000 varys_client-1.0.1/varys_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 10:09:10.000000 varys_client-1.0.1/varys_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 10:09:04.000000 varys_client-1.0.1/version.txt
```

### Comparing `varys-client-1.0.0/LICENSE` & `varys_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/PKG-INFO` & `varys_client-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varys-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pika-based python RabbitMQ client for use in the CLIMB-tree project
 Home-page: https://github.com/climb-tre/varys
 Author: Sam Wilkinson
 Author-email: s.a.j.wilkinson@bham.ac.uk
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -56,15 +56,15 @@
 ---
 
 ### Basic Usage
 
 First the varys object must be instantiated, like so:
 
 ```python
-import varys
+from varys import Varys
 
 varys_client = Varys(
     profile="test_user",
     logfile="/var/log/varys_test.log",
     log_level="DEBUG"
 )
 ```
```

### Comparing `varys-client-1.0.0/README.md` & `varys_client-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ---
 
 ### Basic Usage
 
 First the varys object must be instantiated, like so:
 
 ```python
-import varys
+from varys import Varys
 
 varys_client = Varys(
     profile="test_user",
     logfile="/var/log/varys_test.log",
     log_level="DEBUG"
 )
 ```
```

### Comparing `varys-client-1.0.0/setup.cfg` & `varys_client-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/tests/test_varys.py` & `varys_client-1.0.1/tests/test_varys.py`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/varys/consumer.py` & `varys_client-1.0.1/varys/consumer.py`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/varys/controller.py` & `varys_client-1.0.1/varys/controller.py`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/varys/process.py` & `varys_client-1.0.1/varys/process.py`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/varys/producer.py` & `varys_client-1.0.1/varys/producer.py`

 * *Files identical despite different names*

### Comparing `varys-client-1.0.0/varys/utils.py` & `varys_client-1.0.1/varys/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 
 class configurator:
     def __init__(self, profile, config_path):
         try:
             with open(config_path, "rt") as config_fh:
                 config_obj = json.load(config_fh)
-        except:
+        except Exception as e:
             print(
-                "Configuration JSON does not appear to be valid or does not exist",
+                f"Varys Configuration JSON parsing failed with exception:\n{e}",
                 file=sys.stderr,
             )
             sys.exit(11)
 
         if config_obj["version"] != "0.1":
             print(
                 "Version number in the ROZ configuration file does not appear to be current, ensure configuration format is correct if you experience errors",
```

### Comparing `varys-client-1.0.0/varys_client.egg-info/PKG-INFO` & `varys_client-1.0.1/varys_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varys-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: A pika-based python RabbitMQ client for use in the CLIMB-tree project
 Home-page: https://github.com/climb-tre/varys
 Author: Sam Wilkinson
 Author-email: s.a.j.wilkinson@bham.ac.uk
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -56,15 +56,15 @@
 ---
 
 ### Basic Usage
 
 First the varys object must be instantiated, like so:
 
 ```python
-import varys
+from varys import Varys
 
 varys_client = Varys(
     profile="test_user",
     logfile="/var/log/varys_test.log",
     log_level="DEBUG"
 )
 ```
```


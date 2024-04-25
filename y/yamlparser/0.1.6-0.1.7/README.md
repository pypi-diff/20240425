# Comparing `tmp/yamlparser-0.1.6.tar.gz` & `tmp/yamlparser-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Source/github/yamlparse/dist/.tmp-rcbt7dlj/yamlparser-0.1.6.tar", last modified: Thu Apr 18 15:20:58 2024, max compression
+gzip compressed data, was "/mnt/d/Source/github/yamlparse/dist/.tmp-rjtax01e/yamlparser-0.1.7.tar", last modified: Thu Apr 25 11:31:22 2024, max compression
```

## Comparing `yamlparser-0.1.6.tar` & `yamlparser-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-18 15:20:58.769998 yamlparser-0.1.6/
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)     1559 2023-11-09 10:17:41.000000 yamlparser-0.1.6/LICENSE
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-04-18 15:20:58.767995 yamlparser-0.1.6/PKG-INFO
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    12499 2024-03-27 07:51:12.000000 yamlparser-0.1.6/README.md
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)      819 2024-04-18 15:19:51.000000 yamlparser-0.1.6/pyproject.toml
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2023-12-06 12:16:15.000000 yamlparser-0.1.6/requirements.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       38 2024-04-18 15:20:58.770993 yamlparser-0.1.6/setup.cfg
-drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-18 15:20:58.741995 yamlparser-0.1.6/yamlparser/
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       98 2024-03-26 16:19:18.000000 yamlparser-0.1.6/yamlparser/__init__.py
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    14186 2024-04-18 11:56:06.000000 yamlparser-0.1.6/yamlparser/namespace.py
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)     6353 2024-04-17 17:09:30.000000 yamlparser-0.1.6/yamlparser/parser.py
-drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-18 15:20:58.762009 yamlparser-0.1.6/yamlparser.egg-info/
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-04-18 15:20:58.000000 yamlparser-0.1.6/yamlparser.egg-info/PKG-INFO
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)      286 2024-04-18 15:20:58.000000 yamlparser-0.1.6/yamlparser.egg-info/SOURCES.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)        1 2024-04-18 15:20:58.000000 yamlparser-0.1.6/yamlparser.egg-info/dependency_links.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2024-04-18 15:20:58.000000 yamlparser-0.1.6/yamlparser.egg-info/requires.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       11 2024-04-18 15:20:58.000000 yamlparser-0.1.6/yamlparser.egg-info/top_level.txt
+drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-25 11:31:22.752082 yamlparser-0.1.7/
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)     1559 2023-11-09 10:17:41.000000 yamlparser-0.1.7/LICENSE
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-04-25 11:31:22.751085 yamlparser-0.1.7/PKG-INFO
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    12499 2024-03-27 07:51:12.000000 yamlparser-0.1.7/README.md
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)      819 2024-04-18 19:55:02.000000 yamlparser-0.1.7/pyproject.toml
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2023-12-06 12:16:15.000000 yamlparser-0.1.7/requirements.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       38 2024-04-25 11:31:22.753074 yamlparser-0.1.7/setup.cfg
+drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-25 11:31:22.742071 yamlparser-0.1.7/yamlparser/
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       98 2024-03-26 16:19:18.000000 yamlparser-0.1.7/yamlparser/__init__.py
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    14248 2024-04-18 19:54:35.000000 yamlparser-0.1.7/yamlparser/namespace.py
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)     6353 2024-04-17 17:09:30.000000 yamlparser-0.1.7/yamlparser/parser.py
+drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-25 11:31:22.749093 yamlparser-0.1.7/yamlparser.egg-info/
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-04-25 11:31:22.000000 yamlparser-0.1.7/yamlparser.egg-info/PKG-INFO
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)      286 2024-04-25 11:31:22.000000 yamlparser-0.1.7/yamlparser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)        1 2024-04-25 11:31:22.000000 yamlparser-0.1.7/yamlparser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2024-04-25 11:31:22.000000 yamlparser-0.1.7/yamlparser.egg-info/requires.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       11 2024-04-25 11:31:22.000000 yamlparser-0.1.7/yamlparser.egg-info/top_level.txt
```

### Comparing `yamlparser-0.1.6/LICENSE` & `yamlparser-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlparser-0.1.6/PKG-INFO` & `yamlparser-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlparser
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Package to combine YAML configurations and argument parsing
 Author-email: Manuel Guenther <siebenkopf@googlemail.com>
 Project-URL: Homepage, https://github.com/AIML-IfI/yamlparser
 Project-URL: Bug Tracker, https://github.com/AIML-IfI/yamlparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yamlparser-0.1.6/README.md` & `yamlparser-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `yamlparser-0.1.6/pyproject.toml` & `yamlparser-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yamlparser"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{name="Manuel Guenther", email="siebenkopf@googlemail.com"}]
 description = "A Package to combine YAML configurations and argument parsing"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yamlparser-0.1.6/yamlparser/namespace.py` & `yamlparser-0.1.7/yamlparser/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,11 +342,12 @@
                 raise ValueError(f"The given config file {resource} is not unique in package {package}; candidates are: {candidates}")
             # take the unique file
             config = candidates[0]
 
         else:
             raise ValueError(f"Could not interpret configuration file {config}")
 
+        if not os.path.isfile(config):
+            raise IOError(f"Could not find config file {config}")
 
-        if os.path.isfile(config):
-            with open(config, 'r') as f:
-                return yaml.safe_load(f)
+        with open(config, 'r') as f:
+            return yaml.safe_load(f)
```

### Comparing `yamlparser-0.1.6/yamlparser/parser.py` & `yamlparser-0.1.7/yamlparser/parser.py`

 * *Files identical despite different names*

### Comparing `yamlparser-0.1.6/yamlparser.egg-info/PKG-INFO` & `yamlparser-0.1.7/yamlparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlparser
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Package to combine YAML configurations and argument parsing
 Author-email: Manuel Guenther <siebenkopf@googlemail.com>
 Project-URL: Homepage, https://github.com/AIML-IfI/yamlparser
 Project-URL: Bug Tracker, https://github.com/AIML-IfI/yamlparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


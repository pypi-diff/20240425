# Comparing `tmp/opsdroid-0.9.0.tar.gz` & `tmp/opsdroid-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opsdroid-0.9.0.tar", last modified: Thu Sep 14 07:00:02 2017, max compression
+gzip compressed data, was "dist/opsdroid-0.9.1.tar", last modified: Wed Sep 20 14:21:57 2017, max compression
```

## Comparing `opsdroid-0.9.0.tar` & `opsdroid-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-14 07:00:02.000000 opsdroid-0.9.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid/configuration/
--rw-r--r--   0 travis    (2000) travis    (2000)     5799 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/configuration/example_configuration.yaml
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid/parsers/
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/parsers/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3173 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/parsers/apiai.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1262 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/parsers/crontab.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1490 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/parsers/regex.py
--rw-r--r--   0 travis    (2000) travis    (2000)       30 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3041 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/__main__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2280 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/connector.py
--rw-r--r--   0 travis    (2000) travis    (2000)      688 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/const.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7054 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/core.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2149 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/database.py
--rw-r--r--   0 travis    (2000) travis    (2000)      247 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/helper.py
--rw-r--r--   0 travis    (2000) travis    (2000)    11926 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/loader.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3127 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/matchers.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1651 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/memory.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1165 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/message.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3517 2017-09-14 06:59:15.000000 opsdroid-0.9.0/opsdroid/web.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      263 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      666 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       53 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       55 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        9 2017-09-14 07:00:02.000000 opsdroid-0.9.0/opsdroid.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)    35141 2017-09-14 06:59:15.000000 opsdroid-0.9.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)      136 2017-09-14 06:59:15.000000 opsdroid-0.9.0/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     8296 2017-09-14 06:59:15.000000 opsdroid-0.9.0/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)      214 2017-09-14 07:00:02.000000 opsdroid-0.9.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      973 2017-09-14 06:59:15.000000 opsdroid-0.9.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      263 2017-09-14 07:00:02.000000 opsdroid-0.9.0/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-20 14:21:57.000000 opsdroid-0.9.1/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid/configuration/
+-rw-r--r--   0 travis    (2000) travis    (2000)     5799 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/configuration/example_configuration.yaml
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid/parsers/
+-rw-r--r--   0 travis    (2000) travis    (2000)       38 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/parsers/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3173 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/parsers/apiai.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1262 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/parsers/crontab.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1490 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/parsers/regex.py
+-rw-r--r--   0 travis    (2000) travis    (2000)       30 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3041 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/__main__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2280 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/connector.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      688 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/const.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7054 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/core.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2149 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/database.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      247 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/helper.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    11973 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/loader.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3127 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/matchers.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1651 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/memory.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1165 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/message.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3517 2017-09-20 14:20:53.000000 opsdroid-0.9.1/opsdroid/web.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)      263 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      666 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       53 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (2000) travis    (2000)       55 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        9 2017-09-20 14:21:57.000000 opsdroid-0.9.1/opsdroid.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)    35141 2017-09-20 14:20:53.000000 opsdroid-0.9.1/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)      136 2017-09-20 14:20:53.000000 opsdroid-0.9.1/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     8296 2017-09-20 14:20:53.000000 opsdroid-0.9.1/README.md
+-rw-r--r--   0 travis    (2000) travis    (2000)      214 2017-09-20 14:21:57.000000 opsdroid-0.9.1/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)      973 2017-09-20 14:20:53.000000 opsdroid-0.9.1/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      263 2017-09-20 14:21:57.000000 opsdroid-0.9.1/PKG-INFO
```

### Comparing `opsdroid-0.9.0/opsdroid/configuration/example_configuration.yaml` & `opsdroid-0.9.1/opsdroid/configuration/example_configuration.yaml`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/parsers/apiai.py` & `opsdroid-0.9.1/opsdroid/parsers/apiai.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/parsers/crontab.py` & `opsdroid-0.9.1/opsdroid/parsers/crontab.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/parsers/regex.py` & `opsdroid-0.9.1/opsdroid/parsers/regex.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/__main__.py` & `opsdroid-0.9.1/opsdroid/__main__.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/connector.py` & `opsdroid-0.9.1/opsdroid/connector.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/const.py` & `opsdroid-0.9.1/opsdroid/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constants used by OpsDroid."""
 import os
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 DEFAULT_GIT_URL = "https://github.com/opsdroid/"
 MODULES_DIRECTORY = "opsdroid-modules"
 DEFAULT_ROOT_PATH = os.path.expanduser("~/.opsdroid")
 DEFAULT_LOG_FILENAME = os.path.join(DEFAULT_ROOT_PATH, 'output.log')
 DEFAULT_MODULES_PATH = os.path.join(DEFAULT_ROOT_PATH, "modules")
 DEFAULT_MODULE_DEPS_PATH = os.path.join(DEFAULT_ROOT_PATH, "site-packages")
```

### Comparing `opsdroid-0.9.0/opsdroid/core.py` & `opsdroid-0.9.1/opsdroid/core.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/database.py` & `opsdroid-0.9.1/opsdroid/database.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/loader.py` & `opsdroid-0.9.1/opsdroid/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
         _LOGGER.info("Creating %s.", config_path)
         config_dir, _ = os.path.split(config_path)
         if not os.path.isdir(config_dir):
             os.makedirs(config_dir)
         shutil.copyfile(EXAMPLE_CONFIG_FILE, config_path)
         return config_path
 
-    @staticmethod
-    def _reload_modules(modules):
+    def _reload_modules(self, modules):
         for module in modules:
+            self.current_import_config = module["config"]
             importlib.reload(module["module"])
 
     def load_config_file(self, config_paths):
         """Load a yaml config file from path."""
         config_path = ""
         for possible_path in config_paths:
             if not os.path.isfile(possible_path):
@@ -184,14 +184,15 @@
         else:
             _LOGGER.warning("No databases in configuration")
 
         if 'skills' in config.keys():
             skills = self._load_modules('skill', config['skills'])
             self.opsdroid.skills = []
             self._reload_modules(skills)
+
         else:
             self.opsdroid.critical(
                 "No skills in configuration, at least 1 required", 1)
 
         if 'connectors' in config.keys():
             connectors = self._load_modules('connector', config['connectors'])
         else:
```

### Comparing `opsdroid-0.9.0/opsdroid/matchers.py` & `opsdroid-0.9.1/opsdroid/matchers.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/memory.py` & `opsdroid-0.9.1/opsdroid/memory.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/message.py` & `opsdroid-0.9.1/opsdroid/message.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid/web.py` & `opsdroid-0.9.1/opsdroid/web.py`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/opsdroid.egg-info/SOURCES.txt` & `opsdroid-0.9.1/opsdroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/LICENSE` & `opsdroid-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/README.md` & `opsdroid-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `opsdroid-0.9.0/setup.py` & `opsdroid-0.9.1/setup.py`

 * *Files identical despite different names*


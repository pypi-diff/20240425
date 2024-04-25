# Comparing `tmp/rcsb_utils_config-0.39.tar.gz` & `tmp/rcsb_utils_config-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb_utils_config-0.39.tar", last modified: Tue Apr 16 11:01:02 2024, max compression
+gzip compressed data, was "rcsb_utils_config-0.40.tar", last modified: Thu Apr 25 10:29:05 2024, max compression
```

## Comparing `rcsb_utils_config-0.39.tar` & `rcsb_utils_config-0.40.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/
--rw-r--r--   0 vsts      (1001) docker     (127)     2332 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1951 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1021 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb/utils/config/
--rw-r--r--   0 vsts      (1001) docker     (127)    29277 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/config/ConfigUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/config/ExampleHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/config/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1951 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 11:00:45.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      132 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2427 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 10:29:05.787947 rcsb_utils_config-0.40/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2402 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1951 2024-04-25 10:29:05.787947 rcsb_utils_config-0.40/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1021 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 10:29:05.783947 rcsb_utils_config-0.40/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 10:29:05.787947 rcsb_utils_config-0.40/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 10:29:05.787947 rcsb_utils_config-0.40/rcsb/utils/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)    29707 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/rcsb/utils/config/ConfigUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/rcsb/utils/config/ExampleHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/rcsb/utils/config/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 10:29:05.787947 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1951 2024-04-25 10:29:05.000000 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-25 10:29:05.000000 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 10:29:05.000000 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 10:28:51.000000 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      132 2024-04-25 10:29:05.000000 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-25 10:29:05.000000 rcsb_utils_config-0.40/rcsb.utils.config.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-25 10:29:05.787947 rcsb_utils_config-0.40/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2427 2024-04-25 10:28:17.000000 rcsb_utils_config-0.40/setup.py
```

### Comparing `rcsb_utils_config-0.39/HISTORY.txt` & `rcsb_utils_config-0.40/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,8 +27,9 @@
  3-Feb-2020  - V0.32 Use a generic temporary directory of incorporated configs if cache is not explicitly pathed.
  3-Feb-2020  - V0.33 Change defaults for cache behavior.
 13-May-2020  - V0.34 Update dependencies
 13-May-2020  - V0.35 Update dependencies
 22-Aug-2021  - V0.36 Update install script and fix linting issues
  3-Mar-2022  - V0.37 Clean-up logging messages
  9-Jan-2023  - V0.38 Configuration changes to support tox 4 and testing python 3.9
-16-Apr-2024  - V0.39 Update setuptools config
+16-Apr-2024  - V0.39 Update setuptools config
+17-Apr-2024  - V0.40 Add support for reading in config file remotely
```

### Comparing `rcsb_utils_config-0.39/LICENSE` & `rcsb_utils_config-0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb_utils_config-0.39/PKG-INFO` & `rcsb_utils_config-0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.config
-Version: 0.39
+Version: 0.40
 Summary: RCSB Python Configuration Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_config
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb_utils_config-0.39/README.md` & `rcsb_utils_config-0.40/README.md`

 * *Files identical despite different names*

### Comparing `rcsb_utils_config-0.39/rcsb/utils/config/ConfigUtil.py` & `rcsb_utils_config-0.40/rcsb/utils/config/ConfigUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #   23-Oct-2018  jdw refine export method to manually extract content from configparser structure
 #   24-Oct-2018  jdw if config format is not specified perceive the format from the config filename extension
 #                    change default section name management.
 #    4-Jan-2019  jdw add optional arguments to getPath(...,prefixName=None, prefixSectionName=None)
 #                    add methods getDefaultSectionName(), replaceSectionName(), and getSectionNameReplacement()
 #   10-Mar-2019  jdw add method getEnvValue() to dereference config option as an environmental variable
 #    3-Feb-2020  jdw add __processAppendedSections() to handle nested configuration sections
+#   17-Apr-2024  dwp add support for reading in config file remotely
 ##
 """
  Manage simple configuration options.
 
 """
 
 __docformat__ = "restructuredtext en"
@@ -33,14 +34,15 @@
 
 import base64
 import copy
 import logging
 import os
 import sys
 import tempfile
+import requests
 
 import ruamel.yaml
 from nacl.encoding import HexEncoder
 from nacl.secret import SecretBox
 
 from rcsb.utils.io.FileUtil import FileUtil
 
@@ -544,22 +546,29 @@
             **kwargs: (dict) passed to ConfigParser/configparser
 
         Returns:
             object: On success a ConfigParser dictionary-like object or an empty dictionary on Failure
 
         """
         _ = kwargs
+        fU = FileUtil()
         yaml = ruamel.yaml.YAML()
         yaml.preserve_quotes = True
         yaml.indent(mapping=4, sequence=6, offset=4)
         yaml.explicit_start = True
         rD = {}
         try:
-            with open(configPath, "r", encoding="utf-8") as stream:
-                rD = yaml.load(stream)
+            if fU.isLocal(configPath):
+                with open(configPath, "r", encoding="utf-8") as stream:
+                    rD = yaml.load(stream)
+            else:
+                resp = requests.get(configPath, timeout=60)
+                if not resp.status_code == 200:
+                    raise ValueError("Failed to fetch remote YAML configuration file %s" & configPath)
+                rD = yaml.load(resp.content)
         except Exception as e:
             logger.error("Failed reading YAML configuration file %s with %s", configPath, str(e))
         return rD
 
     def __writeIniFile(self, configPath, configObj, **kwargs):
         """Internal method to write INI-style configuration file using standard ConfigParser/configparser library.
```

### Comparing `rcsb_utils_config-0.39/rcsb.utils.config.egg-info/PKG-INFO` & `rcsb_utils_config-0.40/rcsb.utils.config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.config
-Version: 0.39
+Version: 0.40
 Summary: RCSB Python Configuration Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_config
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb_utils_config-0.39/setup.py` & `rcsb_utils_config-0.40/setup.py`

 * *Files identical despite different names*


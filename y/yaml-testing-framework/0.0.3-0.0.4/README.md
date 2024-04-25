# Comparing `tmp/yaml_testing_framework-0.0.3.tar.gz` & `tmp/yaml_testing_framework-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_testing_framework-0.0.3.tar", last modified: Thu Apr 25 08:20:01 2024, max compression
+gzip compressed data, was "yaml_testing_framework-0.0.4.tar", last modified: Thu Apr 25 08:20:44 2024, max compression
```

## Comparing `yaml_testing_framework-0.0.3.tar` & `yaml_testing_framework-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olufemij  (1000) olufemij  (1000)        0 2024-04-25 08:20:01.025777 yaml_testing_framework-0.0.3/
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)     1074 2023-07-24 19:00:28.000000 yaml_testing_framework-0.0.3/LICENSE
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)      196 2023-12-11 10:35:31.000000 yaml_testing_framework-0.0.3/MANIFEST.in
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)    12017 2024-04-25 08:20:01.025777 yaml_testing_framework-0.0.3/PKG-INFO
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)    11442 2024-04-25 06:53:10.000000 yaml_testing_framework-0.0.3/README.md
-drwxr-xr-x   0 olufemij  (1000) olufemij  (1000)        0 2024-04-25 08:20:01.025777 yaml_testing_framework-0.0.3/main/
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)      808 2024-04-25 08:15:24.000000 yaml_testing_framework-0.0.3/main/__init__.py
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)     8495 2024-04-25 07:58:26.000000 yaml_testing_framework-0.0.3/main/app.py
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)     3356 2024-04-25 07:58:26.000000 yaml_testing_framework-0.0.3/main/plugin.py
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)      641 2024-04-25 05:58:48.000000 yaml_testing_framework-0.0.3/pyproject.toml
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)       38 2024-04-25 08:20:01.025777 yaml_testing_framework-0.0.3/setup.cfg
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)     3050 2024-04-25 06:48:39.000000 yaml_testing_framework-0.0.3/setup.py
-drwxr-xr-x   0 olufemij  (1000) olufemij  (1000)        0 2024-04-25 08:20:01.025777 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)    12017 2024-04-25 08:20:01.000000 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)      371 2024-04-25 08:20:01.000000 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)        1 2024-04-25 08:20:01.000000 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)       48 2024-04-25 08:20:01.000000 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/entry_points.txt
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)        5 2024-04-25 08:20:01.000000 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 olufemij  (1000) olufemij  (1000)        1 2024-04-25 04:27:46.000000 yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/zip-safe
+drwxr-xr-x   0 olufemij  (1000) olufemij  (1000)        0 2024-04-25 08:20:44.582497 yaml_testing_framework-0.0.4/
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)     1074 2023-07-24 19:00:28.000000 yaml_testing_framework-0.0.4/LICENSE
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)      196 2023-12-11 10:35:31.000000 yaml_testing_framework-0.0.4/MANIFEST.in
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)    12017 2024-04-25 08:20:44.582497 yaml_testing_framework-0.0.4/PKG-INFO
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)    11442 2024-04-25 06:53:10.000000 yaml_testing_framework-0.0.4/README.md
+drwxr-xr-x   0 olufemij  (1000) olufemij  (1000)        0 2024-04-25 08:20:44.582497 yaml_testing_framework-0.0.4/main/
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)      808 2024-04-25 08:15:24.000000 yaml_testing_framework-0.0.4/main/__init__.py
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)     8495 2024-04-25 07:58:26.000000 yaml_testing_framework-0.0.4/main/app.py
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)     3356 2024-04-25 07:58:26.000000 yaml_testing_framework-0.0.4/main/plugin.py
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)      641 2024-04-25 05:58:48.000000 yaml_testing_framework-0.0.4/pyproject.toml
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)       38 2024-04-25 08:20:44.582497 yaml_testing_framework-0.0.4/setup.cfg
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)     3050 2024-04-25 06:48:39.000000 yaml_testing_framework-0.0.4/setup.py
+drwxr-xr-x   0 olufemij  (1000) olufemij  (1000)        0 2024-04-25 08:20:44.582497 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)    12017 2024-04-25 08:20:44.000000 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)      371 2024-04-25 08:20:44.000000 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)        1 2024-04-25 08:20:44.000000 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)       48 2024-04-25 08:20:44.000000 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/entry_points.txt
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)        5 2024-04-25 08:20:44.000000 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 olufemij  (1000) olufemij  (1000)        1 2024-04-25 04:27:46.000000 yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/zip-safe
```

### Comparing `yaml_testing_framework-0.0.3/LICENSE` & `yaml_testing_framework-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/PKG-INFO` & `yaml_testing_framework-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-testing-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: A testing framework where tests are defined in YAML files
 Home-page: https://github.com/fjemi/yaml-testing-framework
 Author: Olufemi Jemilohun
 Author-email: olufemi.jemilohun@gmail.com
 License: MIT license
 Keywords: pytest,yaml,testing
 Classifier: Framework :: Pytest
```

### Comparing `yaml_testing_framework-0.0.3/README.md` & `yaml_testing_framework-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/main/__init__.py` & `yaml_testing_framework-0.0.4/main/__init__.py`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/main/app.py` & `yaml_testing_framework-0.0.4/main/app.py`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/main/plugin.py` & `yaml_testing_framework-0.0.4/main/plugin.py`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/pyproject.toml` & `yaml_testing_framework-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/setup.py` & `yaml_testing_framework-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `yaml_testing_framework-0.0.3/yaml_testing_framework.egg-info/PKG-INFO` & `yaml_testing_framework-0.0.4/yaml_testing_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-testing-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: A testing framework where tests are defined in YAML files
 Home-page: https://github.com/fjemi/yaml-testing-framework
 Author: Olufemi Jemilohun
 Author-email: olufemi.jemilohun@gmail.com
 License: MIT license
 Keywords: pytest,yaml,testing
 Classifier: Framework :: Pytest
```


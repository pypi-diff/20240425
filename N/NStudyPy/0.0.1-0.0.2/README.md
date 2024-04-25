# Comparing `tmp/nstudypy-0.0.1.tar.gz` & `tmp/nstudypy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstudypy-0.0.1.tar", last modified: Thu Apr 25 01:51:13 2024, max compression
+gzip compressed data, was "nstudypy-0.0.2.tar", last modified: Thu Apr 25 02:55:57 2024, max compression
```

## Comparing `nstudypy-0.0.1.tar` & `nstudypy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:51:13.738857 nstudypy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 01:51:05.000000 nstudypy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 01:51:13.738857 nstudypy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 01:51:05.000000 nstudypy-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 01:51:05.000000 nstudypy-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:51:05.000000 nstudypy-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:51:13.738857 nstudypy-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:51:13.738857 nstudypy-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:51:13.738857 nstudypy-0.0.1/src/NstudyPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 01:51:13.000000 nstudypy-0.0.1/src/NstudyPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-25 01:51:13.000000 nstudypy-0.0.1/src/NstudyPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:51:13.000000 nstudypy-0.0.1/src/NstudyPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 01:51:13.000000 nstudypy-0.0.1/src/NstudyPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 01:51:05.000000 nstudypy-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 01:51:05.000000 nstudypy-0.0.1/src/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.672266 nstudypy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 02:55:48.000000 nstudypy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 02:55:57.672266 nstudypy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 02:55:48.000000 nstudypy-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 02:55:48.000000 nstudypy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:48.000000 nstudypy-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:55:57.672266 nstudypy-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.668266 nstudypy-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.672266 nstudypy-0.0.2/src/NstudyPy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 02:55:48.000000 nstudypy-0.0.2/src/NstudyPy/PyTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 02:55:48.000000 nstudypy-0.0.2/src/NstudyPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:55:57.672266 nstudypy-0.0.2/src/NstudyPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 02:55:57.000000 nstudypy-0.0.2/src/NstudyPy.egg-info/top_level.txt
```

### Comparing `nstudypy-0.0.1/LICENSE` & `nstudypy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nstudypy-0.0.1/PKG-INFO` & `nstudypy-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: NstudyPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A NstudyPy useful tools
 Author-email: Jack Li <lizhq08@gmail.com>
 Project-URL: Homepage, https://nstudy.org
 Project-URL: Bug Tracker, https://github.com/lizhq/NstudyPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NstudyPy
 NstudyPy工具包
 
+
+## 使用方法
+```bash
+pip install NstudyPy -i https://pypi.org/simple
+```
+
 ## 版本更新历史
 
 ## version 0.0.1
 - 初始化项目
+
+## version 0.0.2
+- 添加一些方法 `from NstudyPy import PyTools`
```

### Comparing `nstudypy-0.0.1/pyproject.toml` & `nstudypy-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.dynamic]
-version = {attr = "src.__version__"}
+version = {attr = "src.NstudyPy.__version__"}
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 "Homepage" = "https://nstudy.org"
 "Bug Tracker" = "https://github.com/lizhq/NstudyPy/issues"
```

### Comparing `nstudypy-0.0.1/src/NstudyPy.egg-info/PKG-INFO` & `nstudypy-0.0.2/src/NstudyPy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: NstudyPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A NstudyPy useful tools
 Author-email: Jack Li <lizhq08@gmail.com>
 Project-URL: Homepage, https://nstudy.org
 Project-URL: Bug Tracker, https://github.com/lizhq/NstudyPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NstudyPy
 NstudyPy工具包
 
+
+## 使用方法
+```bash
+pip install NstudyPy -i https://pypi.org/simple
+```
+
 ## 版本更新历史
 
 ## version 0.0.1
 - 初始化项目
+
+## version 0.0.2
+- 添加一些方法 `from NstudyPy import PyTools`
```


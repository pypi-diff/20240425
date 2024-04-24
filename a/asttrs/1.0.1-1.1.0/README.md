# Comparing `tmp/asttrs-1.0.1.tar.gz` & `tmp/asttrs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asttrs-1.0.1.tar", last modified: Tue Apr 23 16:38:07 2024, max compression
+gzip compressed data, was "asttrs-1.1.0.tar", last modified: Wed Apr 24 23:02:22 2024, max compression
```

## Comparing `asttrs-1.0.1.tar` & `asttrs-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1062 2021-09-26 15:04:09.000000 asttrs-1.0.1/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-23 16:38:07.018184 asttrs-1.0.1/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2547 2023-12-23 20:09:41.000000 asttrs-1.0.1/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      546 2024-04-23 16:37:52.000000 asttrs-1.0.1/pyproject.toml
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2024-04-23 16:38:07.018184 asttrs-1.0.1/setup.cfg
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.006183 asttrs-1.0.1/src/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/src/asttrs/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       28 2022-04-04 10:33:54.000000 asttrs-1.0.1/src/asttrs/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1892 2024-04-23 16:30:14.000000 asttrs-1.0.1/src/asttrs/_ast.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5719 2023-12-31 14:22:25.000000 asttrs-1.0.1/src/asttrs/_base.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    53618 2023-12-23 17:33:56.000000 asttrs-1.0.1/src/asttrs/_py3_10.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    56914 2024-04-23 16:24:32.000000 asttrs-1.0.1/src/asttrs/_py3_11.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    60807 2023-12-23 19:24:22.000000 asttrs-1.0.1/src/asttrs/_py3_12.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-12-23 17:28:57.000000 asttrs-1.0.1/src/asttrs/_py3_7.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9314 2023-12-23 17:29:36.000000 asttrs-1.0.1/src/asttrs/_py3_8.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    41099 2023-12-23 17:30:42.000000 asttrs-1.0.1/src/asttrs/_py3_9.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      857 2023-12-27 04:28:14.000000 asttrs-1.0.1/src/asttrs/utils.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/src/asttrs.egg-info/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      512 2024-04-23 16:38:07.000000 asttrs-1.0.1/src/asttrs.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        7 2024-04-23 16:38:06.000000 asttrs-1.0.1/src/asttrs.egg-info/top_level.txt
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-23 16:38:07.018184 asttrs-1.0.1/tests/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:53:28.000000 asttrs-1.0.1/tests/test_expr.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1266 2022-04-04 12:18:55.000000 asttrs-1.0.1/tests/test_misc.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 17:08:43.000000 asttrs-1.0.1/tests/test_operator.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:54:10.000000 asttrs-1.0.1/tests/test_stmt.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      420 2023-12-23 18:31:52.000000 asttrs-1.0.1/tests/test_utils.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1062 2021-09-26 15:04:09.000000 asttrs-1.1.0/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-24 23:02:22.837069 asttrs-1.1.0/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2547 2023-12-23 20:09:41.000000 asttrs-1.1.0/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      546 2024-04-24 23:01:45.000000 asttrs-1.1.0/pyproject.toml
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2024-04-24 23:02:22.837069 asttrs-1.1.0/setup.cfg
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.833069 asttrs-1.1.0/src/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/src/asttrs/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       28 2022-04-04 10:33:54.000000 asttrs-1.1.0/src/asttrs/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1892 2024-04-23 16:30:14.000000 asttrs-1.1.0/src/asttrs/_ast.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5719 2023-12-31 14:22:25.000000 asttrs-1.1.0/src/asttrs/_base.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    53618 2023-12-23 17:33:56.000000 asttrs-1.1.0/src/asttrs/_py3_10.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    56914 2024-04-23 16:24:32.000000 asttrs-1.1.0/src/asttrs/_py3_11.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    60807 2024-04-24 23:00:08.000000 asttrs-1.1.0/src/asttrs/_py3_12.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-12-23 17:28:57.000000 asttrs-1.1.0/src/asttrs/_py3_7.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9314 2023-12-23 17:29:36.000000 asttrs-1.1.0/src/asttrs/_py3_8.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    41099 2023-12-23 17:30:42.000000 asttrs-1.1.0/src/asttrs/_py3_9.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      857 2023-12-27 04:28:14.000000 asttrs-1.1.0/src/asttrs/utils.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/src/asttrs.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      512 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        7 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:53:28.000000 asttrs-1.1.0/tests/test_expr.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1266 2022-04-04 12:18:55.000000 asttrs-1.1.0/tests/test_misc.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 17:08:43.000000 asttrs-1.1.0/tests/test_operator.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:54:10.000000 asttrs-1.1.0/tests/test_stmt.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      420 2023-12-23 18:31:52.000000 asttrs-1.1.0/tests/test_utils.py
```

### Comparing `asttrs-1.0.1/LICENSE` & `asttrs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/PKG-INFO` & `asttrs-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asttrs
-Version: 1.0.1
+Version: 1.1.0
 Summary: A attrs-style wrapper for python ast
 Author-email: ryanchao2012 <ryanchao2012@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/ryanchao2012/asttrs
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `asttrs-1.0.1/README.md` & `asttrs-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/pyproject.toml` & `asttrs-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "asttrs"
-version = "1.0.1"
+version = "1.1.0"
 description = "A attrs-style wrapper for python ast"
 authors = [
     {name = "ryanchao2012", email = "ryanchao2012@gmail.com"},
 ]
 urls = {repository = "https://github.com/ryanchao2012/asttrs"}
 license = {text = "MIT"}
 readme = "README.md"
```

### Comparing `asttrs-1.0.1/src/asttrs/_ast.py` & `asttrs-1.1.0/src/asttrs/_ast.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_base.py` & `asttrs-1.1.0/src/asttrs/_base.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_py3_10.py` & `asttrs-1.1.0/src/asttrs/_py3_10.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_py3_11.py` & `asttrs-1.1.0/src/asttrs/_py3_11.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_py3_12.py` & `asttrs-1.1.0/src/asttrs/_py3_12.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_py3_7.py` & `asttrs-1.1.0/src/asttrs/_py3_7.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_py3_8.py` & `asttrs-1.1.0/src/asttrs/_py3_8.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/_py3_9.py` & `asttrs-1.1.0/src/asttrs/_py3_9.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs/utils.py` & `asttrs-1.1.0/src/asttrs/utils.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/src/asttrs.egg-info/PKG-INFO` & `asttrs-1.1.0/src/asttrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asttrs
-Version: 1.0.1
+Version: 1.1.0
 Summary: A attrs-style wrapper for python ast
 Author-email: ryanchao2012 <ryanchao2012@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/ryanchao2012/asttrs
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `asttrs-1.0.1/src/asttrs.egg-info/SOURCES.txt` & `asttrs-1.1.0/src/asttrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asttrs-1.0.1/tests/test_misc.py` & `asttrs-1.1.0/tests/test_misc.py`

 * *Files identical despite different names*


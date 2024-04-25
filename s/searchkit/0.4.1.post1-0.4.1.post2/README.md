# Comparing `tmp/searchkit-0.4.1.post1.tar.gz` & `tmp/searchkit-0.4.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.4.1.post1.tar", last modified: Sun Apr 21 17:08:29 2024, max compression
+gzip compressed data, was "searchkit-0.4.1.post2.tar", last modified: Thu Apr 25 16:34:39 2024, max compression
```

## Comparing `searchkit-0.4.1.post1.tar` & `searchkit-0.4.1.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    11357 2023-01-26 18:19:39.000000 searchkit-0.4.1.post1/LICENSE
--rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4503 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4205 2023-05-24 17:19:57.000000 searchkit-0.4.1.post1/README.md
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      734 2023-05-13 07:02:21.000000 searchkit-0.4.1.post1/pyproject.toml
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.870326 searchkit-0.4.1.post1/searchkit/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      121 2023-05-13 07:02:21.000000 searchkit-0.4.1.post1/searchkit/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    36146 2024-04-21 15:19:37.000000 searchkit-0.4.1.post1/searchkit/constraints.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      503 2023-12-15 20:01:02.000000 searchkit-0.4.1.post1/searchkit/log.py
--rwxrwxr-x   0 gizmo     (1000) gizmo     (1000)    51527 2024-04-21 15:27:10.000000 searchkit-0.4.1.post1/searchkit/search.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4053 2023-12-15 20:01:02.000000 searchkit-0.4.1.post1/searchkit/utils.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/searchkit.egg-info/
--rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4503 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      468 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       57 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/requires.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       21 2024-04-21 17:08:29.000000 searchkit-0.4.1.post1/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       76 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/setup.cfg
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       54 2023-01-29 21:19:04.000000 searchkit-0.4.1.post1/setup.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/tests/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-01-26 18:19:39.000000 searchkit-0.4.1.post1/tests/__init__.py
-drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-04-21 17:08:29.874326 searchkit-0.4.1.post1/tests/unit/
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-01-26 18:19:39.000000 searchkit-0.4.1.post1/tests/unit/__init__.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    38115 2024-04-21 15:27:31.000000 searchkit-0.4.1.post1/tests/unit/test_search.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    32883 2023-12-15 20:01:02.000000 searchkit-0.4.1.post1/tests/unit/test_search_constraints.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      871 2023-09-24 18:41:22.000000 searchkit-0.4.1.post1/tests/unit/test_utils.py
--rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1319 2023-09-16 14:38:19.000000 searchkit-0.4.1.post1/tests/unit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.4.1.post2/LICENSE
+-rw-r--r--   0 user1     (1000) user1     (1000)     4503 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.4.1.post2/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-31 12:54:07.000000 searchkit-0.4.1.post2/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-31 12:54:07.000000 searchkit-0.4.1.post2/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    36146 2024-04-22 09:54:35.000000 searchkit-0.4.1.post2/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      491 2024-04-25 16:30:45.000000 searchkit-0.4.1.post2/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    51527 2024-04-22 09:54:35.000000 searchkit-0.4.1.post2/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4053 2023-12-15 13:29:03.000000 searchkit-0.4.1.post2/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/searchkit.egg-info/
+-rw-r--r--   0 user1     (1000) user1     (1000)     4503 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      468 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       21 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       76 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.4.1.post2/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/tests/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.4.1.post2/tests/__init__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/tests/unit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.4.1.post2/tests/unit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    38115 2024-04-22 09:54:35.000000 searchkit-0.4.1.post2/tests/unit/test_search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    32883 2023-12-15 13:30:40.000000 searchkit-0.4.1.post2/tests/unit/test_search_constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      871 2023-09-20 12:14:30.000000 searchkit-0.4.1.post2/tests/unit/test_utils.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1319 2023-09-13 12:24:12.000000 searchkit-0.4.1.post2/tests/unit/utils.py
```

### Comparing `searchkit-0.4.1.post1/LICENSE` & `searchkit-0.4.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/PKG-INFO` & `searchkit-0.4.1.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.4.1.post1
+Version: 0.4.1.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: fasteners
```

### Comparing `searchkit-0.4.1.post1/README.md` & `searchkit-0.4.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/pyproject.toml` & `searchkit-0.4.1.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/searchkit/constraints.py` & `searchkit-0.4.1.post2/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/searchkit/search.py` & `searchkit-0.4.1.post2/searchkit/search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/searchkit/utils.py` & `searchkit-0.4.1.post2/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/searchkit.egg-info/PKG-INFO` & `searchkit-0.4.1.post2/searchkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.4.1.post1
+Version: 0.4.1.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: fasteners
```

### Comparing `searchkit-0.4.1.post1/tests/unit/test_search.py` & `searchkit-0.4.1.post2/tests/unit/test_search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/tests/unit/test_search_constraints.py` & `searchkit-0.4.1.post2/tests/unit/test_search_constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/tests/unit/test_utils.py` & `searchkit-0.4.1.post2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post1/tests/unit/utils.py` & `searchkit-0.4.1.post2/tests/unit/utils.py`

 * *Files identical despite different names*


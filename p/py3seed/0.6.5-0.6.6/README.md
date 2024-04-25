# Comparing `tmp/py3seed-0.6.5.tar.gz` & `tmp/py3seed-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.6.5.tar", last modified: Wed Apr 24 07:30:34 2024, max compression
+gzip compressed data, was "py3seed-0.6.6.tar", last modified: Thu Apr 25 01:05:24 2024, max compression
```

## Comparing `py3seed-0.6.5.tar` & `py3seed-0.6.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.705231 py3seed-0.6.5/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.6.5/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2024-04-24 07:30:34.705000 py3seed-0.6.5/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.6.5/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.6.5/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      925 2024-04-24 07:30:34.706529 py3seed-0.6.5/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.6.5/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.675482 py3seed-0.6.5/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.691149 py3seed-0.6.5/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2023-08-15 08:24:22.000000 py3seed-0.6.5/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.6.5/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.6.5/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     8285 2023-12-08 02:46:38.000000 py3seed-0.6.5/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.696456 py3seed-0.6.5/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.6.5/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    26101 2024-04-24 03:39:28.000000 py3seed-0.6.5/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.6.5/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4272 2023-08-11 02:16:21.000000 py3seed-0.6.5/src/py3seed/ext.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.6.5/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.6.5/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.6.5/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    58526 2023-12-14 02:44:15.000000 py3seed-0.6.5/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14779 2023-12-08 02:47:42.000000 py3seed-0.6.5/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    15254 2024-04-24 03:35:30.000000 py3seed-0.6.5/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    10098 2023-12-07 08:30:01.000000 py3seed-0.6.5/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.704178 py3seed-0.6.5/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       59 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.703146 py3seed-0.6.5/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4386 2023-12-06 02:47:57.000000 py3seed-0.6.5/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7430 2024-04-24 07:26:40.000000 py3seed-0.6.5/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.6.5/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5286 2023-08-09 06:44:01.000000 py3seed-0.6.5/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2080 2023-12-08 02:08:48.000000 py3seed-0.6.5/tests/test_mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2504 2023-12-07 08:27:56.000000 py3seed-0.6.5/tests/test_websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-25 01:05:24.980117 py3seed-0.6.6/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.6.6/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2024-04-25 01:05:24.979934 py3seed-0.6.6/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.6.6/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.6.6/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      925 2024-04-25 01:05:24.980878 py3seed-0.6.6/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.6.6/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-25 01:05:24.956466 py3seed-0.6.6/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-25 01:05:24.971504 py3seed-0.6.6/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2023-08-15 08:24:22.000000 py3seed-0.6.6/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.6.6/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.6.6/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     8285 2023-12-08 02:46:38.000000 py3seed-0.6.6/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-25 01:05:24.975015 py3seed-0.6.6/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.6.6/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    26031 2024-04-25 01:04:25.000000 py3seed-0.6.6/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.6.6/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4272 2023-08-11 02:16:21.000000 py3seed-0.6.6/src/py3seed/ext.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.6.6/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.6.6/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.6.6/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    58526 2023-12-14 02:44:15.000000 py3seed-0.6.6/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14779 2023-12-08 02:47:42.000000 py3seed-0.6.6/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    15254 2024-04-24 03:35:30.000000 py3seed-0.6.6/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    10098 2023-12-07 08:30:01.000000 py3seed-0.6.6/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-25 01:05:24.979457 py3seed-0.6.6/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2024-04-25 01:05:24.000000 py3seed-0.6.6/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2024-04-25 01:05:24.000000 py3seed-0.6.6/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2024-04-25 01:05:24.000000 py3seed-0.6.6/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2024-04-25 01:05:24.000000 py3seed-0.6.6/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       59 2024-04-25 01:05:24.000000 py3seed-0.6.6/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2024-04-25 01:05:24.000000 py3seed-0.6.6/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-25 01:05:24.978692 py3seed-0.6.6/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4386 2023-12-06 02:47:57.000000 py3seed-0.6.6/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7430 2024-04-24 07:26:40.000000 py3seed-0.6.6/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.6.6/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5286 2023-08-09 06:44:01.000000 py3seed-0.6.6/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2080 2023-12-08 02:08:48.000000 py3seed-0.6.6/tests/test_mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2504 2023-12-07 08:27:56.000000 py3seed-0.6.6/tests/test_websupport.py
```

### Comparing `py3seed-0.6.5/LICENSE` & `py3seed-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/PKG-INFO` & `py3seed-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.6.5/setup.cfg` & `py3seed-0.6.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.6.5
+version = 0.6.6
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.6.5/src/py3seed/__init__.py` & `py3seed-0.6.6/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/__main__.py` & `py3seed-0.6.6/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/admin.py` & `py3seed-0.6.6/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/cachesupport.py` & `py3seed-0.6.6/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/commands/gen.py` & `py3seed-0.6.6/src/py3seed/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,19 +531,19 @@
                 # user-profile.html.0 exists, always generate code to user-profile.html.0, then you need to merge manually
                 #
                 # - Output name with additional suffix .1:
                 # Using BASE, THIS and OTHER to perform a 3-way merge
                 # e.g,
                 # user-profile.html.1 exists, coping user-profile.html.1 to user-profile.html.BASE and user-profile.html to user-profile.html.THIS, generating user-profile.html.OTHER, then perform 3-way merge to user-profile.html
                 #
-                o_file_0 = o_name.replace('.jinja2', '.0')
-                o_file_1 = o_name.replace('.jinja2', '.1')
-                o_file_base = o_name.replace('.jinja2', '.BASE')
-                o_file_this = o_name.replace('.jinja2', '.THIS')
-                o_file_other = o_name.replace('.jinja2', '.OTHER')
+                o_file_0 = o_file_raw + '.0'
+                o_file_1 = o_file_raw + '.1'
+                o_file_base = o_file_raw + '.BASE'
+                o_file_this = o_file_raw + '.THIS'
+                o_file_other = o_file_raw + '.OTHER'
                 if os.path.exists(o_file_0):
                     o_file = o_file_0
                 elif os.path.exists(o_file_1):
                     # After manually merge, need to remove BASE/THIS/OTHER files mannually
                     if os.path.exists(o_file_other):
                         msg = f'Please solve last merging conflicts of {o_file_raw}'
                         context['result']['warnings'] += [msg]
```

### Comparing `py3seed-0.6.5/src/py3seed/error.py` & `py3seed-0.6.6/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/ext.py` & `py3seed-0.6.6/src/py3seed/ext.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/inflection.py` & `py3seed-0.6.6/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/log.py` & `py3seed-0.6.6/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/merge3.py` & `py3seed-0.6.6/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/model.py` & `py3seed-0.6.6/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/mongosupport.py` & `py3seed-0.6.6/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/utils.py` & `py3seed-0.6.6/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed/websupport.py` & `py3seed-0.6.6/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.6.6/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.6.5/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.6.6/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/tests/test_cachesupport.py` & `py3seed-0.6.6/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/tests/test_gen.py` & `py3seed-0.6.6/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/tests/test_merge3.py` & `py3seed-0.6.6/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/tests/test_model.py` & `py3seed-0.6.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/tests/test_mongosupport.py` & `py3seed-0.6.6/tests/test_mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.5/tests/test_websupport.py` & `py3seed-0.6.6/tests/test_websupport.py`

 * *Files identical despite different names*


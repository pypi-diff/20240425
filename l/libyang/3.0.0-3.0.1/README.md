# Comparing `tmp/libyang-3.0.0.tar.gz` & `tmp/libyang-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libyang-3.0.0.tar", last modified: Sat Apr  6 10:11:49 2024, max compression
+gzip compressed data, was "libyang-3.0.1.tar", last modified: Thu Apr 25 09:44:48 2024, max compression
```

## Comparing `libyang-3.0.0.tar` & `libyang-3.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-06 10:11:36.000000 libyang-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2024-04-06 10:11:36.000000 libyang-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11559 2024-04-06 10:11:49.907022 libyang-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10916 2024-04-06 10:11:36.000000 libyang-3.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.903022 libyang-3.0.0/cffi/
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-06 10:11:36.000000 libyang-3.0.0/cffi/build.py
--rw-r--r--   0 root         (0) root         (0)    29004 2024-04-06 10:11:36.000000 libyang-3.0.0/cffi/cdefs.h
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-06 10:11:36.000000 libyang-3.0.0/cffi/source.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/libyang/
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-06 10:11:49.907022 libyang-3.0.0/libyang/VERSION
--rw-r--r--   0 root         (0) root         (0)     3314 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15234 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/context.py
--rw-r--r--   0 root         (0) root         (0)    45877 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/data.py
--rw-r--r--   0 root         (0) root         (0)    13429 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/diff.py
--rw-r--r--   0 root         (0) root         (0)     5749 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/keyed_list.py
--rw-r--r--   0 root         (0) root         (0)     2104 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/log.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/py.typed
--rw-r--r--   0 root         (0) root         (0)    54753 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/schema.py
--rw-r--r--   0 root         (0) root         (0)     3640 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/util.py
--rw-r--r--   0 root         (0) root         (0)    18831 2024-04-06 10:11:36.000000 libyang-3.0.0/libyang/xpath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/libyang.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11559 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      590 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-06 10:11:49.000000 libyang-3.0.0/libyang.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      289 2024-04-06 10:11:36.000000 libyang-3.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      713 2024-04-06 10:11:49.907022 libyang-3.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5815 2024-04-06 10:11:36.000000 libyang-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:11:49.907022 libyang-3.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4067 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_context.py
--rw-r--r--   0 root         (0) root         (0)    31724 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_data.py
--rw-r--r--   0 root         (0) root         (0)     4499 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_diff.py
--rw-r--r--   0 root         (0) root         (0)     3547 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_keyedlist.py
--rw-r--r--   0 root         (0) root         (0)    22411 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_schema.py
--rw-r--r--   0 root         (0) root         (0)    15307 2024-04-06 10:11:36.000000 libyang-3.0.0/tests/test_xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:44:48.885374 libyang-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-25 09:44:35.000000 libyang-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2024-04-25 09:44:35.000000 libyang-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11559 2024-04-25 09:44:48.885374 libyang-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10916 2024-04-25 09:44:35.000000 libyang-3.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:44:48.881374 libyang-3.0.1/cffi/
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-25 09:44:35.000000 libyang-3.0.1/cffi/build.py
+-rw-r--r--   0 root         (0) root         (0)    29028 2024-04-25 09:44:35.000000 libyang-3.0.1/cffi/cdefs.h
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-25 09:44:35.000000 libyang-3.0.1/cffi/source.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:44:48.885374 libyang-3.0.1/libyang/
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-25 09:44:48.885374 libyang-3.0.1/libyang/VERSION
+-rw-r--r--   0 root         (0) root         (0)     3314 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15234 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/context.py
+-rw-r--r--   0 root         (0) root         (0)    45877 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/data.py
+-rw-r--r--   0 root         (0) root         (0)    13429 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/diff.py
+-rw-r--r--   0 root         (0) root         (0)     5749 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/keyed_list.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/log.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/py.typed
+-rw-r--r--   0 root         (0) root         (0)    54753 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/util.py
+-rw-r--r--   0 root         (0) root         (0)    18831 2024-04-25 09:44:35.000000 libyang-3.0.1/libyang/xpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:44:48.885374 libyang-3.0.1/libyang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11559 2024-04-25 09:44:48.000000 libyang-3.0.1/libyang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2024-04-25 09:44:48.000000 libyang-3.0.1/libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 09:44:48.000000 libyang-3.0.1/libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 09:44:48.000000 libyang-3.0.1/libyang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-25 09:44:48.000000 libyang-3.0.1/libyang.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-25 09:44:48.000000 libyang-3.0.1/libyang.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2024-04-25 09:44:35.000000 libyang-3.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-25 09:44:48.885374 libyang-3.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5815 2024-04-25 09:44:35.000000 libyang-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:44:48.885374 libyang-3.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     4067 2024-04-25 09:44:35.000000 libyang-3.0.1/tests/test_context.py
+-rw-r--r--   0 root         (0) root         (0)    31724 2024-04-25 09:44:35.000000 libyang-3.0.1/tests/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2024-04-25 09:44:35.000000 libyang-3.0.1/tests/test_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-04-25 09:44:35.000000 libyang-3.0.1/tests/test_keyedlist.py
+-rw-r--r--   0 root         (0) root         (0)    22411 2024-04-25 09:44:35.000000 libyang-3.0.1/tests/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15307 2024-04-25 09:44:35.000000 libyang-3.0.1/tests/test_xpath.py
```

### Comparing `libyang-3.0.0/LICENSE` & `libyang-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/PKG-INFO` & `libyang-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 3.0.0
+Version: 3.0.1
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `libyang-3.0.0/README.rst` & `libyang-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/cffi/build.py` & `libyang-3.0.1/cffi/build.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/cffi/cdefs.h` & `libyang-3.0.1/cffi/cdefs.h`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
 #define LY_LOLOG ...
 #define LY_LOSTORE ...
 #define LY_LOSTORE_LAST ...
 int ly_log_options(int);
 
 LY_LOG_LEVEL ly_log_level(LY_LOG_LEVEL);
-extern "Python" void lypy_log_cb(LY_LOG_LEVEL, const char *, const char *);
+extern "Python" void lypy_log_cb(LY_LOG_LEVEL, const char *, const char *, const char *, uint64_t);
 void ly_set_log_clb(void (*)(LY_LOG_LEVEL, const char *, const char *, const char *, uint64_t));
 const struct ly_err_item *ly_err_first(const struct ly_ctx *);
 const struct ly_err_item *ly_err_last(const struct ly_ctx *);
 void ly_err_clean(struct ly_ctx *, struct ly_err_item *);
 
 #define LYS_UNKNOWN ...
 #define LYS_CONTAINER ...
```

### Comparing `libyang-3.0.0/libyang/__init__.py` & `libyang-3.0.1/libyang/__init__.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/context.py` & `libyang-3.0.1/libyang/context.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/data.py` & `libyang-3.0.1/libyang/data.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/diff.py` & `libyang-3.0.1/libyang/diff.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/keyed_list.py` & `libyang-3.0.1/libyang/keyed_list.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/log.py` & `libyang-3.0.1/libyang/log.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/schema.py` & `libyang-3.0.1/libyang/schema.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/util.py` & `libyang-3.0.1/libyang/util.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang/xpath.py` & `libyang-3.0.1/libyang/xpath.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/libyang.egg-info/PKG-INFO` & `libyang-3.0.1/libyang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libyang
-Version: 3.0.0
+Version: 3.0.1
 Summary: CFFI bindings to libyang
 Home-page: https://github.com/CESNET/libyang-python
 Author: Robin Jarry
 Author-email: robin@jarry.cc
 License: MIT
 Keywords: libyang,cffi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `libyang-3.0.0/libyang.egg-info/SOURCES.txt` & `libyang-3.0.1/libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/setup.cfg` & `libyang-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/setup.py` & `libyang-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/tests/test_context.py` & `libyang-3.0.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/tests/test_data.py` & `libyang-3.0.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/tests/test_diff.py` & `libyang-3.0.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/tests/test_keyedlist.py` & `libyang-3.0.1/tests/test_keyedlist.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/tests/test_schema.py` & `libyang-3.0.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `libyang-3.0.0/tests/test_xpath.py` & `libyang-3.0.1/tests/test_xpath.py`

 * *Files identical despite different names*


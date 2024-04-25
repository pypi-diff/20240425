# Comparing `tmp/func_adl-3.3.0.tar.gz` & `tmp/func_adl-3.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/func_adl-3.3.0.tar", last modified: Thu Apr 25 00:51:17 2024, max compression
+gzip compressed data, was "dist/func_adl-3.3.1b1.tar", last modified: Thu Apr 25 08:00:51 2024, max compression
```

## Comparing `func_adl-3.3.0.tar` & `func_adl-3.3.1b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-25 00:51:17.000000 func_adl-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-25 00:51:09.000000 func_adl-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl/ast/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/aggregate_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/ast_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/call_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/func_adl_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/function_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/syntatic_sugar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/object_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    35421 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/util_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/util_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 00:51:09.000000 func_adl-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:51:17.000000 func_adl-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-25 00:51:09.000000 func_adl-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_object_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    30055 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_type_based_replacement_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_util_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/aggregate_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/ast_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/call_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/func_adl_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/function_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/ast/syntatic_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35421 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/func_adl/util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/func_adl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:00:51.000000 func_adl-3.3.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/tests/test_event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/tests/test_object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30055 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/tests/test_type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/tests/test_type_based_replacement_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/tests/test_util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-25 08:00:47.000000 func_adl-3.3.1b1/tests/test_util_types.py
```

### Comparing `func_adl-3.3.0/PKG-INFO` & `func_adl-3.3.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_adl
-Version: 3.3.0
+Version: 3.3.1b1
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: MIT
```

### Comparing `func_adl-3.3.0/README.md` & `func_adl-3.3.1b1/README.md`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/ast/aggregate_shortcuts.py` & `func_adl-3.3.1b1/func_adl/ast/aggregate_shortcuts.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/ast/call_stack.py` & `func_adl-3.3.1b1/func_adl/ast/call_stack.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/ast/func_adl_ast_utils.py` & `func_adl-3.3.1b1/func_adl/ast/func_adl_ast_utils.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/ast/function_simplifier.py` & `func_adl-3.3.1b1/func_adl/ast/function_simplifier.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/ast/meta_data.py` & `func_adl-3.3.1b1/func_adl/ast/meta_data.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/ast/syntatic_sugar.py` & `func_adl-3.3.1b1/func_adl/ast/syntatic_sugar.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/event_dataset.py` & `func_adl-3.3.1b1/func_adl/event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/functions.py` & `func_adl-3.3.1b1/func_adl/functions.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/object_stream.py` & `func_adl-3.3.1b1/func_adl/object_stream.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/type_based_replacement.py` & `func_adl-3.3.1b1/func_adl/type_based_replacement.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/util_ast.py` & `func_adl-3.3.1b1/func_adl/util_ast.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl/util_types.py` & `func_adl-3.3.1b1/func_adl/util_types.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/func_adl.egg-info/PKG-INFO` & `func_adl-3.3.1b1/func_adl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-adl
-Version: 3.3.0
+Version: 3.3.1b1
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: MIT
```

### Comparing `func_adl-3.3.0/func_adl.egg-info/SOURCES.txt` & `func_adl-3.3.1b1/func_adl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/setup.py` & `func_adl-3.3.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/tests/test_event_dataset.py` & `func_adl-3.3.1b1/tests/test_event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/tests/test_object_stream.py` & `func_adl-3.3.1b1/tests/test_object_stream.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/tests/test_type_based_replacement.py` & `func_adl-3.3.1b1/tests/test_type_based_replacement.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/tests/test_type_based_replacement_py310.py` & `func_adl-3.3.1b1/tests/test_type_based_replacement_py310.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/tests/test_util_ast.py` & `func_adl-3.3.1b1/tests/test_util_ast.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.3.0/tests/test_util_types.py` & `func_adl-3.3.1b1/tests/test_util_types.py`

 * *Files identical despite different names*


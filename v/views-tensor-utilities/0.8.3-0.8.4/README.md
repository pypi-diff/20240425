# Comparing `tmp/views_tensor_utilities-0.8.3.tar.gz` & `tmp/views_tensor_utilities-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "views_tensor_utilities-0.8.3.tar", max compression
+gzip compressed data, was "views_tensor_utilities-0.8.4.tar", max compression
```

## Comparing `views_tensor_utilities-0.8.3.tar` & `views_tensor_utilities-0.8.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.3/README.md
--rw-r--r--   0        0        0      456 2024-04-24 10:52:26.557174 views_tensor_utilities-0.8.3/pyproject.toml
--rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.3/views_tensor_utilities/__init__.py
--rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.3/views_tensor_utilities/defaults.py
--rw-r--r--   0        0        0    17398 2024-04-24 10:51:50.787789 views_tensor_utilities-0.8.3/views_tensor_utilities/mappings.py
--rw-r--r--   0        0        0    11099 2024-04-23 11:49:43.048800 views_tensor_utilities-0.8.3/views_tensor_utilities/objects.py
--rw-r--r--   0        0        0     8754 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     8303 2024-03-04 12:04:18.486295 views_tensor_utilities-0.8.4/README.md
+-rw-r--r--   0        0        0      456 2024-04-25 12:56:24.092953 views_tensor_utilities-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-02-23 12:07:30.835277 views_tensor_utilities-0.8.4/views_tensor_utilities/__init__.py
+-rw-r--r--   0        0        0      406 2024-03-06 13:40:55.851241 views_tensor_utilities-0.8.4/views_tensor_utilities/defaults.py
+-rw-r--r--   0        0        0    17552 2024-04-25 11:54:29.257148 views_tensor_utilities-0.8.4/views_tensor_utilities/mappings.py
+-rw-r--r--   0        0        0    11099 2024-04-23 11:49:43.048800 views_tensor_utilities-0.8.4/views_tensor_utilities/objects.py
+-rw-r--r--   0        0        0     8754 1970-01-01 00:00:00.000000 views_tensor_utilities-0.8.4/PKG-INFO
```

### Comparing `views_tensor_utilities-0.8.3/README.md` & `views_tensor_utilities-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.3/views_tensor_utilities/mappings.py` & `views_tensor_utilities-0.8.4/views_tensor_utilities/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,16 @@
     Obtain correct does-not-exist token based on data type of input dataframe
     """
 
     dtype = __check_df_data_types(df)
 
     if dtype in defaults.allowed_float_types:
         return defaults.fdne
+    elif dtype in defaults.allowed_int_types:
+        return defaults.fdne
     else:
         max_str_length = -1
         for column in df.columns:
             if df[column].dtype in defaults.allowed_string_types:
                 max_str_length = np.max([max_str_length, len(max(df[column].values, key=len))])
 
         return max_str_length*defaults.sdne
@@ -344,14 +346,16 @@
     Obtain correct missing token based on data type of input dataframe
     """
 
     dtype = __check_df_data_types(df)
 
     if dtype in defaults.allowed_float_types:
         return defaults.fmissing
+    elif dtype in defaults.allowed_int_types:
+        return defaults.fmissing
     else:
         return defaults.smissing
 
 
 def __get_dtype(df):
     """
     get_dtype
```

### Comparing `views_tensor_utilities-0.8.3/views_tensor_utilities/objects.py` & `views_tensor_utilities-0.8.4/views_tensor_utilities/objects.py`

 * *Files identical despite different names*

### Comparing `views_tensor_utilities-0.8.3/PKG-INFO` & `views_tensor_utilities-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: views-tensor-utilities
-Version: 0.8.3
+Version: 0.8.4
 Summary: Classes and functions for transforming between VIEWS-compliant dfs and tensors
 Author: jimdale
 Author-email: jimdale@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20.0)
```


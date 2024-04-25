# Comparing `tmp/funcnodes_pandas-0.1.2.tar.gz` & `tmp/funcnodes_pandas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_pandas-0.1.2.tar", max compression
+gzip compressed data, was "funcnodes_pandas-0.1.3.tar", max compression
```

## Comparing `funcnodes_pandas-0.1.2.tar` & `funcnodes_pandas-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1722 2024-04-12 11:28:49.809772 funcnodes_pandas-0.1.2/funcnodes_pandas/__init__.py
--rw-r--r--   0        0        0     9272 2024-04-12 10:54:18.814562 funcnodes_pandas-0.1.2/funcnodes_pandas/dataframe.py
--rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.2/funcnodes_pandas/dataseries.py
--rw-r--r--   0        0        0      460 2024-04-12 11:28:37.497161 funcnodes_pandas-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.2/README.md
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1722 2024-04-25 11:04:06.939574 funcnodes_pandas-0.1.3/funcnodes_pandas/__init__.py
+-rw-r--r--   0        0        0     9272 2024-04-12 10:54:18.814562 funcnodes_pandas-0.1.3/funcnodes_pandas/dataframe.py
+-rw-r--r--   0        0        0     2568 2024-03-22 12:12:52.232463 funcnodes_pandas-0.1.3/funcnodes_pandas/dataseries.py
+-rw-r--r--   0        0        0      467 2024-04-25 11:03:54.168867 funcnodes_pandas-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 16:14:38.723499 funcnodes_pandas-0.1.3/README.md
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 funcnodes_pandas-0.1.3/PKG-INFO
```

### Comparing `funcnodes_pandas-0.1.2/funcnodes_pandas/__init__.py` & `funcnodes_pandas-0.1.3/funcnodes_pandas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         type_to_string(pd.DataFrame): "table",
         type_to_string(pd.Series): "list",
     },
 }
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 __all__ = [
     "NODE_SHELF",
     "to_dict",
     "from_dict",
     "from_csv_str",
     "get_column",
```

### Comparing `funcnodes_pandas-0.1.2/funcnodes_pandas/dataframe.py` & `funcnodes_pandas-0.1.3/funcnodes_pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.2/funcnodes_pandas/dataseries.py` & `funcnodes_pandas-0.1.3/funcnodes_pandas/dataseries.py`

 * *Files identical despite different names*

### Comparing `funcnodes_pandas-0.1.2/PKG-INFO` & `funcnodes_pandas-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: funcnodes-pandas
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.30,<0.2.0)
-Requires-Dist: funcnodes-numpy (>=0.1.51,<0.2.0)
+Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
+Requires-Dist: funcnodes-numpy (>=0.1.5)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
```


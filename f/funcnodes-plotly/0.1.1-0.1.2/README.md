# Comparing `tmp/funcnodes_plotly-0.1.1.tar.gz` & `tmp/funcnodes_plotly-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_plotly-0.1.1.tar", max compression
+gzip compressed data, was "funcnodes_plotly-0.1.2.tar", max compression
```

## Comparing `funcnodes_plotly-0.1.1.tar` & `funcnodes_plotly-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1008 2024-04-25 10:10:00.331002 funcnodes_plotly-0.1.1/funcnodes_plotly/__init__.py
--rw-r--r--   0        0        0     1512 2024-04-25 10:07:50.895177 funcnodes_plotly-0.1.1/funcnodes_plotly/figure.py
--rw-r--r--   0        0        0      476 2024-04-25 07:34:34.883959 funcnodes_plotly-0.1.1/funcnodes_plotly/layout.py
--rw-r--r--   0        0        0     1628 2024-04-25 10:07:33.248130 funcnodes_plotly-0.1.1/funcnodes_plotly/plots.py
--rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.1/funcnodes_plotly/utils.py
--rw-r--r--   0        0        0      472 2024-04-25 10:12:13.570972 funcnodes_plotly-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.1/README.md
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1008 2024-04-25 11:05:47.509097 funcnodes_plotly-0.1.2/funcnodes_plotly/__init__.py
+-rw-r--r--   0        0        0     1512 2024-04-25 10:07:50.895177 funcnodes_plotly-0.1.2/funcnodes_plotly/figure.py
+-rw-r--r--   0        0        0      476 2024-04-25 07:34:34.883959 funcnodes_plotly-0.1.2/funcnodes_plotly/layout.py
+-rw-r--r--   0        0        0     1628 2024-04-25 10:07:33.248130 funcnodes_plotly-0.1.2/funcnodes_plotly/plots.py
+-rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.2/funcnodes_plotly/utils.py
+-rw-r--r--   0        0        0      480 2024-04-25 11:05:24.395224 funcnodes_plotly-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.2/README.md
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.2/PKG-INFO
```

### Comparing `funcnodes_plotly-0.1.1/funcnodes_plotly/__init__.py` & `funcnodes_plotly-0.1.2/funcnodes_plotly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
     ],
     name="Plotly",
     description="A collection of functions for creating plotly plots.",
     subshelves=[],
 )
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `funcnodes_plotly-0.1.1/funcnodes_plotly/figure.py` & `funcnodes_plotly-0.1.2/funcnodes_plotly/figure.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.1/funcnodes_plotly/plots.py` & `funcnodes_plotly-0.1.2/funcnodes_plotly/plots.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.1/funcnodes_plotly/utils.py` & `funcnodes_plotly-0.1.2/funcnodes_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.1/PKG-INFO` & `funcnodes_plotly-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: funcnodes-plotly
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/JulianKimmig/funcnodes_plotly
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
-Requires-Dist: funcnodes (>=0.1.40,<0.2.0)
+Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
 Requires-Dist: plotly (>=5.21.0,<6.0.0)
 Project-URL: Repository, https://github.com/JulianKimmig/funcnodes_plotly
 Description-Content-Type: text/markdown
```


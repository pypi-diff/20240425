# Comparing `tmp/funcnodes_images-0.1.11.tar.gz` & `tmp/funcnodes_images-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_images-0.1.11.tar", max compression
+gzip compressed data, was "funcnodes_images-0.1.12.tar", max compression
```

## Comparing `funcnodes_images-0.1.11.tar` & `funcnodes_images-0.1.12.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      949 2024-04-17 08:27:24.336400 funcnodes_images-0.1.11/funcnodes_images/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.11/funcnodes_images/_numpy.py
--rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.11/funcnodes_images/_pillow.py
--rw-r--r--   0        0        0     4971 2024-04-16 17:00:40.645038 funcnodes_images-0.1.11/funcnodes_images/image_nodes.py
--rw-r--r--   0        0        0     5156 2024-04-16 16:21:39.581875 funcnodes_images-0.1.11/funcnodes_images/imagecontainer.py
--rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.11/funcnodes_images/utils.py
--rw-r--r--   0        0        0      451 2024-04-17 08:27:18.865818 funcnodes_images-0.1.11/pyproject.toml
--rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.11/README.md
--rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 funcnodes_images-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0     1023 2024-04-25 09:31:38.945330 funcnodes_images-0.1.12/funcnodes_images/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.12/funcnodes_images/_numpy.py
+-rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.12/funcnodes_images/_pillow.py
+-rw-r--r--   0        0        0     6566 2024-04-25 09:30:24.746535 funcnodes_images-0.1.12/funcnodes_images/image_nodes.py
+-rw-r--r--   0        0        0     5156 2024-04-16 16:21:39.581875 funcnodes_images-0.1.12/funcnodes_images/imagecontainer.py
+-rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.12/funcnodes_images/utils.py
+-rw-r--r--   0        0        0      480 2024-04-25 09:31:30.261009 funcnodes_images-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.12/README.md
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 funcnodes_images-0.1.12/PKG-INFO
```

### Comparing `funcnodes_images-0.1.11/funcnodes_images/__init__.py` & `funcnodes_images-0.1.12/funcnodes_images/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .imagecontainer import register_imageformat, get_format, ImageFormat
 from ._numpy import NumpyImageFormat
 from ._pillow import PillowImageFormat
 import funcnodes as fn
 from exposedfunctionality.function_parser.types import add_type
 from . import image_nodes as nodes
-
+import funcnodes_numpy as fn_numpy  # noqa: F401 # import for type hinting
 
 add_type(ImageFormat, "ImageFormat")
 
 FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
     "typemap": {
         ImageFormat: "image",
     },
@@ -35,8 +35,8 @@
     "ImageFormat",
     "nodes",
     "FUNCNODES_RENDER_OPTIONS",
     "NODE_SHELF",
 ]
 
 
-__version__ = "0.1.11"
+__version__ = "0.1.12"
```

### Comparing `funcnodes_images-0.1.11/funcnodes_images/_numpy.py` & `funcnodes_images-0.1.12/funcnodes_images/_numpy.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.11/funcnodes_images/_pillow.py` & `funcnodes_images-0.1.12/funcnodes_images/_pillow.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.11/funcnodes_images/imagecontainer.py` & `funcnodes_images-0.1.12/funcnodes_images/imagecontainer.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.11/funcnodes_images/utils.py` & `funcnodes_images-0.1.12/funcnodes_images/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.11/PKG-INFO` & `funcnodes_images-0.1.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: funcnodes_images
-Version: 0.1.11
+Version: 0.1.12
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: funcnodes (>=0.1.30,<0.2.0)
+Requires-Dist: funcnodes-numpy (>=0.1.51,<0.2.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 Bassic functionalities to work with images in Funcnodes
 
 Most important is the extendable "ImageFormat" class, which allows for automatic rendering and conversion of different image formats if they are implemented. Each should have their own respective package, e.g. funcnodes_opencv as this is only the basis for them to prevent reimplementations.
```


# Comparing `tmp/funcnodes_images-0.1.13.tar.gz` & `tmp/funcnodes_images-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_images-0.1.13.tar", max compression
+gzip compressed data, was "funcnodes_images-0.1.14.tar", max compression
```

## Comparing `funcnodes_images-0.1.13.tar` & `funcnodes_images-0.1.14.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1023 2024-04-25 09:44:50.728699 funcnodes_images-0.1.13/funcnodes_images/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.13/funcnodes_images/_numpy.py
--rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.13/funcnodes_images/_pillow.py
--rw-r--r--   0        0        0     6566 2024-04-25 09:30:24.746535 funcnodes_images-0.1.13/funcnodes_images/image_nodes.py
--rw-r--r--   0        0        0     5338 2024-04-25 09:46:23.526949 funcnodes_images-0.1.13/funcnodes_images/imagecontainer.py
--rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.13/funcnodes_images/utils.py
--rw-r--r--   0        0        0      480 2024-04-25 09:45:07.716336 funcnodes_images-0.1.13/pyproject.toml
--rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.13/README.md
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 funcnodes_images-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0     1023 2024-04-25 10:58:29.400006 funcnodes_images-0.1.14/funcnodes_images/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.14/funcnodes_images/_numpy.py
+-rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.14/funcnodes_images/_pillow.py
+-rw-r--r--   0        0        0     6566 2024-04-25 09:30:24.746535 funcnodes_images-0.1.14/funcnodes_images/image_nodes.py
+-rw-r--r--   0        0        0     5338 2024-04-25 09:46:23.526949 funcnodes_images-0.1.14/funcnodes_images/imagecontainer.py
+-rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.14/funcnodes_images/utils.py
+-rw-r--r--   0        0        0      488 2024-04-25 10:58:20.715758 funcnodes_images-0.1.14/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.14/README.md
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 funcnodes_images-0.1.14/PKG-INFO
```

### Comparing `funcnodes_images-0.1.13/funcnodes_images/__init__.py` & `funcnodes_images-0.1.14/funcnodes_images/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "ImageFormat",
     "nodes",
     "FUNCNODES_RENDER_OPTIONS",
     "NODE_SHELF",
 ]
 
 
-__version__ = "0.1.13"
+__version__ = "0.1.14"
```

### Comparing `funcnodes_images-0.1.13/funcnodes_images/_numpy.py` & `funcnodes_images-0.1.14/funcnodes_images/_numpy.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.13/funcnodes_images/_pillow.py` & `funcnodes_images-0.1.14/funcnodes_images/_pillow.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.13/funcnodes_images/image_nodes.py` & `funcnodes_images-0.1.14/funcnodes_images/image_nodes.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.13/funcnodes_images/imagecontainer.py` & `funcnodes_images-0.1.14/funcnodes_images/imagecontainer.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.13/funcnodes_images/utils.py` & `funcnodes_images-0.1.14/funcnodes_images/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.13/PKG-INFO` & `funcnodes_images-0.1.14/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: funcnodes_images
-Version: 0.1.13
+Version: 0.1.14
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.40,<0.2.0)
-Requires-Dist: funcnodes-numpy (>=0.1.51,<0.2.0)
+Requires-Dist: funcnodes (>=0.1.42,<1.0.0)
+Requires-Dist: funcnodes-numpy (>=0.1.52,<0.2.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 Bassic functionalities to work with images in Funcnodes
 
 Most important is the extendable "ImageFormat" class, which allows for automatic rendering and conversion of different image formats if they are implemented. Each should have their own respective package, e.g. funcnodes_opencv as this is only the basis for them to prevent reimplementations.
```


# Comparing `tmp/funcnodes_images-0.1.12.tar.gz` & `tmp/funcnodes_images-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_images-0.1.12.tar", max compression
+gzip compressed data, was "funcnodes_images-0.1.13.tar", max compression
```

## Comparing `funcnodes_images-0.1.12.tar` & `funcnodes_images-0.1.13.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1023 2024-04-25 09:31:38.945330 funcnodes_images-0.1.12/funcnodes_images/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.12/funcnodes_images/_numpy.py
--rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.12/funcnodes_images/_pillow.py
--rw-r--r--   0        0        0     6566 2024-04-25 09:30:24.746535 funcnodes_images-0.1.12/funcnodes_images/image_nodes.py
--rw-r--r--   0        0        0     5156 2024-04-16 16:21:39.581875 funcnodes_images-0.1.12/funcnodes_images/imagecontainer.py
--rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.12/funcnodes_images/utils.py
--rw-r--r--   0        0        0      480 2024-04-25 09:31:30.261009 funcnodes_images-0.1.12/pyproject.toml
--rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.12/README.md
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 funcnodes_images-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0     1023 2024-04-25 09:44:50.728699 funcnodes_images-0.1.13/funcnodes_images/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.13/funcnodes_images/_numpy.py
+-rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.13/funcnodes_images/_pillow.py
+-rw-r--r--   0        0        0     6566 2024-04-25 09:30:24.746535 funcnodes_images-0.1.13/funcnodes_images/image_nodes.py
+-rw-r--r--   0        0        0     5338 2024-04-25 09:46:23.526949 funcnodes_images-0.1.13/funcnodes_images/imagecontainer.py
+-rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.13/funcnodes_images/utils.py
+-rw-r--r--   0        0        0      480 2024-04-25 09:45:07.716336 funcnodes_images-0.1.13/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.13/README.md
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 funcnodes_images-0.1.13/PKG-INFO
```

### Comparing `funcnodes_images-0.1.12/funcnodes_images/__init__.py` & `funcnodes_images-0.1.13/funcnodes_images/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     "ImageFormat",
     "nodes",
     "FUNCNODES_RENDER_OPTIONS",
     "NODE_SHELF",
 ]
 
 
-__version__ = "0.1.12"
+__version__ = "0.1.13"
```

### Comparing `funcnodes_images-0.1.12/funcnodes_images/_numpy.py` & `funcnodes_images-0.1.13/funcnodes_images/_numpy.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.12/funcnodes_images/_pillow.py` & `funcnodes_images-0.1.13/funcnodes_images/_pillow.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.12/funcnodes_images/image_nodes.py` & `funcnodes_images-0.1.13/funcnodes_images/image_nodes.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.12/funcnodes_images/imagecontainer.py` & `funcnodes_images-0.1.13/funcnodes_images/imagecontainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 from typing import Any, TYPE_CHECKING, Generic, TypeVar, Callable, Dict
 import io
 from PIL import Image
 import os
 from .utils import calc_new_size, calc_crop_values
 
+from funcnodes.config import update_render_options
 
 if TYPE_CHECKING:
     from ._numpy import NumpyImageFormat
     from ._pillow import PillowImageFormat
 
 
 T = TypeVar("T")
@@ -163,10 +164,18 @@
                 raise ValueError(
                     f"key '{key} 'already exists in image_formats as {IMAGE_FORMATS[key]}"
                 )
             else:
                 return
     IMAGE_FORMATS[key] = imageformat
 
+    update_render_options(
+        {
+            "typemap": {
+                imageformat: "image",
+            }
+        }
+    )
+
 
 def get_format(key: str) -> Type[ImageFormat]:
     return IMAGE_FORMATS[key]
```

### Comparing `funcnodes_images-0.1.12/funcnodes_images/utils.py` & `funcnodes_images-0.1.13/funcnodes_images/utils.py`

 * *Files identical despite different names*

### Comparing `funcnodes_images-0.1.12/PKG-INFO` & `funcnodes_images-0.1.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: funcnodes_images
-Version: 0.1.12
+Version: 0.1.13
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: funcnodes (>=0.1.30,<0.2.0)
+Requires-Dist: funcnodes (>=0.1.40,<0.2.0)
 Requires-Dist: funcnodes-numpy (>=0.1.51,<0.2.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 Bassic functionalities to work with images in Funcnodes
```


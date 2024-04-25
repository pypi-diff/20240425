# Comparing `tmp/pdf_watermark-2.2.0.tar.gz` & `tmp/pdf_watermark-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_watermark-2.2.0.tar", last modified: Sun Apr 21 11:31:57 2024, max compression
+gzip compressed data, was "pdf_watermark-2.2.1.tar", last modified: Thu Apr 25 20:50:50 2024, max compression
```

## Comparing `pdf_watermark-2.2.0.tar` & `pdf_watermark-2.2.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.462016 pdf_watermark-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.466016 pdf_watermark-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.github/workflows/lint-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.466016 pdf_watermark-2.2.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)   241473 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/images/before.png
--rw-r--r--   0 runner    (1001) docker     (127)   361202 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/images/image.png
--rw-r--r--   0 runner    (1001) docker     (127)   272309 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/images/text.png
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.462016 pdf_watermark-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/src/pdf_watermark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/src/pdf_watermark/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 11:31:57.000000 pdf_watermark-2.2.0/src/pdf_watermark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:31:57.470016 pdf_watermark-2.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/0.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/different_sizes_input.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/different_sizes_output.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/fixtures/input.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/test_add_watermark_from_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/test_different_page_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 11:31:53.000000 pdf_watermark-2.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.165253 pdf_watermark-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.157253 pdf_watermark-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.161253 pdf_watermark-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-04-25 20:50:50.165253 pdf_watermark-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.161253 pdf_watermark-2.2.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   241473 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/images/before.png
+-rw-r--r--   0 runner    (1001) docker     (127)   361202 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/images/image.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272309 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/images/text.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:50:50.165253 pdf_watermark-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.157253 pdf_watermark-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.161253 pdf_watermark-2.2.1/src/pdf_watermark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/src/pdf_watermark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/src/pdf_watermark/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/src/pdf_watermark/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/src/pdf_watermark/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/src/pdf_watermark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/src/pdf_watermark/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.165253 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 20:50:50.000000 pdf_watermark-2.2.1/src/pdf_watermark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.165253 pdf_watermark-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:50:50.165253 pdf_watermark-2.2.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/0.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/3.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/different_sizes_input.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/different_sizes_output.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/fixtures/input.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/test_add_watermark_from_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/test_different_page_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 20:50:46.000000 pdf_watermark-2.2.1/tests/utils.py
```

### Comparing `pdf_watermark-2.2.0/.github/workflows/lint-and-test.yml` & `pdf_watermark-2.2.1/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/.github/workflows/publish-to-pypi.yml` & `pdf_watermark-2.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/LICENSE` & `pdf_watermark-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/PKG-INFO` & `pdf_watermark-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-watermark
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python CLI tool to add watermarks to a PDF
 Author-email: Bastien Le Chenadec <bastien.lechenadec@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Bastien Le Chenadec]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -234,14 +234,16 @@
     * Add --unselectable and --save-as-image options.
     * Fix bug with temporary files on Windows.
 * 2.1.2
     * Fix missing Poppler dependancy.
     * Add test and lint to CI.
 * 2.2.0
     * Support PDFs with pages of different sizes.
+* 2.2.1
+    * Support line breaks in text watermark.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf_watermark-2.2.0/README.md` & `pdf_watermark-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,16 @@
     * Add --unselectable and --save-as-image options.
     * Fix bug with temporary files on Windows.
 * 2.1.2
     * Fix missing Poppler dependancy.
     * Add test and lint to CI.
 * 2.2.0
     * Support PDFs with pages of different sizes.
+* 2.2.1
+    * Support line breaks in text watermark.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf_watermark-2.2.0/images/before.png` & `pdf_watermark-2.2.1/images/before.png`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/images/image.png` & `pdf_watermark-2.2.1/images/image.png`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/images/text.png` & `pdf_watermark-2.2.1/images/text.png`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/pyproject.toml` & `pdf_watermark-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark/draw.py` & `pdf_watermark-2.2.1/src/pdf_watermark/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from math import cos, pi, sin
 from typing import Union
 
 import numpy as np
 from reportlab.pdfgen import canvas
 
 from pdf_watermark.options import Alignments, DrawingOptions, GridOptions, InsertOptions
-from pdf_watermark.utils import change_base, draw_centered_image, fit_image
+from pdf_watermark.utils import (
+    change_base,
+    draw_centered_image,
+    draw_centered_string_with_line_breaks,
+    fit_image,
+)
 
 
 def draw_one_watermark(
     watermark: canvas.Canvas,
     x: float,
     y: float,
     rotation_matrix: np.ndarray,
     drawing_options: DrawingOptions,
     image_width: float,
     image_height: float,
 ):
     x_prime, y_prime = change_base(x, y, rotation_matrix)
 
     if drawing_options.text is not None:
-        watermark.drawCentredString(
+        draw_centered_string_with_line_breaks(
+            watermark,
             x_prime,
             y_prime,
             drawing_options.text,
         )
 
     if drawing_options.image is not None:
         draw_centered_image(
```

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark/handler.py` & `pdf_watermark-2.2.1/src/pdf_watermark/handler.py`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark/options.py` & `pdf_watermark-2.2.1/src/pdf_watermark/options.py`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark/utils.py` & `pdf_watermark-2.2.1/src/pdf_watermark/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,30 @@
         bottom_left_y,
         width=width,
         height=height,
         mask="auto",
     )
 
 
+def draw_centered_string_with_line_breaks(
+    watermark: canvas.Canvas,
+    x: float,
+    y: float,
+    text: str,
+):
+    text_lines = text.split(r"\n")
+    line_height = (
+        watermark._leading
+    )  # line height is set when setting the font of the canvas
+    y += (len(text_lines) - 1) * line_height / 2  # also center the text vertically
+    for line in text_lines:
+        watermark.drawCentredString(x, y, line)
+        y -= watermark._leading
+
+
 def change_base(x: float, y: float, rotation_matrix: np.ndarray) -> Tuple[float, float]:
     # Since we rotated the original coordinates system, use the inverse of the rotation matrix
     # (which is the transposed matrix) to get the coordinates we have to draw at
     new_coordinates = np.transpose(rotation_matrix) @ np.array([[x], [y]])
     return new_coordinates[0, 0], new_coordinates[1, 0]
```

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark/watermark.py` & `pdf_watermark-2.2.1/src/pdf_watermark/watermark.py`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark.egg-info/PKG-INFO` & `pdf_watermark-2.2.1/src/pdf_watermark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-watermark
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python CLI tool to add watermarks to a PDF
 Author-email: Bastien Le Chenadec <bastien.lechenadec@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Bastien Le Chenadec]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -234,14 +234,16 @@
     * Add --unselectable and --save-as-image options.
     * Fix bug with temporary files on Windows.
 * 2.1.2
     * Fix missing Poppler dependancy.
     * Add test and lint to CI.
 * 2.2.0
     * Support PDFs with pages of different sizes.
+* 2.2.1
+    * Support line breaks in text watermark.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf_watermark-2.2.0/src/pdf_watermark.egg-info/SOURCES.txt` & `pdf_watermark-2.2.1/src/pdf_watermark.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,10 +24,12 @@
 src/pdf_watermark.egg-info/top_level.txt
 tests/__init__.py
 tests/test_add_watermark_from_options.py
 tests/test_different_page_sizes.py
 tests/utils.py
 tests/fixtures/0.pdf
 tests/fixtures/1.pdf
+tests/fixtures/2.pdf
+tests/fixtures/3.pdf
 tests/fixtures/different_sizes_input.pdf
 tests/fixtures/different_sizes_output.pdf
 tests/fixtures/input.pdf
```

### Comparing `pdf_watermark-2.2.0/tests/fixtures/0.pdf` & `pdf_watermark-2.2.1/tests/fixtures/0.pdf`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/tests/fixtures/1.pdf` & `pdf_watermark-2.2.1/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/tests/fixtures/different_sizes_input.pdf` & `pdf_watermark-2.2.1/tests/fixtures/different_sizes_input.pdf`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/tests/fixtures/different_sizes_output.pdf` & `pdf_watermark-2.2.1/tests/fixtures/different_sizes_output.pdf`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/tests/fixtures/input.pdf` & `pdf_watermark-2.2.1/tests/fixtures/input.pdf`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/tests/test_add_watermark_from_options.py` & `pdf_watermark-2.2.1/tests/test_add_watermark_from_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     InsertOptions,
 )
 from pdf_watermark.watermark import DEFAULTS
 from tests.utils import assert_pdfs_are_close
 
 INPUT = "tests/fixtures/input.pdf"
 OUTPUT = "output.pdf"
-FIXTURES = ["tests/fixtures/0.pdf", "tests/fixtures/1.pdf"]
+FIXTURES = [
+    "tests/fixtures/0.pdf",
+    "tests/fixtures/1.pdf",
+    "tests/fixtures/2.pdf",
+    "tests/fixtures/3.pdf",
+]
 
 
 @pytest.fixture(autouse=True)
 def cleanup():
     yield
     os.remove(OUTPUT)
 
@@ -35,15 +40,27 @@
         text_color=DEFAULTS.text_color,
         text_font=DEFAULTS.text_font,
         text_size=DEFAULTS.text_size,
         unselectable=DEFAULTS.unselectable,
         image_scale=DEFAULTS.image_scale,
         save_as_image=DEFAULTS.save_as_image,
         dpi=DEFAULTS.dpi,
-    )
+    ),
+    DrawingOptions(
+        watermark=r"watermark\nwith\nline\nbreaks",
+        opacity=DEFAULTS.opacity,
+        angle=DEFAULTS.angle,
+        text_color=DEFAULTS.text_color,
+        text_font=DEFAULTS.text_font,
+        text_size=DEFAULTS.text_size,
+        unselectable=DEFAULTS.unselectable,
+        image_scale=DEFAULTS.image_scale,
+        save_as_image=DEFAULTS.save_as_image,
+        dpi=DEFAULTS.dpi,
+    ),
 ]
 
 FILES_OPTIONS_FIXTURES = [FilesOptions(INPUT, OUTPUT)]
 
 GRID_OPTIONS_FIXTURES = [
     GridOptions(
         horizontal_boxes=DEFAULTS.horizontal_boxes,
```

### Comparing `pdf_watermark-2.2.0/tests/test_different_page_sizes.py` & `pdf_watermark-2.2.1/tests/test_different_page_sizes.py`

 * *Files identical despite different names*

### Comparing `pdf_watermark-2.2.0/tests/utils.py` & `pdf_watermark-2.2.1/tests/utils.py`

 * *Files identical despite different names*


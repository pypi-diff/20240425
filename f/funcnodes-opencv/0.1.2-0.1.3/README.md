# Comparing `tmp/funcnodes_opencv-0.1.2.tar.gz` & `tmp/funcnodes_opencv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_opencv-0.1.2.tar", max compression
+gzip compressed data, was "funcnodes_opencv-0.1.3.tar", max compression
```

## Comparing `funcnodes_opencv-0.1.2.tar` & `funcnodes_opencv-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      101 2024-04-24 13:02:24.215736 funcnodes_opencv-0.1.2/funcnodes_opencv/__init__.py
--rw-r--r--   0        0        0     2956 2024-04-24 13:02:03.732194 funcnodes_opencv-0.1.2/funcnodes_opencv/imageformat.py
--rw-r--r--   0        0        0      361 2024-04-24 13:03:24.333088 funcnodes_opencv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.2/README.md
--rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      101 2024-04-24 13:15:58.915405 funcnodes_opencv-0.1.3/funcnodes_opencv/__init__.py
+-rw-r--r--   0        0        0     2956 2024-04-24 13:09:03.909315 funcnodes_opencv-0.1.3/funcnodes_opencv/imageformat.py
+-rw-r--r--   0        0        0      361 2024-04-24 13:15:54.272908 funcnodes_opencv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.3/README.md
+-rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.3/PKG-INFO
```

### Comparing `funcnodes_opencv-0.1.2/funcnodes_opencv/imageformat.py` & `funcnodes_opencv-0.1.3/funcnodes_opencv/imageformat.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,8 +85,8 @@
 
 
 def pil_to_cv2(pil_img: PillowImageFormat) -> OpenCVImageFormat:
     return pil_img.to_np().to_cv2()
 
 
 OpenCVImageFormat.add_to_converter(PillowImageFormat, cv2_to_pil)
-OpenCVImageFormat.add_to_converter(PillowImageFormat, pil_to_cv2)
+PillowImageFormat.add_to_converter(OpenCVImageFormat, pil_to_cv2)
```


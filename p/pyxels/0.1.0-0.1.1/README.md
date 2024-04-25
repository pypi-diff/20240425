# Comparing `tmp/pyxels-0.1.0.tar.gz` & `tmp/pyxels-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxels-0.1.0.tar", max compression
+gzip compressed data, was "pyxels-0.1.1.tar", max compression
```

## Comparing `pyxels-0.1.0.tar` & `pyxels-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-04-25 03:37:12.002110 pyxels-0.1.0/LICENSE
--rw-r--r--   0        0        0      361 2024-04-25 12:52:06.049336 pyxels-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-25 12:52:08.939852 pyxels-0.1.0/pyxels/__init__.py
--rw-r--r--   0        0        0    12579 2024-04-25 12:57:50.026093 pyxels-0.1.0/pyxels/rgb.py
--rw-r--r--   0        0        0     1570 2024-04-25 13:14:36.671294 pyxels-0.1.0/README.md
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 pyxels-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-25 03:37:12.002110 pyxels-0.1.1/LICENSE
+-rw-r--r--   0        0        0      547 2024-04-25 13:47:26.699450 pyxels-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-25 12:52:08.939852 pyxels-0.1.1/pyxels/__init__.py
+-rw-r--r--   0        0        0    12579 2024-04-25 12:57:50.026093 pyxels-0.1.1/pyxels/rgb.py
+-rw-r--r--   0        0        0     1570 2024-04-25 13:42:47.735556 pyxels-0.1.1/README.md
+-rw-r--r--   0        0        0     2056 1970-01-01 00:00:00.000000 pyxels-0.1.1/PKG-INFO
```

### Comparing `pyxels-0.1.0/LICENSE` & `pyxels-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxels-0.1.0/pyxels/rgb.py` & `pyxels-0.1.1/pyxels/rgb.py`

 * *Files identical despite different names*

### Comparing `pyxels-0.1.0/README.md` & `pyxels-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxels-0.1.0/PKG-INFO` & `pyxels-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyxels
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Pyxels is a low-level image data manipulation library for Python. It is designed to be fast and efficient, and to provide a simple interface for working with image data.
+License: MIT
 Author: DJ Stomp
 Author-email: 85457381+djstompzone@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Pyxels
 
 Pyxels is a low-level image data manipulation library for Python. It is designed to be fast and efficient, and to provide a simple interface for working with image data.
```


# Comparing `tmp/drawpyo-0.1.2.tar.gz` & `tmp/drawpyo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawpyo-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drawpyo-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `drawpyo-0.1.2.tar` & `drawpyo-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4781 2024-03-21 04:48:09.875927 drawpyo-0.1.2/README.md
--rw-r--r--   0        0        0      877 2024-04-02 23:44:43.159162 drawpyo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      150 2024-04-12 01:57:49.929102 drawpyo-0.1.2/src/drawpyo/__init__.py
--rw-r--r--   0        0        0       99 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram/__init__.py
--rw-r--r--   0        0        0    10644 2024-04-12 01:56:48.484739 drawpyo-0.1.2/src/drawpyo/diagram/base_diagram.py
--rw-r--r--   0        0        0    19912 2024-04-02 23:44:43.159162 drawpyo-0.1.2/src/drawpyo/diagram/edges.py
--rw-r--r--   0        0        0    20577 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram/objects.py
--rw-r--r--   0        0        0     6097 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram/text_format.py
--rw-r--r--   0        0        0       49 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram_types/__init__.py
--rw-r--r--   0        0        0     1042 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram_types/class_diagram.py
--rw-r--r--   0        0        0    20255 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram_types/tree.py
--rw-r--r--   0        0        0     4551 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/file.py
--rw-r--r--   0        0        0     2176 2024-04-02 23:44:43.159162 drawpyo-0.1.2/src/drawpyo/formatting_database/edge_styles.toml
--rw-r--r--   0        0        0      217 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/formatting_database/line_styles.toml
--rw-r--r--   0        0        0     4839 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/page.py
--rw-r--r--   0        0        0     4737 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/shape_libraries/flowchart.toml
--rw-r--r--   0        0        0     2716 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/shape_libraries/general.toml
--rw-r--r--   0        0        0     3939 2024-04-02 23:44:43.159162 drawpyo-0.1.2/src/drawpyo/xml_base.py
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 drawpyo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4779 2024-04-25 15:15:52.715634 drawpyo-0.1.3/README.md
+-rw-r--r--   0        0        0      840 2024-04-25 15:15:28.427839 drawpyo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-04-25 15:16:27.535315 drawpyo-0.1.3/src/drawpyo/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/diagram/__init__.py
+-rw-r--r--   0        0        0    10644 2024-04-12 02:03:42.003162 drawpyo-0.1.3/src/drawpyo/diagram/base_diagram.py
+-rw-r--r--   0        0        0    19912 2024-04-02 23:44:43.159162 drawpyo-0.1.3/src/drawpyo/diagram/edges.py
+-rw-r--r--   0        0        0    20577 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/diagram/objects.py
+-rw-r--r--   0        0        0     6097 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/diagram/text_format.py
+-rw-r--r--   0        0        0       49 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/diagram_types/__init__.py
+-rw-r--r--   0        0        0     1042 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/diagram_types/class_diagram.py
+-rw-r--r--   0        0        0    20255 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/diagram_types/tree.py
+-rw-r--r--   0        0        0     4551 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/file.py
+-rw-r--r--   0        0        0     2176 2024-04-02 23:44:43.159162 drawpyo-0.1.3/src/drawpyo/formatting_database/edge_styles.toml
+-rw-r--r--   0        0        0      217 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/formatting_database/line_styles.toml
+-rw-r--r--   0        0        0     4839 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/page.py
+-rw-r--r--   0        0        0     4737 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/shape_libraries/flowchart.toml
+-rw-r--r--   0        0        0     2716 2024-04-02 00:14:21.541936 drawpyo-0.1.3/src/drawpyo/shape_libraries/general.toml
+-rw-r--r--   0        0        0     3939 2024-04-02 23:44:43.159162 drawpyo-0.1.3/src/drawpyo/xml_base.py
+-rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 drawpyo-0.1.3/PKG-INFO
```

### Comparing `drawpyo-0.1.2/README.md` & `drawpyo-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 The basic mode of interacting with drawpyo is to manually create, style, and place objects just like you would using the Draw.io UI. There are a number of ways to style objects and you can write your own functionality for automatically handling style or placement.
 
 ## Make a new file
 
 ```python
 import drawpyo
-diagram = drawpyo.File()
+file = drawpyo.File()
 file.file_path = r"C:\drawpyo"
 file.file_name = "Test Generated Edges.drawio"
 # Add a page
-page = drawpy.Page(file=file)
+page = drawpyo.Page(file=file)
 ```
 
 ## Add an object
 
 ```python
 item = drawpyo.diagram.Object(page=page, value="new object")
 item.position = (0, 0)
```

### Comparing `drawpyo-0.1.2/pyproject.toml` & `drawpyo-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
-    "toml >= 0.10.2; python_version < '3.11'",
-    "mkdocstrings[python] >= 0.18",
+    "toml >= 0.10.2; python_version < '3.11'"
     ]   
 
 [project.urls]
 Homepage = "https://github.com/MerrimanInd/drawpyo"
 Issues = "https://github.com/MerrimanInd/drawpyo/issues"
 
 [tool.pytest.ini_options]
```

### Comparing `drawpyo-0.1.2/src/drawpyo/diagram/base_diagram.py` & `drawpyo-0.1.3/src/drawpyo/diagram/base_diagram.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/diagram/edges.py` & `drawpyo-0.1.3/src/drawpyo/diagram/edges.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/diagram/objects.py` & `drawpyo-0.1.3/src/drawpyo/diagram/objects.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/diagram/text_format.py` & `drawpyo-0.1.3/src/drawpyo/diagram/text_format.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/diagram_types/class_diagram.py` & `drawpyo-0.1.3/src/drawpyo/diagram_types/class_diagram.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/diagram_types/tree.py` & `drawpyo-0.1.3/src/drawpyo/diagram_types/tree.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/file.py` & `drawpyo-0.1.3/src/drawpyo/file.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/formatting_database/edge_styles.toml` & `drawpyo-0.1.3/src/drawpyo/formatting_database/edge_styles.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/page.py` & `drawpyo-0.1.3/src/drawpyo/page.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/shape_libraries/flowchart.toml` & `drawpyo-0.1.3/src/drawpyo/shape_libraries/flowchart.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/shape_libraries/general.toml` & `drawpyo-0.1.3/src/drawpyo/shape_libraries/general.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/src/drawpyo/xml_base.py` & `drawpyo-0.1.3/src/drawpyo/xml_base.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.2/PKG-INFO` & `drawpyo-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: drawpyo
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for programmatically generating Draw.io charts.
 Keywords: draw.io,diagrams.net,diagrams
 Author-email: Xander Cesari <xander@merriman.industries>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: toml >= 0.10.2; python_version < '3.11'
-Requires-Dist: mkdocstrings[python] >= 0.18
 Project-URL: Homepage, https://github.com/MerrimanInd/drawpyo
 Project-URL: Issues, https://github.com/MerrimanInd/drawpyo/issues
 
 # drawpyo
 
 Drawpyo is a Python library for programmatically generating Diagrams.net/Draw.io charts. It enables creating a diagram object, placing and styling objects, then writing the object to a file.
 
@@ -34,19 +33,19 @@
 
 The basic mode of interacting with drawpyo is to manually create, style, and place objects just like you would using the Draw.io UI. There are a number of ways to style objects and you can write your own functionality for automatically handling style or placement.
 
 ## Make a new file
 
 ```python
 import drawpyo
-diagram = drawpyo.File()
+file = drawpyo.File()
 file.file_path = r"C:\drawpyo"
 file.file_name = "Test Generated Edges.drawio"
 # Add a page
-page = drawpy.Page(file=file)
+page = drawpyo.Page(file=file)
 ```
 
 ## Add an object
 
 ```python
 item = drawpyo.diagram.Object(page=page, value="new object")
 item.position = (0, 0)
```


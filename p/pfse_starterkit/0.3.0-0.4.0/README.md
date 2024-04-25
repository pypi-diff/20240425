# Comparing `tmp/pfse_starterkit-0.3.0.tar.gz` & `tmp/pfse_starterkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfse_starterkit-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pfse_starterkit-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pfse_starterkit-0.3.0.tar` & `pfse_starterkit-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1799 2022-12-13 02:38:41.070429 pfse_starterkit-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2022-12-13 02:38:41.070429 pfse_starterkit-0.3.0/LICENSE
--rw-r--r--   0        0        0      600 2023-07-29 18:54:32.430342 pfse_starterkit-0.3.0/README.md
--rw-r--r--   0        0        0      205 2023-07-29 18:59:56.850634 pfse_starterkit-0.3.0/pfse_starterkit/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-29 18:49:22.086100 pfse_starterkit-0.3.0/pfse_starterkit/__main__.py
--rw-r--r--   0        0        0     1497 2023-07-29 18:23:14.482881 pfse_starterkit-0.3.0/pfse_starterkit/sectionproperties_test.py
--rw-r--r--   0        0        0       95 2023-01-27 19:13:51.754840 pfse_starterkit-0.3.0/pfse_starterkit/streamlit_test.py
--rw-r--r--   0        0        0     2512 2023-01-27 19:13:51.754840 pfse_starterkit-0.3.0/pfse_starterkit/vtk_cylinder.py
--rw-r--r--   0        0        0     1154 2023-07-29 18:21:53.863686 pfse_starterkit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 pfse_starterkit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1799 2022-12-13 02:38:41.070429 pfse_starterkit-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2022-12-13 02:38:41.070429 pfse_starterkit-0.4.0/LICENSE
+-rw-r--r--   0        0        0      600 2023-07-29 18:54:32.430342 pfse_starterkit-0.4.0/README.md
+-rw-r--r--   0        0        0      205 2024-04-25 11:11:42.207387 pfse_starterkit-0.4.0/pfse_starterkit/__init__.py
+-rw-r--r--   0        0        0     8695 2024-04-25 11:11:46.375326 pfse_starterkit-0.4.0/pfse_starterkit/__main__.py
+-rw-r--r--   0        0        0     1497 2023-07-29 18:23:14.482881 pfse_starterkit-0.4.0/pfse_starterkit/sectionproperties_test.py
+-rw-r--r--   0        0        0       95 2023-01-27 19:13:51.754840 pfse_starterkit-0.4.0/pfse_starterkit/streamlit_test.py
+-rw-r--r--   0        0        0     2512 2023-01-27 19:13:51.754840 pfse_starterkit-0.4.0/pfse_starterkit/vtk_cylinder.py
+-rw-r--r--   0        0        0     1181 2024-04-25 11:06:26.682248 pfse_starterkit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 pfse_starterkit-0.4.0/PKG-INFO
```

### Comparing `pfse_starterkit-0.3.0/.gitignore` & `pfse_starterkit-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.3.0/LICENSE` & `pfse_starterkit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.3.0/README.md` & `pfse_starterkit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.3.0/pfse_starterkit/__main__.py` & `pfse_starterkit-0.4.0/pfse_starterkit/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 A module to designed to perform package installations, and verification of install,
 in preparation for the StructuralPython "Python for Structural Engineers" ("pfse")
 course.
 """
-__version__ = "0.0.1"
 
 import importlib.util
 import importlib
 import pathlib
 import platform
 import psutil
 import subprocess
@@ -255,15 +254,15 @@
         msg = Text("No additional installations necessary. Ok.")
         msg.stylize("bold green")
         console.print(msg)
 
 
 def install_pfse_kernel():
     proc = subprocess.Popen(
-        ["python", "-m", "ipykernel", "install", "--user", "--name", "pfse", "--display-name", "Python 3.10 (pfse)"],
+        ["python", "-m", "ipykernel", "install", "--user", "--name", "pfse", "--display-name", "Python 3 (pfse)"],
         stdout=subprocess.PIPE,
         text=True,
     )
     msg = Text("PfSE Jupyter Kernel Installed Successfully")
     msg.stylize("bold green")
     console.print(msg)
```

### Comparing `pfse_starterkit-0.3.0/pfse_starterkit/sectionproperties_test.py` & `pfse_starterkit-0.4.0/pfse_starterkit/sectionproperties_test.py`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.3.0/pfse_starterkit/vtk_cylinder.py` & `pfse_starterkit-0.4.0/pfse_starterkit/vtk_cylinder.py`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.3.0/pyproject.toml` & `pfse_starterkit-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,38 +20,40 @@
     "shapely>=2.0.0",
     "vtk",
     "matplotlib",
     "plotly",
     "kaleido",
     "sectionproperties",
     "concreteproperties",
-    "pycba>=0.2.0",
-    "PyNiteFEA>=0.0.78",
-    "anastruct",
+    "pycba>=0.4.0",
+    "PyNiteFEA>=0.0.87",
     "scipy",
     "handcalcs",
+    "more-itertools",
     "forallpeople",
     "pytest",
-    "ipytest",
     "rich",
     "tqdm",
     "papermodels",
     "xlwings",
-    "black",
     "jupyterlab",
     "IPython",
     "ipywidgets",
     "ipykernel",
     "jupyterlab-katex",
     "jupyterlab-mathjax3",
     "nbconvert",
     "pyperclip",
     "typer",
-    "magicgui[pyside2]",
-    "flit"
+    "flit",
+    "python-docx",
+    "constable",
+    "ruff",
+    "black",
+    "isort",
 ]
 
 [project.urls]
 Home = "https://github.com/connorferster/pfse_starterkit"
 
 [project.scripts]
 pfse_verify = "pfse_starterkit.__main__:check_installs"
```

### Comparing `pfse_starterkit-0.3.0/PKG-INFO` & `pfse_starterkit-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfse_starterkit
-Version: 0.3.0
+Version: 0.4.0
 Summary: A module to designed to perform package installations, and verification of install,
 Author-email: Connor Ferster <connor@structuralpython.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: streamlit
 Requires-Dist: numpy
 Requires-Dist: pandas
@@ -14,38 +14,40 @@
 Requires-Dist: shapely>=2.0.0
 Requires-Dist: vtk
 Requires-Dist: matplotlib
 Requires-Dist: plotly
 Requires-Dist: kaleido
 Requires-Dist: sectionproperties
 Requires-Dist: concreteproperties
-Requires-Dist: pycba>=0.2.0
-Requires-Dist: PyNiteFEA>=0.0.78
-Requires-Dist: anastruct
+Requires-Dist: pycba>=0.4.0
+Requires-Dist: PyNiteFEA>=0.0.87
 Requires-Dist: scipy
 Requires-Dist: handcalcs
+Requires-Dist: more-itertools
 Requires-Dist: forallpeople
 Requires-Dist: pytest
-Requires-Dist: ipytest
 Requires-Dist: rich
 Requires-Dist: tqdm
 Requires-Dist: papermodels
 Requires-Dist: xlwings
-Requires-Dist: black
 Requires-Dist: jupyterlab
 Requires-Dist: IPython
 Requires-Dist: ipywidgets
 Requires-Dist: ipykernel
 Requires-Dist: jupyterlab-katex
 Requires-Dist: jupyterlab-mathjax3
 Requires-Dist: nbconvert
 Requires-Dist: pyperclip
 Requires-Dist: typer
-Requires-Dist: magicgui[pyside2]
 Requires-Dist: flit
+Requires-Dist: python-docx
+Requires-Dist: constable
+Requires-Dist: ruff
+Requires-Dist: black
+Requires-Dist: isort
 Project-URL: Home, https://github.com/connorferster/pfse_starterkit
 
 # pfse_starterkit
 A Python package that installs all required packages for the StructuralPython Python for Structural Engineers (pfse) course.
 
 This installs the following packages:
```


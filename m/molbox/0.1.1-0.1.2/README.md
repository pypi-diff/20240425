# Comparing `tmp/molbox-0.1.1.tar.gz` & `tmp/molbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molbox-0.1.1.tar", max compression
+gzip compressed data, was "molbox-0.1.2.tar", max compression
```

## Comparing `molbox-0.1.1.tar` & `molbox-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-04-23 14:10:55.887770 molbox-0.1.1/LICENSE
--rw-r--r--   0        0        0     1064 2024-04-24 13:56:05.236653 molbox-0.1.1/README.md
--rw-r--r--   0        0        0      629 2024-04-24 14:35:31.636824 molbox-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       89 2024-04-22 13:05:40.713884 molbox-0.1.1/src/molbox/__init__.py
--rw-r--r--   0        0        0      210 2024-04-23 11:18:59.633760 molbox-0.1.1/src/molbox/box.py
--rw-r--r--   0        0        0      918 2024-04-24 13:01:38.687094 molbox-0.1.1/src/molbox/lammps_data.py
--rw-r--r--   0        0        0     1114 2024-04-24 13:01:38.687094 molbox-0.1.1/src/molbox/molbox.py
--rw-r--r--   0        0        0     2581 2024-04-24 13:01:38.687094 molbox-0.1.1/src/molbox/rdkit_3d_ops.py
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 molbox-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 14:10:55.887770 molbox-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1064 2024-04-24 13:56:05.236653 molbox-0.1.2/README.md
+-rw-r--r--   0        0        0      702 2024-04-25 06:39:31.269115 molbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-04-22 13:05:40.713884 molbox-0.1.2/src/molbox/__init__.py
+-rw-r--r--   0        0        0      210 2024-04-23 11:18:59.633760 molbox-0.1.2/src/molbox/box.py
+-rw-r--r--   0        0        0      918 2024-04-24 13:01:38.687094 molbox-0.1.2/src/molbox/lammps_data.py
+-rw-r--r--   0        0        0     1114 2024-04-24 13:01:38.687094 molbox-0.1.2/src/molbox/molbox.py
+-rw-r--r--   0        0        0     2581 2024-04-24 13:01:38.687094 molbox-0.1.2/src/molbox/rdkit_3d_ops.py
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 molbox-0.1.2/PKG-INFO
```

### Comparing `molbox-0.1.1/LICENSE` & `molbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molbox-0.1.1/README.md` & `molbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `molbox-0.1.1/pyproject.toml` & `molbox-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "molbox"
-version = "0.1.1"
+version = "0.1.2"
 description = "Create simulation boxes for LAMMPS."
 authors = ["Niklas Kappel <niklas.kappel@kit.edu>"]
 readme = "README.md"
 packages = [{ include = "molbox", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.9"
 rdkit = "^2023.9.5"
 scipy = "^1.13.0"
 openbabel-wheel = "^3.1.1.19"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 
+[tool.poetry.urls]
+repository = "https://github.com/NiklasKappel/molbox"
+
 [tool.pyright]
 reportAttributeAccessIssue = false
 
 [tool.ruff]
 lint.extend-select = ["I"]
 
 [build-system]
```

### Comparing `molbox-0.1.1/src/molbox/lammps_data.py` & `molbox-0.1.2/src/molbox/lammps_data.py`

 * *Files identical despite different names*

### Comparing `molbox-0.1.1/src/molbox/molbox.py` & `molbox-0.1.2/src/molbox/molbox.py`

 * *Files identical despite different names*

### Comparing `molbox-0.1.1/src/molbox/rdkit_3d_ops.py` & `molbox-0.1.2/src/molbox/rdkit_3d_ops.py`

 * *Files identical despite different names*

### Comparing `molbox-0.1.1/PKG-INFO` & `molbox-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: molbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create simulation boxes for LAMMPS.
 Author: Niklas Kappel
 Author-email: niklas.kappel@kit.edu
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openbabel-wheel (>=3.1.1.19,<4.0.0.0)
 Requires-Dist: rdkit (>=2023.9.5,<2024.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Project-URL: repository, https://github.com/NiklasKappel/molbox
 Description-Content-Type: text/markdown
 
 # molbox
 
 Molbox is a simple Python package that extends [rdkit](https://www.rdkit.org/) with spatial [transformations](src/molbox/rdkit_3d_ops.py) of 3D molecules and semantics for multiple molecules in a rectangular [box](src/molbox/molbox.py). It allows you to quickly create simulation boxes and write them to data files that can be read by [LAMMPS](https://www.lammps.org/).
 
 ## Installation
```


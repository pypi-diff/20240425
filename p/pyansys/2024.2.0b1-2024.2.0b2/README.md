# Comparing `tmp/pyansys-2024.2.0b1.tar.gz` & `tmp/pyansys-2024.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyansys-2024.2.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyansys-2024.2.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyansys-2024.2.0b1.tar` & `pyansys-2024.2.0b2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1089 2024-04-15 13:17:47.237010 pyansys-2024.2.0b1/LICENSE
--rw-r--r--   0        0        0    12171 2024-04-15 13:17:47.237010 pyansys-2024.2.0b1/README.rst
--rw-r--r--   0        0        0     3265 2024-04-15 13:17:47.261010 pyansys-2024.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     1353 2024-04-15 13:17:47.261010 pyansys-2024.2.0b1/src/pyansys/__init__.py
--rw-r--r--   0        0        0    15282 1970-01-01 00:00:00.000000 pyansys-2024.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-25 10:59:23.048147 pyansys-2024.2.0b2/LICENSE
+-rw-r--r--   0        0        0    12171 2024-04-25 10:59:23.048147 pyansys-2024.2.0b2/README.rst
+-rw-r--r--   0        0        0     3233 2024-04-25 10:59:23.072147 pyansys-2024.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1353 2024-04-25 10:59:23.072147 pyansys-2024.2.0b2/src/pyansys/__init__.py
+-rw-r--r--   0        0        0    15243 1970-01-01 00:00:00.000000 pyansys-2024.2.0b2/PKG-INFO
```

### Comparing `pyansys-2024.2.0b1/LICENSE` & `pyansys-2024.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyansys-2024.2.0b1/README.rst` & `pyansys-2024.2.0b2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 a fresh Python installation or on a virtual environment.
 
 For example, on Linux with Python 3.9, unzip the wheelhouse archive and install it with the following
 commands:
 
 .. code:: bash
 
-    unzip pyansys-v2024.2.0b1-wheelhouse-Linux-3.9-core.zip wheelhouse
+    unzip pyansys-v2024.2.0b2-wheelhouse-Linux-3.9-core.zip wheelhouse
     pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
 the same ``pip`` command as in the previous example.
 
 Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
```

### Comparing `pyansys-2024.2.0b1/pyproject.toml` & `pyansys-2024.2.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pyansys"
-version = "2024.2.0b1"
+version = "2024.2.0b2"
 description = "Pythonic interfaces to Ansys products"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.support@ansys.com" }]
 maintainers = [
     { name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com" },
@@ -25,67 +25,66 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "ansys-acp-core==0.1b1",
     "ansys-additive-core==0.17.2",
-    "ansys-dpf-composites==0.4.0",
+    "ansys-dpf-composites==0.4.1",
     "ansys-dpf-core==0.12.0",
     "ansys-dpf-post==0.8.0",
-    "ansys-dpf-gate==0.4.1",
     "ansys-dyna-core==0.4.15",
-    "ansys-dynamicreporting-core==0.5.1",
+    "ansys-dynamicreporting-core==0.6.0",
     "ansys-edb-core==0.1.4",
     "ansys-fluent-core==0.20.0",
-    "ansys-geometry-core==0.4.14",
+    "ansys-geometry-core==0.5.0",
     "ansys-hps-client==0.8.0",
     "ansys-mapdl-core==0.68.1",
-    "ansys-math-core==0.1.3",
+    "ansys-math-core==0.1.5",
     "ansys-mechanical-core==0.10.9",
     "ansys-meshing-prime==0.5.1",
     "ansys-modelcenter-workflow==0.1.1",
     "ansys-motorcad-core==0.4.3",
     "ansys-openapi-common==1.5.1",
     "ansys-optislang-core==0.6.3",
     "ansys-platform-instancemanagement==1.1.2",
-    "ansys-pyensight-core==0.7.11",
+    "ansys-pyensight-core==0.8.0",
     "ansys-rocky-core==0.1.0",
     "ansys-seascape==0.2.0",
-    "ansys-sherlock-core==0.5.0",
-    "ansys-simai-core==0.1.4",
+    "ansys-sherlock-core==0.6.0",
+    "ansys-simai-core==0.1.5",
     "ansys-systemcoupling-core==0.4.1",
     "ansys-turbogrid-core==0.4.0",
-    "pyaedt==0.8.7",
-    "pyedb==0.7.1",
+    "pyaedt==0.8.9",
+    "pyedb==0.8.0",
     "pygranta==2024.1.0",
     "pytwin==0.6.0",
 ]
 
 [project.optional-dependencies]
 mapdl-all = ["ansys-mapdl-reader==0.53.0"]
 fluent-all = [
     "ansys-fluent-visualization==0.9.0",
     "ansys-fluent-parametric==0.10.0",
 ]
 tools = [
     "ansys-units==0.3.2",
-    "ansys-tools-path==0.5.1",
+    "ansys-tools-path==0.5.2",
     "pyansys-tools-report==0.7.0",
     "pyansys-tools-versioning==0.5.0",
 ]
 all = [
     # MAPDL - ALL
     "ansys-mapdl-reader==0.53.0",
     # FLUENT - ALL
     "ansys-fluent-visualization==0.9.0",
     "ansys-fluent-parametric==0.10.0",
     # TOOLS
     "ansys-units==0.3.2",
-    "ansys-tools-path==0.5.1",
+    "ansys-tools-path==0.5.2",
     # "ansys-tools-protoc-helper==0.4.0; python_version<='3.10'",
     "pyansys-tools-report==0.7.0",
     "pyansys-tools-versioning==0.5.0",
 ]
 doc = [
     "Sphinx==7.2.6",
     "ansys-sphinx-theme==0.15.2",
```

### Comparing `pyansys-2024.2.0b1/src/pyansys/__init__.py` & `pyansys-2024.2.0b2/src/pyansys/__init__.py`

 * *Files identical despite different names*

### Comparing `pyansys-2024.2.0b1/PKG-INFO` & `pyansys-2024.2.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyansys
-Version: 2024.2.0b1
+Version: 2024.2.0b2
 Summary: Pythonic interfaces to Ansys products
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -13,60 +13,59 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ansys-acp-core==0.1b1
 Requires-Dist: ansys-additive-core==0.17.2
-Requires-Dist: ansys-dpf-composites==0.4.0
+Requires-Dist: ansys-dpf-composites==0.4.1
 Requires-Dist: ansys-dpf-core==0.12.0
 Requires-Dist: ansys-dpf-post==0.8.0
-Requires-Dist: ansys-dpf-gate==0.4.1
 Requires-Dist: ansys-dyna-core==0.4.15
-Requires-Dist: ansys-dynamicreporting-core==0.5.1
+Requires-Dist: ansys-dynamicreporting-core==0.6.0
 Requires-Dist: ansys-edb-core==0.1.4
 Requires-Dist: ansys-fluent-core==0.20.0
-Requires-Dist: ansys-geometry-core==0.4.14
+Requires-Dist: ansys-geometry-core==0.5.0
 Requires-Dist: ansys-hps-client==0.8.0
 Requires-Dist: ansys-mapdl-core==0.68.1
-Requires-Dist: ansys-math-core==0.1.3
+Requires-Dist: ansys-math-core==0.1.5
 Requires-Dist: ansys-mechanical-core==0.10.9
 Requires-Dist: ansys-meshing-prime==0.5.1
 Requires-Dist: ansys-modelcenter-workflow==0.1.1
 Requires-Dist: ansys-motorcad-core==0.4.3
 Requires-Dist: ansys-openapi-common==1.5.1
 Requires-Dist: ansys-optislang-core==0.6.3
 Requires-Dist: ansys-platform-instancemanagement==1.1.2
-Requires-Dist: ansys-pyensight-core==0.7.11
+Requires-Dist: ansys-pyensight-core==0.8.0
 Requires-Dist: ansys-rocky-core==0.1.0
 Requires-Dist: ansys-seascape==0.2.0
-Requires-Dist: ansys-sherlock-core==0.5.0
-Requires-Dist: ansys-simai-core==0.1.4
+Requires-Dist: ansys-sherlock-core==0.6.0
+Requires-Dist: ansys-simai-core==0.1.5
 Requires-Dist: ansys-systemcoupling-core==0.4.1
 Requires-Dist: ansys-turbogrid-core==0.4.0
-Requires-Dist: pyaedt==0.8.7
-Requires-Dist: pyedb==0.7.1
+Requires-Dist: pyaedt==0.8.9
+Requires-Dist: pyedb==0.8.0
 Requires-Dist: pygranta==2024.1.0
 Requires-Dist: pytwin==0.6.0
 Requires-Dist: ansys-mapdl-reader==0.53.0 ; extra == "all"
 Requires-Dist: ansys-fluent-visualization==0.9.0 ; extra == "all"
 Requires-Dist: ansys-fluent-parametric==0.10.0 ; extra == "all"
 Requires-Dist: ansys-units==0.3.2 ; extra == "all"
-Requires-Dist: ansys-tools-path==0.5.1 ; extra == "all"
+Requires-Dist: ansys-tools-path==0.5.2 ; extra == "all"
 Requires-Dist: pyansys-tools-report==0.7.0 ; extra == "all"
 Requires-Dist: pyansys-tools-versioning==0.5.0 ; extra == "all"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-design==0.5.0 ; extra == "doc"
 Requires-Dist: ansys-fluent-visualization==0.9.0 ; extra == "fluent-all"
 Requires-Dist: ansys-fluent-parametric==0.10.0 ; extra == "fluent-all"
 Requires-Dist: ansys-mapdl-reader==0.53.0 ; extra == "mapdl-all"
 Requires-Dist: ansys-units==0.3.2 ; extra == "tools"
-Requires-Dist: ansys-tools-path==0.5.1 ; extra == "tools"
+Requires-Dist: ansys-tools-path==0.5.2 ; extra == "tools"
 Requires-Dist: pyansys-tools-report==0.7.0 ; extra == "tools"
 Requires-Dist: pyansys-tools-versioning==0.5.0 ; extra == "tools"
 Project-URL: Documentation, https://docs.pyansys.com
 Project-URL: Source, https://github.com/ansys/pyansys
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: fluent-all
@@ -255,15 +254,15 @@
 a fresh Python installation or on a virtual environment.
 
 For example, on Linux with Python 3.9, unzip the wheelhouse archive and install it with the following
 commands:
 
 .. code:: bash
 
-    unzip pyansys-v2024.2.0b1-wheelhouse-Linux-3.9-core.zip wheelhouse
+    unzip pyansys-v2024.2.0b2-wheelhouse-Linux-3.9-core.zip wheelhouse
     pip install pyansys -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip to a wheelhouse directory and then install using
 the same ``pip`` command as in the previous example.
 
 Consider installing using a `virtual environment <https://docs.python.org/3/library/venv.html>`_.
```


# Comparing `tmp/pyalf-2.5.post5.tar.gz` & `tmp/pyalf-2.5.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalf-2.5.post5.tar", last modified: Wed Apr 17 19:42:33 2024, max compression
+gzip compressed data, was "pyalf-2.5.post6.tar", last modified: Wed Apr 17 20:37:32 2024, max compression
```

## Comparing `pyalf-2.5.post5.tar` & `pyalf-2.5.post6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:42:33.028179 pyalf-2.5.post5/
--rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 19:42:20.000000 pyalf-2.5.post5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 19:42:20.000000 pyalf-2.5.post5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 19:42:33.028179 pyalf-2.5.post5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-17 19:42:20.000000 pyalf-2.5.post5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:42:33.028179 pyalf-2.5.post5/pyALF.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 19:42:33.000000 pyalf-2.5.post5/pyALF.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 19:42:33.000000 pyalf-2.5.post5/pyALF.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 19:42:33.000000 pyalf-2.5.post5/pyALF.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 19:42:33.000000 pyalf-2.5.post5/pyALF.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 19:42:33.000000 pyalf-2.5.post5/pyALF.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 19:42:33.000000 pyalf-2.5.post5/pyALF.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:42:33.024179 pyalf-2.5.post5/py_alf/
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/alf_source.py
--rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/ana.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/check_common.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/check_rebin_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/check_rebin_tk.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/check_warmup_ipy.py
--rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/check_warmup_tk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:42:33.028179 pyalf-2.5.post5/py_alf/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/alf_bin_count.py
--rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/alf_del_bins.py
--rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/alf_postprocess.py
--rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/alf_run.py
--rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/alf_show_obs.py
--rwxrwxrwx   0 root         (0) root         (0)     6039 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/alf_test_branch.py
--rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/cli/minimal_ALF_run.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/init_layout.py
--rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/lattice.py
--rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/lattices_armv8.4-a.so
--rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/lattices_x86-64.so
--rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 19:42:20.000000 pyalf-2.5.post5/py_alf/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-04-17 19:42:20.000000 pyalf-2.5.post5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 19:42:33.028179 pyalf-2.5.post5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 19:42:33.028179 pyalf-2.5.post5/tests/
--rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 19:42:20.000000 pyalf-2.5.post5/tests/test_lattice_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:32.750496 pyalf-2.5.post6/
+-rw-rw-rw-   0 root         (0) root         (0)    18029 2024-04-17 20:37:20.000000 pyalf-2.5.post6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-17 20:37:20.000000 pyalf-2.5.post6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25994 2024-04-17 20:37:32.750496 pyalf-2.5.post6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-17 20:37:20.000000 pyalf-2.5.post6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:32.750496 pyalf-2.5.post6/pyALF.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25994 2024-04-17 20:37:32.000000 pyalf-2.5.post6/pyALF.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-17 20:37:32.000000 pyalf-2.5.post6/pyALF.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:37:32.000000 pyalf-2.5.post6/pyALF.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 20:37:32.000000 pyalf-2.5.post6/pyALF.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-17 20:37:32.000000 pyalf-2.5.post6/pyALF.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 20:37:32.000000 pyalf-2.5.post6/pyALF.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:32.750496 pyalf-2.5.post6/py_alf/
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/alf_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    27314 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/ana.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/check_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3445 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/check_rebin_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/check_rebin_tk.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/check_warmup_ipy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4313 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/check_warmup_tk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:32.750496 pyalf-2.5.post6/py_alf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1269 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/alf_bin_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     1136 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/alf_del_bins.py
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/alf_postprocess.py
+-rwxrwxrwx   0 root         (0) root         (0)     3124 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/alf_run.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/alf_show_obs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6039 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/alf_test_branch.py
+-rwxrwxrwx   0 root         (0) root         (0)     2035 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/cli/minimal_ALF_run.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/init_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)    18037 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/lattice.py
+-rwxrwxrwx   0 root         (0) root         (0)   103762 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/lattices_armv8.4-a.so
+-rwxrwxrwx   0 root         (0) root         (0)    97280 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/lattices_x86-64.so
+-rw-rw-rw-   0 root         (0) root         (0)    24446 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-17 20:37:20.000000 pyalf-2.5.post6/py_alf/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2024-04-17 20:37:20.000000 pyalf-2.5.post6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:37:32.750496 pyalf-2.5.post6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:37:32.750496 pyalf-2.5.post6/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     1288 2024-04-17 20:37:20.000000 pyalf-2.5.post6/tests/test_lattice_init.py
```

### Comparing `pyalf-2.5.post5/LICENSE` & `pyalf-2.5.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/PKG-INFO` & `pyalf-2.5.post6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: pyALF
-Version: 2.5.post5
-Summary: Python interface for ALF, plus scripts and Jupyter notebooks.
-Author-email: ALF Collaboration <alf@physik.uni-wuerzburg.de>, Jonas Schwab <jonas.schwab@uni-wuerzburg.de>
-Project-URL: Homepage, https://git.physik.uni-wuerzburg.de/ALF/pyALF
-Project-URL: Issues, https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: f90nml
-Requires-Dist: h5py
-Requires-Dist: ipympl
-Requires-Dist: ipywidgets
-Requires-Dist: matplotlib
-Requires-Dist: numba
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Provides-Extra: gui
-Requires-Dist: tkinter; extra == "gui"
-
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](http://unitary.fund)
 
 ## pyALF
 
 A Python package building on top of [ALF](https://git.physik.uni-wuerzburg.de/ALF/ALF), meant to simplify the different steps of working with ALF, including:
 
 * Obtaining and compiling the ALF source code
```

### Comparing `pyalf-2.5.post5/pyALF.egg-info/SOURCES.txt` & `pyalf-2.5.post6/pyALF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/__init__.py` & `pyalf-2.5.post6/py_alf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/alf_source.py` & `pyalf-2.5.post6/py_alf/alf_source.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/ana.py` & `pyalf-2.5.post6/py_alf/ana.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/analysis.py` & `pyalf-2.5.post6/py_alf/analysis.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/check_common.py` & `pyalf-2.5.post6/py_alf/check_common.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/check_rebin_ipy.py` & `pyalf-2.5.post6/py_alf/check_rebin_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/check_rebin_tk.py` & `pyalf-2.5.post6/py_alf/check_rebin_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/check_warmup_ipy.py` & `pyalf-2.5.post6/py_alf/check_warmup_ipy.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/check_warmup_tk.py` & `pyalf-2.5.post6/py_alf/check_warmup_tk.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/alf_bin_count.py` & `pyalf-2.5.post6/py_alf/cli/alf_bin_count.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/alf_del_bins.py` & `pyalf-2.5.post6/py_alf/cli/alf_del_bins.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/alf_postprocess.py` & `pyalf-2.5.post6/py_alf/cli/alf_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/alf_run.py` & `pyalf-2.5.post6/py_alf/cli/alf_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/alf_show_obs.py` & `pyalf-2.5.post6/py_alf/cli/alf_show_obs.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/alf_test_branch.py` & `pyalf-2.5.post6/py_alf/cli/alf_test_branch.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/cli/minimal_ALF_run.py` & `pyalf-2.5.post6/py_alf/cli/minimal_ALF_run.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/init_layout.py` & `pyalf-2.5.post6/py_alf/init_layout.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/lattice.py` & `pyalf-2.5.post6/py_alf/lattice.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/lattices_armv8.4-a.so` & `pyalf-2.5.post6/py_alf/lattices_armv8.4-a.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/lattices_x86-64.so` & `pyalf-2.5.post6/py_alf/lattices_x86-64.so`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/simulation.py` & `pyalf-2.5.post6/py_alf/simulation.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/py_alf/utils.py` & `pyalf-2.5.post6/py_alf/utils.py`

 * *Files identical despite different names*

### Comparing `pyalf-2.5.post5/pyproject.toml` & `pyalf-2.5.post6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 dynamic = ["version"]
 name = "pyALF"
 authors = [
   { name="ALF Collaboration", email="alf@physik.uni-wuerzburg.de" },
   { name="Jonas Schwab", email="jonas.schwab@uni-wuerzburg.de" },
 ]
 description = "Python interface for ALF, plus scripts and Jupyter notebooks."
+license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+    "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "f90nml",
   "h5py",
   "ipympl",
   "ipywidgets",
@@ -39,16 +40,18 @@
 [project.optional-dependencies]
 GUI = ["tkinter"]
 
 [tool.setuptools.packages.find]
 include = ["py_alf", "py_alf.cli"]
 
 [project.urls]
-Homepage = "https://git.physik.uni-wuerzburg.de/ALF/pyALF"
+Documentation = "https://gitpages.physik.uni-wuerzburg.de/Jonas_schwab/pyalf-docu/source/front.html"
+Repository = "https://git.physik.uni-wuerzburg.de/ALF/pyALF"
 Issues = "https://git.physik.uni-wuerzburg.de/ALF/pyALF/-/issues"
+"ALF Homepage" = "https://alf.physik.uni-wuerzburg.de/"
 
 [project.scripts]
 alf_bin_count = 'py_alf.cli.alf_bin_count:_main'
 alf_del_bins = 'py_alf.cli.alf_del_bins:_main'
 alf_postprocess = 'py_alf.cli.alf_postprocess:_main'
 alf_run = 'py_alf.cli.alf_run:_main'
 alf_show_obs = 'py_alf.cli.alf_show_obs:_main'
```

### Comparing `pyalf-2.5.post5/tests/test_lattice_init.py` & `pyalf-2.5.post6/tests/test_lattice_init.py`

 * *Files identical despite different names*


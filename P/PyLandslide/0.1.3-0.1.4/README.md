# Comparing `tmp/PyLandslide-0.1.3.tar.gz` & `tmp/PyLandslide-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLandslide-0.1.3.tar", last modified: Thu Mar  7 03:13:56 2024, max compression
+gzip compressed data, was "PyLandslide-0.1.4.tar", last modified: Thu Apr 25 12:23:48 2024, max compression
```

## Comparing `PyLandslide-0.1.3.tar` & `PyLandslide-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 03:13:56.201300 PyLandslide-0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-12-01 01:14:16.000000 PyLandslide-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3431 2024-03-07 03:13:56.200303 PyLandslide-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-07 03:13:56.188344 PyLandslide-0.1.3/PyLandslide/
--rw-rw-rw-   0        0        0       54 2023-12-01 01:14:16.000000 PyLandslide-0.1.3/PyLandslide/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-12-01 01:52:39.000000 PyLandslide-0.1.3/PyLandslide/cli.py
--rw-rw-rw-   0        0        0    12096 2024-03-06 22:59:41.000000 PyLandslide-0.1.3/PyLandslide/data_preparation.py
--rw-rw-rw-   0        0        0    14905 2023-12-01 01:14:16.000000 PyLandslide-0.1.3/PyLandslide/sensitivity.py
--rw-rw-rw-   0        0        0    10112 2023-12-01 01:14:16.000000 PyLandslide-0.1.3/PyLandslide/weightrange.py
-drwxrwxrwx   0        0        0        0 2024-03-07 03:13:56.199307 PyLandslide-0.1.3/PyLandslide.egg-info/
--rw-rw-rw-   0        0        0     3431 2024-03-07 03:13:56.000000 PyLandslide-0.1.3/PyLandslide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-03-07 03:13:56.000000 PyLandslide-0.1.3/PyLandslide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 03:13:56.000000 PyLandslide-0.1.3/PyLandslide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-07 03:13:56.000000 PyLandslide-0.1.3/PyLandslide.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-03-07 03:13:56.000000 PyLandslide-0.1.3/PyLandslide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-07 03:13:56.000000 PyLandslide-0.1.3/PyLandslide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2596 2024-02-07 18:04:07.000000 PyLandslide-0.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-07 03:13:56.201300 PyLandslide-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1161 2024-03-07 03:13:04.000000 PyLandslide-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 03:13:56.198310 PyLandslide-0.1.3/tests/
--rw-rw-rw-   0        0        0      101 2023-12-01 01:14:17.000000 PyLandslide-0.1.3/tests/test_sensitivity.py
--rw-rw-rw-   0        0        0     3572 2023-12-01 01:14:17.000000 PyLandslide-0.1.3/tests/test_weightrange.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:23:48.737717 PyLandslide-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-12-01 01:14:16.000000 PyLandslide-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3921 2024-04-25 12:23:48.736720 PyLandslide-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 12:23:48.726753 PyLandslide-0.1.4/PyLandslide/
+-rw-rw-rw-   0        0        0       54 2023-12-01 01:14:16.000000 PyLandslide-0.1.4/PyLandslide/__init__.py
+-rw-rw-rw-   0        0        0     3980 2023-12-01 01:52:39.000000 PyLandslide-0.1.4/PyLandslide/cli.py
+-rw-rw-rw-   0        0        0    12096 2024-04-25 12:21:45.000000 PyLandslide-0.1.4/PyLandslide/data_preparation.py
+-rw-rw-rw-   0        0        0    14905 2023-12-01 01:14:16.000000 PyLandslide-0.1.4/PyLandslide/sensitivity.py
+-rw-rw-rw-   0        0        0    10112 2023-12-01 01:14:16.000000 PyLandslide-0.1.4/PyLandslide/weightrange.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:23:48.732734 PyLandslide-0.1.4/PyLandslide.egg-info/
+-rw-rw-rw-   0        0        0     3921 2024-04-25 12:23:48.000000 PyLandslide-0.1.4/PyLandslide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-04-25 12:23:48.000000 PyLandslide-0.1.4/PyLandslide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:23:48.000000 PyLandslide-0.1.4/PyLandslide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-25 12:23:48.000000 PyLandslide-0.1.4/PyLandslide.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-25 12:23:48.000000 PyLandslide-0.1.4/PyLandslide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-25 12:23:48.000000 PyLandslide-0.1.4/PyLandslide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3064 2024-04-25 12:21:45.000000 PyLandslide-0.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:23:48.738713 PyLandslide-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2024-04-25 12:21:45.000000 PyLandslide-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:23:48.735724 PyLandslide-0.1.4/tests/
+-rw-rw-rw-   0        0        0      101 2023-12-01 01:14:17.000000 PyLandslide-0.1.4/tests/test_sensitivity.py
+-rw-rw-rw-   0        0        0     3572 2023-12-01 01:14:17.000000 PyLandslide-0.1.4/tests/test_weightrange.py
```

### Comparing `PyLandslide-0.1.3/LICENSE` & `PyLandslide-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.3/PKG-INFO` & `PyLandslide-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyLandslide
-Version: 0.1.3
-Summary: Tools for landslide hazard uncertainty analysis.
-Home-page: https://github.com/IERRG/PyLandslide
+Version: 0.1.4
+Summary: Tool for landslide susceptibility mapping and uncertainty analysis.
+Home-page: https://github.com/WRHGroup/PyLandslide
 Author: Mohammed Basheer
 Author-email: mohammedadamabbaker@gmail.com
 License: GNU
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
@@ -73,15 +73,16 @@
 
 Citation
 ========
 
 Please cite the following papers when using PyLandslide:
 
 
-    1. To be added.
+    1. Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
+    2. Basheer, M., Oommen, T., Takamatsu, M., Suzuki, S., 2022. Machine learning and sensitivity analysis approach to quantify uncertainty in landslide susceptibility mapping, Policy Research Working Paper. Washington, D.C. https://doi.org/10.1596/1813-9450-10264.
 
 
 License
 =======
 
 Copyright (C) 2023, `Mohammed Basheer <https://scholar.google.com/citations?user=KM_oVpkAAAAJ&hl=en>`__ and `Thomas Oommen <https://scholar.google.com/citations?user=EP89cqIAAAAJ&hl=en>`__.
```

### Comparing `PyLandslide-0.1.3/PyLandslide/cli.py` & `PyLandslide-0.1.4/PyLandslide/cli.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.3/PyLandslide/data_preparation.py` & `PyLandslide-0.1.4/PyLandslide/data_preparation.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.3/PyLandslide/sensitivity.py` & `PyLandslide-0.1.4/PyLandslide/sensitivity.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.3/PyLandslide/weightrange.py` & `PyLandslide-0.1.4/PyLandslide/weightrange.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.1.3/PyLandslide.egg-info/PKG-INFO` & `PyLandslide-0.1.4/PyLandslide.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyLandslide
-Version: 0.1.3
-Summary: Tools for landslide hazard uncertainty analysis.
-Home-page: https://github.com/IERRG/PyLandslide
+Version: 0.1.4
+Summary: Tool for landslide susceptibility mapping and uncertainty analysis.
+Home-page: https://github.com/WRHGroup/PyLandslide
 Author: Mohammed Basheer
 Author-email: mohammedadamabbaker@gmail.com
 License: GNU
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
@@ -73,15 +73,16 @@
 
 Citation
 ========
 
 Please cite the following papers when using PyLandslide:
 
 
-    1. To be added.
+    1. Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
+    2. Basheer, M., Oommen, T., Takamatsu, M., Suzuki, S., 2022. Machine learning and sensitivity analysis approach to quantify uncertainty in landslide susceptibility mapping, Policy Research Working Paper. Washington, D.C. https://doi.org/10.1596/1813-9450-10264.
 
 
 License
 =======
 
 Copyright (C) 2023, `Mohammed Basheer <https://scholar.google.com/citations?user=KM_oVpkAAAAJ&hl=en>`__ and `Thomas Oommen <https://scholar.google.com/citations?user=EP89cqIAAAAJ&hl=en>`__.
```

### Comparing `PyLandslide-0.1.3/README.rst` & `PyLandslide-0.1.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 
 Citation
 ========
 
 Please cite the following papers when using PyLandslide:
 
 
-    1. To be added.
+    1. Basheer, M., Oommen, T., 2024. PyLandslide: A Python tool for landslide susceptibility mapping and uncertainty analysis. Environmental Modelling and Software. 106055. https://doi.org/10.1016/j.envsoft.2024.106055.
+    2. Basheer, M., Oommen, T., Takamatsu, M., Suzuki, S., 2022. Machine learning and sensitivity analysis approach to quantify uncertainty in landslide susceptibility mapping, Policy Research Working Paper. Washington, D.C. https://doi.org/10.1596/1813-9450-10264.
 
 
 License
 =======
 
 Copyright (C) 2023, `Mohammed Basheer <https://scholar.google.com/citations?user=KM_oVpkAAAAJ&hl=en>`__ and `Thomas Oommen <https://scholar.google.com/citations?user=EP89cqIAAAAJ&hl=en>`__.
```

### Comparing `PyLandslide-0.1.3/setup.py` & `PyLandslide-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='PyLandslide',
-    version='0.1.3',
+    version='0.1.4',
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    description='Tools for landslide hazard uncertainty analysis.',
-    url='https://github.com/IERRG/PyLandslide',
+    description='Tool for landslide susceptibility mapping and uncertainty analysis.',
+    url='https://github.com/WRHGroup/PyLandslide',
     author='Mohammed Basheer',
     author_email='mohammedadamabbaker@gmail.com',
     license='GNU',
     install_requires=['click','pandas','numpy','scikit-learn','geopandas','rasterio'],
     packages=find_packages(),
     package_data={
         'PyLandslide': ['json/*.json'],
```

### Comparing `PyLandslide-0.1.3/tests/test_weightrange.py` & `PyLandslide-0.1.4/tests/test_weightrange.py`

 * *Files identical despite different names*


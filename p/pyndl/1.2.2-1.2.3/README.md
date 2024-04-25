# Comparing `tmp/pyndl-1.2.2.tar.gz` & `tmp/pyndl-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyndl-1.2.2.tar", max compression
+gzip compressed data, was "pyndl-1.2.3.tar", max compression
```

## Comparing `pyndl-1.2.2.tar` & `pyndl-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1185 2023-11-28 13:52:08.417557 pyndl-1.2.2/LICENSE
--rw-r--r--   0        0        0     3686 2023-11-28 13:52:08.417557 pyndl-1.2.2/README.rst
--rw-r--r--   0        0        0     1687 2023-11-28 13:52:08.425557 pyndl-1.2.2/build.py
--rw-r--r--   0        0        0     2949 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/__init__.py
--rw-r--r--   0        0        0     7016 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/activation.py
--rw-r--r--   0        0        0     6224 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/corpus.py
--rw-r--r--   0        0        0     3749 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/correlation.py
--rw-r--r--   0        0        0     2103 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/correlation_openmp.pyx
--rw-r--r--   0        0        0     6102 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/count.py
--rw-r--r--   0        0        0      383 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/error_codes.pxd
--rw-r--r--   0        0        0     6984 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/io.py
--rw-r--r--   0        0        0    21304 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/ndl.py
--rw-r--r--   0        0        0    10619 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/ndl_openmp.pyx
--rw-r--r--   0        0        0     1034 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/ndl_parallel.pxd
--rw-r--r--   0        0        0    20197 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/ndl_parallel.pyx
--rw-r--r--   0        0        0    33122 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/preprocess.py
--rw-r--r--   0        0        0    44601 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyndl/wh.py
--rw-r--r--   0        0        0     2178 2023-11-28 13:52:08.433557 pyndl-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 pyndl-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1185 2024-04-25 17:14:29.543166 pyndl-1.2.3/LICENSE
+-rw-r--r--   0        0        0     3516 2024-04-25 17:14:29.543166 pyndl-1.2.3/README.rst
+-rw-r--r--   0        0        0     1687 2024-04-25 17:14:29.551166 pyndl-1.2.3/build.py
+-rw-r--r--   0        0        0     2949 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/__init__.py
+-rw-r--r--   0        0        0     7016 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/activation.py
+-rw-r--r--   0        0        0     6224 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/corpus.py
+-rw-r--r--   0        0        0     3749 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/correlation.py
+-rw-r--r--   0        0        0     2103 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/correlation_openmp.pyx
+-rw-r--r--   0        0        0     6102 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/count.py
+-rw-r--r--   0        0        0      383 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/error_codes.pxd
+-rw-r--r--   0        0        0     6984 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/io.py
+-rw-r--r--   0        0        0    21304 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/ndl.py
+-rw-r--r--   0        0        0    10619 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/ndl_openmp.pyx
+-rw-r--r--   0        0        0     1034 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/ndl_parallel.pxd
+-rw-r--r--   0        0        0    20197 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/ndl_parallel.pyx
+-rw-r--r--   0        0        0    33122 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/preprocess.py
+-rw-r--r--   0        0        0    44601 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyndl/wh.py
+-rw-r--r--   0        0        0     2241 2024-04-25 17:14:29.559167 pyndl-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4985 1970-01-01 00:00:00.000000 pyndl-1.2.3/PKG-INFO
```

### Comparing `pyndl-1.2.2/LICENSE` & `pyndl-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/README.rst` & `pyndl-1.2.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 .. image:: https://github.com/quantling/pyndl/actions/workflows/python-test.yml/badge.svg?branch=main
     :target: https://github.com/quantling/pyndl/actions/workflows/python-test.yml
 
 .. image:: https://codecov.io/gh/quantling/pyndl/branch/main/graph/badge.svg?token=2GWUXRA9PD
     :target: https://codecov.io/gh/quantling/pyndl
 
-.. image:: https://img.shields.io/lgtm/grade/python/g/quantling/pyndl.svg?logo=lgtm&logoWidth=18
-    :target: https://lgtm.com/projects/g/quantling/pyndl/context:python
-
 .. image:: https://img.shields.io/pypi/pyversions/pyndl.svg
     :target: https://pypi.python.org/pypi/pyndl/
 
 .. image:: https://img.shields.io/github/license/quantling/pyndl.svg
     :target: https://github.com/quantling/pyndl/blob/main/LICENSE
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.597964.svg
```

### Comparing `pyndl-1.2.2/build.py` & `pyndl-1.2.3/build.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/__init__.py` & `pyndl-1.2.3/pyndl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/activation.py` & `pyndl-1.2.3/pyndl/activation.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/corpus.py` & `pyndl-1.2.3/pyndl/corpus.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/correlation.py` & `pyndl-1.2.3/pyndl/correlation.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/correlation_openmp.pyx` & `pyndl-1.2.3/pyndl/correlation_openmp.pyx`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/count.py` & `pyndl-1.2.3/pyndl/count.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/io.py` & `pyndl-1.2.3/pyndl/io.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/ndl.py` & `pyndl-1.2.3/pyndl/ndl.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/ndl_openmp.pyx` & `pyndl-1.2.3/pyndl/ndl_openmp.pyx`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/ndl_parallel.pxd` & `pyndl-1.2.3/pyndl/ndl_parallel.pxd`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/ndl_parallel.pyx` & `pyndl-1.2.3/pyndl/ndl_parallel.pyx`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/preprocess.py` & `pyndl-1.2.3/pyndl/preprocess.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyndl/wh.py` & `pyndl-1.2.3/pyndl/wh.py`

 * *Files identical despite different names*

### Comparing `pyndl-1.2.2/pyproject.toml` & `pyndl-1.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyndl"
-version = "1.2.2"
+version = "1.2.3"
 description = "Naive discriminative learning implements learning and classification models based on the Rescorla-Wagner equations."
 
 license = "MIT"
 
 authors = ["Konstantin Sering <konstantin.sering@uni-tuebingen.de>",
            "Marc Weitz",
            "David-Elias Künstle",
@@ -24,37 +24,39 @@
                'Operating System :: MacOS',
                'Operating System :: Microsoft :: Windows',
                'Topic :: Scientific/Engineering',
                'Topic :: Scientific/Engineering :: Artificial Intelligence',
                'Topic :: Scientific/Engineering :: Information Analysis',]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"  # Compatible python versions must be declared here
-numpy = "^1.23.1"
-scipy = "^1.9.0"
-pandas = "^1.4.3"
-xarray = "^2022.6.0"
-netCDF4 = "^1.6.0"
-Cython = "^3.0.0"
+python = ">=3.9,<3.13"  # Compatible python versions must be declared here
+numpy = ">=1.24.1"
+scipy = ">=1.13.0"
+pandas = ">=1.4.3"
+xarray = ">=2022.6.0"
+netCDF4 = ">=1.6.0"
+Cython = ">=3.0.0"
+toml = ">=0.10.2"
+setuptools = ">=69.2.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
-pytest-cov = "^2.4"
-pydocstyle = "^6.1.1"
-flake8 = "^4.0.1"
-sphinx = "^1.4"
-sphinx_rtd_theme = "^1.0.0"
-notebook = "^6.4.10"
-seaborn = "^0.12.1"
-numpydoc = "^1.2"
-sphinx-copybutton = "^0.5.1"
-pylint = "^2.0.0"
-nbsphinx = "^0.8.8"
-vulture = "^2.3"
-Jinja2 = "<3.1.0"
+pytest = ">=7.0"
+pytest-cov = ">=2.4"
+pydocstyle = ">=6.1.1"
+flake8 = ">=4.0.1"
+sphinx = ">=1.4"
+sphinx_rtd_theme = ">=1.0.0"
+notebook = ">=6.4.10"
+seaborn = ">=0.12.1"
+numpydoc = ">=1.2"
+sphinx-copybutton = ">=0.5.1"
+pylint = ">=2.0.0"
+nbsphinx = ">=0.8.8"
+vulture = ">=2.3"
+Jinja2 = ">=3.1.3"
 
 [tool.pytest.ini_options]
 addopts = '--doctest-glob "*.rst"'
 
 [tool.pylint]
   [tool.pylint.basic]
   good-names = ["nn", "ii", "_", "jj", "df"]
```

### Comparing `pyndl-1.2.2/PKG-INFO` & `pyndl-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: pyndl
-Version: 1.2.2
+Version: 1.2.3
 Summary: Naive discriminative learning implements learning and classification models based on the Rescorla-Wagner equations.
 Home-page: https://pyndl.readthedocs.io/en/latest/
 License: MIT
 Author: Konstantin Sering
 Author-email: konstantin.sering@uni-tuebingen.de
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Dist: Cython (>=3.0.0,<4.0.0)
-Requires-Dist: netCDF4 (>=1.6.0,<2.0.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: scipy (>=1.9.0,<2.0.0)
-Requires-Dist: xarray (>=2022.6.0,<2023.0.0)
+Requires-Dist: Cython (>=3.0.0)
+Requires-Dist: netCDF4 (>=1.6.0)
+Requires-Dist: numpy (>=1.24.1)
+Requires-Dist: pandas (>=1.4.3)
+Requires-Dist: scipy (>=1.13.0)
+Requires-Dist: setuptools (>=69.2.0)
+Requires-Dist: toml (>=0.10.2)
+Requires-Dist: xarray (>=2022.6.0)
 Project-URL: Repository, https://github.com/quantling/pyndl
 Description-Content-Type: text/x-rst
 
 ===============================================
 Pyndl - Naive Discriminative Learning in Python
 ===============================================
 
 .. image:: https://github.com/quantling/pyndl/actions/workflows/python-test.yml/badge.svg?branch=main
     :target: https://github.com/quantling/pyndl/actions/workflows/python-test.yml
 
 .. image:: https://codecov.io/gh/quantling/pyndl/branch/main/graph/badge.svg?token=2GWUXRA9PD
     :target: https://codecov.io/gh/quantling/pyndl
 
-.. image:: https://img.shields.io/lgtm/grade/python/g/quantling/pyndl.svg?logo=lgtm&logoWidth=18
-    :target: https://lgtm.com/projects/g/quantling/pyndl/context:python
-
 .. image:: https://img.shields.io/pypi/pyversions/pyndl.svg
     :target: https://pypi.python.org/pypi/pyndl/
 
 .. image:: https://img.shields.io/github/license/quantling/pyndl.svg
     :target: https://github.com/quantling/pyndl/blob/main/LICENSE
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.597964.svg
```


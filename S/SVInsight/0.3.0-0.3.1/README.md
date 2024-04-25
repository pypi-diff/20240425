# Comparing `tmp/svinsight-0.3.0.tar.gz` & `tmp/svinsight-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svinsight-0.3.0.tar", last modified: Wed Apr 24 16:03:35 2024, max compression
+gzip compressed data, was "svinsight-0.3.1.tar", last modified: Thu Apr 25 18:20:11 2024, max compression
```

## Comparing `svinsight-0.3.0.tar` & `svinsight-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.993900 svinsight-0.3.0/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     1073 2024-04-12 14:13:08.000000 svinsight-0.3.0/LICENSE
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      982 2024-04-24 16:03:35.993697 svinsight-0.3.0/PKG-INFO
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     3082 2024-04-24 15:50:56.000000 svinsight-0.3.0/README.md
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.991435 svinsight-0.3.0/SVInsight/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       57 2024-04-24 15:57:57.000000 svinsight-0.3.0/SVInsight/__init__.py
--rw-r--r--   0 matthewpreisser   (501) staff       (20)    17061 2024-04-15 15:22:19.000000 svinsight-0.3.0/SVInsight/census_variables.py
--rw-r--r--   0 matthewpreisser   (501) staff       (20)    76938 2024-04-23 20:46:50.000000 svinsight-0.3.0/SVInsight/svi.py
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.993473 svinsight-0.3.0/SVInsight.egg-info/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      982 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/PKG-INFO
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      462 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/SOURCES.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)        1 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/dependency_links.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       86 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/requires.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       10 2024-04-24 16:03:35.000000 svinsight-0.3.0/SVInsight.egg-info/top_level.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     1057 2024-04-24 15:58:08.000000 svinsight-0.3.0/pyproject.toml
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       38 2024-04-24 16:03:35.993939 svinsight-0.3.0/setup.cfg
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      828 2024-04-24 15:58:01.000000 svinsight-0.3.0/setup.py
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-24 16:03:35.993265 svinsight-0.3.0/tests/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     7918 2024-04-18 18:30:46.000000 svinsight-0.3.0/tests/test_svinsight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:11.558405 svinsight-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-25 18:20:06.000000 svinsight-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-25 18:20:11.558405 svinsight-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-25 18:20:06.000000 svinsight-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:11.554405 svinsight-0.3.1/SVInsight/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 18:20:06.000000 svinsight-0.3.1/SVInsight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-25 18:20:06.000000 svinsight-0.3.1/SVInsight/census_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76938 2024-04-25 18:20:06.000000 svinsight-0.3.1/SVInsight/svi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:11.558405 svinsight-0.3.1/SVInsight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-25 18:20:11.000000 svinsight-0.3.1/SVInsight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-25 18:20:11.000000 svinsight-0.3.1/SVInsight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:20:11.000000 svinsight-0.3.1/SVInsight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 18:20:11.000000 svinsight-0.3.1/SVInsight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 18:20:11.000000 svinsight-0.3.1/SVInsight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 18:20:06.000000 svinsight-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:20:11.558405 svinsight-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-25 18:20:06.000000 svinsight-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:11.558405 svinsight-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-25 18:20:07.000000 svinsight-0.3.1/tests/test_svinsight.py
```

### Comparing `svinsight-0.3.0/LICENSE` & `svinsight-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.0/README.md` & `svinsight-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SVInsight: Social Vulnerability Index Creation 
 ![pages-build-deployment](https://github.com/mdp0023/SVInsight/actions/workflows/pages/pages-build-deployment/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/svinsight)
 [![PyPI version](https://badge.fury.io/py/svinsight.svg)](https://badge.fury.io/py/svinsight)
 
 
-SVInsight is a python package for calculating an exploratory social vulnerability index. This package calculates SVI using two methods: (1) an iterative factor analysis method and (2) a rank method, both of which have been heavily utilized in scholarly research. This package automates the creation and comparisons of indices using U.S. American Community Survey 5-Year Data (ACS5) at the block group or tract level. Users can customize which social, demographic, and economic variables are included in their own custom indices.
+*SVInsight* is a python package for calculating an exploratory social vulnerability index. This package calculates SVI using two methods: (1) an iterative factor analysis method and (2) a rank method, both of which have been heavily utilized in scholarly research. This package automates the creation and comparisons of indices using U.S. American Community Survey 5-Year Data (ACS5) at the block group or tract level. Users can customize which social, demographic, and economic variables are included in their own custom indices.
 
 This package is a tool to efficiently calculate an exploratory estimate of social vulnerability for a given region. Social vulnerability is an incredibly complex and constantly evolving concept, and researchers, practitioners, and users of this software should always consult relevant peer-reviewed literature and local experts to validate findings.
 
 For user guides, examples, and a more indepth discussion of social vulnerability indices, refer to the [documentation](https://mdp0023.github.io/SVInsight/).
 
 
 
@@ -16,17 +16,14 @@
 *Travis County SVI estimates from 2013 to 2021*
 
 ## Installation: 
 To quickly install the package, use `pip` to install via PyPI:
     
     pip install SVInsight
 
-SVInsight will be avialable via conda-forge in the near future.
-
-
 SVInsight can then be imported into python:
 
     >>> from SVInsight import SVInsight as svi
 
 
 ## Contributing
 We welcome contributions to SVInsight. Please open an issue or a pull request if there is functionality you would like to see or propose. Refer to our [contributing guide](https://mdp0023.github.io/SVInsight/Contributions/contributions.htmll) for more information.
```

### Comparing `svinsight-0.3.0/SVInsight/census_variables.py` & `svinsight-0.3.1/SVInsight/census_variables.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.0/SVInsight/svi.py` & `svinsight-0.3.1/SVInsight/svi.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.0/pyproject.toml` & `svinsight-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SVInsight"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
     "census",
     "factor_analyzer",
     "geopandas",
     "numpy",
     "pandas",
     "PyYAML",
@@ -20,15 +20,15 @@
 authors = [
   {name = "Matthew Preisser", email = "mattpreisser@gmail.com"},
   {name = "Paola Passalacqua"},
   {name = "R. Patrick Bixler"}
 
 ]
 description = "Create social vulnerabilty index"
-readme = "README.rst"
+readme = "README.md"
 license = {file = "LICENSE.txt"}
 keywords = ["SVI",
             "Social-Vulnerability",
             "Hazards",
             "Census",
             "Demographics"]
 classifiers = [
```

### Comparing `svinsight-0.3.0/setup.py` & `svinsight-0.3.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import os
 from setuptools import setup, find_packages
 #from SVInsight import __version__ as version
 
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
+
 setup(
     name='SVInsight',
-    version='0.3.0',
+    version='0.3.1',
     license='MIT',
     description='SVInsight - A python package for calculating an exploratory social vulnerability index',
     author='M. Preisser, P. Passalacqua, R. P. Bixler',
     author_email='mattpreisser@gmail.com',
     url='https://github.com/mdp0023/SVInsight/',
     packages= find_packages(exclude=['*.tests']),
     package_data = {'' : ['*.txt', '*.npz']},
-    long_description = 'See preojct webpage for details',
+    long_description = long_description,
+    long_description_content_type='text/markdown',
     classifiers=[],
     install_requires=['census',
                     'factor_analyzer',
                     'geopandas',
                     'numpy',
                     'pandas',
                     'PyYAML',
```

### Comparing `svinsight-0.3.0/tests/test_svinsight.py` & `svinsight-0.3.1/tests/test_svinsight.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,58 +125,58 @@
 # create fixture of project
 @pytest.fixture
 def project():
     return svi(project_name, file_path, api_key, geoids)
 
 api_key = os.environ.get('API_KEY')
 
-# ##############################################################################################
-# # develop a test project for single county
-# project_name = 'test_project_single_county' 
-# file_path = os.path.dirname(os.path.realpath(__file__))
-# geoids = ['48453']
-# boundaries = ['bg', 'tract']
-# years = [2015, 2020]
-# config='config'
-
-# @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
-# def test_single_county_project(project, boundary, year, overwrite=False):
-#     """test creating and running a single county project for different years and boundaries"""
-#     run_svi_workflow(project, boundary, year, overwrite=overwrite)
-# ##############################################################################################
+##############################################################################################
+# develop a test project for single county
+project_name = 'test_project_single_county' 
+file_path = os.path.dirname(os.path.realpath(__file__))
+geoids = ['48453']
+boundaries = ['bg', 'tract']
+years = [2015, 2020]
+config='config'
+
+@pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
+def test_single_county_project(project, boundary, year, overwrite=False):
+    """test creating and running a single county project for different years and boundaries"""
+    run_svi_workflow(project, boundary, year, overwrite=overwrite)
+##############################################################################################
  
-# ##############################################################################################
-# # develop a test project for multiple counties
-# project_name = 'test_project_multiple_counties' 
-# file_path = os.path.dirname(os.path.realpath(__file__))
-# geoids = ['48453','21117']
-# boundaries = ['bg', 'tract']
-# years = [2015, 2020]
-# config='config'
-
-# @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
-# def test_multiple_county_project(project, boundary, year, overwrite=False):
-#     """test creating and running a multiple counties project for different years and boundaries"""
-#     run_svi_workflow(project, boundary, year, overwrite=overwrite)
-# ##############################################################################################
-
-# ##############################################################################################
-# # develop a test project for multiple states
-# project_name = 'test_project_multiple_states' 
-# file_path = os.path.dirname(os.path.realpath(__file__))
-# geoids = ['25','44']
-# boundaries = ['bg', 'tract']
-# years = [2015]
-# config='config'
-
-# @pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
-# def test_multiple_states_project(project, boundary, year, overwrite=False):
-#     """test creating and running a multiple states project for different years and boundaries"""
-#     run_svi_workflow(project, boundary, year, overwrite=overwrite)
-# ##############################################################################################
+##############################################################################################
+# develop a test project for multiple counties
+project_name = 'test_project_multiple_counties' 
+file_path = os.path.dirname(os.path.realpath(__file__))
+geoids = ['48453','21117']
+boundaries = ['bg', 'tract']
+years = [2015, 2020]
+config='config'
+
+@pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
+def test_multiple_county_project(project, boundary, year, overwrite=False):
+    """test creating and running a multiple counties project for different years and boundaries"""
+    run_svi_workflow(project, boundary, year, overwrite=overwrite)
+##############################################################################################
+
+##############################################################################################
+# develop a test project for multiple states
+project_name = 'test_project_multiple_states' 
+file_path = os.path.dirname(os.path.realpath(__file__))
+geoids = ['25','44']
+boundaries = ['bg', 'tract']
+years = [2015]
+config='config'
+
+@pytest.mark.parametrize("boundary, year", [(b, y) for b in boundaries for y in years])
+def test_multiple_states_project(project, boundary, year, overwrite=False):
+    """test creating and running a multiple states project for different years and boundaries"""
+    run_svi_workflow(project, boundary, year, overwrite=overwrite)
+##############################################################################################
 
 ##############################################################################################
 # develop a test project for single county, economic index
 project_name = 'test_project_economic_index' 
 file_path = os.path.dirname(os.path.realpath(__file__))
 geoids = ['48453']
 boundaries = ['bg']
```


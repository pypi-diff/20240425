# Comparing `tmp/polar_route-0.3.9.tar.gz` & `tmp/polar_route-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_route-0.3.9.tar", last modified: Thu Nov 30 17:33:47 2023, max compression
+gzip compressed data, was "polar_route-0.4.0.tar", last modified: Thu Apr 25 15:05:22 2024, max compression
```

## Comparing `polar_route-0.3.9.tar` & `polar_route-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-30 17:33:47.124286 polar_route-0.3.9/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-05-18 13:54:43.000000 polar_route-0.3.9/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2023-11-22 13:09:49.000000 polar_route-0.3.9/MANIFEST.in
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5001 2023-11-30 17:33:47.120286 polar_route-0.3.9/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3862 2023-08-11 08:35:36.000000 polar_route-0.3.9/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-30 17:33:47.116286 polar_route-0.3.9/polar_route/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1025 2023-11-30 17:33:37.000000 polar_route-0.3.9/polar_route/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6923 2023-11-21 15:32:49.000000 polar_route-0.3.9/polar_route/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-30 17:33:47.120286 polar_route-0.3.9/polar_route/config_validation/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-08-11 08:54:10.000000 polar_route-0.3.9/polar_route/config_validation/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4110 2023-09-26 08:38:57.000000 polar_route-0.3.9/polar_route/config_validation/config_validator.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1144 2023-08-11 08:54:10.000000 polar_route-0.3.9/polar_route/config_validation/route_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      481 2023-09-26 08:38:57.000000 polar_route-0.3.9/polar_route/config_validation/vessel_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       64 2023-08-11 08:54:10.000000 polar_route-0.3.9/polar_route/config_validation/waypoints_schema.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    18891 2023-08-11 08:54:10.000000 polar_route-0.3.9/polar_route/crossing.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    67444 2023-11-30 11:26:37.000000 polar_route-0.3.9/polar_route/crossing_smoothing.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    13029 2023-11-21 15:32:49.000000 polar_route-0.3.9/polar_route/route_calc.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    33080 2023-11-30 17:33:37.000000 polar_route-0.3.9/polar_route/route_planner.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11275 2023-11-21 15:32:49.000000 polar_route-0.3.9/polar_route/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-30 17:33:47.120286 polar_route-0.3.9/polar_route/vessel_performance/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.3.9/polar_route/vessel_performance/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1397 2023-11-08 10:37:37.000000 polar_route-0.3.9/polar_route/vessel_performance/abstract_vessel.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1445 2023-11-22 13:09:49.000000 polar_route-0.3.9/polar_route/vessel_performance/vessel_factory.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3181 2023-11-08 10:37:37.000000 polar_route-0.3.9/polar_route/vessel_performance/vessel_performance_modeller.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-30 17:33:47.120286 polar_route-0.3.9/polar_route/vessel_performance/vessels/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11678 2023-11-08 10:37:37.000000 polar_route-0.3.9/polar_route/vessel_performance/vessels/SDA.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.3.9/polar_route/vessel_performance/vessels/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5418 2023-11-08 10:37:37.000000 polar_route-0.3.9/polar_route/vessel_performance/vessels/abstract_glider.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6983 2023-11-22 13:09:49.000000 polar_route-0.3.9/polar_route/vessel_performance/vessels/abstract_ship.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2404 2023-11-08 10:37:37.000000 polar_route-0.3.9/polar_route/vessel_performance/vessels/slocum.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-11-30 17:33:47.120286 polar_route-0.3.9/polar_route.egg-info/
--rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5001 2023-11-30 17:33:47.000000 polar_route-0.3.9/polar_route.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1160 2023-11-30 17:33:47.000000 polar_route-0.3.9/polar_route.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-11-30 17:33:47.000000 polar_route-0.3.9/polar_route.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      232 2023-11-30 17:33:47.000000 polar_route-0.3.9/polar_route.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-09-01 09:10:15.000000 polar_route-0.3.9/polar_route.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      149 2023-11-30 17:33:47.000000 polar_route-0.3.9/polar_route.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-11-30 17:33:47.000000 polar_route-0.3.9/polar_route.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2023-11-30 17:33:47.124286 polar_route-0.3.9/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1791 2023-11-22 10:18:46.000000 polar_route-0.3.9/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 15:05:22.542345 polar_route-0.4.0/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-05-18 13:54:43.000000 polar_route-0.4.0/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2024-04-11 13:48:07.000000 polar_route-0.4.0/MANIFEST.in
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5248 2024-04-25 15:05:22.542345 polar_route-0.4.0/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4201 2024-04-17 08:34:55.000000 polar_route-0.4.0/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 15:05:22.538345 polar_route-0.4.0/polar_route/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      987 2024-04-25 15:02:31.000000 polar_route-0.4.0/polar_route/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    10958 2024-04-25 15:02:24.000000 polar_route-0.4.0/polar_route/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 15:05:22.538345 polar_route-0.4.0/polar_route/config_validation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/config_validation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4110 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/config_validation/config_validator.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1144 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/config_validation/route_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      481 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/config_validation/vessel_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       64 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/config_validation/waypoints_schema.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    18891 2024-04-11 13:27:48.000000 polar_route-0.4.0/polar_route/crossing.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    67588 2024-04-17 08:34:55.000000 polar_route-0.4.0/polar_route/crossing_smoothing.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    14283 2024-04-17 08:34:55.000000 polar_route-0.4.0/polar_route/route_calc.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    41253 2024-04-25 15:02:31.000000 polar_route-0.4.0/polar_route/route_planner.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    14697 2024-04-11 13:28:05.000000 polar_route-0.4.0/polar_route/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 15:05:22.538345 polar_route-0.4.0/polar_route/vessel_performance/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.4.0/polar_route/vessel_performance/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1397 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/vessel_performance/abstract_vessel.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1765 2024-04-17 08:34:55.000000 polar_route-0.4.0/polar_route/vessel_performance/vessel_factory.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5528 2024-04-25 15:02:31.000000 polar_route-0.4.0/polar_route/vessel_performance/vessel_performance_modeller.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 15:05:22.542345 polar_route-0.4.0/polar_route/vessel_performance/vessels/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11678 2024-02-13 15:14:33.000000 polar_route-0.4.0/polar_route/vessel_performance/vessels/SDA.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.4.0/polar_route/vessel_performance/vessels/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5418 2024-04-10 12:48:44.000000 polar_route-0.4.0/polar_route/vessel_performance/vessels/abstract_glider.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     6983 2024-04-11 13:48:07.000000 polar_route-0.4.0/polar_route/vessel_performance/vessels/abstract_ship.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11567 2024-04-11 13:28:05.000000 polar_route-0.4.0/polar_route/vessel_performance/vessels/example_ship.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2404 2024-04-17 08:34:55.000000 polar_route-0.4.0/polar_route/vessel_performance/vessels/slocum.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2024-04-25 15:05:22.538345 polar_route-0.4.0/polar_route.egg-info/
+-rw-r--r--   0 gecoomb   (1001) gecoomb   (1001)     5248 2024-04-25 15:05:22.000000 polar_route-0.4.0/polar_route.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1230 2024-04-25 15:05:22.000000 polar_route-0.4.0/polar_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2024-04-25 15:05:22.000000 polar_route-0.4.0/polar_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      284 2024-04-25 15:05:22.000000 polar_route-0.4.0/polar_route.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-09-01 09:10:15.000000 polar_route-0.4.0/polar_route.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      151 2024-04-25 15:05:22.000000 polar_route-0.4.0/polar_route.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2024-04-25 15:05:22.000000 polar_route-0.4.0/polar_route.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       80 2024-02-15 11:34:54.000000 polar_route-0.4.0/pyproject.toml
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2024-04-25 15:05:22.542345 polar_route-0.4.0/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1842 2024-04-25 15:03:03.000000 polar_route-0.4.0/setup.py
```

### Comparing `polar_route-0.3.9/LICENSE` & `polar_route-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/PKG-INFO` & `polar_route-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 Metadata-Version: 2.1
 Name: polar_route
-Version: 0.3.9
+Version: 0.4.0
 Summary: PolarRoute: Long-distance maritime polar route planning taking into account complex changing environmental conditions
 Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox
-Author-email: polarroute@bas.ac.uk
-Maintainer: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox
-Maintainer-email: polarroute@bas.ac.uk
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk
 License: MIT
-Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
-Classifier: 
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
+# PolarRoute
+
 ![](logo.jpg)
 
-<a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
 <a href="https://antarctica.github.io/PolarRoute/"><img src="https://img.shields.io/badge/Manual%20-github.io%2FPolarRoute%2F-red" alt="Manual Page">
-<a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPi">
+<a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
+<a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPI">
 <a href="https://github.com/antarctica/PolarRoute/tags"><img src="https://img.shields.io/github/v/tag/antarctica/PolarRoute" alt="Release Tag"></a>
 <a href="https://github.com/antarctica/PolarRoute/issues"><img src="https://img.shields.io/github/issues/antarctica/PolarRoute" alt="Issues"></a>
 <a href="https://github.com/antarctica/PolarRoute/blob/main/LICENSE"><img src="https://img.shields.io/github/license/antarctica/PolarRoute" alt="License"></a>
 
-# PolarRoute
-PolarRoute is a long-distance maritime polar route planning package, taking into account complex changing environmental conditions. The codebase allows the construction of optimised routes through three main stages: discrete modelling of the environmental conditions using a non-uniform mesh, the construction of mesh-optimal paths, and physics informed path smoothing. In order to account for different vehicle properties we construct a series of data driven functions that can be applied to the environmental mesh to determine the speed limitations and fuel requirements for a given vessel and mesh cell, representing these quantities graphically and geospatially.
+PolarRoute is a long-distance maritime polar route planning package, able to take into account complex and changing environmental conditions. It allows the construction of optimised routes through three main stages: discrete modelling of the environmental conditions using a non-uniform mesh, the construction of mesh-optimal paths, and physics informed path smoothing. In order to account for different vehicle properties we construct a series of data-driven functions that can be applied to the environmental mesh to determine the speed limitations and fuel requirements for a given vessel and mesh cell. The environmental modelling component of this functionality is provided by the [MeshiPhi](https://github.com/antarctica/MeshiPhi) library.
 
 ## Installation
-The PolarRoute package requires GDAL files to be installed. This software can be installed on Windows by running the required wheels for GDAL and FIONA. More information can be found in the manual pages linked above. Once these requirements are met then the software can be installed by:
 
-Github:
+PolarRoute is available from PyPI and can be installed by running: 
 ```
-git clone https://github.com/Antarctica/PolarRoute
-python setup.py install
+pip install polar-route
 ```
 
- Pip: 
+Alternatively you can install PolarRoute by downloading the source code from GitHub:
 ```
-pip install polar-route
+git clone https://github.com/Antarctica/PolarRoute
+pip install -e ./PolarRoute
 ```
+Use of `-e` is optional, based on whether you want to be able to edit the installed copy of the package.
 
-> NOTE: The installation process may vary slightly dependent on OS. Please consult the documentation for further installation guidance.
+> NOTE: Some features of the PolarRoute package require GDAL to be installed. Please consult the documentation for further guidance.
 
 ## Required Data sources
-Polar-route has been built to work with a variety of open-source atmospheric and oceanographic data sources. 
-A list of supported data sources and their associated data-loaders is given in the 
-'Data Loaders' section of the manual
+PolarRoute has been built to work with a variety of open-source atmospheric and oceanographic data sources. For testing and demonstration purposes it is also possible to generate artificial Gaussian Random Field data.  
+
+A full list of supported data sources and their associated dataloaders is given in the 
+'Dataloader Overview' section of the [MeshiPhi manual](https://antarctica.github.io/MeshiPhi/)
 
 ## Documentation
-Sphinx is used to generate documentation for this project. The dependencies can be installed through pip:
+The documentation for the package is available to read at: https://antarctica.github.io/PolarRoute/
+
+If you make changes to the source of the documentation you will need to rebuild the corresponding html files using Sphinx.
+The dependencies for this can be installed through pip:
 ```
 pip install sphinx sphinx_markdown_builder sphinx_rtd_theme rinohtype
 ```
 When updating the docs, run the following command within the PolarRoute directory to recompile.
 ```
 sphinx-build -b html ./docs/source ./docs/html
 ```
 Sometimes the cache needs to be cleared for internal links to update. If facing this problem, run this from the PolarRoute directory.
 ```
-rm -r docs/build/.doctrees/
+rm -r docs/html/.doctrees/
 ```
 ## Developers
-Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox, Harrison Abbot, Ayat Fekry
+Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 
 ## Collaboration
-We are currently assessing the best practice for collaboration on the codebase, until then please contact [polarroute@bas.ac.uk](polarroute@bas.ac.uk) for further info.
-
+We are currently assessing the best practice for collaboration on the codebase, until then please contact [amop@bas.ac.uk](amop@bas.ac.uk) for further info.
 
 ## License
 This software is licensed under a MIT license, but request users cite our publication.  
 
-Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne,  J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox,  (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
+Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne, J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox, (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
 
 For more information please see the attached ``LICENSE`` file. 
 
 [version]: https://img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square
```

#### html2text {}

```diff
@@ -1,54 +1,58 @@
-Metadata-Version: 2.1 Name: polar_route Version: 0.3.9 Summary: PolarRoute:
+Metadata-Version: 2.1 Name: polar_route Version: 0.4.0 Summary: PolarRoute:
 Long-distance maritime polar route planning taking into account complex
 changing environmental conditions Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry,
-James Byrne, Michael Thorne, Maria Fox Author-email: polarroute@bas.ac.uk
-Maintainer: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat
-Fekry, James Byrne, Michael Thorne, Maria Fox Maintainer-email:
-polarroute@bas.ac.uk License: MIT Classifier: Classifier: Development Status ::
-3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: System Administrators Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Topic :: Scientific/Engineering Classifier: Description-
-Content-Type: text/markdown Provides-Extra: tests License-File: LICENSE ![]
-(logo.jpg) _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_#
-_P_o_l_a_r_R_o_u_t_e_ _P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_ _l_o_n_g_-_d_i_s_t_a_n_c_e_ _m_a_r_i_t_i_m_e_ _p_o_l_a_r_ _r_o_u_t_e_ _p_l_a_n_n_i_n_g_ _p_a_c_k_a_g_e_,
-_t_a_k_i_n_g_ _i_n_t_o_ _a_c_c_o_u_n_t_ _c_o_m_p_l_e_x_ _c_h_a_n_g_i_n_g_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_._ _T_h_e_ _c_o_d_e_b_a_s_e
-_a_l_l_o_w_s_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _o_p_t_i_m_i_s_e_d_ _r_o_u_t_e_s_ _t_h_r_o_u_g_h_ _t_h_r_e_e_ _m_a_i_n_ _s_t_a_g_e_s_:_ _d_i_s_c_r_e_t_e
-_m_o_d_e_l_l_i_n_g_ _o_f_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_ _u_s_i_n_g_ _a_ _n_o_n_-_u_n_i_f_o_r_m_ _m_e_s_h_,_ _t_h_e
-_c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _m_e_s_h_-_o_p_t_i_m_a_l_ _p_a_t_h_s_,_ _a_n_d_ _p_h_y_s_i_c_s_ _i_n_f_o_r_m_e_d_ _p_a_t_h_ _s_m_o_o_t_h_i_n_g_._ _I_n
-_o_r_d_e_r_ _t_o_ _a_c_c_o_u_n_t_ _f_o_r_ _d_i_f_f_e_r_e_n_t_ _v_e_h_i_c_l_e_ _p_r_o_p_e_r_t_i_e_s_ _w_e_ _c_o_n_s_t_r_u_c_t_ _a_ _s_e_r_i_e_s_ _o_f_ _d_a_t_a
-_d_r_i_v_e_n_ _f_u_n_c_t_i_o_n_s_ _t_h_a_t_ _c_a_n_ _b_e_ _a_p_p_l_i_e_d_ _t_o_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_e_s_h_ _t_o_ _d_e_t_e_r_m_i_n_e_ _t_h_e
-_s_p_e_e_d_ _l_i_m_i_t_a_t_i_o_n_s_ _a_n_d_ _f_u_e_l_ _r_e_q_u_i_r_e_m_e_n_t_s_ _f_o_r_ _a_ _g_i_v_e_n_ _v_e_s_s_e_l_ _a_n_d_ _m_e_s_h_ _c_e_l_l_,
-_r_e_p_r_e_s_e_n_t_i_n_g_ _t_h_e_s_e_ _q_u_a_n_t_i_t_i_e_s_ _g_r_a_p_h_i_c_a_l_l_y_ _a_n_d_ _g_e_o_s_p_a_t_i_a_l_l_y_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e
-_P_o_l_a_r_R_o_u_t_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_s_ _G_D_A_L_ _f_i_l_e_s_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_._ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _c_a_n_ _b_e
-_i_n_s_t_a_l_l_e_d_ _o_n_ _W_i_n_d_o_w_s_ _b_y_ _r_u_n_n_i_n_g_ _t_h_e_ _r_e_q_u_i_r_e_d_ _w_h_e_e_l_s_ _f_o_r_ _G_D_A_L_ _a_n_d_ _F_I_O_N_A_._ _M_o_r_e
-_i_n_f_o_r_m_a_t_i_o_n_ _c_a_n_ _b_e_ _f_o_u_n_d_ _i_n_ _t_h_e_ _m_a_n_u_a_l_ _p_a_g_e_s_ _l_i_n_k_e_d_ _a_b_o_v_e_._ _O_n_c_e_ _t_h_e_s_e
-_r_e_q_u_i_r_e_m_e_n_t_s_ _a_r_e_ _m_e_t_ _t_h_e_n_ _t_h_e_ _s_o_f_t_w_a_r_e_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _b_y_:_ _G_i_t_h_u_b_:_ _`_`_`_ _g_i_t
-_c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_P_o_l_a_r_R_o_u_t_e_ _p_y_t_h_o_n_ _s_e_t_u_p_._p_y_ _i_n_s_t_a_l_l_ _`_`_`_ _P_i_p_:
-_`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_o_l_a_r_-_r_o_u_t_e_ _`_`_`_ _>_ _N_O_T_E_:_ _T_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s_ _m_a_y_ _v_a_r_y
-_s_l_i_g_h_t_l_y_ _d_e_p_e_n_d_e_n_t_ _o_n_ _O_S_._ _P_l_e_a_s_e_ _c_o_n_s_u_l_t_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _f_u_r_t_h_e_r
-_i_n_s_t_a_l_l_a_t_i_o_n_ _g_u_i_d_a_n_c_e_._ _#_#_ _R_e_q_u_i_r_e_d_ _D_a_t_a_ _s_o_u_r_c_e_s_ _P_o_l_a_r_-_r_o_u_t_e_ _h_a_s_ _b_e_e_n_ _b_u_i_l_t_ _t_o
-_w_o_r_k_ _w_i_t_h_ _a_ _v_a_r_i_e_t_y_ _o_f_ _o_p_e_n_-_s_o_u_r_c_e_ _a_t_m_o_s_p_h_e_r_i_c_ _a_n_d_ _o_c_e_a_n_o_g_r_a_p_h_i_c_ _d_a_t_a_ _s_o_u_r_c_e_s_.
-_A_ _l_i_s_t_ _o_f_ _s_u_p_p_o_r_t_e_d_ _d_a_t_a_ _s_o_u_r_c_e_s_ _a_n_d_ _t_h_e_i_r_ _a_s_s_o_c_i_a_t_e_d_ _d_a_t_a_-_l_o_a_d_e_r_s_ _i_s_ _g_i_v_e_n_ _i_n
-_t_h_e_ _'_D_a_t_a_ _L_o_a_d_e_r_s_'_ _s_e_c_t_i_o_n_ _o_f_ _t_h_e_ _m_a_n_u_a_l_ _#_#_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_p_h_i_n_x_ _i_s_ _u_s_e_d_ _t_o
-_g_e_n_e_r_a_t_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _t_h_i_s_ _p_r_o_j_e_c_t_._ _T_h_e_ _d_e_p_e_n_d_e_n_c_i_e_s_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d
-_t_h_r_o_u_g_h_ _p_i_p_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _s_p_h_i_n_x_ _s_p_h_i_n_x___m_a_r_k_d_o_w_n___b_u_i_l_d_e_r_ _s_p_h_i_n_x___r_t_d___t_h_e_m_e
-_r_i_n_o_h_t_y_p_e_ _`_`_`_ _W_h_e_n_ _u_p_d_a_t_i_n_g_ _t_h_e_ _d_o_c_s_,_ _r_u_n_ _t_h_e_ _f_o_l_l_o_w_i_n_g_ _c_o_m_m_a_n_d_ _w_i_t_h_i_n_ _t_h_e
-_P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_ _t_o_ _r_e_c_o_m_p_i_l_e_._ _`_`_`_ _s_p_h_i_n_x_-_b_u_i_l_d_ _-_b_ _h_t_m_l_ _._/_d_o_c_s_/_s_o_u_r_c_e_ _._/
-_d_o_c_s_/_h_t_m_l_ _`_`_`_ _S_o_m_e_t_i_m_e_s_ _t_h_e_ _c_a_c_h_e_ _n_e_e_d_s_ _t_o_ _b_e_ _c_l_e_a_r_e_d_ _f_o_r_ _i_n_t_e_r_n_a_l_ _l_i_n_k_s_ _t_o
-_u_p_d_a_t_e_._ _I_f_ _f_a_c_i_n_g_ _t_h_i_s_ _p_r_o_b_l_e_m_,_ _r_u_n_ _t_h_i_s_ _f_r_o_m_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_._ _`_`_`_ _r_m
-_-_r_ _d_o_c_s_/_b_u_i_l_d_/_._d_o_c_t_r_e_e_s_/_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_e_r_s_ _J_o_n_a_t_h_a_n_ _S_m_i_t_h_,_ _S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e
-_C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _T_h_o_r_n_e_,_ _M_a_r_i_a_ _F_o_x_,_ _H_a_r_r_i_s_o_n_ _A_b_b_o_t_,_ _A_y_a_t_ _F_e_k_r_y_ _#_#
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British
+Antarctic Survey Author-email: amop@bas.ac.uk Maintainer: Autonomous Marine
+Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey Maintainer-
+email: amop@bas.ac.uk License: MIT Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: System Administrators Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
+markdown Provides-Extra: tests License-File: LICENSE # PolarRoute ![](logo.jpg)
+_[_M_a_n_u_a_l_ _P_a_g_e_]_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_P_y_P_I_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_P_o_l_a_r_R_o_u_t_e_ _i_s_ _a
+_l_o_n_g_-_d_i_s_t_a_n_c_e_ _m_a_r_i_t_i_m_e_ _p_o_l_a_r_ _r_o_u_t_e_ _p_l_a_n_n_i_n_g_ _p_a_c_k_a_g_e_,_ _a_b_l_e_ _t_o_ _t_a_k_e_ _i_n_t_o_ _a_c_c_o_u_n_t
+_c_o_m_p_l_e_x_ _a_n_d_ _c_h_a_n_g_i_n_g_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_._ _I_t_ _a_l_l_o_w_s_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f
+_o_p_t_i_m_i_s_e_d_ _r_o_u_t_e_s_ _t_h_r_o_u_g_h_ _t_h_r_e_e_ _m_a_i_n_ _s_t_a_g_e_s_:_ _d_i_s_c_r_e_t_e_ _m_o_d_e_l_l_i_n_g_ _o_f_ _t_h_e
+_e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_ _u_s_i_n_g_ _a_ _n_o_n_-_u_n_i_f_o_r_m_ _m_e_s_h_,_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _m_e_s_h_-
+_o_p_t_i_m_a_l_ _p_a_t_h_s_,_ _a_n_d_ _p_h_y_s_i_c_s_ _i_n_f_o_r_m_e_d_ _p_a_t_h_ _s_m_o_o_t_h_i_n_g_._ _I_n_ _o_r_d_e_r_ _t_o_ _a_c_c_o_u_n_t_ _f_o_r
+_d_i_f_f_e_r_e_n_t_ _v_e_h_i_c_l_e_ _p_r_o_p_e_r_t_i_e_s_ _w_e_ _c_o_n_s_t_r_u_c_t_ _a_ _s_e_r_i_e_s_ _o_f_ _d_a_t_a_-_d_r_i_v_e_n_ _f_u_n_c_t_i_o_n_s
+_t_h_a_t_ _c_a_n_ _b_e_ _a_p_p_l_i_e_d_ _t_o_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_e_s_h_ _t_o_ _d_e_t_e_r_m_i_n_e_ _t_h_e_ _s_p_e_e_d
+_l_i_m_i_t_a_t_i_o_n_s_ _a_n_d_ _f_u_e_l_ _r_e_q_u_i_r_e_m_e_n_t_s_ _f_o_r_ _a_ _g_i_v_e_n_ _v_e_s_s_e_l_ _a_n_d_ _m_e_s_h_ _c_e_l_l_._ _T_h_e
+_e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_o_d_e_l_l_i_n_g_ _c_o_m_p_o_n_e_n_t_ _o_f_ _t_h_i_s_ _f_u_n_c_t_i_o_n_a_l_i_t_y_ _i_s_ _p_r_o_v_i_d_e_d_ _b_y_ _t_h_e_ 
+_[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_ _l_i_b_r_a_r_y_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n
+_P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_v_a_i_l_a_b_l_e_ _f_r_o_m_ _P_y_P_I_ _a_n_d_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _b_y_ _r_u_n_n_i_n_g_:_ _`_`_`_ _p_i_p
+_i_n_s_t_a_l_l_ _p_o_l_a_r_-_r_o_u_t_e_ _`_`_`_ _A_l_t_e_r_n_a_t_i_v_e_l_y_ _y_o_u_ _c_a_n_ _i_n_s_t_a_l_l_ _P_o_l_a_r_R_o_u_t_e_ _b_y_ _d_o_w_n_l_o_a_d_i_n_g
+_t_h_e_ _s_o_u_r_c_e_ _c_o_d_e_ _f_r_o_m_ _G_i_t_H_u_b_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/
+_P_o_l_a_r_R_o_u_t_e_ _p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_P_o_l_a_r_R_o_u_t_e_ _`_`_`_ _U_s_e_ _o_f_ _`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n
+_w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t_ _t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d_ _c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _>_ _N_O_T_E_:
+_S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_._ _P_l_e_a_s_e
+_c_o_n_s_u_l_t_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _f_u_r_t_h_e_r_ _g_u_i_d_a_n_c_e_._ _#_#_ _R_e_q_u_i_r_e_d_ _D_a_t_a_ _s_o_u_r_c_e_s
+_P_o_l_a_r_R_o_u_t_e_ _h_a_s_ _b_e_e_n_ _b_u_i_l_t_ _t_o_ _w_o_r_k_ _w_i_t_h_ _a_ _v_a_r_i_e_t_y_ _o_f_ _o_p_e_n_-_s_o_u_r_c_e_ _a_t_m_o_s_p_h_e_r_i_c_ _a_n_d
+_o_c_e_a_n_o_g_r_a_p_h_i_c_ _d_a_t_a_ _s_o_u_r_c_e_s_._ _F_o_r_ _t_e_s_t_i_n_g_ _a_n_d_ _d_e_m_o_n_s_t_r_a_t_i_o_n_ _p_u_r_p_o_s_e_s_ _i_t_ _i_s_ _a_l_s_o
+_p_o_s_s_i_b_l_e_ _t_o_ _g_e_n_e_r_a_t_e_ _a_r_t_i_f_i_c_i_a_l_ _G_a_u_s_s_i_a_n_ _R_a_n_d_o_m_ _F_i_e_l_d_ _d_a_t_a_._ _A_ _f_u_l_l_ _l_i_s_t_ _o_f
+_s_u_p_p_o_r_t_e_d_ _d_a_t_a_ _s_o_u_r_c_e_s_ _a_n_d_ _t_h_e_i_r_ _a_s_s_o_c_i_a_t_e_d_ _d_a_t_a_l_o_a_d_e_r_s_ _i_s_ _g_i_v_e_n_ _i_n_ _t_h_e
+_'_D_a_t_a_l_o_a_d_e_r_ _O_v_e_r_v_i_e_w_'_ _s_e_c_t_i_o_n_ _o_f_ _t_h_e_ _[_M_e_s_h_i_P_h_i_ _m_a_n_u_a_l_]_(_h_t_t_p_s_:_/_/
+_a_n_t_a_r_c_t_i_c_a_._g_i_t_h_u_b_._i_o_/_M_e_s_h_i_P_h_i_/_)_ _#_#_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _T_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _t_h_e
+_p_a_c_k_a_g_e_ _i_s_ _a_v_a_i_l_a_b_l_e_ _t_o_ _r_e_a_d_ _a_t_:_ _h_t_t_p_s_:_/_/_a_n_t_a_r_c_t_i_c_a_._g_i_t_h_u_b_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_ _I_f
+_y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _t_h_e_ _s_o_u_r_c_e_ _o_f_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _y_o_u_ _w_i_l_l_ _n_e_e_d_ _t_o_ _r_e_b_u_i_l_d
+_t_h_e_ _c_o_r_r_e_s_p_o_n_d_i_n_g_ _h_t_m_l_ _f_i_l_e_s_ _u_s_i_n_g_ _S_p_h_i_n_x_._ _T_h_e_ _d_e_p_e_n_d_e_n_c_i_e_s_ _f_o_r_ _t_h_i_s_ _c_a_n_ _b_e
+_i_n_s_t_a_l_l_e_d_ _t_h_r_o_u_g_h_ _p_i_p_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _s_p_h_i_n_x_ _s_p_h_i_n_x___m_a_r_k_d_o_w_n___b_u_i_l_d_e_r
+_s_p_h_i_n_x___r_t_d___t_h_e_m_e_ _r_i_n_o_h_t_y_p_e_ _`_`_`_ _W_h_e_n_ _u_p_d_a_t_i_n_g_ _t_h_e_ _d_o_c_s_,_ _r_u_n_ _t_h_e_ _f_o_l_l_o_w_i_n_g
+_c_o_m_m_a_n_d_ _w_i_t_h_i_n_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_ _t_o_ _r_e_c_o_m_p_i_l_e_._ _`_`_`_ _s_p_h_i_n_x_-_b_u_i_l_d_ _-_b_ _h_t_m_l
+_._/_d_o_c_s_/_s_o_u_r_c_e_ _._/_d_o_c_s_/_h_t_m_l_ _`_`_`_ _S_o_m_e_t_i_m_e_s_ _t_h_e_ _c_a_c_h_e_ _n_e_e_d_s_ _t_o_ _b_e_ _c_l_e_a_r_e_d_ _f_o_r
+_i_n_t_e_r_n_a_l_ _l_i_n_k_s_ _t_o_ _u_p_d_a_t_e_._ _I_f_ _f_a_c_i_n_g_ _t_h_i_s_ _p_r_o_b_l_e_m_,_ _r_u_n_ _t_h_i_s_ _f_r_o_m_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e
+_d_i_r_e_c_t_o_r_y_._ _`_`_`_ _r_m_ _-_r_ _d_o_c_s_/_h_t_m_l_/_._d_o_c_t_r_e_e_s_/_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_e_r_s_ _A_u_t_o_n_o_m_o_u_s_ _M_a_r_i_n_e
+_O_p_e_r_a_t_i_o_n_s_ _P_l_a_n_n_i_n_g_ _(_A_M_O_P_)_ _T_e_a_m_,_ _A_I_ _L_a_b_,_ _B_r_i_t_i_s_h_ _A_n_t_a_r_c_t_i_c_ _S_u_r_v_e_y_ _#_#
 _C_o_l_l_a_b_o_r_a_t_i_o_n_ _W_e_ _a_r_e_ _c_u_r_r_e_n_t_l_y_ _a_s_s_e_s_s_i_n_g_ _t_h_e_ _b_e_s_t_ _p_r_a_c_t_i_c_e_ _f_o_r_ _c_o_l_l_a_b_o_r_a_t_i_o_n_ _o_n
-_t_h_e_ _c_o_d_e_b_a_s_e_,_ _u_n_t_i_l_ _t_h_e_n_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_]
-_(_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_)_ _f_o_r_ _f_u_r_t_h_e_r_ _i_n_f_o_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _i_s_ _l_i_c_e_n_s_e_d
-_u_n_d_e_r_ _a_ _M_I_T_ _l_i_c_e_n_s_e_,_ _b_u_t_ _r_e_q_u_e_s_t_ _u_s_e_r_s_ _c_i_t_e_ _o_u_r_ _p_u_b_l_i_c_a_t_i_o_n_._ _J_o_n_a_t_h_a_n_ _D_._ _S_m_i_t_h_,
-_S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e_ _C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _A_._ _S_._ _T_h_o_r_n_e_,_ _J_._ _A_l_e_x_a_n_d_e_r
-_B_r_e_a_r_l_e_y_,_ _D_e_r_e_k_ _L_o_n_g_,_ _M_i_c_h_a_e_l_ _M_e_r_e_d_i_t_h_,_ _M_a_r_i_a_ _F_o_x_,_ _(_2_0_2_2_)_,_ _A_u_t_o_n_o_m_o_u_s_ _P_a_s_s_a_g_e
-_P_l_a_n_n_i_n_g_ _f_o_r_ _a_ _P_o_l_a_r_ _V_e_s_s_e_l_,_ _a_r_X_i_v_,_ _h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_2_0_9_._0_2_3_8_9_ _F_o_r_ _m_o_r_e
-_i_n_f_o_r_m_a_t_i_o_n_ _p_l_e_a_s_e_ _s_e_e_ _t_h_e_ _a_t_t_a_c_h_e_d_ _`_`_L_I_C_E_N_S_E_`_`_ _f_i_l_e_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:
-_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
+_t_h_e_ _c_o_d_e_b_a_s_e_,_ _u_n_t_i_l_ _t_h_e_n_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_a_m_o_p_@_b_a_s_._a_c_._u_k_]_(_a_m_o_p_@_b_a_s_._a_c_._u_k_)_ _f_o_r
+_f_u_r_t_h_e_r_ _i_n_f_o_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _a_ _M_I_T_ _l_i_c_e_n_s_e_,_ _b_u_t
+_r_e_q_u_e_s_t_ _u_s_e_r_s_ _c_i_t_e_ _o_u_r_ _p_u_b_l_i_c_a_t_i_o_n_._ _J_o_n_a_t_h_a_n_ _D_._ _S_m_i_t_h_,_ _S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e
+_C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _A_._ _S_._ _T_h_o_r_n_e_,_ _J_._ _A_l_e_x_a_n_d_e_r_ _B_r_e_a_r_l_e_y_,_ _D_e_r_e_k_ _L_o_n_g_,
+_M_i_c_h_a_e_l_ _M_e_r_e_d_i_t_h_,_ _M_a_r_i_a_ _F_o_x_,_ _(_2_0_2_2_)_,_ _A_u_t_o_n_o_m_o_u_s_ _P_a_s_s_a_g_e_ _P_l_a_n_n_i_n_g_ _f_o_r_ _a_ _P_o_l_a_r
+_V_e_s_s_e_l_,_ _a_r_X_i_v_,_ _h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_2_0_9_._0_2_3_8_9_ _F_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_ _p_l_e_a_s_e_ _s_e_e
+_t_h_e_ _a_t_t_a_c_h_e_d_ _`_`_L_I_C_E_N_S_E_`_`_ _f_i_l_e_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_v_/
+_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_P_o_l_a_r_R_o_u_t_e_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
```

### Comparing `polar_route-0.3.9/README.md` & `polar_route-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,66 @@
+# PolarRoute
+
 ![](logo.jpg)
 
-<a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
 <a href="https://antarctica.github.io/PolarRoute/"><img src="https://img.shields.io/badge/Manual%20-github.io%2FPolarRoute%2F-red" alt="Manual Page">
-<a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPi">
+<a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
+<a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPI">
 <a href="https://github.com/antarctica/PolarRoute/tags"><img src="https://img.shields.io/github/v/tag/antarctica/PolarRoute" alt="Release Tag"></a>
 <a href="https://github.com/antarctica/PolarRoute/issues"><img src="https://img.shields.io/github/issues/antarctica/PolarRoute" alt="Issues"></a>
 <a href="https://github.com/antarctica/PolarRoute/blob/main/LICENSE"><img src="https://img.shields.io/github/license/antarctica/PolarRoute" alt="License"></a>
 
-# PolarRoute
-PolarRoute is a long-distance maritime polar route planning package, taking into account complex changing environmental conditions. The codebase allows the construction of optimised routes through three main stages: discrete modelling of the environmental conditions using a non-uniform mesh, the construction of mesh-optimal paths, and physics informed path smoothing. In order to account for different vehicle properties we construct a series of data driven functions that can be applied to the environmental mesh to determine the speed limitations and fuel requirements for a given vessel and mesh cell, representing these quantities graphically and geospatially.
+PolarRoute is a long-distance maritime polar route planning package, able to take into account complex and changing environmental conditions. It allows the construction of optimised routes through three main stages: discrete modelling of the environmental conditions using a non-uniform mesh, the construction of mesh-optimal paths, and physics informed path smoothing. In order to account for different vehicle properties we construct a series of data-driven functions that can be applied to the environmental mesh to determine the speed limitations and fuel requirements for a given vessel and mesh cell. The environmental modelling component of this functionality is provided by the [MeshiPhi](https://github.com/antarctica/MeshiPhi) library.
 
 ## Installation
-The PolarRoute package requires GDAL files to be installed. This software can be installed on Windows by running the required wheels for GDAL and FIONA. More information can be found in the manual pages linked above. Once these requirements are met then the software can be installed by:
 
-Github:
+PolarRoute is available from PyPI and can be installed by running: 
 ```
-git clone https://github.com/Antarctica/PolarRoute
-python setup.py install
+pip install polar-route
 ```
 
- Pip: 
+Alternatively you can install PolarRoute by downloading the source code from GitHub:
 ```
-pip install polar-route
+git clone https://github.com/Antarctica/PolarRoute
+pip install -e ./PolarRoute
 ```
+Use of `-e` is optional, based on whether you want to be able to edit the installed copy of the package.
 
-> NOTE: The installation process may vary slightly dependent on OS. Please consult the documentation for further installation guidance.
+> NOTE: Some features of the PolarRoute package require GDAL to be installed. Please consult the documentation for further guidance.
 
 ## Required Data sources
-Polar-route has been built to work with a variety of open-source atmospheric and oceanographic data sources. 
-A list of supported data sources and their associated data-loaders is given in the 
-'Data Loaders' section of the manual
+PolarRoute has been built to work with a variety of open-source atmospheric and oceanographic data sources. For testing and demonstration purposes it is also possible to generate artificial Gaussian Random Field data.  
+
+A full list of supported data sources and their associated dataloaders is given in the 
+'Dataloader Overview' section of the [MeshiPhi manual](https://antarctica.github.io/MeshiPhi/)
 
 ## Documentation
-Sphinx is used to generate documentation for this project. The dependencies can be installed through pip:
+The documentation for the package is available to read at: https://antarctica.github.io/PolarRoute/
+
+If you make changes to the source of the documentation you will need to rebuild the corresponding html files using Sphinx.
+The dependencies for this can be installed through pip:
 ```
 pip install sphinx sphinx_markdown_builder sphinx_rtd_theme rinohtype
 ```
 When updating the docs, run the following command within the PolarRoute directory to recompile.
 ```
 sphinx-build -b html ./docs/source ./docs/html
 ```
 Sometimes the cache needs to be cleared for internal links to update. If facing this problem, run this from the PolarRoute directory.
 ```
-rm -r docs/build/.doctrees/
+rm -r docs/html/.doctrees/
 ```
 ## Developers
-Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox, Harrison Abbot, Ayat Fekry
+Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 
 ## Collaboration
-We are currently assessing the best practice for collaboration on the codebase, until then please contact [polarroute@bas.ac.uk](polarroute@bas.ac.uk) for further info.
-
+We are currently assessing the best practice for collaboration on the codebase, until then please contact [amop@bas.ac.uk](amop@bas.ac.uk) for further info.
 
 ## License
 This software is licensed under a MIT license, but request users cite our publication.  
 
-Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne,  J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox,  (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
+Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne, J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox, (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
 
 For more information please see the attached ``LICENSE`` file. 
 
 [version]: https://img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square
```

#### html2text {}

```diff
@@ -1,39 +1,44 @@
-![](logo.jpg) _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_#
-_P_o_l_a_r_R_o_u_t_e_ _P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_ _l_o_n_g_-_d_i_s_t_a_n_c_e_ _m_a_r_i_t_i_m_e_ _p_o_l_a_r_ _r_o_u_t_e_ _p_l_a_n_n_i_n_g_ _p_a_c_k_a_g_e_,
-_t_a_k_i_n_g_ _i_n_t_o_ _a_c_c_o_u_n_t_ _c_o_m_p_l_e_x_ _c_h_a_n_g_i_n_g_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_._ _T_h_e_ _c_o_d_e_b_a_s_e
-_a_l_l_o_w_s_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _o_p_t_i_m_i_s_e_d_ _r_o_u_t_e_s_ _t_h_r_o_u_g_h_ _t_h_r_e_e_ _m_a_i_n_ _s_t_a_g_e_s_:_ _d_i_s_c_r_e_t_e
-_m_o_d_e_l_l_i_n_g_ _o_f_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_ _u_s_i_n_g_ _a_ _n_o_n_-_u_n_i_f_o_r_m_ _m_e_s_h_,_ _t_h_e
-_c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _m_e_s_h_-_o_p_t_i_m_a_l_ _p_a_t_h_s_,_ _a_n_d_ _p_h_y_s_i_c_s_ _i_n_f_o_r_m_e_d_ _p_a_t_h_ _s_m_o_o_t_h_i_n_g_._ _I_n
-_o_r_d_e_r_ _t_o_ _a_c_c_o_u_n_t_ _f_o_r_ _d_i_f_f_e_r_e_n_t_ _v_e_h_i_c_l_e_ _p_r_o_p_e_r_t_i_e_s_ _w_e_ _c_o_n_s_t_r_u_c_t_ _a_ _s_e_r_i_e_s_ _o_f_ _d_a_t_a
-_d_r_i_v_e_n_ _f_u_n_c_t_i_o_n_s_ _t_h_a_t_ _c_a_n_ _b_e_ _a_p_p_l_i_e_d_ _t_o_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_e_s_h_ _t_o_ _d_e_t_e_r_m_i_n_e_ _t_h_e
-_s_p_e_e_d_ _l_i_m_i_t_a_t_i_o_n_s_ _a_n_d_ _f_u_e_l_ _r_e_q_u_i_r_e_m_e_n_t_s_ _f_o_r_ _a_ _g_i_v_e_n_ _v_e_s_s_e_l_ _a_n_d_ _m_e_s_h_ _c_e_l_l_,
-_r_e_p_r_e_s_e_n_t_i_n_g_ _t_h_e_s_e_ _q_u_a_n_t_i_t_i_e_s_ _g_r_a_p_h_i_c_a_l_l_y_ _a_n_d_ _g_e_o_s_p_a_t_i_a_l_l_y_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e
-_P_o_l_a_r_R_o_u_t_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_s_ _G_D_A_L_ _f_i_l_e_s_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_._ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _c_a_n_ _b_e
-_i_n_s_t_a_l_l_e_d_ _o_n_ _W_i_n_d_o_w_s_ _b_y_ _r_u_n_n_i_n_g_ _t_h_e_ _r_e_q_u_i_r_e_d_ _w_h_e_e_l_s_ _f_o_r_ _G_D_A_L_ _a_n_d_ _F_I_O_N_A_._ _M_o_r_e
-_i_n_f_o_r_m_a_t_i_o_n_ _c_a_n_ _b_e_ _f_o_u_n_d_ _i_n_ _t_h_e_ _m_a_n_u_a_l_ _p_a_g_e_s_ _l_i_n_k_e_d_ _a_b_o_v_e_._ _O_n_c_e_ _t_h_e_s_e
-_r_e_q_u_i_r_e_m_e_n_t_s_ _a_r_e_ _m_e_t_ _t_h_e_n_ _t_h_e_ _s_o_f_t_w_a_r_e_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _b_y_:_ _G_i_t_h_u_b_:_ _`_`_`_ _g_i_t
-_c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_P_o_l_a_r_R_o_u_t_e_ _p_y_t_h_o_n_ _s_e_t_u_p_._p_y_ _i_n_s_t_a_l_l_ _`_`_`_ _P_i_p_:
-_`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_o_l_a_r_-_r_o_u_t_e_ _`_`_`_ _>_ _N_O_T_E_:_ _T_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s_ _m_a_y_ _v_a_r_y
-_s_l_i_g_h_t_l_y_ _d_e_p_e_n_d_e_n_t_ _o_n_ _O_S_._ _P_l_e_a_s_e_ _c_o_n_s_u_l_t_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _f_u_r_t_h_e_r
-_i_n_s_t_a_l_l_a_t_i_o_n_ _g_u_i_d_a_n_c_e_._ _#_#_ _R_e_q_u_i_r_e_d_ _D_a_t_a_ _s_o_u_r_c_e_s_ _P_o_l_a_r_-_r_o_u_t_e_ _h_a_s_ _b_e_e_n_ _b_u_i_l_t_ _t_o
-_w_o_r_k_ _w_i_t_h_ _a_ _v_a_r_i_e_t_y_ _o_f_ _o_p_e_n_-_s_o_u_r_c_e_ _a_t_m_o_s_p_h_e_r_i_c_ _a_n_d_ _o_c_e_a_n_o_g_r_a_p_h_i_c_ _d_a_t_a_ _s_o_u_r_c_e_s_.
-_A_ _l_i_s_t_ _o_f_ _s_u_p_p_o_r_t_e_d_ _d_a_t_a_ _s_o_u_r_c_e_s_ _a_n_d_ _t_h_e_i_r_ _a_s_s_o_c_i_a_t_e_d_ _d_a_t_a_-_l_o_a_d_e_r_s_ _i_s_ _g_i_v_e_n_ _i_n
-_t_h_e_ _'_D_a_t_a_ _L_o_a_d_e_r_s_'_ _s_e_c_t_i_o_n_ _o_f_ _t_h_e_ _m_a_n_u_a_l_ _#_#_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_p_h_i_n_x_ _i_s_ _u_s_e_d_ _t_o
-_g_e_n_e_r_a_t_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _t_h_i_s_ _p_r_o_j_e_c_t_._ _T_h_e_ _d_e_p_e_n_d_e_n_c_i_e_s_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d
-_t_h_r_o_u_g_h_ _p_i_p_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _s_p_h_i_n_x_ _s_p_h_i_n_x___m_a_r_k_d_o_w_n___b_u_i_l_d_e_r_ _s_p_h_i_n_x___r_t_d___t_h_e_m_e
-_r_i_n_o_h_t_y_p_e_ _`_`_`_ _W_h_e_n_ _u_p_d_a_t_i_n_g_ _t_h_e_ _d_o_c_s_,_ _r_u_n_ _t_h_e_ _f_o_l_l_o_w_i_n_g_ _c_o_m_m_a_n_d_ _w_i_t_h_i_n_ _t_h_e
-_P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_ _t_o_ _r_e_c_o_m_p_i_l_e_._ _`_`_`_ _s_p_h_i_n_x_-_b_u_i_l_d_ _-_b_ _h_t_m_l_ _._/_d_o_c_s_/_s_o_u_r_c_e_ _._/
-_d_o_c_s_/_h_t_m_l_ _`_`_`_ _S_o_m_e_t_i_m_e_s_ _t_h_e_ _c_a_c_h_e_ _n_e_e_d_s_ _t_o_ _b_e_ _c_l_e_a_r_e_d_ _f_o_r_ _i_n_t_e_r_n_a_l_ _l_i_n_k_s_ _t_o
-_u_p_d_a_t_e_._ _I_f_ _f_a_c_i_n_g_ _t_h_i_s_ _p_r_o_b_l_e_m_,_ _r_u_n_ _t_h_i_s_ _f_r_o_m_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_._ _`_`_`_ _r_m
-_-_r_ _d_o_c_s_/_b_u_i_l_d_/_._d_o_c_t_r_e_e_s_/_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_e_r_s_ _J_o_n_a_t_h_a_n_ _S_m_i_t_h_,_ _S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e
-_C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _T_h_o_r_n_e_,_ _M_a_r_i_a_ _F_o_x_,_ _H_a_r_r_i_s_o_n_ _A_b_b_o_t_,_ _A_y_a_t_ _F_e_k_r_y_ _#_#
+# PolarRoute ![](logo.jpg) _[_M_a_n_u_a_l_ _P_a_g_e_]_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_P_y_P_I_]_[_R_e_l_e_a_s_e_ _T_a_g_]
+_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_ _l_o_n_g_-_d_i_s_t_a_n_c_e_ _m_a_r_i_t_i_m_e_ _p_o_l_a_r_ _r_o_u_t_e_ _p_l_a_n_n_i_n_g
+_p_a_c_k_a_g_e_,_ _a_b_l_e_ _t_o_ _t_a_k_e_ _i_n_t_o_ _a_c_c_o_u_n_t_ _c_o_m_p_l_e_x_ _a_n_d_ _c_h_a_n_g_i_n_g_ _e_n_v_i_r_o_n_m_e_n_t_a_l
+_c_o_n_d_i_t_i_o_n_s_._ _I_t_ _a_l_l_o_w_s_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _o_p_t_i_m_i_s_e_d_ _r_o_u_t_e_s_ _t_h_r_o_u_g_h_ _t_h_r_e_e_ _m_a_i_n
+_s_t_a_g_e_s_:_ _d_i_s_c_r_e_t_e_ _m_o_d_e_l_l_i_n_g_ _o_f_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_ _u_s_i_n_g_ _a_ _n_o_n_-_u_n_i_f_o_r_m
+_m_e_s_h_,_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _m_e_s_h_-_o_p_t_i_m_a_l_ _p_a_t_h_s_,_ _a_n_d_ _p_h_y_s_i_c_s_ _i_n_f_o_r_m_e_d_ _p_a_t_h
+_s_m_o_o_t_h_i_n_g_._ _I_n_ _o_r_d_e_r_ _t_o_ _a_c_c_o_u_n_t_ _f_o_r_ _d_i_f_f_e_r_e_n_t_ _v_e_h_i_c_l_e_ _p_r_o_p_e_r_t_i_e_s_ _w_e_ _c_o_n_s_t_r_u_c_t_ _a
+_s_e_r_i_e_s_ _o_f_ _d_a_t_a_-_d_r_i_v_e_n_ _f_u_n_c_t_i_o_n_s_ _t_h_a_t_ _c_a_n_ _b_e_ _a_p_p_l_i_e_d_ _t_o_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_e_s_h
+_t_o_ _d_e_t_e_r_m_i_n_e_ _t_h_e_ _s_p_e_e_d_ _l_i_m_i_t_a_t_i_o_n_s_ _a_n_d_ _f_u_e_l_ _r_e_q_u_i_r_e_m_e_n_t_s_ _f_o_r_ _a_ _g_i_v_e_n_ _v_e_s_s_e_l_ _a_n_d
+_m_e_s_h_ _c_e_l_l_._ _T_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_o_d_e_l_l_i_n_g_ _c_o_m_p_o_n_e_n_t_ _o_f_ _t_h_i_s_ _f_u_n_c_t_i_o_n_a_l_i_t_y_ _i_s
+_p_r_o_v_i_d_e_d_ _b_y_ _t_h_e_ _[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_ _l_i_b_r_a_r_y_._ _#_#
+_I_n_s_t_a_l_l_a_t_i_o_n_ _P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_v_a_i_l_a_b_l_e_ _f_r_o_m_ _P_y_P_I_ _a_n_d_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _b_y_ _r_u_n_n_i_n_g_:
+_`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_o_l_a_r_-_r_o_u_t_e_ _`_`_`_ _A_l_t_e_r_n_a_t_i_v_e_l_y_ _y_o_u_ _c_a_n_ _i_n_s_t_a_l_l_ _P_o_l_a_r_R_o_u_t_e_ _b_y
+_d_o_w_n_l_o_a_d_i_n_g_ _t_h_e_ _s_o_u_r_c_e_ _c_o_d_e_ _f_r_o_m_ _G_i_t_H_u_b_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_A_n_t_a_r_c_t_i_c_a_/_P_o_l_a_r_R_o_u_t_e_ _p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_P_o_l_a_r_R_o_u_t_e_ _`_`_`_ _U_s_e_ _o_f_ _`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,
+_b_a_s_e_d_ _o_n_ _w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t_ _t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d_ _c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_.
+_>_ _N_O_T_E_:_ _S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_.
+_P_l_e_a_s_e_ _c_o_n_s_u_l_t_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _f_u_r_t_h_e_r_ _g_u_i_d_a_n_c_e_._ _#_#_ _R_e_q_u_i_r_e_d_ _D_a_t_a_ _s_o_u_r_c_e_s
+_P_o_l_a_r_R_o_u_t_e_ _h_a_s_ _b_e_e_n_ _b_u_i_l_t_ _t_o_ _w_o_r_k_ _w_i_t_h_ _a_ _v_a_r_i_e_t_y_ _o_f_ _o_p_e_n_-_s_o_u_r_c_e_ _a_t_m_o_s_p_h_e_r_i_c_ _a_n_d
+_o_c_e_a_n_o_g_r_a_p_h_i_c_ _d_a_t_a_ _s_o_u_r_c_e_s_._ _F_o_r_ _t_e_s_t_i_n_g_ _a_n_d_ _d_e_m_o_n_s_t_r_a_t_i_o_n_ _p_u_r_p_o_s_e_s_ _i_t_ _i_s_ _a_l_s_o
+_p_o_s_s_i_b_l_e_ _t_o_ _g_e_n_e_r_a_t_e_ _a_r_t_i_f_i_c_i_a_l_ _G_a_u_s_s_i_a_n_ _R_a_n_d_o_m_ _F_i_e_l_d_ _d_a_t_a_._ _A_ _f_u_l_l_ _l_i_s_t_ _o_f
+_s_u_p_p_o_r_t_e_d_ _d_a_t_a_ _s_o_u_r_c_e_s_ _a_n_d_ _t_h_e_i_r_ _a_s_s_o_c_i_a_t_e_d_ _d_a_t_a_l_o_a_d_e_r_s_ _i_s_ _g_i_v_e_n_ _i_n_ _t_h_e
+_'_D_a_t_a_l_o_a_d_e_r_ _O_v_e_r_v_i_e_w_'_ _s_e_c_t_i_o_n_ _o_f_ _t_h_e_ _[_M_e_s_h_i_P_h_i_ _m_a_n_u_a_l_]_(_h_t_t_p_s_:_/_/
+_a_n_t_a_r_c_t_i_c_a_._g_i_t_h_u_b_._i_o_/_M_e_s_h_i_P_h_i_/_)_ _#_#_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _T_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _t_h_e
+_p_a_c_k_a_g_e_ _i_s_ _a_v_a_i_l_a_b_l_e_ _t_o_ _r_e_a_d_ _a_t_:_ _h_t_t_p_s_:_/_/_a_n_t_a_r_c_t_i_c_a_._g_i_t_h_u_b_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_ _I_f
+_y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _t_h_e_ _s_o_u_r_c_e_ _o_f_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _y_o_u_ _w_i_l_l_ _n_e_e_d_ _t_o_ _r_e_b_u_i_l_d
+_t_h_e_ _c_o_r_r_e_s_p_o_n_d_i_n_g_ _h_t_m_l_ _f_i_l_e_s_ _u_s_i_n_g_ _S_p_h_i_n_x_._ _T_h_e_ _d_e_p_e_n_d_e_n_c_i_e_s_ _f_o_r_ _t_h_i_s_ _c_a_n_ _b_e
+_i_n_s_t_a_l_l_e_d_ _t_h_r_o_u_g_h_ _p_i_p_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _s_p_h_i_n_x_ _s_p_h_i_n_x___m_a_r_k_d_o_w_n___b_u_i_l_d_e_r
+_s_p_h_i_n_x___r_t_d___t_h_e_m_e_ _r_i_n_o_h_t_y_p_e_ _`_`_`_ _W_h_e_n_ _u_p_d_a_t_i_n_g_ _t_h_e_ _d_o_c_s_,_ _r_u_n_ _t_h_e_ _f_o_l_l_o_w_i_n_g
+_c_o_m_m_a_n_d_ _w_i_t_h_i_n_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_ _t_o_ _r_e_c_o_m_p_i_l_e_._ _`_`_`_ _s_p_h_i_n_x_-_b_u_i_l_d_ _-_b_ _h_t_m_l
+_._/_d_o_c_s_/_s_o_u_r_c_e_ _._/_d_o_c_s_/_h_t_m_l_ _`_`_`_ _S_o_m_e_t_i_m_e_s_ _t_h_e_ _c_a_c_h_e_ _n_e_e_d_s_ _t_o_ _b_e_ _c_l_e_a_r_e_d_ _f_o_r
+_i_n_t_e_r_n_a_l_ _l_i_n_k_s_ _t_o_ _u_p_d_a_t_e_._ _I_f_ _f_a_c_i_n_g_ _t_h_i_s_ _p_r_o_b_l_e_m_,_ _r_u_n_ _t_h_i_s_ _f_r_o_m_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e
+_d_i_r_e_c_t_o_r_y_._ _`_`_`_ _r_m_ _-_r_ _d_o_c_s_/_h_t_m_l_/_._d_o_c_t_r_e_e_s_/_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_e_r_s_ _A_u_t_o_n_o_m_o_u_s_ _M_a_r_i_n_e
+_O_p_e_r_a_t_i_o_n_s_ _P_l_a_n_n_i_n_g_ _(_A_M_O_P_)_ _T_e_a_m_,_ _A_I_ _L_a_b_,_ _B_r_i_t_i_s_h_ _A_n_t_a_r_c_t_i_c_ _S_u_r_v_e_y_ _#_#
 _C_o_l_l_a_b_o_r_a_t_i_o_n_ _W_e_ _a_r_e_ _c_u_r_r_e_n_t_l_y_ _a_s_s_e_s_s_i_n_g_ _t_h_e_ _b_e_s_t_ _p_r_a_c_t_i_c_e_ _f_o_r_ _c_o_l_l_a_b_o_r_a_t_i_o_n_ _o_n
-_t_h_e_ _c_o_d_e_b_a_s_e_,_ _u_n_t_i_l_ _t_h_e_n_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_]
-_(_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_)_ _f_o_r_ _f_u_r_t_h_e_r_ _i_n_f_o_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _i_s_ _l_i_c_e_n_s_e_d
-_u_n_d_e_r_ _a_ _M_I_T_ _l_i_c_e_n_s_e_,_ _b_u_t_ _r_e_q_u_e_s_t_ _u_s_e_r_s_ _c_i_t_e_ _o_u_r_ _p_u_b_l_i_c_a_t_i_o_n_._ _J_o_n_a_t_h_a_n_ _D_._ _S_m_i_t_h_,
-_S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e_ _C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _A_._ _S_._ _T_h_o_r_n_e_,_ _J_._ _A_l_e_x_a_n_d_e_r
-_B_r_e_a_r_l_e_y_,_ _D_e_r_e_k_ _L_o_n_g_,_ _M_i_c_h_a_e_l_ _M_e_r_e_d_i_t_h_,_ _M_a_r_i_a_ _F_o_x_,_ _(_2_0_2_2_)_,_ _A_u_t_o_n_o_m_o_u_s_ _P_a_s_s_a_g_e
-_P_l_a_n_n_i_n_g_ _f_o_r_ _a_ _P_o_l_a_r_ _V_e_s_s_e_l_,_ _a_r_X_i_v_,_ _h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_2_0_9_._0_2_3_8_9_ _F_o_r_ _m_o_r_e
-_i_n_f_o_r_m_a_t_i_o_n_ _p_l_e_a_s_e_ _s_e_e_ _t_h_e_ _a_t_t_a_c_h_e_d_ _`_`_L_I_C_E_N_S_E_`_`_ _f_i_l_e_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:
-_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
+_t_h_e_ _c_o_d_e_b_a_s_e_,_ _u_n_t_i_l_ _t_h_e_n_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_a_m_o_p_@_b_a_s_._a_c_._u_k_]_(_a_m_o_p_@_b_a_s_._a_c_._u_k_)_ _f_o_r
+_f_u_r_t_h_e_r_ _i_n_f_o_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _a_ _M_I_T_ _l_i_c_e_n_s_e_,_ _b_u_t
+_r_e_q_u_e_s_t_ _u_s_e_r_s_ _c_i_t_e_ _o_u_r_ _p_u_b_l_i_c_a_t_i_o_n_._ _J_o_n_a_t_h_a_n_ _D_._ _S_m_i_t_h_,_ _S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e
+_C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _A_._ _S_._ _T_h_o_r_n_e_,_ _J_._ _A_l_e_x_a_n_d_e_r_ _B_r_e_a_r_l_e_y_,_ _D_e_r_e_k_ _L_o_n_g_,
+_M_i_c_h_a_e_l_ _M_e_r_e_d_i_t_h_,_ _M_a_r_i_a_ _F_o_x_,_ _(_2_0_2_2_)_,_ _A_u_t_o_n_o_m_o_u_s_ _P_a_s_s_a_g_e_ _P_l_a_n_n_i_n_g_ _f_o_r_ _a_ _P_o_l_a_r
+_V_e_s_s_e_l_,_ _a_r_X_i_v_,_ _h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_2_0_9_._0_2_3_8_9_ _F_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_ _p_l_e_a_s_e_ _s_e_e
+_t_h_e_ _a_t_t_a_c_h_e_d_ _`_`_L_I_C_E_N_S_E_`_`_ _f_i_l_e_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_v_/
+_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_P_o_l_a_r_R_o_u_t_e_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
```

### Comparing `polar_route-0.3.9/polar_route/__init__.py` & `polar_route-0.4.0/polar_route/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-__version__ = "0.3.9"
+__version__ = "0.4.0"
 __description__ = "PolarRoute: Long-distance maritime polar route planning taking into account complex changing environmental conditions"
 __license__ = "MIT"
-__author__ = "Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox"
-__email__ = "polarroute@bas.ac.uk"
-__copyright__ = "2022-2023, BAS AI Lab"
+__author__ = "Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey"
+__email__ = "amop@bas.ac.uk"
+__copyright__ = "2021-, BAS AI Lab"
 
 # Wrapped in try-except so that setup.py can import polar_route without crashing due to dependency errors
 try:
     from meshiphi.mesh_generation.mesh_builder import MeshBuilder as MeshBuilder
     from meshiphi.dataloaders.factory import DataLoaderFactory as DataLoaderFactory
     from meshiphi.mesh_generation.boundary import Boundary as Boundary
 
     from polar_route.vessel_performance.vessel_performance_modeller import VesselPerformanceModeller as VesselPerformanceModeller
 
     from polar_route.route_planner import RoutePlanner as RoutePlanner
 
 except ModuleNotFoundError as err:
-    print(f'{err}\n Is PolarRoute installed correctly?')
+    print(f'{err}\n Is PolarRoute installed correctly?')
```

### Comparing `polar_route-0.3.9/polar_route/config_validation/config_validator.py` & `polar_route-0.4.0/polar_route/config_validation/config_validator.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/config_validation/route_schema.py` & `polar_route-0.4.0/polar_route/config_validation/route_schema.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/crossing.py` & `polar_route-0.4.0/polar_route/crossing.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/crossing_smoothing.py` & `polar_route-0.4.0/polar_route/crossing_smoothing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1033,26 +1033,28 @@
     def blocked(self,new_cell,cell_a,cell_b):
         '''
             Function that determines if the new cell being introduced is worse off than the original two cells.
             Currently, this is hard encoded to not enter a cell 5% worse off in Sea-Ice-Concentration
 
             Args:
                 new_cell (dict) - New cell to add environmental parameters as dict
-                cell_a (dict) - Start cell to add environmental parameters as dict
-                cell_b (dict) - End cell to add environmental parameters as dict
+                cell_a (dict)   - Start cell to add environmental parameters as dict
+                cell_b (dict)   - End cell to add environmental parameters as dict
 
             Return:
                 True if the cell cannot be entered, False if the cell can
         '''
         start = cell_a['SIC']
         end   = cell_b['SIC']
         max_new = new_cell['SIC']
 
-        percentage_diff = (max_new-start)
-        if percentage_diff < self.blocked_sic:
+        percentage_diff1  = (max_new-start)*100
+        percentage_diff2  = (max_new-end)*100
+
+        if (percentage_diff1 <= self.blocked_sic*start) or (percentage_diff2 <= self.blocked_sic*end) or (max_new<=self.blocked_sic):
             return False
         else:
             return True
                 
 
     def clip(self,cell_a,cell_b,case,x):
         '''
```

### Comparing `polar_route-0.3.9/polar_route/route_calc.py` & `polar_route-0.4.0/polar_route/route_calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import numpy as np
 import pandas as pd
 import geopandas as gpd
-from shapely import wkt
+from shapely import wkt, distance
 from shapely.geometry import Point, LineString, MultiLineString, Polygon
+from polar_route.utils import gpx_route_import
 
 
 # Define ordering of cases in array data
 case_indices = np.array([1, 2, 3, 4, -1, -2, -3, -4])
 
 def traveltime_in_cell(xdist, ydist, u, v, s):
     """
@@ -71,15 +72,20 @@
     m_long = 111.321 * 1000
     m_lat = 111.386 * 1000
     x = (cp[0] - wp[0]) * m_long * np.cos(wp[1] * (np.pi / 180))
     y = (cp[1] - wp[1]) * m_lat
     su = cellbox[vector_x]
     sv = cellbox[vector_y]
     ssp = cellbox[speed][idx] * (1000 / (60 * 60))
-    traveltime, distance = traveltime_in_cell(x, y, su, sv, ssp)
+    try:
+        traveltime, distance = traveltime_in_cell(x, y, su, sv, ssp)
+    except:
+        traveltime=0
+        distance=0
+
     return traveltime, distance
 
 
 def case_from_angle(start, end):
     """
         Determine the direction of travel between two points and return the associated case
 
@@ -129,14 +135,15 @@
 
         Returns:
             df (Dataframe): Dataframe with route info
             from_wp (str): Name of start waypoint
             to_wp (str) Name of end waypoint
 
     """
+    logging.info(f"Loading route from: {route_file}")
     # Loading route from csv file
     if route_file[-3:] == "csv":
         df = pd.read_csv(route_file)
         to_wp = df['Name'].iloc[-1]
         from_wp = df['Name'].iloc[0]
     # Loading route from geojson file
     elif route_file[-4:] == "json":
@@ -146,18 +153,30 @@
         to_wp = route_json['features'][0]['properties']['to']
         from_wp = route_json['features'][0]['properties']['from']
         longs = [c[0] for c in route_coords]
         lats = [c[1] for c in route_coords]
         df = pd.DataFrame()
         df['Long'] = longs
         df['Lat'] = lats
+    elif route_file[-3:] == "gpx":
+        route_json = gpx_route_import(route_file)
+        route_coords = route_json['features'][0]['geometry']['coordinates']
+        to_wp = route_json['features'][0]['properties']['to']
+        from_wp = route_json['features'][0]['properties']['from']
+        longs = [c[0] for c in route_coords]
+        lats = [c[1] for c in route_coords]
+        df = pd.DataFrame()
+        df['Long'] = longs
+        df['Lat'] = lats
     else:
-        logging.warning("Invalid route input! Please supply either a csv or geojson file with the route waypoints.")
+        logging.warning("Invalid route input! Please supply either a csv, gpx or geojson file with the route waypoints.")
         return None
 
+    logging.info(f"Route start waypoint: {from_wp}")
+    logging.info(f"Route end waypoint: {to_wp}")
     logging.debug(f"Route has {len(df)} waypoints")
     df['id'] = 1
     df['order'] = np.arange(len(df))
 
     return df, from_wp, to_wp
 
 
@@ -166,14 +185,15 @@
         Load mesh from file into GeoDataFrame
         Args:
             mesh_file (str): Path to mesh with vehicle information
 
         Returns:
             mesh (GeoDataFrame): Mesh in GeoDataFrame format
     """
+    logging.info(f"Loading mesh from: {mesh_file}")
     # Loading mesh information
     with open(mesh_file, 'r') as fp:
         info = json.load(fp)
     mesh = pd.DataFrame(info['cellboxes'])
     mesh['geometry'] = mesh['geometry'].apply(wkt.loads)
     mesh = gpd.GeoDataFrame(mesh, crs='EPSG:4326', geometry='geometry')
 
@@ -250,37 +270,35 @@
     pathing = True
     track_id = np.where(track_points['startPoints'] == start_point)[0][0]
     path_point = []
     cell_ids = []
 
     # Loop through crossing points to order them into a track along the route
     while pathing:
-        try:
-            start_point_segment = track_points['startPoints'].iloc[track_id]
-            end_point_segment = track_points['endPoints'].iloc[track_id]
-            path_point.append(start_point_segment)
-            cell_ids.append(track_points['cellID'].iloc[track_id])
-
-            if len(track_points['midPoints'].iloc[track_id]) != 0:
-                for midpnt in track_points['midPoints'].iloc[track_id]:
-                    path_point.append(midpnt)
-                    cell_ids.append(track_points['cellID'].iloc[track_id])
-
-            if end_point_segment == end_point:
-                pathing = False
-            track_id = np.where(track_points['startPoints'] == end_point_segment)[0][0]
-        except IndexError:
+        start_point_segment = track_points['startPoints'].iloc[track_id]
+        end_point_segment = track_points['endPoints'].iloc[track_id]
+        path_point.append(start_point_segment)
+        cell_ids.append(track_points['cellID'].iloc[track_id])
+
+        if len(track_points['midPoints'].iloc[track_id]) != 0:
+            for midpnt in track_points['midPoints'].iloc[track_id]:
+                path_point.append(midpnt)
+                cell_ids.append(track_points['cellID'].iloc[track_id])
+
+        if  distance(end_point_segment,end_point) < 0.05:
             pathing = False
-            path_point.append(end_point_segment)
-            cell_ids.append('NaN')
+        else:
+            track_id     = np.argmin([distance(entry,end_point_segment) for entry in track_points['startPoints']])
+            track_misfit = min([distance(entry,end_point_segment) for entry in track_points['startPoints']])
+            if track_misfit >= 0.05:
+                raise Exception('Path Segmentment not adding - ID={},Misfit={},distance from end={}'.format(track_id,track_misfit,distance(end_point_segment,end_point)))
 
     user_track = pd.DataFrame({'Point': path_point, 'CellID': cell_ids})
     return user_track
 
-
 def route_calc(route_file, mesh_file):
     """
         Function to calculate the fuel/time cost of a user defined route in a given mesh
 
         Args:
             route_file (str): Path to user defined route
             mesh_file (str): Path to mesh with vehicle information
@@ -322,16 +340,21 @@
         start_point = np.array((user_track['Point'].iloc[idx].xy[0][0], user_track['Point'].iloc[idx].xy[1][0]))
         end_point = np.array((user_track['Point'].iloc[idx+1].xy[0][0], user_track['Point'].iloc[idx+1].xy[1][0]))
         cell_box = mesh.iloc[user_track['CellID'].iloc[idx]]
         case = case_from_angle(start_point, end_point)
         # Check for inaccessible cells on user defined route
         if cell_box['inaccessible']:
             logging.warning(f"This route crosses an inaccessible cell! Cell located at Lat: {cell_box['cy']} "
-                         f"Long: {cell_box['cx']}. Please reroute around it.")
-            return None
+                         f"Long: {cell_box['cx']}")
+            logging.info("Trying with speed and fuel from previous cells, reroute for more accurate results")
+            i = 0
+            # Go back along path to find previous accessible cell
+            while cell_box['inaccessible']:
+                i += 1
+                cell_box = mesh.iloc[user_track['CellID'].iloc[idx-i]]
 
         traveltime_s, distance_m = traveltime_distance(cell_box, start_point, end_point, speed='speed', vector_x='uC',
                                                    vector_y='vC', case=case)
         traveltime = ((traveltime_s / 60) / 60) / 24
         distance = distance_m / 1000
         traveltimes.append(traveltime)
         distances.append(distance)
```

### Comparing `polar_route-0.3.9/polar_route/route_planner.py` & `polar_route-0.4.0/polar_route/route_planner.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,28 @@
     environmental mesh between a series of user defined waypoints
 '''
 
 import copy, json, ast, warnings
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
-from shapely import wkt
-from shapely.geometry.polygon import Point
+from shapely import wkt, Point, LineString, STRtree, Polygon
 import geopandas as gpd
 import logging
+from io import StringIO  
 
-from pandas.core.common import SettingWithCopyWarning
-warnings.simplefilter(action="ignore", category=SettingWithCopyWarning)
+# Squelching SettingWithCopyWarning 
+pd.options.mode.chained_assignment = None
 
 from polar_route.crossing import NewtonianDistance
 from polar_route.crossing_smoothing import Smoothing,PathValues,find_edge
 from polar_route.config_validation.config_validator import validate_route_config
 from polar_route.config_validation.config_validator import validate_waypoints
+from meshiphi import Boundary
+from meshiphi.utils import longitude_domain
 
 def _flattenCases(id,mesh):
     neighbour_case = []
     neighbour_indx = []
     neighbours = mesh['neighbour_graph'][id]
     for case in neighbours.keys():
         for neighbour in neighbours[case]:
@@ -119,18 +121,73 @@
     elif type(input) is str:
         try:
             output = pd.read_csv(input)
         except:
             raise Exception("Unable to load '{}', please check path name".format(input))
     return output
 
+def _mesh_boundary_polygon(mesh):
+    '''
+    Creates a polygon from the mesh boundary
+    '''
+
+    # Defining a tiny value
+    tiny_value = 1e-10
 
+    lat_min = mesh['config']['mesh_info']['region']['lat_min']-tiny_value
+    lat_max = mesh['config']['mesh_info']['region']['lat_max']+tiny_value
+    long_min = mesh['config']['mesh_info']['region']['long_min']-tiny_value
+    long_max = mesh['config']['mesh_info']['region']['long_max']+tiny_value
 
+    bounds = Boundary([lat_min, lat_max], [long_min, long_max])
 
+    return bounds.to_polygon()
 
+def _adjust_waypoints(point, cellboxes, max_distance=5):
+    '''
+    Moves waypoint to closest accessible cellbox if it isn't already in one
+    Allows up to 5 degrees flexibility by default
+    '''
+    # Extract cellboxes from mesh
+    cbs = gpd.GeoDataFrame.from_records(cellboxes)
+    # Prune inaccessible waypoints from search
+    cbs = cbs[cbs['inaccessible'] == False]
+    # Find nearest cellbox to point that is accessible
+    tree = STRtree(wkt.loads(cbs['geometry']))
+    nearest_cb = cbs.iloc[tree.nearest(point)]
+    cb_polygon = wkt.loads(nearest_cb['geometry'])
+    
+    if point.within(cb_polygon):
+        logging.debug(f'({point.y},{point.x}) in accessible cellbox')
+        return point
+    else:
+        logging.debug(f'({point.y},{point.x}) not in accessible cellbox')
+        # Create a line between CB centre and point
+        cb_centre = Point([nearest_cb['cx'],nearest_cb['cy']])
+        connecting_line = LineString([point, cb_centre])
+        # Extract segment of line inside the accessible cellbox    
+        intersecting_line = connecting_line.intersection(cb_polygon)
+        
+        # Put limit on how far it's allowed to adjust waypoint
+        distance_away = connecting_line.length - intersecting_line.length
+        if distance_away > max_distance:
+            logging.info(f'Waypoint too far from accessible cellbox!')
+            return point
+        
+        # Find where it meets the cellbox boundary
+        boundary_point = connecting_line.intersection(cb_polygon.exterior)
+        # Draw a small circle around it
+        buffered_point = boundary_point.buffer(intersecting_line.length*1e-3)
+        # Find point along line that intersects circle
+        adjusted_point = buffered_point.exterior.intersection(intersecting_line)
+        # Interior point is now a point inside the cellbox 
+        # that is not on the boundary
+        logging.info(f'({point.y},{point.x}) not accessible cellbox')
+        logging.info(f'Adjusted to ({adjusted_point.y},{adjusted_point.x})')
+        return adjusted_point
 class RoutePlanner:
     """
         ---
 
         RoutePlanner optimises the route paths between a series of waypoints. 
         The routes are constructed in a two stage process:
 
@@ -239,29 +296,53 @@
         """
         validate_route_config(config)
         validate_waypoints(waypoints)
         # Load in the current cell structure & Optimisation Info̦
         self.mesh             = _json_str(mesh)
         self.config           = _json_str(config)
         waypoints_df          = _pandas_dataframe_str(waypoints)
+
+        mesh_boundary = _mesh_boundary_polygon(self.mesh)
+        # Move waypoint to closest accessible cellbox if it isn't in one already
+        for idx, row in waypoints_df.iterrows():
+            point = Point([row['Long'], row['Lat']])
+            # Only allow waypoints within an existing mesh
+            assert(point.within(mesh_boundary)), \
+                f"Waypoint {row['Name']} outside of mesh boundary! {point}"
+            
+        
+
+            adjusted_point = _adjust_waypoints(point, self.mesh['cellboxes'])
+            
+            waypoints_df.loc[idx, 'Long'] = adjusted_point.x
+            waypoints_df.loc[idx, 'Lat'] = adjusted_point.y
+        
         source_waypoints_df   = waypoints_df[waypoints_df['Source'] == "X"]
         des_waypoints_df      = waypoints_df[waypoints_df['Destination'] == "X"]
 
         self.source_waypoints = list(source_waypoints_df['Name'])
         self.end_waypoints    = list(des_waypoints_df['Name'])
 
         # Case indices
         self.indx_type = np.array([1, 2, 3, 4, -1, -2, -3, -4])
 
         # Creating a blank path construct
         self.paths          = None
         self.smoothed_paths = None
         self.dijkstra_info = {}
 
+
+
+
+
+
         # ====== Loading Mesh & Neighbour Graph ======
+        # Zeroing currents if vectors names are not defined or zero_currents is defined
+        self.mesh = self._zero_currents(self.mesh)
+
         # Formatting the Mesh and Neighbour Graph to the right form
         self.neighbour_graph = pd.DataFrame(self.mesh['cellboxes']).set_index('id')
         self.neighbour_graph['geometry'] = self.neighbour_graph['geometry'].apply(wkt.loads)
         self.neighbour_graph = gpd.GeoDataFrame(self.neighbour_graph, crs='EPSG:4326', geometry='geometry')
 
         # Removing any point not in accessible positions
         self.neighbour_graph = self.neighbour_graph.loc[list(self.mesh['neighbour_graph'].keys())]
@@ -274,21 +355,21 @@
         # Renaming the vector columns
         self.neighbour_graph = self.neighbour_graph.rename(columns={self.config['vector_names'][0]: "Vector_x", 
                                                                     self.config['vector_names'][1]: "Vector_y"})
 
         # ====== Speed Function Checking ======
         # Checking if Speed defined in file
         if 'speed' not in self.neighbour_graph:
-            print(self.neighbour_graph.columns)
             raise Exception('Vessel Speed not in the mesh information ! Please run vessel performance')
         
         # ======= Sea-Ice Concentration ======
         if 'SIC' not in self.neighbour_graph:
             self.neighbour_graph['SIC'] = 0.0
 
+
         # ====== Objective Function Information ======
         #  Checking if objective function is in the dijkstra            
         if self.config['objective_function'] != 'traveltime':
             if self.config['objective_function'] not in self.neighbour_graph:
                 raise Exception("Objective Function require '{}' column in mesh dataframe".format(self.config['objective_function']))
 
         # ===== Dijkstra Graph =====
@@ -315,15 +396,14 @@
             self.neighbour_graph['speed'] = self.variable_speed
             cbxs = pd.DataFrame(self.mesh['cellboxes'])
             cbxs['speed'] = self.variable_speed
             self.mesh['cellboxes'] = cbxs.to_dict('records')
 
         # ====== Waypoints ======
         self.mesh['waypoints'] = waypoints_df
-
         # Initialising Waypoints positions and cell index
         wpts = self.mesh['waypoints']
         wpts['index'] = np.nan
         for idx,wpt in wpts.iterrows():
             indices = self.neighbour_graph[self.neighbour_graph['geometry'].contains(Point(wpt[['Long','Lat']]))].index
             # Waypoint is not within a mesh cell, but could still be on the edge of one. So perturbing the position slightly to the north-east and checking again. 
             #If this is not the case then the waypoint is not within the navigable domain and will continue
@@ -333,22 +413,22 @@
                 except:
                     continue
             if len(indices) == 0:
                 continue
             if len(indices) > 1:
                 raise Exception('Waypoint lies in multiple cell boxes. Please check mesh ! ')
             else:
-                wpts['index'].loc[idx] = int(indices[0])
+                wpts.loc[idx, 'index'] = int(indices[0])
 
         self.mesh['waypoints'] = wpts[~wpts['index'].isnull()]
         self.mesh['waypoints']['index'] = self.mesh['waypoints']['index'].astype(int)
         self.mesh['waypoints'] =  self.mesh['waypoints'].to_json()
 
         # ==== Printing Configuration and Information
-        self.mesh['waypoints'] =  pd.read_json(self.mesh['waypoints'])
+        self.mesh['waypoints'] =  pd.read_json(StringIO(self.mesh['waypoints']))
 
         # # ===== Running the route planner for the given information
         # if ("dijkstra_only" in self.config) and self.config['dijkstra_only']:
         #     self.compute_routes()
         # else:
         #     self.compute_routes()
         #     self.compute_smoothed_routes()
@@ -358,25 +438,118 @@
         # output = self.to_json()
         # if ('output' in self.config) and (type(self.config['output']) == str):
         #     with open(self.config['output'], 'w') as f:
         #         json.dump(output,f)
         # else:
         #     self.output = output
 
+    def _zero_currents(self,mesh):
+        '''
+            Applying zero currents to mesh
+
+            Input 
+                mesh (JSON) - MeshiPhi Mesh input
+            Output:
+                mesh (JSON) - MeshiPhi Mesh Corrected
+        '''
+
+        # Zeroing currents if both vectors are defined and zeroed
+        if ('zero_currents' in self.config) and ("vector_names" in self.config):
+            if self.config['zero_currents']:
+                logging.info('Zero Currents for Mesh !')
+                for idx,cell in enumerate(mesh['cellboxes']):
+                    cell[self.config['vector_names'][0]] = 0.0
+                    cell[self.config['vector_names'][1]] = 0.0
+                    mesh['cellboxes'][idx] = cell
+
+        # If no vectors are defined then add zero currents to mesh
+        if 'vector_names' not in self.config:
+            self.config['vector_names'] = ['Vector_x','Vector_y']
+            logging.info('No vector_names defined in config. Zeroing currents in mesh !')
+            for idx,cell in enumerate(mesh['cellboxes']):
+                cell[self.config['vector_names'][0]] = 0.0
+                cell[self.config['vector_names'][1]] = 0.0
+                mesh['cellboxes'][idx] = cell    
+            
+        return mesh
 
 
     def to_json(self):
         '''
             Outputting the information in JSON format
         '''
         mesh = copy.copy(self.mesh)
         mesh['waypoints'] = mesh['waypoints'].to_dict()
         output_json = json.loads(json.dumps(mesh))
         del mesh
         return output_json
+    
+    def to_charttracker_csv(self, route_name='PolarRoutePath'):
+        '''
+            Outputting route to chart tracker csv file
+        '''
+        def dd_to_dmm(dd, axis):    
+            '''
+            Converts decimal degrees to dmm formatted string
+            '''
+            if dd >= 0:
+                degs, mins = divmod(dd,1)
+                cardinal_dir = 'E' if axis == 'long' else 'N'
+            else:
+                degs, mins = divmod(-dd, 1)
+                cardinal_dir = 'W' if axis == 'long' else 'S'
+            return f"{int(degs)}-{60*mins:.3f}'{cardinal_dir}"
+        
+        def get_bearing(lat1, long1, lat2, long2):
+            '''
+            Calculates bearing of travel from lat/long pairs
+            '''
+            dlon = long2-long1
+            x = np.cos(np.radians(lat2)) * np.sin(np.radians(dlon))
+            y = np.cos(np.radians(lat1)) * np.sin(np.radians(lat2)) - \
+                np.sin(np.radians(lat1)) * np.cos(np.radians(lat2)) * np.cos(np.radians(dlon))
+            bearing = np.arctan2(x,y)
+            return np.degrees(bearing)
+        
+        # For each path, generate a csv string and add to list
+        path_csvs = []
+        for path_num, path in enumerate(self.smoothed_paths['features']):
+            header = f"Route Name:,{route_name}_{path_num}\n" + \
+                      "Way Point,Position,,Radius,Reach,ROT,XTD,SPD,RL/GC,Leg,Disance(NM),,ETA\n" + \
+                      "ID,LAT,LON,,,,,,,,To WPT,TOTAL\n"
+            # Turn coords into DMM format
+            coords = np.array(path['geometry']['coordinates'])
+            long = [dd_to_dmm(long, 'long') for long in coords[:,0]]
+            lat = [dd_to_dmm(lat, 'lat') for lat in coords[:,1]]
+            # Distance column
+            cumulative_distance = np.array(path['properties']['distance']) * 0.000539957 # In nautical miles  
+            distance = np.diff(cumulative_distance)
+            # Waypoint names
+            wps = [f'WP{i}' for i in range(len(cumulative_distance))]
+            leg = get_bearing(coords[:,1][:-1], coords[:,0][:-1],
+                            coords[:,1][1:], coords[:,0][1:])%360
+            eta = path['properties']['traveltime']
+            # Construct table with information
+            path_df = pd.DataFrame({'ID':wps,
+                                      'LAT':lat,
+                                      'LON':long,
+                                      'Radius':'',
+                                      'Reach':'',
+                                      'ROT':'',
+                                      'XTD':'',
+                                      'SPD':'',
+                                      'RL/GC':'RL',
+                                      'Leg':np.concatenate((leg, [np.nan])),
+                                      'To WPT':np.concatenate(([np.nan],distance)),
+                                      'TOTAL': cumulative_distance})
+            # Combine to one string and add to list of strs
+            csv_str = header + path_df.to_csv()
+            path_csvs += [csv_str]
+        # Return list of csv strings with each smoothed path
+        return path_csvs
 
     def _dijkstra_paths(self, start_waypoints, end_waypoints):
         """
             Hidden function. Given internal variables and start and end waypoints this function
             returns a GEOJSON formatted path dict object
 
             INPUTS:
@@ -404,14 +577,16 @@
                     try:
                         graph = self.dijkstra_info[wpt_a_name]
                         path = dict()
                         path['type'] = "Feature"
                         path['geometry'] = {}
                         path['geometry']['type'] = "LineString"
                         path_points = (np.array(wpt_a_loc+list(np.array(graph['pathPoints'].loc[wpt_b_index])[:-1, :])+wpt_b_loc))
+                        # Ensure all coordinates are in domain -180:180
+                        path_points[:,0] = longitude_domain(path_points[:,0])
                         path['geometry']['coordinates'] = path_points.tolist()
 
                         path['properties'] = {}
                         path['properties']['name'] = 'Route Path - {} to {}'.format(wpt_a_name, wpt_b_name)
                         path['properties']['from'] = '{}'.format(wpt_a_name)
                         path['properties']['to'] = '{}'.format(wpt_b_name)
 
@@ -534,15 +709,15 @@
         """
             Runs dijkstra across the whole of the domain.
         """
         # Including only the End Waypoints defined by the user
         wpts = self.mesh['waypoints'][self.mesh['waypoints']['Name'].isin(self.end_waypoints)]
         
         # Initialising zero traveltime at the source location
-        source_index = int(self.mesh['waypoints'][self.mesh['waypoints']['Name'] == wpt_name]['index'])
+        source_index = int(self.mesh['waypoints'][self.mesh['waypoints']['Name'] == wpt_name]['index'].iloc[0])
 
         for vrbl in self.config['path_variables']:
             self.dijkstra_info[wpt_name].loc[source_index, 'shortest_{}'.format(vrbl)] = 0.0
         self.dijkstra_info[wpt_name].loc[source_index, 'pathIndex'].append(source_index)
         
         # # Updating Dijkstra as long as all the waypoints are not visited or for full graph
         if self.config['early_stopping_criterion']:
@@ -648,14 +823,16 @@
             self.sf.forward()
 
             
             # ------ Smooth Path Values -----
             # Given a smoothed route path now determine the along path parameters.
             pv             = PathValues()
             path_info      = pv.objective_function(sf.aps,sf.start_waypoint,sf.end_waypoint)
+            # Ensure all coordinates are in domain -180:180
+            path_info['path'][:,0] = longitude_domain(path_info['path'][:,0])
             variables      = path_info['variables']
             TravelTimeLegs = variables['traveltime']['path_values']
             DistanceLegs   = variables['distance']['path_values'] 
             pathIndex      = variables['cell_index']['path_values'] 
             FuelLegs       = variables['fuel']['path_values'] 
             SpeedLegs      = variables['speed']['path_values'] 
 
@@ -674,11 +851,13 @@
             SmoothedPath['properties']['total_traveltime'] = SmoothedPath['properties']['traveltime'][-1]
             SmoothedPath['properties']['fuel']       = list(FuelLegs)
             SmoothedPath['properties']['total_fuel'] = SmoothedPath['properties']['fuel'][-1]
             SmoothedPath['properties']['distance']   = list(DistanceLegs)
             SmoothedPath['properties']['speed']      = list(SpeedLegs)
             SmoothedPaths += [SmoothedPath]
 
+            logging.info('{} iterations'.format(sf.jj))
+
         geojson['type'] = "FeatureCollection"
         geojson['features'] = SmoothedPaths
         self.smoothed_paths = geojson
         self.mesh['paths'] = self.smoothed_paths
```

### Comparing `polar_route-0.3.9/polar_route/utils.py` & `polar_route-0.4.0/polar_route/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Miscellaneous utility functions that may be of use throughout PolarRoute
 """
 
 import logging
 import time
 import tracemalloc
 import numpy as np
+import pandas as pd
+import geopandas as gpd
 
 from datetime import datetime, timedelta
 from functools import wraps
 from calendar import monthrange
 from scipy.fftpack import fftshift
 import json
     
@@ -354,7 +356,94 @@
             if unit == 'km/hr':
                 val = val*(1000/(60*60))
             if unit == 'knots':
                 val = (val*0.51)
             return val
         else:
             return None
+
+def gpx_route_import(f_name):
+    """
+        Function to import a route in gpx format and convert it to geojson format
+
+        Args:
+            f_name: Filename of gpx route file
+
+        Returns:
+            geojson: Route in geojson format
+    """
+    gdf_r = gpd.read_file(f_name, layer="routes")
+    gdf_p = gpd.read_file(f_name, layer="route_points")
+
+    # Drop empty fields from original gpx file
+    gdf_r = gdf_r.dropna(how='all', axis=1)
+    # Convert route to geojson linestring
+    geojson = json.loads(gdf_r.to_json())
+
+    # Extract start and end waypoints and add to geojson properties
+    geojson['features'][0]['properties']['from'] = gdf_p['name'].iloc[0]
+    geojson['features'][0]['properties']['to'] = gdf_p['name'].iloc[-1]
+
+    return geojson
+
+def to_chart_track_csv(route):
+    """
+        Output a route in Chart Track csv format
+    """
+
+    def dd_to_dmm(dd, axis):
+        """
+        Converts decimal degrees to dmm formatted string
+        """
+        if dd >= 0:
+            degs, mins = divmod(dd, 1)
+            cardinal_dir = 'E' if axis == 'long' else 'N'
+        else:
+            degs, mins = divmod(-dd, 1)
+            cardinal_dir = 'W' if axis == 'long' else 'S'
+        return f"{int(degs)}-{60 * mins:.3f}'{cardinal_dir}"
+
+    def get_bearing(lat1, long1, lat2, long2):
+        """
+        Calculate bearing of travel from lat/long pairs
+        """
+        dlon = long2 - long1
+        x = np.cos(np.radians(lat2)) * np.sin(np.radians(dlon))
+        y = np.cos(np.radians(lat1)) * np.sin(np.radians(lat2)) - \
+            np.sin(np.radians(lat1)) * np.cos(np.radians(lat2)) * np.cos(np.radians(dlon))
+        bearing = np.arctan2(x, y)
+        return np.degrees(bearing)
+
+    # For path, generate a csv string (typo to match output from Chart Track)
+    header = f"Route Name:,{route['properties']['from']}_{route['properties']['to']}\n" + \
+             "Way Point,Position,,Radius,Reach,ROT,XTD,SPD,RL/GC,Leg,Disance(NM),,ETA\n" + \
+             "ID,LAT,LON,,,,,,,,To WPT,TOTAL\n"
+    # Turn coords into DMM format
+    coords = np.array(route['geometry']['coordinates'])
+    long = [dd_to_dmm(long, 'long') for long in coords[:, 0]]
+    lat = [dd_to_dmm(lat, 'lat') for lat in coords[:, 1]]
+    # Distance column
+    cumulative_distance = np.array(route['properties']['distance']) * 0.000539957  # In nautical miles
+    distance = np.diff(cumulative_distance)
+    # Waypoint names
+    wps = [f'WP{i}' for i in range(len(cumulative_distance))]
+    leg = get_bearing(coords[:, 1][:-1], coords[:, 0][:-1],
+                      coords[:, 1][1:], coords[:, 0][1:]) % 360
+    eta = route['properties']['traveltime']
+    # Construct table with information
+    path_df = pd.DataFrame({'ID': wps,
+                            'LAT': lat,
+                            'LON': long,
+                            'Radius': '',
+                            'Reach': '',
+                            'ROT': '',
+                            'XTD': '',
+                            'SPD': '',
+                            'RL/GC': 'RL',
+                            'Leg': np.concatenate((leg, [np.nan])),
+                            'To WPT': np.concatenate(([np.nan], distance)),
+                            'TOTAL': cumulative_distance})
+    # Combine to one string and add to list of strs
+    csv_str = header + path_df.to_csv()
+    return csv_str
+
+
```

### Comparing `polar_route-0.3.9/polar_route/vessel_performance/abstract_vessel.py` & `polar_route-0.4.0/polar_route/vessel_performance/abstract_vessel.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/vessel_performance/vessel_factory.py` & `polar_route-0.4.0/polar_route/vessel_performance/vessel_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from polar_route.vessel_performance.vessels.SDA import SDA
 from polar_route.vessel_performance.vessels.slocum import SlocumGlider
+from polar_route.vessel_performance.vessels.example_ship import ExampleShip
 
 class VesselFactory:
     """
         Factory class to produce initialised vessel objects.
     """
     @classmethod
     def get_vessel(cls, config):
@@ -14,15 +15,18 @@
                 config (dict): a vessel config dictionary
 
             Returns:
                 vessel: an instance of a vessel class designed for performance modelling
         """
         vessel_requirements = {"SDA": (SDA, ["max_speed", "unit", "beam", "hull_type", "force_limit", "max_ice_conc",
                                              "min_depth"]),
-                               "Slocum": (SlocumGlider, ["max_speed", "unit", "max_ice_conc", "min_depth"])}
+                               "Slocum": (SlocumGlider, ["max_speed", "unit", "max_ice_conc", "min_depth"]),
+                               "example_ship": (ExampleShip, ["max_speed", "unit", "beam", "hull_type", "force_limit",
+                                                              "max_ice_conc", "min_depth"])
+                               }
 
         vessel_type = config['vessel_type']
 
         if vessel_type in vessel_requirements:
             vessel_class = vessel_requirements[vessel_type][0]
             required_params = vessel_requirements[vessel_type][1]
         else:
```

### Comparing `polar_route-0.3.9/polar_route/vessel_performance/vessels/SDA.py` & `polar_route-0.4.0/polar_route/vessel_performance/vessels/SDA.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/vessel_performance/vessels/abstract_glider.py` & `polar_route-0.4.0/polar_route/vessel_performance/vessels/abstract_glider.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/vessel_performance/vessels/abstract_ship.py` & `polar_route-0.4.0/polar_route/vessel_performance/vessels/abstract_ship.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route/vessel_performance/vessels/slocum.py` & `polar_route-0.4.0/polar_route/vessel_performance/vessels/slocum.py`

 * *Files identical despite different names*

### Comparing `polar_route-0.3.9/polar_route.egg-info/PKG-INFO` & `polar_route-0.4.0/polar_route.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 Metadata-Version: 2.1
 Name: polar-route
-Version: 0.3.9
+Version: 0.4.0
 Summary: PolarRoute: Long-distance maritime polar route planning taking into account complex changing environmental conditions
 Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox
-Author-email: polarroute@bas.ac.uk
-Maintainer: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox
-Maintainer-email: polarroute@bas.ac.uk
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Author-email: amop@bas.ac.uk
+Maintainer: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
+Maintainer-email: amop@bas.ac.uk
 License: MIT
-Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
-Classifier: 
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
+# PolarRoute
+
 ![](logo.jpg)
 
-<a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
 <a href="https://antarctica.github.io/PolarRoute/"><img src="https://img.shields.io/badge/Manual%20-github.io%2FPolarRoute%2F-red" alt="Manual Page">
-<a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPi">
+<a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
+<a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPI">
 <a href="https://github.com/antarctica/PolarRoute/tags"><img src="https://img.shields.io/github/v/tag/antarctica/PolarRoute" alt="Release Tag"></a>
 <a href="https://github.com/antarctica/PolarRoute/issues"><img src="https://img.shields.io/github/issues/antarctica/PolarRoute" alt="Issues"></a>
 <a href="https://github.com/antarctica/PolarRoute/blob/main/LICENSE"><img src="https://img.shields.io/github/license/antarctica/PolarRoute" alt="License"></a>
 
-# PolarRoute
-PolarRoute is a long-distance maritime polar route planning package, taking into account complex changing environmental conditions. The codebase allows the construction of optimised routes through three main stages: discrete modelling of the environmental conditions using a non-uniform mesh, the construction of mesh-optimal paths, and physics informed path smoothing. In order to account for different vehicle properties we construct a series of data driven functions that can be applied to the environmental mesh to determine the speed limitations and fuel requirements for a given vessel and mesh cell, representing these quantities graphically and geospatially.
+PolarRoute is a long-distance maritime polar route planning package, able to take into account complex and changing environmental conditions. It allows the construction of optimised routes through three main stages: discrete modelling of the environmental conditions using a non-uniform mesh, the construction of mesh-optimal paths, and physics informed path smoothing. In order to account for different vehicle properties we construct a series of data-driven functions that can be applied to the environmental mesh to determine the speed limitations and fuel requirements for a given vessel and mesh cell. The environmental modelling component of this functionality is provided by the [MeshiPhi](https://github.com/antarctica/MeshiPhi) library.
 
 ## Installation
-The PolarRoute package requires GDAL files to be installed. This software can be installed on Windows by running the required wheels for GDAL and FIONA. More information can be found in the manual pages linked above. Once these requirements are met then the software can be installed by:
 
-Github:
+PolarRoute is available from PyPI and can be installed by running: 
 ```
-git clone https://github.com/Antarctica/PolarRoute
-python setup.py install
+pip install polar-route
 ```
 
- Pip: 
+Alternatively you can install PolarRoute by downloading the source code from GitHub:
 ```
-pip install polar-route
+git clone https://github.com/Antarctica/PolarRoute
+pip install -e ./PolarRoute
 ```
+Use of `-e` is optional, based on whether you want to be able to edit the installed copy of the package.
 
-> NOTE: The installation process may vary slightly dependent on OS. Please consult the documentation for further installation guidance.
+> NOTE: Some features of the PolarRoute package require GDAL to be installed. Please consult the documentation for further guidance.
 
 ## Required Data sources
-Polar-route has been built to work with a variety of open-source atmospheric and oceanographic data sources. 
-A list of supported data sources and their associated data-loaders is given in the 
-'Data Loaders' section of the manual
+PolarRoute has been built to work with a variety of open-source atmospheric and oceanographic data sources. For testing and demonstration purposes it is also possible to generate artificial Gaussian Random Field data.  
+
+A full list of supported data sources and their associated dataloaders is given in the 
+'Dataloader Overview' section of the [MeshiPhi manual](https://antarctica.github.io/MeshiPhi/)
 
 ## Documentation
-Sphinx is used to generate documentation for this project. The dependencies can be installed through pip:
+The documentation for the package is available to read at: https://antarctica.github.io/PolarRoute/
+
+If you make changes to the source of the documentation you will need to rebuild the corresponding html files using Sphinx.
+The dependencies for this can be installed through pip:
 ```
 pip install sphinx sphinx_markdown_builder sphinx_rtd_theme rinohtype
 ```
 When updating the docs, run the following command within the PolarRoute directory to recompile.
 ```
 sphinx-build -b html ./docs/source ./docs/html
 ```
 Sometimes the cache needs to be cleared for internal links to update. If facing this problem, run this from the PolarRoute directory.
 ```
-rm -r docs/build/.doctrees/
+rm -r docs/html/.doctrees/
 ```
 ## Developers
-Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox, Harrison Abbot, Ayat Fekry
+Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey
 
 ## Collaboration
-We are currently assessing the best practice for collaboration on the codebase, until then please contact [polarroute@bas.ac.uk](polarroute@bas.ac.uk) for further info.
-
+We are currently assessing the best practice for collaboration on the codebase, until then please contact [amop@bas.ac.uk](amop@bas.ac.uk) for further info.
 
 ## License
 This software is licensed under a MIT license, but request users cite our publication.  
 
-Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne,  J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox,  (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
+Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne, J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox, (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
 
 For more information please see the attached ``LICENSE`` file. 
 
 [version]: https://img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square
```

#### html2text {}

```diff
@@ -1,54 +1,58 @@
-Metadata-Version: 2.1 Name: polar-route Version: 0.3.9 Summary: PolarRoute:
+Metadata-Version: 2.1 Name: polar-route Version: 0.4.0 Summary: PolarRoute:
 Long-distance maritime polar route planning taking into account complex
 changing environmental conditions Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry,
-James Byrne, Michael Thorne, Maria Fox Author-email: polarroute@bas.ac.uk
-Maintainer: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat
-Fekry, James Byrne, Michael Thorne, Maria Fox Maintainer-email:
-polarroute@bas.ac.uk License: MIT Classifier: Classifier: Development Status ::
-3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: System Administrators Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Topic :: Scientific/Engineering Classifier: Description-
-Content-Type: text/markdown Provides-Extra: tests License-File: LICENSE ![]
-(logo.jpg) _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_M_a_n_u_a_l_ _P_a_g_e_]_[_P_y_P_i_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_#
-_P_o_l_a_r_R_o_u_t_e_ _P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_ _l_o_n_g_-_d_i_s_t_a_n_c_e_ _m_a_r_i_t_i_m_e_ _p_o_l_a_r_ _r_o_u_t_e_ _p_l_a_n_n_i_n_g_ _p_a_c_k_a_g_e_,
-_t_a_k_i_n_g_ _i_n_t_o_ _a_c_c_o_u_n_t_ _c_o_m_p_l_e_x_ _c_h_a_n_g_i_n_g_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_._ _T_h_e_ _c_o_d_e_b_a_s_e
-_a_l_l_o_w_s_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _o_p_t_i_m_i_s_e_d_ _r_o_u_t_e_s_ _t_h_r_o_u_g_h_ _t_h_r_e_e_ _m_a_i_n_ _s_t_a_g_e_s_:_ _d_i_s_c_r_e_t_e
-_m_o_d_e_l_l_i_n_g_ _o_f_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_ _u_s_i_n_g_ _a_ _n_o_n_-_u_n_i_f_o_r_m_ _m_e_s_h_,_ _t_h_e
-_c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _m_e_s_h_-_o_p_t_i_m_a_l_ _p_a_t_h_s_,_ _a_n_d_ _p_h_y_s_i_c_s_ _i_n_f_o_r_m_e_d_ _p_a_t_h_ _s_m_o_o_t_h_i_n_g_._ _I_n
-_o_r_d_e_r_ _t_o_ _a_c_c_o_u_n_t_ _f_o_r_ _d_i_f_f_e_r_e_n_t_ _v_e_h_i_c_l_e_ _p_r_o_p_e_r_t_i_e_s_ _w_e_ _c_o_n_s_t_r_u_c_t_ _a_ _s_e_r_i_e_s_ _o_f_ _d_a_t_a
-_d_r_i_v_e_n_ _f_u_n_c_t_i_o_n_s_ _t_h_a_t_ _c_a_n_ _b_e_ _a_p_p_l_i_e_d_ _t_o_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_e_s_h_ _t_o_ _d_e_t_e_r_m_i_n_e_ _t_h_e
-_s_p_e_e_d_ _l_i_m_i_t_a_t_i_o_n_s_ _a_n_d_ _f_u_e_l_ _r_e_q_u_i_r_e_m_e_n_t_s_ _f_o_r_ _a_ _g_i_v_e_n_ _v_e_s_s_e_l_ _a_n_d_ _m_e_s_h_ _c_e_l_l_,
-_r_e_p_r_e_s_e_n_t_i_n_g_ _t_h_e_s_e_ _q_u_a_n_t_i_t_i_e_s_ _g_r_a_p_h_i_c_a_l_l_y_ _a_n_d_ _g_e_o_s_p_a_t_i_a_l_l_y_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n_ _T_h_e
-_P_o_l_a_r_R_o_u_t_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_s_ _G_D_A_L_ _f_i_l_e_s_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_._ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _c_a_n_ _b_e
-_i_n_s_t_a_l_l_e_d_ _o_n_ _W_i_n_d_o_w_s_ _b_y_ _r_u_n_n_i_n_g_ _t_h_e_ _r_e_q_u_i_r_e_d_ _w_h_e_e_l_s_ _f_o_r_ _G_D_A_L_ _a_n_d_ _F_I_O_N_A_._ _M_o_r_e
-_i_n_f_o_r_m_a_t_i_o_n_ _c_a_n_ _b_e_ _f_o_u_n_d_ _i_n_ _t_h_e_ _m_a_n_u_a_l_ _p_a_g_e_s_ _l_i_n_k_e_d_ _a_b_o_v_e_._ _O_n_c_e_ _t_h_e_s_e
-_r_e_q_u_i_r_e_m_e_n_t_s_ _a_r_e_ _m_e_t_ _t_h_e_n_ _t_h_e_ _s_o_f_t_w_a_r_e_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _b_y_:_ _G_i_t_h_u_b_:_ _`_`_`_ _g_i_t
-_c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/_P_o_l_a_r_R_o_u_t_e_ _p_y_t_h_o_n_ _s_e_t_u_p_._p_y_ _i_n_s_t_a_l_l_ _`_`_`_ _P_i_p_:
-_`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _p_o_l_a_r_-_r_o_u_t_e_ _`_`_`_ _>_ _N_O_T_E_:_ _T_h_e_ _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s_ _m_a_y_ _v_a_r_y
-_s_l_i_g_h_t_l_y_ _d_e_p_e_n_d_e_n_t_ _o_n_ _O_S_._ _P_l_e_a_s_e_ _c_o_n_s_u_l_t_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _f_u_r_t_h_e_r
-_i_n_s_t_a_l_l_a_t_i_o_n_ _g_u_i_d_a_n_c_e_._ _#_#_ _R_e_q_u_i_r_e_d_ _D_a_t_a_ _s_o_u_r_c_e_s_ _P_o_l_a_r_-_r_o_u_t_e_ _h_a_s_ _b_e_e_n_ _b_u_i_l_t_ _t_o
-_w_o_r_k_ _w_i_t_h_ _a_ _v_a_r_i_e_t_y_ _o_f_ _o_p_e_n_-_s_o_u_r_c_e_ _a_t_m_o_s_p_h_e_r_i_c_ _a_n_d_ _o_c_e_a_n_o_g_r_a_p_h_i_c_ _d_a_t_a_ _s_o_u_r_c_e_s_.
-_A_ _l_i_s_t_ _o_f_ _s_u_p_p_o_r_t_e_d_ _d_a_t_a_ _s_o_u_r_c_e_s_ _a_n_d_ _t_h_e_i_r_ _a_s_s_o_c_i_a_t_e_d_ _d_a_t_a_-_l_o_a_d_e_r_s_ _i_s_ _g_i_v_e_n_ _i_n
-_t_h_e_ _'_D_a_t_a_ _L_o_a_d_e_r_s_'_ _s_e_c_t_i_o_n_ _o_f_ _t_h_e_ _m_a_n_u_a_l_ _#_#_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_p_h_i_n_x_ _i_s_ _u_s_e_d_ _t_o
-_g_e_n_e_r_a_t_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _t_h_i_s_ _p_r_o_j_e_c_t_._ _T_h_e_ _d_e_p_e_n_d_e_n_c_i_e_s_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d
-_t_h_r_o_u_g_h_ _p_i_p_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _s_p_h_i_n_x_ _s_p_h_i_n_x___m_a_r_k_d_o_w_n___b_u_i_l_d_e_r_ _s_p_h_i_n_x___r_t_d___t_h_e_m_e
-_r_i_n_o_h_t_y_p_e_ _`_`_`_ _W_h_e_n_ _u_p_d_a_t_i_n_g_ _t_h_e_ _d_o_c_s_,_ _r_u_n_ _t_h_e_ _f_o_l_l_o_w_i_n_g_ _c_o_m_m_a_n_d_ _w_i_t_h_i_n_ _t_h_e
-_P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_ _t_o_ _r_e_c_o_m_p_i_l_e_._ _`_`_`_ _s_p_h_i_n_x_-_b_u_i_l_d_ _-_b_ _h_t_m_l_ _._/_d_o_c_s_/_s_o_u_r_c_e_ _._/
-_d_o_c_s_/_h_t_m_l_ _`_`_`_ _S_o_m_e_t_i_m_e_s_ _t_h_e_ _c_a_c_h_e_ _n_e_e_d_s_ _t_o_ _b_e_ _c_l_e_a_r_e_d_ _f_o_r_ _i_n_t_e_r_n_a_l_ _l_i_n_k_s_ _t_o
-_u_p_d_a_t_e_._ _I_f_ _f_a_c_i_n_g_ _t_h_i_s_ _p_r_o_b_l_e_m_,_ _r_u_n_ _t_h_i_s_ _f_r_o_m_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_._ _`_`_`_ _r_m
-_-_r_ _d_o_c_s_/_b_u_i_l_d_/_._d_o_c_t_r_e_e_s_/_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_e_r_s_ _J_o_n_a_t_h_a_n_ _S_m_i_t_h_,_ _S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e
-_C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _T_h_o_r_n_e_,_ _M_a_r_i_a_ _F_o_x_,_ _H_a_r_r_i_s_o_n_ _A_b_b_o_t_,_ _A_y_a_t_ _F_e_k_r_y_ _#_#
+Author: Autonomous Marine Operations Planning (AMOP) Team, AI Lab, British
+Antarctic Survey Author-email: amop@bas.ac.uk Maintainer: Autonomous Marine
+Operations Planning (AMOP) Team, AI Lab, British Antarctic Survey Maintainer-
+email: amop@bas.ac.uk License: MIT Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: System Administrators Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
+markdown Provides-Extra: tests License-File: LICENSE # PolarRoute ![](logo.jpg)
+_[_M_a_n_u_a_l_ _P_a_g_e_]_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_P_y_P_I_]_[_R_e_l_e_a_s_e_ _T_a_g_]_[_I_s_s_u_e_s_]_[_L_i_c_e_n_s_e_]_P_o_l_a_r_R_o_u_t_e_ _i_s_ _a
+_l_o_n_g_-_d_i_s_t_a_n_c_e_ _m_a_r_i_t_i_m_e_ _p_o_l_a_r_ _r_o_u_t_e_ _p_l_a_n_n_i_n_g_ _p_a_c_k_a_g_e_,_ _a_b_l_e_ _t_o_ _t_a_k_e_ _i_n_t_o_ _a_c_c_o_u_n_t
+_c_o_m_p_l_e_x_ _a_n_d_ _c_h_a_n_g_i_n_g_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_._ _I_t_ _a_l_l_o_w_s_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f
+_o_p_t_i_m_i_s_e_d_ _r_o_u_t_e_s_ _t_h_r_o_u_g_h_ _t_h_r_e_e_ _m_a_i_n_ _s_t_a_g_e_s_:_ _d_i_s_c_r_e_t_e_ _m_o_d_e_l_l_i_n_g_ _o_f_ _t_h_e
+_e_n_v_i_r_o_n_m_e_n_t_a_l_ _c_o_n_d_i_t_i_o_n_s_ _u_s_i_n_g_ _a_ _n_o_n_-_u_n_i_f_o_r_m_ _m_e_s_h_,_ _t_h_e_ _c_o_n_s_t_r_u_c_t_i_o_n_ _o_f_ _m_e_s_h_-
+_o_p_t_i_m_a_l_ _p_a_t_h_s_,_ _a_n_d_ _p_h_y_s_i_c_s_ _i_n_f_o_r_m_e_d_ _p_a_t_h_ _s_m_o_o_t_h_i_n_g_._ _I_n_ _o_r_d_e_r_ _t_o_ _a_c_c_o_u_n_t_ _f_o_r
+_d_i_f_f_e_r_e_n_t_ _v_e_h_i_c_l_e_ _p_r_o_p_e_r_t_i_e_s_ _w_e_ _c_o_n_s_t_r_u_c_t_ _a_ _s_e_r_i_e_s_ _o_f_ _d_a_t_a_-_d_r_i_v_e_n_ _f_u_n_c_t_i_o_n_s
+_t_h_a_t_ _c_a_n_ _b_e_ _a_p_p_l_i_e_d_ _t_o_ _t_h_e_ _e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_e_s_h_ _t_o_ _d_e_t_e_r_m_i_n_e_ _t_h_e_ _s_p_e_e_d
+_l_i_m_i_t_a_t_i_o_n_s_ _a_n_d_ _f_u_e_l_ _r_e_q_u_i_r_e_m_e_n_t_s_ _f_o_r_ _a_ _g_i_v_e_n_ _v_e_s_s_e_l_ _a_n_d_ _m_e_s_h_ _c_e_l_l_._ _T_h_e
+_e_n_v_i_r_o_n_m_e_n_t_a_l_ _m_o_d_e_l_l_i_n_g_ _c_o_m_p_o_n_e_n_t_ _o_f_ _t_h_i_s_ _f_u_n_c_t_i_o_n_a_l_i_t_y_ _i_s_ _p_r_o_v_i_d_e_d_ _b_y_ _t_h_e_ 
+_[_M_e_s_h_i_P_h_i_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_n_t_a_r_c_t_i_c_a_/_M_e_s_h_i_P_h_i_)_ _l_i_b_r_a_r_y_._ _#_#_ _I_n_s_t_a_l_l_a_t_i_o_n
+_P_o_l_a_r_R_o_u_t_e_ _i_s_ _a_v_a_i_l_a_b_l_e_ _f_r_o_m_ _P_y_P_I_ _a_n_d_ _c_a_n_ _b_e_ _i_n_s_t_a_l_l_e_d_ _b_y_ _r_u_n_n_i_n_g_:_ _`_`_`_ _p_i_p
+_i_n_s_t_a_l_l_ _p_o_l_a_r_-_r_o_u_t_e_ _`_`_`_ _A_l_t_e_r_n_a_t_i_v_e_l_y_ _y_o_u_ _c_a_n_ _i_n_s_t_a_l_l_ _P_o_l_a_r_R_o_u_t_e_ _b_y_ _d_o_w_n_l_o_a_d_i_n_g
+_t_h_e_ _s_o_u_r_c_e_ _c_o_d_e_ _f_r_o_m_ _G_i_t_H_u_b_:_ _`_`_`_ _g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_n_t_a_r_c_t_i_c_a_/
+_P_o_l_a_r_R_o_u_t_e_ _p_i_p_ _i_n_s_t_a_l_l_ _-_e_ _._/_P_o_l_a_r_R_o_u_t_e_ _`_`_`_ _U_s_e_ _o_f_ _`_-_e_`_ _i_s_ _o_p_t_i_o_n_a_l_,_ _b_a_s_e_d_ _o_n
+_w_h_e_t_h_e_r_ _y_o_u_ _w_a_n_t_ _t_o_ _b_e_ _a_b_l_e_ _t_o_ _e_d_i_t_ _t_h_e_ _i_n_s_t_a_l_l_e_d_ _c_o_p_y_ _o_f_ _t_h_e_ _p_a_c_k_a_g_e_._ _>_ _N_O_T_E_:
+_S_o_m_e_ _f_e_a_t_u_r_e_s_ _o_f_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _p_a_c_k_a_g_e_ _r_e_q_u_i_r_e_ _G_D_A_L_ _t_o_ _b_e_ _i_n_s_t_a_l_l_e_d_._ _P_l_e_a_s_e
+_c_o_n_s_u_l_t_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _f_u_r_t_h_e_r_ _g_u_i_d_a_n_c_e_._ _#_#_ _R_e_q_u_i_r_e_d_ _D_a_t_a_ _s_o_u_r_c_e_s
+_P_o_l_a_r_R_o_u_t_e_ _h_a_s_ _b_e_e_n_ _b_u_i_l_t_ _t_o_ _w_o_r_k_ _w_i_t_h_ _a_ _v_a_r_i_e_t_y_ _o_f_ _o_p_e_n_-_s_o_u_r_c_e_ _a_t_m_o_s_p_h_e_r_i_c_ _a_n_d
+_o_c_e_a_n_o_g_r_a_p_h_i_c_ _d_a_t_a_ _s_o_u_r_c_e_s_._ _F_o_r_ _t_e_s_t_i_n_g_ _a_n_d_ _d_e_m_o_n_s_t_r_a_t_i_o_n_ _p_u_r_p_o_s_e_s_ _i_t_ _i_s_ _a_l_s_o
+_p_o_s_s_i_b_l_e_ _t_o_ _g_e_n_e_r_a_t_e_ _a_r_t_i_f_i_c_i_a_l_ _G_a_u_s_s_i_a_n_ _R_a_n_d_o_m_ _F_i_e_l_d_ _d_a_t_a_._ _A_ _f_u_l_l_ _l_i_s_t_ _o_f
+_s_u_p_p_o_r_t_e_d_ _d_a_t_a_ _s_o_u_r_c_e_s_ _a_n_d_ _t_h_e_i_r_ _a_s_s_o_c_i_a_t_e_d_ _d_a_t_a_l_o_a_d_e_r_s_ _i_s_ _g_i_v_e_n_ _i_n_ _t_h_e
+_'_D_a_t_a_l_o_a_d_e_r_ _O_v_e_r_v_i_e_w_'_ _s_e_c_t_i_o_n_ _o_f_ _t_h_e_ _[_M_e_s_h_i_P_h_i_ _m_a_n_u_a_l_]_(_h_t_t_p_s_:_/_/
+_a_n_t_a_r_c_t_i_c_a_._g_i_t_h_u_b_._i_o_/_M_e_s_h_i_P_h_i_/_)_ _#_#_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _T_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _f_o_r_ _t_h_e
+_p_a_c_k_a_g_e_ _i_s_ _a_v_a_i_l_a_b_l_e_ _t_o_ _r_e_a_d_ _a_t_:_ _h_t_t_p_s_:_/_/_a_n_t_a_r_c_t_i_c_a_._g_i_t_h_u_b_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_ _I_f
+_y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _t_h_e_ _s_o_u_r_c_e_ _o_f_ _t_h_e_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ _y_o_u_ _w_i_l_l_ _n_e_e_d_ _t_o_ _r_e_b_u_i_l_d
+_t_h_e_ _c_o_r_r_e_s_p_o_n_d_i_n_g_ _h_t_m_l_ _f_i_l_e_s_ _u_s_i_n_g_ _S_p_h_i_n_x_._ _T_h_e_ _d_e_p_e_n_d_e_n_c_i_e_s_ _f_o_r_ _t_h_i_s_ _c_a_n_ _b_e
+_i_n_s_t_a_l_l_e_d_ _t_h_r_o_u_g_h_ _p_i_p_:_ _`_`_`_ _p_i_p_ _i_n_s_t_a_l_l_ _s_p_h_i_n_x_ _s_p_h_i_n_x___m_a_r_k_d_o_w_n___b_u_i_l_d_e_r
+_s_p_h_i_n_x___r_t_d___t_h_e_m_e_ _r_i_n_o_h_t_y_p_e_ _`_`_`_ _W_h_e_n_ _u_p_d_a_t_i_n_g_ _t_h_e_ _d_o_c_s_,_ _r_u_n_ _t_h_e_ _f_o_l_l_o_w_i_n_g
+_c_o_m_m_a_n_d_ _w_i_t_h_i_n_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e_ _d_i_r_e_c_t_o_r_y_ _t_o_ _r_e_c_o_m_p_i_l_e_._ _`_`_`_ _s_p_h_i_n_x_-_b_u_i_l_d_ _-_b_ _h_t_m_l
+_._/_d_o_c_s_/_s_o_u_r_c_e_ _._/_d_o_c_s_/_h_t_m_l_ _`_`_`_ _S_o_m_e_t_i_m_e_s_ _t_h_e_ _c_a_c_h_e_ _n_e_e_d_s_ _t_o_ _b_e_ _c_l_e_a_r_e_d_ _f_o_r
+_i_n_t_e_r_n_a_l_ _l_i_n_k_s_ _t_o_ _u_p_d_a_t_e_._ _I_f_ _f_a_c_i_n_g_ _t_h_i_s_ _p_r_o_b_l_e_m_,_ _r_u_n_ _t_h_i_s_ _f_r_o_m_ _t_h_e_ _P_o_l_a_r_R_o_u_t_e
+_d_i_r_e_c_t_o_r_y_._ _`_`_`_ _r_m_ _-_r_ _d_o_c_s_/_h_t_m_l_/_._d_o_c_t_r_e_e_s_/_ _`_`_`_ _#_#_ _D_e_v_e_l_o_p_e_r_s_ _A_u_t_o_n_o_m_o_u_s_ _M_a_r_i_n_e
+_O_p_e_r_a_t_i_o_n_s_ _P_l_a_n_n_i_n_g_ _(_A_M_O_P_)_ _T_e_a_m_,_ _A_I_ _L_a_b_,_ _B_r_i_t_i_s_h_ _A_n_t_a_r_c_t_i_c_ _S_u_r_v_e_y_ _#_#
 _C_o_l_l_a_b_o_r_a_t_i_o_n_ _W_e_ _a_r_e_ _c_u_r_r_e_n_t_l_y_ _a_s_s_e_s_s_i_n_g_ _t_h_e_ _b_e_s_t_ _p_r_a_c_t_i_c_e_ _f_o_r_ _c_o_l_l_a_b_o_r_a_t_i_o_n_ _o_n
-_t_h_e_ _c_o_d_e_b_a_s_e_,_ _u_n_t_i_l_ _t_h_e_n_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_]
-_(_p_o_l_a_r_r_o_u_t_e_@_b_a_s_._a_c_._u_k_)_ _f_o_r_ _f_u_r_t_h_e_r_ _i_n_f_o_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _i_s_ _l_i_c_e_n_s_e_d
-_u_n_d_e_r_ _a_ _M_I_T_ _l_i_c_e_n_s_e_,_ _b_u_t_ _r_e_q_u_e_s_t_ _u_s_e_r_s_ _c_i_t_e_ _o_u_r_ _p_u_b_l_i_c_a_t_i_o_n_._ _J_o_n_a_t_h_a_n_ _D_._ _S_m_i_t_h_,
-_S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e_ _C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _A_._ _S_._ _T_h_o_r_n_e_,_ _J_._ _A_l_e_x_a_n_d_e_r
-_B_r_e_a_r_l_e_y_,_ _D_e_r_e_k_ _L_o_n_g_,_ _M_i_c_h_a_e_l_ _M_e_r_e_d_i_t_h_,_ _M_a_r_i_a_ _F_o_x_,_ _(_2_0_2_2_)_,_ _A_u_t_o_n_o_m_o_u_s_ _P_a_s_s_a_g_e
-_P_l_a_n_n_i_n_g_ _f_o_r_ _a_ _P_o_l_a_r_ _V_e_s_s_e_l_,_ _a_r_X_i_v_,_ _h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_2_0_9_._0_2_3_8_9_ _F_o_r_ _m_o_r_e
-_i_n_f_o_r_m_a_t_i_o_n_ _p_l_e_a_s_e_ _s_e_e_ _t_h_e_ _a_t_t_a_c_h_e_d_ _`_`_L_I_C_E_N_S_E_`_`_ _f_i_l_e_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_v_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:
-_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
+_t_h_e_ _c_o_d_e_b_a_s_e_,_ _u_n_t_i_l_ _t_h_e_n_ _p_l_e_a_s_e_ _c_o_n_t_a_c_t_ _[_a_m_o_p_@_b_a_s_._a_c_._u_k_]_(_a_m_o_p_@_b_a_s_._a_c_._u_k_)_ _f_o_r
+_f_u_r_t_h_e_r_ _i_n_f_o_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _s_o_f_t_w_a_r_e_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _a_ _M_I_T_ _l_i_c_e_n_s_e_,_ _b_u_t
+_r_e_q_u_e_s_t_ _u_s_e_r_s_ _c_i_t_e_ _o_u_r_ _p_u_b_l_i_c_a_t_i_o_n_._ _J_o_n_a_t_h_a_n_ _D_._ _S_m_i_t_h_,_ _S_a_m_u_e_l_ _H_a_l_l_,_ _G_e_o_r_g_e
+_C_o_o_m_b_s_,_ _J_a_m_e_s_ _B_y_r_n_e_,_ _M_i_c_h_a_e_l_ _A_._ _S_._ _T_h_o_r_n_e_,_ _J_._ _A_l_e_x_a_n_d_e_r_ _B_r_e_a_r_l_e_y_,_ _D_e_r_e_k_ _L_o_n_g_,
+_M_i_c_h_a_e_l_ _M_e_r_e_d_i_t_h_,_ _M_a_r_i_a_ _F_o_x_,_ _(_2_0_2_2_)_,_ _A_u_t_o_n_o_m_o_u_s_ _P_a_s_s_a_g_e_ _P_l_a_n_n_i_n_g_ _f_o_r_ _a_ _P_o_l_a_r
+_V_e_s_s_e_l_,_ _a_r_X_i_v_,_ _h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_2_0_9_._0_2_3_8_9_ _F_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_ _p_l_e_a_s_e_ _s_e_e
+_t_h_e_ _a_t_t_a_c_h_e_d_ _`_`_L_I_C_E_N_S_E_`_`_ _f_i_l_e_._ _[_v_e_r_s_i_o_n_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_P_o_l_a_r_R_o_u_t_e_/_v_/
+_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_ _[_d_o_w_n_l_o_a_d_s_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_P_o_l_a_r_R_o_u_t_e_/_d_m_/_d_a_t_a_d_o_g_-_m_e_t_r_i_c_s_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e
```

### Comparing `polar_route-0.3.9/polar_route.egg-info/SOURCES.txt` & `polar_route-0.4.0/polar_route.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 polar_route/__init__.py
 polar_route/cli.py
 polar_route/crossing.py
 polar_route/crossing_smoothing.py
 polar_route/route_calc.py
 polar_route/route_planner.py
@@ -25,8 +26,9 @@
 polar_route/vessel_performance/abstract_vessel.py
 polar_route/vessel_performance/vessel_factory.py
 polar_route/vessel_performance/vessel_performance_modeller.py
 polar_route/vessel_performance/vessels/SDA.py
 polar_route/vessel_performance/vessels/__init__.py
 polar_route/vessel_performance/vessels/abstract_glider.py
 polar_route/vessel_performance/vessels/abstract_ship.py
+polar_route/vessel_performance/vessels/example_ship.py
 polar_route/vessel_performance/vessels/slocum.py
```

### Comparing `polar_route-0.3.9/setup.py` & `polar_route-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,31 @@
     author=polar_route.__author__,
     author_email=polar_route.__email__,
     maintainer=polar_route.__author__,
     maintainer_email=polar_route.__email__,
     url="https://www.github.com/antarctica",
     project_urls={
     },
-    classifiers=[el.lstrip() for el in """
-        Development Status :: 3 - Alpha
+    classifiers=[el.lstrip() for el in """Development Status :: 3 - Alpha
         Intended Audience :: Science/Research
         Intended Audience :: System Administrators
         License :: OSI Approved :: MIT License
         Natural Language :: English
         Operating System :: OS Independent
         Programming Language :: Python
         Programming Language :: Python :: 3
         Programming Language :: Python :: 3.7
-        Topic :: Scientific/Engineering
-    """.split('\n')],
+        Topic :: Scientific/Engineering""".split('\n')],
     entry_points={
         'console_scripts': [
             "add_vehicle=polar_route.cli:add_vehicle_cli",
             "optimise_routes=polar_route.cli:optimise_routes_cli",
             "calculate_route=polar_route.cli:calculate_route_cli",
-            "resimulate_vehicle=polar_route.cli:resimulate_vehicle_cli"],
+            "resimulate_vehicle=polar_route.cli:resimulate_vehicle_cli",
+            "extract_routes=polar_route.cli:extract_routes_cli"],
     },
     keywords=[],
     packages=find_packages(),
     install_requires=requirements,
     tests_require=["pytest"],
     extras_require={
         "tests": get_content("tests/requirements.txt"),
```


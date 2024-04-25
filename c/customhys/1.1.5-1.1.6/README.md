# Comparing `tmp/customhys-1.1.5.tar.gz` & `tmp/customhys-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customhys-1.1.5.tar", last modified: Wed Oct 25 16:19:51 2023, max compression
+gzip compressed data, was "customhys-1.1.6.tar", last modified: Thu Apr 25 20:43:12 2024, max compression
```

## Comparing `customhys-1.1.5.tar` & `customhys-1.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-10-25 16:19:51.388192 customhys-1.1.5/
--rw-r--r--   0 jcrvz      (501) staff       (20)     1080 2023-03-16 23:22:43.000000 customhys-1.1.5/LICENSE
--rw-r--r--   0 jcrvz      (501) staff       (20)      122 2023-03-16 23:22:43.000000 customhys-1.1.5/MANIFEST.in
--rw-r--r--   0 jcrvz      (501) staff       (20)    11963 2023-10-25 16:19:51.388090 customhys-1.1.5/PKG-INFO
--rw-r--r--   0 jcrvz      (501) staff       (20)    10931 2023-03-16 23:22:43.000000 customhys-1.1.5/README.md
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-10-25 16:19:51.366211 customhys-1.1.5/customhys/
--rw-r--r--   0 jcrvz      (501) staff       (20)      218 2023-10-25 16:19:39.000000 customhys-1.1.5/customhys/__init__.py
--rw-r--r--   0 jcrvz      (501) staff       (20)   126574 2023-04-15 01:56:12.000000 customhys-1.1.5/customhys/benchmark_func.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     8163 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/characterisation.py
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-10-25 16:19:51.372260 customhys-1.1.5/customhys/collections/
--rw-r--r--   0 jcrvz      (501) staff       (20)  1265347 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/collections/automatic.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)     8469 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/collections/basicmetaheuristics.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)    21255 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/collections/default.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)    92837 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/collections/operators_collection.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)   255391 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/collections/operators_weights.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     2842 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/collections/short_collection.txt
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-10-25 16:19:51.373252 customhys-1.1.5/customhys/exconf/
--rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/basic_metaheuristic.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1717 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/brute_force.json
--rw-r--r--   0 jcrvz      (501) staff       (20)      299 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/demo.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1147 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/demo_neural_network.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/long1.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1763 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/short1.json
--rw-r--r--   0 jcrvz      (501) staff       (20)     1713 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/exconf/short2.json
--rw-r--r--   0 jcrvz      (501) staff       (20)    18483 2023-10-25 15:54:05.000000 customhys-1.1.5/customhys/experiment.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    62806 2023-10-25 15:55:13.000000 customhys-1.1.5/customhys/hyperheuristic.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    13900 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/machine_learning.py
--rw-r--r--   0 jcrvz      (501) staff       (20)     7898 2023-07-14 01:06:31.000000 customhys-1.1.5/customhys/metaheuristic.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    45091 2023-10-25 15:55:13.000000 customhys-1.1.5/customhys/operators.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    15755 2023-07-14 00:11:45.000000 customhys-1.1.5/customhys/population.py
--rw-r--r--   0 jcrvz      (501) staff       (20)      483 2023-03-16 23:22:43.000000 customhys-1.1.5/customhys/test_solvers.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    19308 2023-10-25 15:55:13.000000 customhys-1.1.5/customhys/tools.py
--rw-r--r--   0 jcrvz      (501) staff       (20)    11413 2023-03-22 04:12:13.000000 customhys-1.1.5/customhys/visualisation.py
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-10-25 16:19:51.366866 customhys-1.1.5/customhys.egg-info/
--rw-r--r--   0 jcrvz      (501) staff       (20)    11963 2023-10-25 16:19:51.000000 customhys-1.1.5/customhys.egg-info/PKG-INFO
--rw-r--r--   0 jcrvz      (501) staff       (20)     1287 2023-10-25 16:19:51.000000 customhys-1.1.5/customhys.egg-info/SOURCES.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)        1 2023-10-25 16:19:51.000000 customhys-1.1.5/customhys.egg-info/dependency_links.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)      227 2023-10-25 16:19:51.000000 customhys-1.1.5/customhys.egg-info/requires.txt
--rw-r--r--   0 jcrvz      (501) staff       (20)       10 2023-10-25 16:19:51.000000 customhys-1.1.5/customhys.egg-info/top_level.txt
-drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2023-10-25 16:19:51.386127 customhys-1.1.5/docfiles/
--rw-r--r--   0 jcrvz      (501) staff       (20)   905189 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/SearchOperators_CEC.pdf
--rw-r--r--   0 jcrvz      (501) staff       (20)    16429 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/cas_logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)    42755 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/chm_logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)    28786 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/conacyt-logo.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   209268 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/dependency_diagram.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   743430 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/heuristics.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   137732 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/logoTEC_full.png
--rw-r--r--   0 jcrvz      (501) staff       (20)  1614825 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/methodology_cec_a.png
--rw-r--r--   0 jcrvz      (501) staff       (20)  2074059 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/methodology_cec_b.png
--rw-r--r--   0 jcrvz      (501) staff       (20)   452031 2023-03-16 23:22:43.000000 customhys-1.1.5/docfiles/operators.png
--rw-r--r--   0 jcrvz      (501) staff       (20)       86 2023-03-16 23:22:43.000000 customhys-1.1.5/pyproject.toml
--rw-r--r--   0 jcrvz      (501) staff       (20)       81 2023-10-25 16:19:51.388424 customhys-1.1.5/setup.cfg
--rw-r--r--   0 jcrvz      (501) staff       (20)     1387 2023-10-25 16:19:17.000000 customhys-1.1.5/setup.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2024-04-25 20:43:12.322037 customhys-1.1.6/
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1080 2023-03-16 23:22:43.000000 customhys-1.1.6/LICENSE
+-rw-r--r--   0 jcrvz      (501) staff       (20)      122 2023-03-16 23:22:43.000000 customhys-1.1.6/MANIFEST.in
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11963 2024-04-25 20:43:12.321906 customhys-1.1.6/PKG-INFO
+-rw-r--r--   0 jcrvz      (501) staff       (20)    10931 2023-03-16 23:22:43.000000 customhys-1.1.6/README.md
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2024-04-25 20:43:12.301591 customhys-1.1.6/customhys/
+-rw-r--r--   0 jcrvz      (501) staff       (20)      218 2024-04-25 20:42:37.000000 customhys-1.1.6/customhys/__init__.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)   126574 2023-04-15 01:56:12.000000 customhys-1.1.6/customhys/benchmark_func.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)     8163 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/characterisation.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2024-04-25 20:43:12.306238 customhys-1.1.6/customhys/collections/
+-rw-r--r--   0 jcrvz      (501) staff       (20)  1265347 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/collections/automatic.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)     8469 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/collections/basicmetaheuristics.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)    21255 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/collections/default.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)    92837 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/collections/operators_collection.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)   255391 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/collections/operators_weights.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     2842 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/collections/short_collection.txt
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2024-04-25 20:43:12.307561 customhys-1.1.6/customhys/exconf/
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/basic_metaheuristic.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1717 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/brute_force.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)      299 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/demo.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1147 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/demo_neural_network.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1747 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/long1.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1763 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/short1.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1713 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/exconf/short2.json
+-rw-r--r--   0 jcrvz      (501) staff       (20)    18483 2023-10-25 15:54:05.000000 customhys-1.1.6/customhys/experiment.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    62870 2023-10-26 18:01:20.000000 customhys-1.1.6/customhys/hyperheuristic.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    13900 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/machine_learning.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)     7898 2023-07-14 01:06:31.000000 customhys-1.1.6/customhys/metaheuristic.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    45112 2024-04-25 20:28:09.000000 customhys-1.1.6/customhys/operators.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    15755 2023-07-14 00:11:45.000000 customhys-1.1.6/customhys/population.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)      483 2023-03-16 23:22:43.000000 customhys-1.1.6/customhys/test_solvers.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    19308 2023-10-25 15:55:13.000000 customhys-1.1.6/customhys/tools.py
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11413 2023-03-22 04:12:13.000000 customhys-1.1.6/customhys/visualisation.py
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2024-04-25 20:43:12.302551 customhys-1.1.6/customhys.egg-info/
+-rw-r--r--   0 jcrvz      (501) staff       (20)    11963 2024-04-25 20:43:12.000000 customhys-1.1.6/customhys.egg-info/PKG-INFO
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1287 2024-04-25 20:43:12.000000 customhys-1.1.6/customhys.egg-info/SOURCES.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)        1 2024-04-25 20:43:12.000000 customhys-1.1.6/customhys.egg-info/dependency_links.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)      227 2024-04-25 20:43:12.000000 customhys-1.1.6/customhys.egg-info/requires.txt
+-rw-r--r--   0 jcrvz      (501) staff       (20)       10 2024-04-25 20:43:12.000000 customhys-1.1.6/customhys.egg-info/top_level.txt
+drwxr-xr-x   0 jcrvz      (501) staff       (20)        0 2024-04-25 20:43:12.318101 customhys-1.1.6/docfiles/
+-rw-r--r--   0 jcrvz      (501) staff       (20)   905189 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/SearchOperators_CEC.pdf
+-rw-r--r--   0 jcrvz      (501) staff       (20)    16429 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/cas_logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)    42755 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/chm_logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)    28786 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/conacyt-logo.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   209268 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/dependency_diagram.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   743430 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/heuristics.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   137732 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/logoTEC_full.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)  1614825 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/methodology_cec_a.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)  2074059 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/methodology_cec_b.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)   452031 2023-03-16 23:22:43.000000 customhys-1.1.6/docfiles/operators.png
+-rw-r--r--   0 jcrvz      (501) staff       (20)       86 2023-03-16 23:22:43.000000 customhys-1.1.6/pyproject.toml
+-rw-r--r--   0 jcrvz      (501) staff       (20)       81 2024-04-25 20:43:12.322284 customhys-1.1.6/setup.cfg
+-rw-r--r--   0 jcrvz      (501) staff       (20)     1387 2024-04-25 20:42:37.000000 customhys-1.1.6/setup.py
```

### Comparing `customhys-1.1.5/LICENSE` & `customhys-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/PKG-INFO` & `customhys-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customhys
-Version: 1.1.5
+Version: 1.1.6
 Summary: This framework provides tools for solving, but not limited to, continuous optimisation problems using a hyper-heuristic approach for customising metaheuristics. 
 Home-page: https://github.com/jcrvz/customhys
 Author: Jorge Mario Cruz-Duarte
 Author-email: jorge.cruz@tec.mx
 License: MIT License
 Keywords: metaheuristics,hyper-heuristic,optimization,automatic design,global optimization,evolutionary computation,bio-inspired,algorithm design
 Requires-Python: >=3.8
```

### Comparing `customhys-1.1.5/README.md` & `customhys-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/benchmark_func.py` & `customhys-1.1.6/customhys/benchmark_func.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/characterisation.py` & `customhys-1.1.6/customhys/characterisation.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/collections/automatic.txt` & `customhys-1.1.6/customhys/collections/automatic.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/collections/basicmetaheuristics.txt` & `customhys-1.1.6/customhys/collections/basicmetaheuristics.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/collections/default.txt` & `customhys-1.1.6/customhys/collections/default.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/collections/operators_collection.txt` & `customhys-1.1.6/customhys/collections/operators_collection.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/collections/operators_weights.json` & `customhys-1.1.6/customhys/collections/operators_weights.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/collections/short_collection.txt` & `customhys-1.1.6/customhys/collections/short_collection.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/exconf/basic_metaheuristic.json` & `customhys-1.1.6/customhys/exconf/basic_metaheuristic.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/exconf/brute_force.json` & `customhys-1.1.6/customhys/exconf/brute_force.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/exconf/demo_neural_network.json` & `customhys-1.1.6/customhys/exconf/demo_neural_network.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/exconf/long1.json` & `customhys-1.1.6/customhys/exconf/long1.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/exconf/short1.json` & `customhys-1.1.6/customhys/exconf/short1.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/exconf/short2.json` & `customhys-1.1.6/customhys/exconf/short2.json`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/experiment.py` & `customhys-1.1.6/customhys/experiment.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/hyperheuristic.py` & `customhys-1.1.6/customhys/hyperheuristic.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             heuristics like metaheuristics, and lvl:2 to high-level heuristics like hyper-heuristics.
         :param str file_label: Optional.
             Tag or label for saving files. The default is ''.
         :param numpy.array weights_array: Optional.
             Weights of the search operators, if there is a-priori information about them. The default is None.
         """
         # Read the heuristic space
+        # TODO: fix for any OS (now, it only works for Windows)
         if isinstance(heuristic_space, list):
             self.heuristic_space_label = 'custom_list'
             self.heuristic_space = heuristic_space
         elif isinstance(heuristic_space, str):
             self.heuristic_space_label = heuristic_space[:heuristic_space.rfind('.')].split('_')[0]
             with open('collections/' + heuristic_space, 'r', encoding='utf-8') as operators_file:
                 self.heuristic_space = [eval(line.rstrip('\n')) for line in operators_file]
```

### Comparing `customhys-1.1.5/customhys/machine_learning.py` & `customhys-1.1.6/customhys/machine_learning.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/metaheuristic.py` & `customhys-1.1.6/customhys/metaheuristic.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/operators.py` & `customhys-1.1.6/customhys/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,33 +500,35 @@
         dimension_indices = np.random.randint(0, pop.num_dimensions, num_mutations)
 
         if num_elite > 0:
             agent_indices = np.argsort(pop.fitness)[np.random.randint(num_elite, pop.num_agents, num_mutations)]
         else:
             agent_indices = np.random.randint(num_elite, pop.num_agents, num_mutations)
 
-        # Transform indices
-        rows, columns = np.meshgrid(agent_indices, dimension_indices)
+        flat_rows = agent_indices.flatten()
+        flat_columns = dimension_indices.flatten()
+
+        total_mutations = len(flat_rows)
 
         # Perform mutation according to the random distribution
         if distribution == 'uniform':
-            mutants = np.random.uniform(-1, 1, num_mutations ** 2)
+            mutants = np.random.uniform(-1, 1, total_mutations)
 
         elif distribution == 'gaussian':
             # Normal with mu = 0 and sigma = parameter
-            mutants = np.random.standard_normal(num_mutations ** 2)
+            mutants = np.random.standard_normal(total_mutations)
 
         elif distribution == 'levy':
-            mutants = _random_levy(num_mutations ** 2, 1.5)
+            mutants = _random_levy(total_mutations, 1.5)
 
         else:
             raise OperatorsError('Invalid distribution!')
 
         # Store mutants
-        pop.positions[rows.flatten(), columns.flatten()] = scale * mutants
+        pop.positions[flat_rows, flat_columns] += scale * mutants
 
 
 def gravitational_search(pop, gravity=1.0, alpha=0.02):
     """
     Apply the gravitational search from Gravitational Search Algorithm (GSA) to the population's positions
     (pop.positions).
```

### Comparing `customhys-1.1.5/customhys/population.py` & `customhys-1.1.6/customhys/population.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/tools.py` & `customhys-1.1.6/customhys/tools.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys/visualisation.py` & `customhys-1.1.6/customhys/visualisation.py`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/customhys.egg-info/PKG-INFO` & `customhys-1.1.6/customhys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customhys
-Version: 1.1.5
+Version: 1.1.6
 Summary: This framework provides tools for solving, but not limited to, continuous optimisation problems using a hyper-heuristic approach for customising metaheuristics. 
 Home-page: https://github.com/jcrvz/customhys
 Author: Jorge Mario Cruz-Duarte
 Author-email: jorge.cruz@tec.mx
 License: MIT License
 Keywords: metaheuristics,hyper-heuristic,optimization,automatic design,global optimization,evolutionary computation,bio-inspired,algorithm design
 Requires-Python: >=3.8
```

### Comparing `customhys-1.1.5/customhys.egg-info/SOURCES.txt` & `customhys-1.1.6/customhys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/SearchOperators_CEC.pdf` & `customhys-1.1.6/docfiles/SearchOperators_CEC.pdf`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/cas_logo.png` & `customhys-1.1.6/docfiles/cas_logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/chm_logo.png` & `customhys-1.1.6/docfiles/chm_logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/conacyt-logo.png` & `customhys-1.1.6/docfiles/conacyt-logo.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/dependency_diagram.png` & `customhys-1.1.6/docfiles/dependency_diagram.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/heuristics.png` & `customhys-1.1.6/docfiles/heuristics.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/logoTEC_full.png` & `customhys-1.1.6/docfiles/logoTEC_full.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/methodology_cec_a.png` & `customhys-1.1.6/docfiles/methodology_cec_a.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/methodology_cec_b.png` & `customhys-1.1.6/docfiles/methodology_cec_b.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/docfiles/operators.png` & `customhys-1.1.6/docfiles/operators.png`

 * *Files identical despite different names*

### Comparing `customhys-1.1.5/setup.py` & `customhys-1.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 # The text of the README file
 README = (pathlib.Path(__file__).parent / 'README.md').read_text(encoding='utf-8')
 
 setuptools.setup(
     name='customhys',
-    version='1.1.5',
+    version='1.1.6',
     packages=setuptools.find_packages(),
     url='https://github.com/jcrvz/customhys',
     license='MIT License',
     author='Jorge Mario Cruz-Duarte',
     author_email='jorge.cruz@tec.mx',
     description='This framework provides tools for solving, but not limited to, continuous optimisation problems '
                 'using a hyper-heuristic approach for customising metaheuristics. ',
```


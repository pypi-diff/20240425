# Comparing `tmp/setga-1.3.5.tar.gz` & `tmp/setga-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setga-1.3.5.tar", last modified: Mon Apr 15 13:47:26 2024, max compression
+gzip compressed data, was "setga-1.4.tar", last modified: Thu Apr 25 13:23:37 2024, max compression
```

## Comparing `setga-1.3.5.tar` & `setga-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:26.078578 setga-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 13:47:23.000000 setga-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 13:47:26.078578 setga-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-15 13:47:23.000000 setga-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:26.078578 setga-1.3.5/setga/
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-15 13:47:23.000000 setga-1.3.5/setga/select_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-15 13:47:23.000000 setga-1.3.5/setga/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:47:26.078578 setga-1.3.5/setga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 13:47:26.000000 setga-1.3.5/setga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 13:47:26.000000 setga-1.3.5/setga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:47:26.000000 setga-1.3.5/setga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:47:26.000000 setga-1.3.5/setga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 13:47:26.000000 setga-1.3.5/setga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 13:47:26.078578 setga-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 13:47:24.000000 setga-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:23:37.567104 setga-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 13:23:35.000000 setga-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 13:23:37.567104 setga-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 13:23:35.000000 setga-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:23:37.567104 setga-1.4/setga/
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-25 13:23:35.000000 setga-1.4/setga/select_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-25 13:23:35.000000 setga-1.4/setga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:23:37.567104 setga-1.4/setga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 13:23:37.000000 setga-1.4/setga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-25 13:23:37.000000 setga-1.4/setga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:23:37.000000 setga-1.4/setga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 13:23:37.000000 setga-1.4/setga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 13:23:37.000000 setga-1.4/setga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 13:23:37.567104 setga-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 13:23:36.000000 setga-1.4/setup.py
```

### Comparing `setga-1.3.5/LICENSE` & `setga-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `setga-1.3.5/PKG-INFO` & `setga-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.3.5
+Version: 1.4
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
 Project-URL: Documentation, https://setga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
```

### Comparing `setga-1.3.5/README.md` & `setga-1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. image:: https://readthedocs.org/projects/setga/badge/?version=latest
+    :target: https://setga.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
 # Minimal Subset Optimizer
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
 ![Visitors](https://api.visitorbadge.io/api/visitors?path=https://github.com/lavakin/TraP-GA&label=Visitors&countColor=%23263759&style=flat)
 
 ## Overview
```

### Comparing `setga-1.3.5/setga/select_subset.py` & `setga-1.4/setga/select_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,18 @@
     if callable(crossover):
         toolbox.register("mate", crossover)
     if crossover not in ["uniform", "onepoint","twopoint","partialy_matched","ordered","uniform_partialy_matched"] and not callable(crossover):
         raise WrongType("Unknown type of crossover")
 
     if selection == "SPEA2":
         toolbox.register("select", tools.selSPEA2)
-    if selection == "NGSA2":
-        toolbox.register("select", tools.selNGSA2)
+    if selection == "NSGA2":
+        toolbox.register("select", tools.selNSGA2)
+    if crossover not in ["SPEA2","NSGA2"]:
+        raise WrongType("Unknown type of mating")
     
     toolbox.register("migrate",tools.migRing,k=10,selection = toolbox.select)
 
     stats = tools.Statistics()
 
     for i,s in enumerate(["Num removed"] + stats_names):
         stats.register(s, lambda x, i=i, stats_by=stats_by: x[np.argmin([ind.fitness.values[stats_by] for ind in x])].fitness.values[i])
```

### Comparing `setga-1.3.5/setga/utils.py` & `setga-1.4/setga/utils.py`

 * *Files identical despite different names*

### Comparing `setga-1.3.5/setga.egg-info/PKG-INFO` & `setga-1.4/setga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setga
-Version: 1.3.5
+Version: 1.4
 Summary: library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.
 Home-page: https://github.com/lavakin/setga
 Author: Nikola Kalábová
 Author-email: nikola@kalabova.eu
 License: MIT
 Project-URL: Documentation, https://setga.readthedocs.io/en/latest/genindex.html
 Keywords: Genetic algorithms,minimal subset,multi-objective,optimization
```

### Comparing `setga-1.3.5/setup.py` & `setga-1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   name = 'setga',         
   packages = ['setga'], 
   license='MIT',       
   description = 'library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.',   # Give a short description about your library
   author = 'Nikola Kalábová',              
   author_email = 'nikola@kalabova.eu',     
   url = 'https://github.com/lavakin/setga',  
-  version = "1.3.5",    
+  version = "1.4",    
   keywords = ['Genetic algorithms', 'minimal subset', 'multi-objective', "optimization"],   
   long_description = "library designed to extract a minimal subset from a given set, optimizing a given (set of) objective(s). Based on the DEAP library.",
   project_urls = {"Documentation" :"https://setga.readthedocs.io/en/latest/genindex.html"},
   install_requires=[          
           'numpy',
           'deap',
           "matplotlib",
```


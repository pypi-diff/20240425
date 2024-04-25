# Comparing `tmp/centurypy-1.0.1.tar.gz` & `tmp/centurypy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centurypy-1.0.1.tar", last modified: Fri Dec 29 04:40:48 2023, max compression
+gzip compressed data, was "centurypy-1.0.2.tar", last modified: Thu Apr 25 04:37:07 2024, max compression
```

## Comparing `centurypy-1.0.1.tar` & `centurypy-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2023-12-29 04:40:48.819929 centurypy-1.0.1/
--rw-r--r--   0 gerardovivas   (501) staff       (20)     1070 2023-12-18 17:56:28.000000 centurypy-1.0.1/LICENSE
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2023-12-29 04:40:48.819498 centurypy-1.0.1/PKG-INFO
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2612 2023-12-29 04:38:18.000000 centurypy-1.0.1/README.md
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2023-12-29 04:40:48.814571 centurypy-1.0.1/centurypy/
--rw-r--r--   0 gerardovivas   (501) staff       (20)       27 2023-10-13 17:46:30.000000 centurypy-1.0.1/centurypy/__init__.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2334 2023-12-12 02:06:35.000000 centurypy-1.0.1/centurypy/century.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     5273 2023-12-14 16:39:55.000000 centurypy-1.0.1/centurypy/genetic.py
--rw-r--r--   0 gerardovivas   (501) staff       (20)     4977 2023-12-16 16:23:00.000000 centurypy-1.0.1/centurypy/main.py
-drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2023-12-29 04:40:48.818745 centurypy-1.0.1/centurypy.egg-info/
--rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2023-12-29 04:40:48.000000 centurypy-1.0.1/centurypy.egg-info/PKG-INFO
--rw-r--r--   0 gerardovivas   (501) staff       (20)      272 2023-12-29 04:40:48.000000 centurypy-1.0.1/centurypy.egg-info/SOURCES.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)        1 2023-12-29 04:40:48.000000 centurypy-1.0.1/centurypy.egg-info/dependency_links.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       19 2023-12-29 04:40:48.000000 centurypy-1.0.1/centurypy.egg-info/requires.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       10 2023-12-29 04:40:48.000000 centurypy-1.0.1/centurypy.egg-info/top_level.txt
--rw-r--r--   0 gerardovivas   (501) staff       (20)       38 2023-12-29 04:40:48.820097 centurypy-1.0.1/setup.cfg
--rw-r--r--   0 gerardovivas   (501) staff       (20)      873 2023-12-29 04:38:09.000000 centurypy-1.0.1/setup.py
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-25 04:37:07.031980 centurypy-1.0.2/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     1070 2023-12-18 17:56:28.000000 centurypy-1.0.2/LICENSE
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-25 04:37:07.031350 centurypy-1.0.2/PKG-INFO
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2612 2023-12-29 04:38:18.000000 centurypy-1.0.2/README.md
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-25 04:37:07.027035 centurypy-1.0.2/centurypy/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       27 2023-10-13 17:46:30.000000 centurypy-1.0.2/centurypy/__init__.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2334 2023-12-12 02:06:35.000000 centurypy-1.0.2/centurypy/century.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     5220 2024-04-25 04:01:06.000000 centurypy-1.0.2/centurypy/genetic.py
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     4977 2023-12-16 16:23:00.000000 centurypy-1.0.2/centurypy/main.py
+drwxr-xr-x   0 gerardovivas   (501) staff       (20)        0 2024-04-25 04:37:07.030559 centurypy-1.0.2/centurypy.egg-info/
+-rw-r--r--   0 gerardovivas   (501) staff       (20)     2925 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/PKG-INFO
+-rw-r--r--   0 gerardovivas   (501) staff       (20)      272 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/SOURCES.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)        1 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/dependency_links.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       19 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/requires.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       10 2024-04-25 04:37:06.000000 centurypy-1.0.2/centurypy.egg-info/top_level.txt
+-rw-r--r--   0 gerardovivas   (501) staff       (20)       38 2024-04-25 04:37:07.032132 centurypy-1.0.2/setup.cfg
+-rw-r--r--   0 gerardovivas   (501) staff       (20)      873 2024-04-25 04:00:39.000000 centurypy-1.0.2/setup.py
```

### Comparing `centurypy-1.0.1/LICENSE` & `centurypy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.1/PKG-INFO` & `centurypy-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centurypy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to train and run the CENTURY (Soil Organic Matter) model
 Home-page: https://github.com/vivas24/centurypy
 Author: Gerardo Vivas
 Author-email: vivas.fermin24@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `centurypy-1.0.1/README.md` & `centurypy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.1/centurypy/century.py` & `centurypy-1.0.2/centurypy/century.py`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.1/centurypy/genetic.py` & `centurypy-1.0.2/centurypy/genetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,14 @@
 
     def update_error(self):
         fitness_sorted = sorted(self.fitness)
         error = fitness_sorted[0]
         if(error < self.error and error >= 0):
             self.error = error
             self.milestones.append([self.generation, self.error])
-            return True
-        return False
 
     def choose_parents(self):
         fitness_tmp = []
         population_tmp = []
         for i in range(int(self.population_size * self.selection_rate)):
             index = np.random.choice(self.population_size)
             fitness_tmp.append(self.fitness[index])
@@ -99,18 +97,18 @@
             offspring += [ parents[0][:cross_point] + parents[1][cross_point:] ]
             offspring += [ parents[1][:cross_point] + parents[0][cross_point:] ]
         return offspring
 
 
     def evolve(self, generations):
         for _ in range(generations):
-            self.mutate()
             self.evaluate_population()
-            if self.update_error():
-                self.population = self.select_offspring()
+            self.update_error()
+            self.population = self.select_offspring()
+            self.mutate()
             self.print_status()
             self.generation += 1
         self.print_status(True)
 
     def format_time(self, seconds):
         hh = int(seconds // 3600)
         mm = int((seconds - (hh * 3600)) // 60)
```

### Comparing `centurypy-1.0.1/centurypy/main.py` & `centurypy-1.0.2/centurypy/main.py`

 * *Files identical despite different names*

### Comparing `centurypy-1.0.1/centurypy.egg-info/PKG-INFO` & `centurypy-1.0.2/centurypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centurypy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to train and run the CENTURY (Soil Organic Matter) model
 Home-page: https://github.com/vivas24/centurypy
 Author: Gerardo Vivas
 Author-email: vivas.fermin24@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `centurypy-1.0.1/setup.py` & `centurypy-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 PACKAGE_NAME = 'centurypy'
 AUTHOR = 'Gerardo Vivas'
 AUTHOR_EMAIL = 'vivas.fermin24@gmail.com'
 URL = 'https://github.com/vivas24/centurypy'
 LICENSE = 'MIT'
 DESCRIPTION = 'Library to train and run the CENTURY (Soil Organic Matter) model' 
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
```


# Comparing `tmp/KBDD-0.2.0.tar.gz` & `tmp/KBDD-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.2.0.tar", last modified: Thu Apr 25 18:03:24 2024, max compression
+gzip compressed data, was "KBDD-0.2.1.tar", last modified: Thu Apr 25 18:06:28 2024, max compression
```

## Comparing `KBDD-0.2.0.tar` & `KBDD-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:03:24.252817 KBDD-0.2.0/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:03:24.251433 KBDD-0.2.0/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.2.0/KBDD/EGtest.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.0/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.0/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 17:51:06.000000 KBDD-0.2.0/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1256 2024-04-25 18:00:46.000000 KBDD-0.2.0/KBDD/alpha_estimation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.2.0/KBDD/connect_adj_set.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.0/KBDD/import_references.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.2.0/KBDD/left_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.2.0/KBDD/net_gen.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.2.0/KBDD/rightmost_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.0/KBDD/show_graph_with_labels.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.2.0/KBDD/truncated_power_law.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:03:24.252294 KBDD-0.2.0/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:03:24.000000 KBDD-0.2.0/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      417 2024-04-25 18:03:24.000000 KBDD-0.2.0/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 18:03:24.000000 KBDD-0.2.0/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 18:03:24.000000 KBDD-0.2.0/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.0/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:03:24.252542 KBDD-0.2.0/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.0/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 18:03:24.252908 KBDD-0.2.0/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 18:03:08.000000 KBDD-0.2.0/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:06:28.963464 KBDD-0.2.1/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:06:28.962056 KBDD-0.2.1/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.2.1/KBDD/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.1/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.1/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      335 2024-04-25 18:06:18.000000 KBDD-0.2.1/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1256 2024-04-25 18:00:46.000000 KBDD-0.2.1/KBDD/alpha_estimation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.2.1/KBDD/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.1/KBDD/import_references.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.2.1/KBDD/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.2.1/KBDD/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.2.1/KBDD/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.1/KBDD/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.2.1/KBDD/truncated_power_law.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:06:28.962909 KBDD-0.2.1/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:06:28.000000 KBDD-0.2.1/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      417 2024-04-25 18:06:28.000000 KBDD-0.2.1/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 18:06:28.000000 KBDD-0.2.1/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 18:06:28.000000 KBDD-0.2.1/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.1/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:06:28.963181 KBDD-0.2.1/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.1/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 18:06:28.963531 KBDD-0.2.1/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 18:06:24.000000 KBDD-0.2.1/setup.py
```

### Comparing `KBDD-0.2.0/KBDD/EGtest.py` & `KBDD-0.2.1/KBDD/EGtest.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/KGML_to_Matrix.py` & `KBDD-0.2.1/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/Network_score_with_cor.py` & `KBDD-0.2.1/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/alpha_estimation.py` & `KBDD-0.2.1/KBDD/alpha_estimation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/connect_adj_set.py` & `KBDD-0.2.1/KBDD/connect_adj_set.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/import_references.py` & `KBDD-0.2.1/KBDD/import_references.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/left_adj.py` & `KBDD-0.2.1/KBDD/left_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/net_gen.py` & `KBDD-0.2.1/KBDD/net_gen.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/rightmost_adj.py` & `KBDD-0.2.1/KBDD/rightmost_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/show_graph_with_labels.py` & `KBDD-0.2.1/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD/truncated_power_law.py` & `KBDD-0.2.1/KBDD/truncated_power_law.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/KBDD.egg-info/PKG-INFO` & `KBDD-0.2.1/KBDD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.0/LICENSE.txt` & `KBDD-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.0/PKG-INFO` & `KBDD-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.0/setup.py` & `KBDD-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.2.0',
+    version='0.2.1',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


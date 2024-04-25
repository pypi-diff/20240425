# Comparing `tmp/KBDD-0.1.7.tar.gz` & `tmp/KBDD-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.1.7.tar", last modified: Thu Apr 25 16:28:56 2024, max compression
+gzip compressed data, was "KBDD-0.1.8.tar", last modified: Thu Apr 25 16:38:21 2024, max compression
```

## Comparing `KBDD-0.1.7.tar` & `KBDD-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:28:56.150897 KBDD-0.1.7/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:28:56.149390 KBDD-0.1.7/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.7/KBDD/EGtest.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:21:28.000000 KBDD-0.1.7/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.7/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 12:14:06.000000 KBDD-0.1.7/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.7/KBDD/connect_adj_set.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.7/KBDD/left_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.7/KBDD/net_gen.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.7/KBDD/rightmost_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.7/KBDD/show_graph_with_labels.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.7/KBDD/truncated_power_law.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:28:56.150250 KBDD-0.1.7/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.7/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 16:28:56.150565 KBDD-0.1.7/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.7/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 16:28:56.150974 KBDD-0.1.7/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 16:28:42.000000 KBDD-0.1.7/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:38:21.704938 KBDD-0.1.8/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:38:21.703399 KBDD-0.1.8/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.8/KBDD/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.1.8/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.8/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 12:14:06.000000 KBDD-0.1.8/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.8/KBDD/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.8/KBDD/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.8/KBDD/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.8/KBDD/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.8/KBDD/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.8/KBDD/truncated_power_law.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:38:21.704352 KBDD-0.1.8/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 16:38:21.000000 KBDD-0.1.8/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 16:38:21.000000 KBDD-0.1.8/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 16:38:21.000000 KBDD-0.1.8/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 16:38:21.000000 KBDD-0.1.8/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.8/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 16:38:21.704636 KBDD-0.1.8/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.8/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 16:38:21.705005 KBDD-0.1.8/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 16:38:13.000000 KBDD-0.1.8/setup.py
```

### Comparing `KBDD-0.1.7/KBDD/EGtest.py` & `KBDD-0.1.8/KBDD/EGtest.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/KGML_to_Matrix.py` & `KBDD-0.1.8/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/Network_score_with_cor.py` & `KBDD-0.1.8/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/connect_adj_set.py` & `KBDD-0.1.8/KBDD/connect_adj_set.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/left_adj.py` & `KBDD-0.1.8/KBDD/left_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/net_gen.py` & `KBDD-0.1.8/KBDD/net_gen.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/rightmost_adj.py` & `KBDD-0.1.8/KBDD/rightmost_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/show_graph_with_labels.py` & `KBDD-0.1.8/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD/truncated_power_law.py` & `KBDD-0.1.8/KBDD/truncated_power_law.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/KBDD.egg-info/PKG-INFO` & `KBDD-0.1.8/KBDD.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.7/LICENSE.txt` & `KBDD-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.7/PKG-INFO` & `KBDD-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.7/setup.py` & `KBDD-0.1.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.1.7',
+    version='0.1.8',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


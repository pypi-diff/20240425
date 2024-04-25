# Comparing `tmp/KBDD-0.1.2.tar.gz` & `tmp/KBDD-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.1.2.tar", last modified: Thu Apr 25 10:59:47 2024, max compression
+gzip compressed data, was "KBDD-0.1.3.tar", last modified: Thu Apr 25 11:18:34 2024, max compression
```

## Comparing `KBDD-0.1.2.tar` & `KBDD-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:59:47.022984 KBDD-0.1.2/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:59:47.022397 KBDD-0.1.2/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.2/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 10:59:47.022697 KBDD-0.1.2/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.2/README.md
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:59:47.021952 KBDD-0.1.2/kbdd/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.2/kbdd/EGtest.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8144 2024-04-25 09:20:03.000000 KBDD-0.1.2/kbdd/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.2/kbdd/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)        0 2024-04-25 08:38:06.000000 KBDD-0.1.2/kbdd/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.2/kbdd/connect_adj_set.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.2/kbdd/left_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.2/kbdd/net_gen.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.2/kbdd/rightmost_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.2/kbdd/show_graph_with_labels.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.2/kbdd/truncated_power_law.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 10:59:47.023051 KBDD-0.1.2/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 10:53:37.000000 KBDD-0.1.2/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 11:18:34.106130 KBDD-0.1.3/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 11:18:34.105409 KBDD-0.1.3/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.3/KBDD/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8144 2024-04-25 09:20:03.000000 KBDD-0.1.3/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.3/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        0 2024-04-25 08:38:06.000000 KBDD-0.1.3/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.3/KBDD/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.3/KBDD/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.3/KBDD/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.3/KBDD/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.3/KBDD/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.3/KBDD/truncated_power_law.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 11:18:34.105591 KBDD-0.1.3/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 11:18:34.000000 KBDD-0.1.3/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      590 2024-04-25 11:18:34.000000 KBDD-0.1.3/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 11:18:34.000000 KBDD-0.1.3/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 11:18:34.000000 KBDD-0.1.3/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.3/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 11:18:34.105859 KBDD-0.1.3/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.3/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 11:18:34.106195 KBDD-0.1.3/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 11:05:55.000000 KBDD-0.1.3/setup.py
```

### Comparing `KBDD-0.1.2/KBDD.egg-info/PKG-INFO` & `KBDD-0.1.3/KBDD.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.2/LICENSE.txt` & `KBDD-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/PKG-INFO` & `KBDD-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.2/kbdd/EGtest.py` & `KBDD-0.1.3/KBDD/EGtest.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/KGML_to_Matrix.py` & `KBDD-0.1.3/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/Network_score_with_cor.py` & `KBDD-0.1.3/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/connect_adj_set.py` & `KBDD-0.1.3/KBDD/connect_adj_set.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/left_adj.py` & `KBDD-0.1.3/KBDD/left_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/net_gen.py` & `KBDD-0.1.3/KBDD/net_gen.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/rightmost_adj.py` & `KBDD-0.1.3/KBDD/rightmost_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/show_graph_with_labels.py` & `KBDD-0.1.3/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/kbdd/truncated_power_law.py` & `KBDD-0.1.3/KBDD/truncated_power_law.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.2/setup.py` & `KBDD-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.1.2',
+    version='0.1.3',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


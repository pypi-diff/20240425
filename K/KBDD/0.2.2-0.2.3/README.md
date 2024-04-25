# Comparing `tmp/KBDD-0.2.2.tar.gz` & `tmp/KBDD-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.2.2.tar", last modified: Thu Apr 25 18:12:25 2024, max compression
+gzip compressed data, was "KBDD-0.2.3.tar", last modified: Thu Apr 25 18:29:36 2024, max compression
```

## Comparing `KBDD-0.2.2.tar` & `KBDD-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:12:25.724736 KBDD-0.2.2/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:12:25.722776 KBDD-0.2.2/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.2.2/KBDD/EGtest.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.2/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.2/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      335 2024-04-25 18:06:18.000000 KBDD-0.2.2/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.2/KBDD/alpha_estimation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.2.2/KBDD/connect_adj_set.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.2/KBDD/import_references.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.2.2/KBDD/left_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.2.2/KBDD/net_gen.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.2.2/KBDD/rightmost_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.2/KBDD/show_graph_with_labels.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.2.2/KBDD/truncated_power_law.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:12:25.724099 KBDD-0.2.2/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:12:25.000000 KBDD-0.2.2/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      417 2024-04-25 18:12:25.000000 KBDD-0.2.2/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 18:12:25.000000 KBDD-0.2.2/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 18:12:25.000000 KBDD-0.2.2/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.2/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:12:25.724422 KBDD-0.2.2/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.2/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 18:12:25.724810 KBDD-0.2.2/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 18:12:22.000000 KBDD-0.2.2/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:29:36.444563 KBDD-0.2.3/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:29:36.443157 KBDD-0.2.3/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.2.3/KBDD/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.3/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.3/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      335 2024-04-25 18:06:18.000000 KBDD-0.2.3/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.3/KBDD/alpha_estimation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.2.3/KBDD/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.3/KBDD/import_references.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.2.3/KBDD/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.2.3/KBDD/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.2.3/KBDD/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.3/KBDD/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.2.3/KBDD/truncated_power_law.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:29:36.444023 KBDD-0.2.3/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:29:36.000000 KBDD-0.2.3/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      417 2024-04-25 18:29:36.000000 KBDD-0.2.3/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 18:29:36.000000 KBDD-0.2.3/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 18:29:36.000000 KBDD-0.2.3/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.3/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:29:36.444280 KBDD-0.2.3/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.3/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 18:29:36.444626 KBDD-0.2.3/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 18:29:32.000000 KBDD-0.2.3/setup.py
```

### Comparing `KBDD-0.2.2/KBDD/EGtest.py` & `KBDD-0.2.3/KBDD/EGtest.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/KGML_to_Matrix.py` & `KBDD-0.2.3/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/Network_score_with_cor.py` & `KBDD-0.2.3/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/alpha_estimation.py` & `KBDD-0.2.3/KBDD/alpha_estimation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/connect_adj_set.py` & `KBDD-0.2.3/KBDD/connect_adj_set.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/import_references.py` & `KBDD-0.2.3/KBDD/import_references.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/left_adj.py` & `KBDD-0.2.3/KBDD/left_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/net_gen.py` & `KBDD-0.2.3/KBDD/net_gen.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/rightmost_adj.py` & `KBDD-0.2.3/KBDD/rightmost_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/show_graph_with_labels.py` & `KBDD-0.2.3/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD/truncated_power_law.py` & `KBDD-0.2.3/KBDD/truncated_power_law.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/KBDD.egg-info/PKG-INFO` & `KBDD-0.2.3/KBDD.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.2/LICENSE.txt` & `KBDD-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.2/PKG-INFO` & `KBDD-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.2/setup.py` & `KBDD-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.2.2',
+    version='0.2.3',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


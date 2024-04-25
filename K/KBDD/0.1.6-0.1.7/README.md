# Comparing `tmp/KBDD-0.1.6.tar.gz` & `tmp/KBDD-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.1.6.tar", last modified: Thu Apr 25 14:32:56 2024, max compression
+gzip compressed data, was "KBDD-0.1.7.tar", last modified: Thu Apr 25 16:28:56 2024, max compression
```

## Comparing `KBDD-0.1.6.tar` & `KBDD-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 14:32:56.359711 KBDD-0.1.6/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 14:32:56.358186 KBDD-0.1.6/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.6/KBDD/EGtest.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8170 2024-04-25 14:32:08.000000 KBDD-0.1.6/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.6/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 12:14:06.000000 KBDD-0.1.6/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.6/KBDD/connect_adj_set.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.6/KBDD/left_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.6/KBDD/net_gen.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.6/KBDD/rightmost_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.6/KBDD/show_graph_with_labels.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.6/KBDD/truncated_power_law.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 14:32:56.359071 KBDD-0.1.6/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.6/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 14:32:56.359388 KBDD-0.1.6/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.6/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 14:32:56.359800 KBDD-0.1.6/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 14:32:43.000000 KBDD-0.1.6/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:28:56.150897 KBDD-0.1.7/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:28:56.149390 KBDD-0.1.7/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.7/KBDD/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:21:28.000000 KBDD-0.1.7/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.7/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 12:14:06.000000 KBDD-0.1.7/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.7/KBDD/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.7/KBDD/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.7/KBDD/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.7/KBDD/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.7/KBDD/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.7/KBDD/truncated_power_law.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 16:28:56.150250 KBDD-0.1.7/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 16:28:56.000000 KBDD-0.1.7/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.7/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 16:28:56.150565 KBDD-0.1.7/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.7/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 16:28:56.150974 KBDD-0.1.7/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 16:28:42.000000 KBDD-0.1.7/setup.py
```

### Comparing `KBDD-0.1.6/KBDD/EGtest.py` & `KBDD-0.1.7/KBDD/EGtest.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/KGML_to_Matrix.py` & `KBDD-0.1.7/KBDD/KGML_to_Matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
         relation_new = []
         for ii in range(len(data_relation.index)):
             if [i in data_relation.iloc[ii,].iloc[0] for i in separate_from].count(True) > 0:
                 relation1 = [separate_to[i] for i, v in enumerate([i in data_relation.iloc[ii,].iloc[0] for i in separate_from]) if v == True]
             else:
                 relation1 = [data_relation.iloc[ii,].iloc[0]]
-            if [i in data_relation.iloc[ii,][1] for i in separate_from].count(True) > 0:
-                relation2 = [separate_to[i] for i, v in enumerate([i in data_relation.iloc[ii,][1] for i in separate_from]) if v == True]
+            if [i in data_relation.iloc[ii, 1] for i in separate_from].count(True) > 0:
+                relation2 = [separate_to[i] for i, v in enumerate([i in data_relation.iloc[ii, 1] for i in separate_from]) if v == True]
 
             else:
                 relation2 = [data_relation.iloc[ii,].iloc[1]]
             relation_new.append([(x, y) for x in relation1 for y in relation2])
         relation_new = pd.concat(list(map(pd.DataFrame, relation_new)))
         relation_new.columns = ["Var1", "Var2"]
         relation_new = relation_new.reset_index(drop = True)
```

### Comparing `KBDD-0.1.6/KBDD/Network_score_with_cor.py` & `KBDD-0.1.7/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/connect_adj_set.py` & `KBDD-0.1.7/KBDD/connect_adj_set.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/left_adj.py` & `KBDD-0.1.7/KBDD/left_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/net_gen.py` & `KBDD-0.1.7/KBDD/net_gen.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/rightmost_adj.py` & `KBDD-0.1.7/KBDD/rightmost_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/show_graph_with_labels.py` & `KBDD-0.1.7/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD/truncated_power_law.py` & `KBDD-0.1.7/KBDD/truncated_power_law.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/KBDD.egg-info/PKG-INFO` & `KBDD-0.1.7/KBDD.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.6/LICENSE.txt` & `KBDD-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.6/PKG-INFO` & `KBDD-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.6/setup.py` & `KBDD-0.1.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.1.6',
+    version='0.1.7',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


# Comparing `tmp/KBDD-0.2.5.tar.gz` & `tmp/KBDD-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.2.5.tar", last modified: Thu Apr 25 18:57:30 2024, max compression
+gzip compressed data, was "KBDD-0.2.6.tar", last modified: Thu Apr 25 19:01:41 2024, max compression
```

## Comparing `KBDD-0.2.5.tar` & `KBDD-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:57:30.143465 KBDD-0.2.5/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:57:30.141960 KBDD-0.2.5/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.5/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.5/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      203 2024-04-25 18:53:41.000000 KBDD-0.2.5/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.5/KBDD/alpha_estimation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      964 2024-04-25 18:57:13.000000 KBDD-0.2.5/KBDD/deviation_calculation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.5/KBDD/import_references.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)    11323 2024-04-25 18:53:31.000000 KBDD-0.2.5/KBDD/pns_construction.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.5/KBDD/show_graph_with_labels.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 18:57:30.142900 KBDD-0.2.5/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:57:30.000000 KBDD-0.2.5/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      350 2024-04-25 18:57:30.000000 KBDD-0.2.5/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 18:57:30.000000 KBDD-0.2.5/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 18:57:30.000000 KBDD-0.2.5/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.5/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 18:57:30.143177 KBDD-0.2.5/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.5/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 18:57:30.143542 KBDD-0.2.5/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 18:57:25.000000 KBDD-0.2.5/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:01:41.341220 KBDD-0.2.6/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:01:41.339654 KBDD-0.2.6/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.6/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.6/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      203 2024-04-25 18:53:41.000000 KBDD-0.2.6/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.6/KBDD/alpha_estimation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      964 2024-04-25 18:57:13.000000 KBDD-0.2.6/KBDD/deviation_calculation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.6/KBDD/import_references.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)    11230 2024-04-25 19:01:26.000000 KBDD-0.2.6/KBDD/pns_construction.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.6/KBDD/show_graph_with_labels.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:01:41.340645 KBDD-0.2.6/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      350 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.6/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:01:41.340933 KBDD-0.2.6/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.6/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 19:01:41.341290 KBDD-0.2.6/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 19:01:39.000000 KBDD-0.2.6/setup.py
```

### Comparing `KBDD-0.2.5/KBDD/KGML_to_Matrix.py` & `KBDD-0.2.6/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/KBDD/Network_score_with_cor.py` & `KBDD-0.2.6/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/KBDD/alpha_estimation.py` & `KBDD-0.2.6/KBDD/alpha_estimation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/KBDD/deviation_calculation.py` & `KBDD-0.2.6/KBDD/deviation_calculation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/KBDD/import_references.py` & `KBDD-0.2.6/KBDD/import_references.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/KBDD/pns_construction.py` & `KBDD-0.2.6/KBDD/pns_construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,13 +284,11 @@
             EG_result = EGtest(sample_DS)
 
         sample_net = net_gen(np.array(sample_DS))
         sample_DS_data.append(sample_DS)
         for net_index in range(len(sample_net)):
             potential_net.append(sample_net[net_index])
 
-    end_time = time.time()
-    run_time = (end_time - start_time) / 60  # convert to minutes
     print("Total potential network structures:", len(potential_net))
     
     return potential_net, sample_DS_data
```

### Comparing `KBDD-0.2.5/KBDD/show_graph_with_labels.py` & `KBDD-0.2.6/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/KBDD.egg-info/PKG-INFO` & `KBDD-0.2.6/KBDD.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.5/LICENSE.txt` & `KBDD-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.5/PKG-INFO` & `KBDD-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.5/setup.py` & `KBDD-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.2.5',
+    version='0.2.6',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


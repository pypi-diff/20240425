# Comparing `tmp/KBDD-0.2.6.tar.gz` & `tmp/KBDD-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.2.6.tar", last modified: Thu Apr 25 19:01:41 2024, max compression
+gzip compressed data, was "KBDD-0.2.7.tar", last modified: Thu Apr 25 19:10:52 2024, max compression
```

## Comparing `KBDD-0.2.6.tar` & `KBDD-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:01:41.341220 KBDD-0.2.6/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:01:41.339654 KBDD-0.2.6/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.6/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.2.6/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      203 2024-04-25 18:53:41.000000 KBDD-0.2.6/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.6/KBDD/alpha_estimation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      964 2024-04-25 18:57:13.000000 KBDD-0.2.6/KBDD/deviation_calculation.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.6/KBDD/import_references.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)    11230 2024-04-25 19:01:26.000000 KBDD-0.2.6/KBDD/pns_construction.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.6/KBDD/show_graph_with_labels.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:01:41.340645 KBDD-0.2.6/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      350 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 19:01:41.000000 KBDD-0.2.6/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.6/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:01:41.340933 KBDD-0.2.6/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.6/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 19:01:41.341290 KBDD-0.2.6/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 19:01:39.000000 KBDD-0.2.6/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:10:52.442810 KBDD-0.2.7/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:10:52.441270 KBDD-0.2.7/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8168 2024-04-25 16:37:55.000000 KBDD-0.2.7/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5906 2024-04-25 19:10:30.000000 KBDD-0.2.7/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      241 2024-04-25 19:03:43.000000 KBDD-0.2.7/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1275 2024-04-25 18:12:10.000000 KBDD-0.2.7/KBDD/alpha_estimation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      964 2024-04-25 18:57:13.000000 KBDD-0.2.7/KBDD/deviation_calculation.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1492 2024-04-25 17:58:42.000000 KBDD-0.2.7/KBDD/import_references.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)    11230 2024-04-25 19:01:26.000000 KBDD-0.2.7/KBDD/pns_construction.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.2.7/KBDD/show_graph_with_labels.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 19:10:52.442243 KBDD-0.2.7/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      350 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 19:10:52.000000 KBDD-0.2.7/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.2.7/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 19:10:52.442522 KBDD-0.2.7/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.2.7/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 19:10:52.442881 KBDD-0.2.7/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 19:10:46.000000 KBDD-0.2.7/setup.py
```

### Comparing `KBDD-0.2.6/KBDD/KGML_to_Matrix.py` & `KBDD-0.2.7/KBDD/KGML_to_Matrix.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/KBDD/Network_score_with_cor.py` & `KBDD-0.2.7/KBDD/Network_score_with_cor.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,9 +113,23 @@
 
             conv_net_score.append(tmp_conv_net_score)
             update_net_score.append(tmp_update_net_score)
             Permute_gene_label.append(tmp_Permute_gene_label)
             final_gene_label.append(gene_label)
             final_net_score.append(net_score)
             Permute_size_list.append(tmp_Permute_size_list)
-            
-    return final_structure_list, final_gene_label, final_net_score
+    
+    # Sort by network score
+    sorted_index = np.argsort(final_net_score)
+    sorted_index = sorted_index[::-1]
+    sorted_structure_output = []
+    sorted_score_output = []
+    sorted_gene_label_output = []
+
+    for i in sorted_index:
+        sorted_structure_output.append(final_structure_list[i])
+        sorted_score_output.append(final_net_score[i])
+        sorted_gene_label_output.append(final_gene_label[i])
+
+    return sorted_structure_output, sorted_gene_label_output, sorted_score_output
+    
+
```

### Comparing `KBDD-0.2.6/KBDD/alpha_estimation.py` & `KBDD-0.2.7/KBDD/alpha_estimation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/KBDD/deviation_calculation.py` & `KBDD-0.2.7/KBDD/deviation_calculation.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/KBDD/import_references.py` & `KBDD-0.2.7/KBDD/import_references.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/KBDD/pns_construction.py` & `KBDD-0.2.7/KBDD/pns_construction.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/KBDD/show_graph_with_labels.py` & `KBDD-0.2.7/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/KBDD.egg-info/PKG-INFO` & `KBDD-0.2.7/KBDD.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.6/LICENSE.txt` & `KBDD-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.2.6/PKG-INFO` & `KBDD-0.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.2.6/setup.py` & `KBDD-0.2.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.2.6',
+    version='0.2.7',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


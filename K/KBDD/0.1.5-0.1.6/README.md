# Comparing `tmp/KBDD-0.1.5.tar.gz` & `tmp/KBDD-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.1.5.tar", last modified: Thu Apr 25 12:15:11 2024, max compression
+gzip compressed data, was "KBDD-0.1.6.tar", last modified: Thu Apr 25 14:32:56 2024, max compression
```

## Comparing `KBDD-0.1.5.tar` & `KBDD-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 12:15:11.410477 KBDD-0.1.5/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 12:15:11.408615 KBDD-0.1.5/KBDD/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.5/KBDD/EGtest.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     8144 2024-04-25 09:20:03.000000 KBDD-0.1.5/KBDD/KGML_to_Matrix.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.5/KBDD/Network_score_with_cor.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 12:14:06.000000 KBDD-0.1.5/KBDD/__init__.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.5/KBDD/connect_adj_set.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.5/KBDD/left_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.5/KBDD/net_gen.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.5/KBDD/rightmost_adj.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.5/KBDD/show_graph_with_labels.py
--rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.5/KBDD/truncated_power_law.py
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 12:15:11.409778 KBDD-0.1.5/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 12:15:11.000000 KBDD-0.1.5/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 12:15:11.000000 KBDD-0.1.5/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 12:15:11.000000 KBDD-0.1.5/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 12:15:11.000000 KBDD-0.1.5/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.5/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 12:15:11.410150 KBDD-0.1.5/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.5/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 12:15:11.410547 KBDD-0.1.5/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 12:14:21.000000 KBDD-0.1.5/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 14:32:56.359711 KBDD-0.1.6/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 14:32:56.358186 KBDD-0.1.6/KBDD/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.6/KBDD/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8170 2024-04-25 14:32:08.000000 KBDD-0.1.6/KBDD/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.6/KBDD/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      270 2024-04-25 12:14:06.000000 KBDD-0.1.6/KBDD/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.6/KBDD/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.6/KBDD/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.6/KBDD/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.6/KBDD/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.6/KBDD/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.6/KBDD/truncated_power_law.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 14:32:56.359071 KBDD-0.1.6/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 14:32:56.000000 KBDD-0.1.6/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.6/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 14:32:56.359388 KBDD-0.1.6/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.6/README.md
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 14:32:56.359800 KBDD-0.1.6/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 14:32:43.000000 KBDD-0.1.6/setup.py
```

### Comparing `KBDD-0.1.5/KBDD/EGtest.py` & `KBDD-0.1.6/KBDD/EGtest.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/KGML_to_Matrix.py` & `KBDD-0.1.6/KBDD/KGML_to_Matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,23 +94,23 @@
         return print("There are no relation in the ", pathway_name, "!")
     else:
         separate_from = list(data_entry_new[data_entry_new["type"] == "group"]["id"])
         separate_to = list(data_entry_new["component"][data_entry_new["component"].isnull() == False])
 
         relation_new = []
         for ii in range(len(data_relation.index)):
-            if [i in data_relation.iloc[ii,][0] for i in separate_from].count(True) > 0:
-                relation1 = [separate_to[i] for i, v in enumerate([i in data_relation.iloc[ii,][0] for i in separate_from]) if v == True]
+            if [i in data_relation.iloc[ii,].iloc[0] for i in separate_from].count(True) > 0:
+                relation1 = [separate_to[i] for i, v in enumerate([i in data_relation.iloc[ii,].iloc[0] for i in separate_from]) if v == True]
             else:
-                relation1 = [data_relation.iloc[ii,][0]]
+                relation1 = [data_relation.iloc[ii,].iloc[0]]
             if [i in data_relation.iloc[ii,][1] for i in separate_from].count(True) > 0:
                 relation2 = [separate_to[i] for i, v in enumerate([i in data_relation.iloc[ii,][1] for i in separate_from]) if v == True]
 
             else:
-                relation2 = [data_relation.iloc[ii,][1]]
+                relation2 = [data_relation.iloc[ii,].iloc[1]]
             relation_new.append([(x, y) for x in relation1 for y in relation2])
         relation_new = pd.concat(list(map(pd.DataFrame, relation_new)))
         relation_new.columns = ["Var1", "Var2"]
         relation_new = relation_new.reset_index(drop = True)
 
         def relation_group_fn(xx):
             sub_group = [separate_to[i] for i, v in enumerate([i in xx for i in separate_from]) if v == True]
@@ -143,15 +143,15 @@
                 relationship.iloc[:, pos2[ii]] = relationship.iloc[:, pos2[ii]] + relationship.iloc[:, pos1[ii]]
         if len(pos1) > 0:
             pos1_relationship = [relationship.columns[ii] for ii in pos1]
             relationship = relationship.drop(pos1_relationship, axis = 1)
             relationship = relationship.drop(pos1_relationship, axis = 0)
 
             data_entry.index = list(data_entry["id"])
-            entry_pos1 = [data_entry["id"][ii] for ii in pos1]
+            entry_pos1 = [data_entry["id"].iloc[ii] for ii in pos1]
             node_detail = data_entry.drop(entry_pos1, axis = 0)
             node_detail = node_detail[["name", "type", "node_name"]]
 
             if list(data_entry["type"] == "group").count(True) != 0:
                 delete_group = data_entry.drop(entry_pos1, axis = 0)
                 delete_group_drop = [delete_group.index[ii] for ii, vv in enumerate(delete_group["type"] == "group") if vv == True]
                 relationship = relationship.drop(delete_group_drop, axis = 0)
@@ -167,8 +167,8 @@
                     relationship.iloc[ii, jj] = 1
         adj_matrix = relationship
 
         file_name = save_path + pathway_name + "(directed)"
         adj_matrix.to_pickle(file_name)
         file_name = save_path + pathway_name + "(node_detail)"
         node_detail.to_pickle(file_name)
-        return "Success"
+        return "Success"
```

### Comparing `KBDD-0.1.5/KBDD/Network_score_with_cor.py` & `KBDD-0.1.6/KBDD/Network_score_with_cor.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/connect_adj_set.py` & `KBDD-0.1.6/KBDD/connect_adj_set.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/left_adj.py` & `KBDD-0.1.6/KBDD/left_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/net_gen.py` & `KBDD-0.1.6/KBDD/net_gen.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/rightmost_adj.py` & `KBDD-0.1.6/KBDD/rightmost_adj.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/show_graph_with_labels.py` & `KBDD-0.1.6/KBDD/show_graph_with_labels.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD/truncated_power_law.py` & `KBDD-0.1.6/KBDD/truncated_power_law.py`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/KBDD.egg-info/PKG-INFO` & `KBDD-0.1.6/KBDD.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.5/LICENSE.txt` & `KBDD-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `KBDD-0.1.5/PKG-INFO` & `KBDD-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KBDD
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for KBDD: a knowledge-based and data-driven method for genetic network construction
 Author: Chen-Po Liao
 Author-email: liaochenpo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `KBDD-0.1.5/setup.py` & `KBDD-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='KBDD',
-    version='0.1.5',
+    version='0.1.6',
     packages=setuptools.find_packages(),
     description='A package for KBDD: a knowledge-based and data-driven method for genetic network construction',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chen-Po Liao',
     author_email='liaochenpo@gmail.com',
     license='MIT',
```


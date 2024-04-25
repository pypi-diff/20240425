# Comparing `tmp/STAIR-tools-1.1.4.tar.gz` & `tmp/STAIR-tools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.1.4.tar", last modified: Thu Apr 25 02:41:33 2024, max compression
+gzip compressed data, was "STAIR-tools-1.1.5.tar", last modified: Thu Apr 25 02:45:00 2024, max compression
```

## Comparing `STAIR-tools-1.1.4.tar` & `STAIR-tools-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:41:33.184914 STAIR-tools-1.1.4/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:41:33.184710 STAIR-tools-1.1.4/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.4/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:41:33.181764 STAIR-tools-1.1.4/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.4/STAIR/ABA_annotation.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.4/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18494 2024-04-25 02:37:18.000000 STAIR-tools-1.1.4/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:41:33.183793 STAIR-tools-1.1.4/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.4/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.4/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3889 2023-12-23 11:23:12.000000 STAIR-tools-1.1.4/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.4/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.4/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.4/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.4/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12304 2023-12-23 11:23:12.000000 STAIR-tools-1.1.4/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14182 2023-12-23 11:23:11.000000 STAIR-tools-1.1.4/STAIR/loc_prediction.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      174 2023-12-23 11:23:13.000000 STAIR-tools-1.1.4/STAIR/test.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.4/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:41:33.184495 STAIR-tools-1.1.4/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:41:33.000000 STAIR-tools-1.1.4/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      505 2024-04-25 02:41:33.000000 STAIR-tools-1.1.4/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-25 02:41:33.000000 STAIR-tools-1.1.4/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-25 02:41:33.000000 STAIR-tools-1.1.4/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-25 02:41:33.184966 STAIR-tools-1.1.4/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-25 02:41:29.000000 STAIR-tools-1.1.4/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:45:00.118810 STAIR-tools-1.1.5/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:45:00.118631 STAIR-tools-1.1.5/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.5/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:45:00.114307 STAIR-tools-1.1.5/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.5/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:45:00.114552 STAIR-tools-1.1.5/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.5/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.5/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18500 2024-04-25 02:43:23.000000 STAIR-tools-1.1.5/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:45:00.116275 STAIR-tools-1.1.5/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.5/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.5/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3889 2023-12-23 11:23:12.000000 STAIR-tools-1.1.5/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.5/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.5/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.5/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.5/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12324 2024-04-25 02:44:23.000000 STAIR-tools-1.1.5/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14202 2024-04-25 02:44:36.000000 STAIR-tools-1.1.5/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:45:00.117811 STAIR-tools-1.1.5/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.5/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.1.5/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.1.5/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.1.5/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.1.5/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.1.5/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.5/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:45:00.118436 STAIR-tools-1.1.5/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:45:00.000000 STAIR-tools-1.1.5/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-04-25 02:45:00.000000 STAIR-tools-1.1.5/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-25 02:45:00.000000 STAIR-tools-1.1.5/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-25 02:45:00.000000 STAIR-tools-1.1.5/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-25 02:45:00.118858 STAIR-tools-1.1.5/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-25 02:43:28.000000 STAIR-tools-1.1.5/setup.py
```

### Comparing `STAIR-tools-1.1.4/README.md` & `STAIR-tools-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/ABA_annotation.py` & `STAIR-tools-1.1.5/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/emb_alignment.py` & `STAIR-tools-1.1.5/STAIR/emb_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from STAIR.embedding.module_ae import ae_dict
 from STAIR.embedding.module_hgat import HGAT
 from STAIR.embedding.dataset_ae import MyDataset
 from STAIR.embedding.dataset_hgat import hgat_data
 from STAIR.embedding.loss import nll_loss
 
-from utils import MakeLogClass
+from STAIR.utils import MakeLogClass
 
 
 class Emb_Align(object):
 
     """
     
     Spatial embedding alignment of multiplt ST slices, including CE alignment and SE alignment.
```

### Comparing `STAIR-tools-1.1.4/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.1.5/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.1.5/STAIR/embedding/dataset_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/embedding/loss.py` & `STAIR-tools-1.1.5/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/embedding/module_ae.py` & `STAIR-tools-1.1.5/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.1.5/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.1.5/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.4/STAIR/loc_alignment.py` & `STAIR-tools-1.1.5/STAIR/loc_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import numpy as np
 import anndata as ad
 import matplotlib.pyplot as plt
 
-from .location.align_init import initial_alignment
-from .location.align_fine import fine_alignment
-from .location.edge_detection import alpha_shape, calcu_lisi, select_clustered_domains, detect_edge_of_domains
-from .utils import MakeLogClass
+from STAIR.location.align_init import initial_alignment
+from STAIR.location.align_fine import fine_alignment
+from STAIR.location.edge_detection import alpha_shape, calcu_lisi, select_clustered_domains, detect_edge_of_domains
+from STAIR.utils import MakeLogClass
 
 
 class Loc_Align(object):
     
     """
     
     Location alignment of multiplt ST slices, including initial alignment and fine alignment.
```

### Comparing `STAIR-tools-1.1.4/STAIR/loc_prediction.py` & `STAIR-tools-1.1.5/STAIR/loc_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import numpy as np
 import scanpy as sc
 import matplotlib.pyplot as plt 
 from sklearn.neighbors import NearestNeighbors
 
-from .location.transformation import best_fit_transform, transform
-from .location.edge_detection import alpha_shape
-from .location.align_fine import fine_alignment
-from .utils import MakeLogClass
+from STAIR.location.transformation import best_fit_transform, transform
+from STAIR.location.edge_detection import alpha_shape
+from STAIR.location.align_fine import fine_alignment
+from STAIR.utils import MakeLogClass
 
 
 def sort_slices(atte, return_tree=False):
     
     import networkx as nx
     
     matrix = 1 - (atte + atte.T)/2
```

### Comparing `STAIR-tools-1.1.4/STAIR/utils.py` & `STAIR-tools-1.1.5/STAIR/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/STAIR-tools-1.1.2.tar.gz` & `tmp/STAIR-tools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.1.2.tar", last modified: Thu Apr 25 02:34:00 2024, max compression
+gzip compressed data, was "STAIR-tools-1.1.3.tar", last modified: Thu Apr 25 02:37:43 2024, max compression
```

## Comparing `STAIR-tools-1.1.2.tar` & `STAIR-tools-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,18 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:34:00.685774 STAIR-tools-1.1.2/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:34:00.685573 STAIR-tools-1.1.2/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.2/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:34:00.683122 STAIR-tools-1.1.2/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.2/STAIR/ABA_annotation.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.2/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18495 2024-04-25 02:32:00.000000 STAIR-tools-1.1.2/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:34:00.684747 STAIR-tools-1.1.2/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.2/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.2/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3889 2023-12-23 11:23:12.000000 STAIR-tools-1.1.2/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.2/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.2/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.2/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.2/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12304 2023-12-23 11:23:12.000000 STAIR-tools-1.1.2/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14182 2023-12-23 11:23:11.000000 STAIR-tools-1.1.2/STAIR/loc_prediction.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      174 2023-12-23 11:23:13.000000 STAIR-tools-1.1.2/STAIR/test.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.2/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:34:00.685385 STAIR-tools-1.1.2/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:34:00.000000 STAIR-tools-1.1.2/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      505 2024-04-25 02:34:00.000000 STAIR-tools-1.1.2/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-25 02:34:00.000000 STAIR-tools-1.1.2/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-25 02:34:00.000000 STAIR-tools-1.1.2/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-25 02:34:00.685824 STAIR-tools-1.1.2/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-25 02:33:51.000000 STAIR-tools-1.1.2/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:37:43.951015 STAIR-tools-1.1.3/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:37:43.950837 STAIR-tools-1.1.3/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.3/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:37:43.949921 STAIR-tools-1.1.3/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.3/STAIR/ABA_annotation.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.3/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18494 2024-04-25 02:37:18.000000 STAIR-tools-1.1.3/STAIR/emb_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12304 2023-12-23 11:23:12.000000 STAIR-tools-1.1.3/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14182 2023-12-23 11:23:11.000000 STAIR-tools-1.1.3/STAIR/loc_prediction.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      174 2023-12-23 11:23:13.000000 STAIR-tools-1.1.3/STAIR/test.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.3/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-25 02:37:43.950653 STAIR-tools-1.1.3/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-25 02:37:43.000000 STAIR-tools-1.1.3/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      299 2024-04-25 02:37:43.000000 STAIR-tools-1.1.3/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-25 02:37:43.000000 STAIR-tools-1.1.3/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-25 02:37:43.000000 STAIR-tools-1.1.3/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-25 02:37:43.951086 STAIR-tools-1.1.3/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      317 2024-04-25 02:37:40.000000 STAIR-tools-1.1.3/setup.py
```

### Comparing `STAIR-tools-1.1.2/README.md` & `STAIR-tools-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.2/STAIR/ABA_annotation.py` & `STAIR-tools-1.1.3/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.2/STAIR/emb_alignment.py` & `STAIR-tools-1.1.3/STAIR/emb_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from tqdm import tqdm
 import matplotlib.pyplot as plt
 
 import torch
 from torch.utils.data import DataLoader
 import torch.nn.functional as F
 
-from embedding import module_ae
-from embedding.module_ae import ae_dict
-from embedding.module_hgat import HGAT
-from embedding.dataset_ae import MyDataset
-from embedding.dataset_hgat import hgat_data
-from embedding.loss import nll_loss
+
+from STAIR.embedding.module_ae import ae_dict
+from STAIR.embedding.module_hgat import HGAT
+from STAIR.embedding.dataset_ae import MyDataset
+from STAIR.embedding.dataset_hgat import hgat_data
+from STAIR.embedding.loss import nll_loss
 
 from utils import MakeLogClass
 
 
 class Emb_Align(object):
 
     """
```

### Comparing `STAIR-tools-1.1.2/STAIR/loc_alignment.py` & `STAIR-tools-1.1.3/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.2/STAIR/loc_prediction.py` & `STAIR-tools-1.1.3/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.2/STAIR/utils.py` & `STAIR-tools-1.1.3/STAIR/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/gingerai-0.1.0.tar.gz` & `tmp/gingerai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gingerai-0.1.0.tar", last modified: Thu Apr 25 13:07:05 2024, max compression
+gzip compressed data, was "gingerai-0.1.1.tar", last modified: Thu Apr 25 13:14:26 2024, max compression
```

## Comparing `gingerai-0.1.0.tar` & `gingerai-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:07:05.614880 gingerai-0.1.0/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:07:05.614880 gingerai-0.1.0/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:07:05.000000 gingerai-0.1.0/README.md
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:07:05.614880 gingerai-0.1.0/gingerai/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       92 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai/__init__.py
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     2067 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai/torch.py
-drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:07:05.614880 gingerai-0.1.0/gingerai.egg-info/
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai.egg-info/PKG-INFO
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      216 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai.egg-info/SOURCES.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai.egg-info/dependency_links.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai.egg-info/requires.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:07:05.000000 gingerai-0.1.0/gingerai.egg-info/top_level.txt
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:07:05.624880 gingerai-0.1.0/setup.cfg
--rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:07:05.000000 gingerai-0.1.0/setup.py
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:14:26.345333 gingerai-0.1.1/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:14:26.345333 gingerai-0.1.1/PKG-INFO
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:14:25.000000 gingerai-0.1.1/README.md
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:14:26.345333 gingerai-0.1.1/gingerai/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       92 2024-04-25 13:14:25.000000 gingerai-0.1.1/gingerai/__init__.py
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)     2063 2024-04-25 13:14:25.000000 gingerai-0.1.1/gingerai/torch.py
+drwxr-xr-x   0 tomjurien  (1000) tomjurien  (1000)        0 2024-04-25 13:14:26.345333 gingerai-0.1.1/gingerai.egg-info/
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      340 2024-04-25 13:14:26.000000 gingerai-0.1.1/gingerai.egg-info/PKG-INFO
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      216 2024-04-25 13:14:26.000000 gingerai-0.1.1/gingerai.egg-info/SOURCES.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        1 2024-04-25 13:14:26.000000 gingerai-0.1.1/gingerai.egg-info/dependency_links.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        6 2024-04-25 13:14:26.000000 gingerai-0.1.1/gingerai.egg-info/requires.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)        9 2024-04-25 13:14:26.000000 gingerai-0.1.1/gingerai.egg-info/top_level.txt
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)       38 2024-04-25 13:14:26.345333 gingerai-0.1.1/setup.cfg
+-rw-r--r--   0 tomjurien  (1000) tomjurien  (1000)      439 2024-04-25 13:14:25.000000 gingerai-0.1.1/setup.py
```

### Comparing `gingerai-0.1.0/gingerai/torch.py` & `gingerai-0.1.1/gingerai/torch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import pickle
 import copy
 from torch import optim
 from torch.nn import functional as F
 
-def save_torch_model(model, optimizer_class, loss_fn_class, dataset, save_path):
+def save_torch_model(model, optimizer, loss_fn, dataset, save_path):
     """
     Save a PyTorch model with its structure, optimizer, loss function, and dataset to a serialized file.
     """
     # Deep copy the model structure without weights
     new_model = copy.deepcopy(model)
 
     # Reset parameters to ensure no weights are copied
@@ -16,19 +16,19 @@
         if hasattr(layer, 'reset_parameters'):
             layer.reset_parameters()
 
     new_model.apply(reset_parameters)
 
     # Store only the class of the optimizer and loss function
     optimizer_info = {
-        'class_name': optimizer_class.__name__,
+        'class_name': optimizer.__class__.__name__,
     }
 
     loss_info = {
-        'class_name': loss_fn_class.__name__,
+        'class_name': loss_fn.__class__.__name__,
     }
 
     # Include the dataset in the serialized data structure
     model_data = {
         'model': new_model,
         'optimizer': optimizer_info,
         'loss': loss_info,
```


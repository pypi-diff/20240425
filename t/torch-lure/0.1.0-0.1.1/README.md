# Comparing `tmp/torch_lure-0.1.0.tar.gz` & `tmp/torch_lure-0.1.1.tar.gz`

## Comparing `torch_lure-0.1.0.tar` & `torch_lure-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 torch_lure-0.1.0/.python-version
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 torch_lure-0.1.0/src/torch_lure/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 torch_lure-0.1.0/src/torch_lure/optimizers.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 torch_lure-0.1.0/src/torch_lure/utils.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 torch_lure-0.1.0/src/torch_lure/functional/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 torch_lure-0.1.0/.gitignore
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 torch_lure-0.1.0/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 torch_lure-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 torch_lure-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 torch_lure-0.1.1/.python-version
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/__init__.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/noise_schedulers.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/optim.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/utils.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/functional/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 torch_lure-0.1.1/src/torch_lure/modules/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 torch_lure-0.1.1/.gitignore
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 torch_lure-0.1.1/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 torch_lure-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 torch_lure-0.1.1/PKG-INFO
```

### Comparing `torch_lure-0.1.0/src/torch_lure/utils.py` & `torch_lure-0.1.1/src/torch_lure/utils.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.0/src/torch_lure/functional/__init__.py` & `torch_lure-0.1.1/src/torch_lure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_lure-0.1.0/pyproject.toml` & `torch_lure-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "torch-lure"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     { name = "fuyutarow", email = "fuyutarow@gmail.com" }
 ]
 dependencies = [
     "torch>=2.1",
     "numpy>=1.26.4",
     "sophia-opt>=0.2.2",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
-eywords = ["pytorch"]
+keywords = ["pytorch"]
 
 [project.urls]
 Homepage = "https://github.com/fuyutarow/torch-lure"
 Repository = "https://github.com/fuyutarow/torch-lure"
 
 [build-system]
 requires = ["hatchling"]
```

### Comparing `torch_lure-0.1.0/PKG-INFO` & `torch_lure-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: torch-lure
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Homepage, https://github.com/fuyutarow/torch-lure
 Project-URL: Repository, https://github.com/fuyutarow/torch-lure
 Author-email: fuyutarow <fuyutarow@gmail.com>
+Keywords: pytorch
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: sophia-opt>=0.2.2
 Requires-Dist: torch>=2.1
 Description-Content-Type: text/markdown
 
 # Torch Lure
@@ -23,18 +24,23 @@
 ```
 
 
 # Usage
 ```py
 import torch_lure as lure
 
-
 # Optimizers
 lure.SophiaG(lr=1e-3, weight_decay=0.2)
 
 # Functions
 lure.tanh_exp(x)
 lure.TanhExp()
 
 lure.quantile_loss(y_pred, y_target, quantile=0.5)
 lure.QuantileLoss(quantile=0.5)
+
+lure.RMSNrom(dim=256, eps=1e-6)
+
+# Noise Scheduler
+lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
+lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000):
 ```
```

#### html2text {}

```diff
@@ -1,10 +1,13 @@
-Metadata-Version: 2.3 Name: torch-lure Version: 0.1.0 Project-URL: Homepage,
+Metadata-Version: 2.3 Name: torch-lure Version: 0.1.1 Project-URL: Homepage,
 https://github.com/fuyutarow/torch-lure Project-URL: Repository, https://
 github.com/fuyutarow/torch-lure Author-email: fuyutarow
-gmail.com> Requires-Python: >=3.8 Requires-Dist: numpy>=1.26.4 Requires-Dist:
-sophia-opt>=0.2.2 Requires-Dist: torch>=2.1 Description-Content-Type: text/
-markdown # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]```sh pip install torch-lure ``` # Usage
-```py import torch_lure as lure # Optimizers lure.SophiaG(lr=1e-3,
-weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
-lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
-(quantile=0.5) ```
+gmail.com> Keywords: pytorch Requires-Python: >=3.8 Requires-Dist:
+numpy>=1.26.4 Requires-Dist: sophia-opt>=0.2.2 Requires-Dist: torch>=2.1
+Description-Content-Type: text/markdown # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]```sh pip
+install torch-lure ``` # Usage ```py import torch_lure as lure # Optimizers
+lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
+lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
+lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
+Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
+num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
+num_timesteps=1000): ```
```


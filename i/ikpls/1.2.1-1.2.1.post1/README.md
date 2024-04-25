# Comparing `tmp/ikpls-1.2.1.tar.gz` & `tmp/ikpls-1.2.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikpls-1.2.1.tar", max compression
+gzip compressed data, was "ikpls-1.2.1.post1.tar", max compression
```

## Comparing `ikpls-1.2.1.tar` & `ikpls-1.2.1.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11433 2024-04-24 17:27:10.449547 ikpls-1.2.1/LICENSE
--rw-r--r--   0        0        0     7664 2024-04-24 17:27:10.449547 ikpls-1.2.1/README.md
--rw-r--r--   0        0        0       22 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/fast_cross_validation/__init__.py
--rw-r--r--   0        0        0    24042 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/fast_cross_validation/numpy_ikpls.py
--rw-r--r--   0        0        0    15583 2024-04-24 17:27:10.449547 ikpls-1.2.1/ikpls/jax_ikpls_alg_1.py
--rw-r--r--   0        0        0    13495 2024-04-24 17:27:10.453547 ikpls-1.2.1/ikpls/jax_ikpls_alg_2.py
--rw-r--r--   0        0        0    41664 2024-04-24 17:27:10.453547 ikpls-1.2.1/ikpls/jax_ikpls_base.py
--rw-r--r--   0        0        0    10170 2024-04-24 17:27:10.453547 ikpls-1.2.1/ikpls/numpy_ikpls.py
--rw-r--r--   0        0        0      552 2024-04-24 17:27:10.453547 ikpls-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8586 1970-01-01 00:00:00.000000 ikpls-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11433 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/LICENSE
+-rw-r--r--   0        0        0     7650 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/README.md
+-rw-r--r--   0        0        0       28 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/fast_cross_validation/__init__.py
+-rw-r--r--   0        0        0    24042 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/fast_cross_validation/numpy_ikpls.py
+-rw-r--r--   0        0        0    15583 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/jax_ikpls_alg_1.py
+-rw-r--r--   0        0        0    13495 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/jax_ikpls_alg_2.py
+-rw-r--r--   0        0        0    41664 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/jax_ikpls_base.py
+-rw-r--r--   0        0        0    10170 2024-04-25 14:01:23.815035 ikpls-1.2.1.post1/ikpls/numpy_ikpls.py
+-rw-r--r--   0        0        0      558 2024-04-25 14:01:23.819035 ikpls-1.2.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     8578 1970-01-01 00:00:00.000000 ikpls-1.2.1.post1/PKG-INFO
```

### Comparing `ikpls-1.2.1/LICENSE` & `ikpls-1.2.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1/README.md` & `ikpls-1.2.1.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,14 @@
     JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py)
 
 ## Contribute
 
 To contribute, please read the [Contribution
 Guidelines](https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.md).
 
-(references)=
 ## References
 
 1. [Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. *Journal of Chemometrics*, 11(1), 73-85.](https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?)
 2. [Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. *Statistical Papers*, 50, 711-720.](https://doi.org/10.1007/s00362-009-0251-7)
 3. [Andersson, M. (2009). A comparison of nine PLS1 algorithms. *Journal of Chemometrics*, 23(10), 518-529.](https://doi.org/10.1002/cem.1248)
 4. [NumPy](https://numpy.org/)
 5. [scikit-learn](https://scikit-learn.org/stable/)
```

### Comparing `ikpls-1.2.1/ikpls/fast_cross_validation/numpy_ikpls.py` & `ikpls-1.2.1.post1/ikpls/fast_cross_validation/numpy_ikpls.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1/ikpls/jax_ikpls_alg_1.py` & `ikpls-1.2.1.post1/ikpls/jax_ikpls_alg_1.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1/ikpls/jax_ikpls_alg_2.py` & `ikpls-1.2.1.post1/ikpls/jax_ikpls_alg_2.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1/ikpls/jax_ikpls_base.py` & `ikpls-1.2.1.post1/ikpls/jax_ikpls_base.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1/ikpls/numpy_ikpls.py` & `ikpls-1.2.1.post1/ikpls/numpy_ikpls.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.1/pyproject.toml` & `ikpls-1.2.1.post1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ikpls"
-version = "1.2.1"
+version = "1.2.1.post1"
 description = ""
 authors = ["Sm00thix <oleemail@icloud.com>"]
 maintainers = ["Sm00thix <oleemail@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://ikpls.readthedocs.io/en/latest/"
 repository = "https://github.com/Sm00thix/IKPLS"
```

### Comparing `ikpls-1.2.1/PKG-INFO` & `ikpls-1.2.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikpls
-Version: 1.2.1
+Version: 1.2.1.post1
 Summary: 
 Home-page: https://ikpls.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Sm00thix
 Author-email: oleemail@icloud.com
 Maintainer: Sm00thix
 Maintainer-email: oleemail@icloud.com
@@ -177,15 +177,14 @@
     JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py)
 
 ## Contribute
 
 To contribute, please read the [Contribution
 Guidelines](https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.md).
 
-(references)=
 ## References
 
 1. [Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. *Journal of Chemometrics*, 11(1), 73-85.](https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?)
 2. [Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. *Statistical Papers*, 50, 711-720.](https://doi.org/10.1007/s00362-009-0251-7)
 3. [Andersson, M. (2009). A comparison of nine PLS1 algorithms. *Journal of Chemometrics*, 23(10), 518-529.](https://doi.org/10.1002/cem.1248)
 4. [NumPy](https://numpy.org/)
 5. [scikit-learn](https://scikit-learn.org/stable/)
```


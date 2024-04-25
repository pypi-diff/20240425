# Comparing `tmp/sklearn_ml-2.1.tar.gz` & `tmp/sklearn_ml-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_ml-2.1.tar", last modified: Thu Apr 25 14:27:32 2024, max compression
+gzip compressed data, was "sklearn_ml-2.2.tar", last modified: Thu Apr 25 14:39:17 2024, max compression
```

## Comparing `sklearn_ml-2.1.tar` & `sklearn_ml-2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:27:32.846328 sklearn_ml-2.1/
--rw-rw-rw-   0        0        0     1266 2024-04-25 14:27:32.846328 sklearn_ml-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-10-15 09:08:17.000000 sklearn_ml-2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 14:27:32.846328 sklearn_ml-2.1/setup.cfg
--rw-rw-rw-   0        0        0     2035 2024-04-25 13:55:16.000000 sklearn_ml-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:27:32.843328 sklearn_ml-2.1/sklearn_ml/
--rw-rw-rw-   0        0        0       34 2023-10-15 09:35:08.000000 sklearn_ml-2.1/sklearn_ml/__init__.py
--rw-rw-rw-   0        0        0    21398 2024-04-25 13:46:21.000000 sklearn_ml-2.1/sklearn_ml/_core.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:27:32.845327 sklearn_ml-2.1/sklearn_ml.egg-info/
--rw-rw-rw-   0        0        0     1266 2024-04-25 14:27:32.000000 sklearn_ml-2.1/sklearn_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-25 14:27:32.000000 sklearn_ml-2.1/sklearn_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:27:32.000000 sklearn_ml-2.1/sklearn_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-25 14:27:32.000000 sklearn_ml-2.1/sklearn_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 14:27:32.000000 sklearn_ml-2.1/sklearn_ml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 14:39:17.359908 sklearn_ml-2.2/
+-rw-rw-rw-   0        0        0     1266 2024-04-25 14:39:17.359908 sklearn_ml-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-10-15 09:08:17.000000 sklearn_ml-2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:39:17.359908 sklearn_ml-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2035 2024-04-25 14:39:07.000000 sklearn_ml-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:39:17.356908 sklearn_ml-2.2/sklearn_ml/
+-rw-rw-rw-   0        0        0       34 2023-10-15 09:35:08.000000 sklearn_ml-2.2/sklearn_ml/__init__.py
+-rw-rw-rw-   0        0        0    21414 2024-04-25 14:38:02.000000 sklearn_ml-2.2/sklearn_ml/_core.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:39:17.358908 sklearn_ml-2.2/sklearn_ml.egg-info/
+-rw-rw-rw-   0        0        0     1266 2024-04-25 14:39:17.000000 sklearn_ml-2.2/sklearn_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-25 14:39:17.000000 sklearn_ml-2.2/sklearn_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:39:17.000000 sklearn_ml-2.2/sklearn_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-25 14:39:17.000000 sklearn_ml-2.2/sklearn_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 14:39:17.000000 sklearn_ml-2.2/sklearn_ml.egg-info/top_level.txt
```

### Comparing `sklearn_ml-2.1/PKG-INFO` & `sklearn_ml-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn_ml
-Version: 2.1
+Version: 2.2
 Summary: A light package build on scikit-learn, which is used for machine learning missions.By using it, you could conveniently train and use models at the same time, and do some model comparison.
 Home-page: https://github.com/ChaneMo/sklearn-ml
 Author: ChaneMo
 Author-email: 
 License: Apache 2.0
 Keywords: scikit-learn,sklearn,classification,regression,cluster,machine learning,model comparison
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sklearn_ml-2.1/setup.py` & `sklearn_ml-2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="sklearn_ml",
-    version="2.1",
+    version="2.2",
     author="ChaneMo",
     author_email="",
     description="A light package build on scikit-learn, which is used for machine learning missions.By using it, you could conveniently train and use models at the same time, and do some model comparison.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChaneMo/sklearn-ml",
     packages=setuptools.find_packages(),
```

### Comparing `sklearn_ml-2.1/sklearn_ml/_core.py` & `sklearn_ml-2.2/sklearn_ml/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         print('Binary classification models:', self.binary_classification_models)
         print('Multiclass classification models:', self.multiclass_classification_models)
         print('Regression models:', self.regression_models)
         print('Clustering models:', self.cluster_models)
         print('-' * 130)
         print('functions:')
         print('initialize_models(self, model_names=None, mission=None, seed=None, param=None)')
-        print("fit_models(self, models_container=None, data=[], label=[], mission=None,  test_size=0.3, use_normalization='none')")
+        print("fit_models(self, models_container=None, data=[], label=[], stratify=None, mission=None,  test_size=0.3, use_normalization='none')")
         print('-' * 130)
 
     # define function to initialize models
     def initialize_models(self, model_names=None, mission=None, seed=None, param=None):
         '''
         :param model_names: models for mission, only support models in initialize lists
         :param mission: binary_classification, classification_classification, regression or clustering
@@ -238,15 +238,15 @@
 
 
         # fit classification models
         if mission=='multiclass_classification' or mission=='binary_classification':
             if not label:
                 print('Please make sure that your label are inputted!')
                 return
-            X_train, X_test, y_train, y_test = train_test_split(data, label, stratify=stratify,test_size=test_size)
+            X_train, X_test, y_train, y_test = train_test_split(data, label, stratify=stratify, test_size=test_size)
 
             # standardization
             if use_normalization=='minmax':
                 scaler = MinMaxScaler()
                 X_train = scaler.fit_transform(X_train)
                 X_test = scaler.fit_transform(X_test)
             if use_normalization=='standard':
```

### Comparing `sklearn_ml-2.1/sklearn_ml.egg-info/PKG-INFO` & `sklearn_ml-2.2/sklearn_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-ml
-Version: 2.1
+Version: 2.2
 Summary: A light package build on scikit-learn, which is used for machine learning missions.By using it, you could conveniently train and use models at the same time, and do some model comparison.
 Home-page: https://github.com/ChaneMo/sklearn-ml
 Author: ChaneMo
 Author-email: 
 License: Apache 2.0
 Keywords: scikit-learn,sklearn,classification,regression,cluster,machine learning,model comparison
 Classifier: Development Status :: 3 - Alpha
```


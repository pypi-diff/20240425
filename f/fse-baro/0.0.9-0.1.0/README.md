# Comparing `tmp/fse_baro-0.0.9.tar.gz` & `tmp/fse_baro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.0.9.tar", last modified: Thu Apr 25 03:48:49 2024, max compression
+gzip compressed data, was "fse_baro-0.1.0.tar", last modified: Thu Apr 25 05:39:39 2024, max compression
```

## Comparing `fse_baro-0.0.9.tar` & `fse_baro-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.149528 fse_baro-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.141528 fse_baro-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-25 03:48:41.000000 fse_baro-0.0.9/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-25 03:48:41.000000 fse_baro-0.0.9/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 03:48:41.000000 fse_baro-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-25 03:48:49.145528 fse_baro-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-25 03:48:41.000000 fse_baro-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 03:48:41.000000 fse_baro-0.0.9/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 03:48:41.000000 fse_baro-0.0.9/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 03:48:41.000000 fse_baro-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:48:49.149528 fse_baro-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-25 03:48:41.000000 fse_baro-0.0.9/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-25 03:48:41.000000 fse_baro-0.0.9/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.418404 fse_baro-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.414404 fse_baro-0.1.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 05:39:34.000000 fse_baro-0.1.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.410405 fse_baro-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.414404 fse_baro-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-25 05:39:34.000000 fse_baro-0.1.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 05:39:34.000000 fse_baro-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-25 05:39:34.000000 fse_baro-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-25 05:39:34.000000 fse_baro-0.1.0/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-25 05:39:34.000000 fse_baro-0.1.0/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 05:39:34.000000 fse_baro-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-25 05:39:39.418404 fse_baro-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-25 05:39:34.000000 fse_baro-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 05:39:34.000000 fse_baro-0.1.0/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 05:39:34.000000 fse_baro-0.1.0/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.414404 fse_baro-0.1.0/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 05:39:34.000000 fse_baro-0.1.0/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-25 05:39:34.000000 fse_baro-0.1.0/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-25 05:39:34.000000 fse_baro-0.1.0/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 05:39:34.000000 fse_baro-0.1.0/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 05:39:34.000000 fse_baro-0.1.0/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.418404 fse_baro-0.1.0/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-25 05:39:39.000000 fse_baro-0.1.0/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-25 05:39:39.000000 fse_baro-0.1.0/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 05:39:39.000000 fse_baro-0.1.0/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 05:39:39.000000 fse_baro-0.1.0/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 05:39:39.000000 fse_baro-0.1.0/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 05:39:34.000000 fse_baro-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 05:39:39.418404 fse_baro-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.418404 fse_baro-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-25 05:39:34.000000 fse_baro-0.1.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:39:39.418404 fse_baro-0.1.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-25 05:39:34.000000 fse_baro-0.1.0/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.0.9/.circleci/config.yml` & `fse_baro-0.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/.github/workflows/build-and-test.yml` & `fse_baro-0.1.0/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/.github/workflows/python-publish.yml` & `fse_baro-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/.gitignore` & `fse_baro-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/INSTALL.md` & `fse_baro-0.1.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/LICENSE` & `fse_baro-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/PKG-INFO` & `fse_baro-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.9
+Version: 0.1.0
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,15 +88,19 @@
 Our datasets are publicly available in Zenodo repository with the following information:
 
 - Dataset DOI: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11046533.svg)](https://doi.org/10.5281/zenodo.11046533)
 - Dataset URL: https://zenodo.org/records/11046533
 
 ## Reproducibility
 
-Check the Jupyter Notebook at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb) to reproduce the performance of BARO.
+To reproduce the performance of our BARO, we have prepared two Google Colab Notebooks as follows,
+1. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/120svKTl53cK8KId1rFSrw0BOqnReMB0j?usp=sharing): This notebook reproduces the RCA performance of BARO (also at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb)).
+2. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TObicUGcP9Z9xqML-iJxDo_Vlttp1Lpm?usp=sharing): This nodebook reproduces the output of the Multivariate BOCPD module. 
+
+
 
 ## Citation
 
 ```
 @inproceedings{pham2024baro,
   title={BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection},
   author={Luan Pham, Huong Ha, and Hongyu Zhang},
```

### Comparing `fse_baro-0.0.9/README.md` & `fse_baro-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -49,15 +49,19 @@
 Our datasets are publicly available in Zenodo repository with the following information:
 
 - Dataset DOI: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11046533.svg)](https://doi.org/10.5281/zenodo.11046533)
 - Dataset URL: https://zenodo.org/records/11046533
 
 ## Reproducibility
 
-Check the Jupyter Notebook at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb) to reproduce the performance of BARO.
+To reproduce the performance of our BARO, we have prepared two Google Colab Notebooks as follows,
+1. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/120svKTl53cK8KId1rFSrw0BOqnReMB0j?usp=sharing): This notebook reproduces the RCA performance of BARO (also at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb)).
+2. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TObicUGcP9Z9xqML-iJxDo_Vlttp1Lpm?usp=sharing): This nodebook reproduces the output of the Multivariate BOCPD module. 
+
+
 
 ## Citation
 
 ```
 @inproceedings{pham2024baro,
   title={BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection},
   author={Luan Pham, Huong Ha, and Hongyu Zhang},
```

### Comparing `fse_baro-0.0.9/REQUIREMENTS.md` & `fse_baro-0.1.0/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/STATUS.md` & `fse_baro-0.1.0/STATUS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/baro/_bocpd.py` & `fse_baro-0.1.0/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/baro/anomaly_detection.py` & `fse_baro-0.1.0/baro/anomaly_detection.py`

 * *Files 21% similar despite different names*

```diff
@@ -46,20 +46,14 @@
     return merged_anomalies, anomalies
 
 
 def bocpd(data):
     from functools import partial
     from baro._bocpd import online_changepoint_detection, constant_hazard, MultivariateT
     data = data.copy()
-    # "    data = pd.read_csv(data_path)   \n",
-    # "    selected_cols = [c for c in data.columns if \"latency-50\" in c]\n",
-    # "    data = data[selected_cols]\n",
-    # "    data = data.fillna(method=\"ffill\")\n",
-    # "    data = data.fillna(0)\n",
-    # "\n",
     time_col = data['time']
     data.drop(columns=['time'], inplace=True)
     for c in data.columns:
         data[c] = (data[c] - np.min(data[c])) / (np.max(data[c]) - np.min(data[c]))
     data = data.ffill()
     data = data.fillna(0)
     data = data.to_numpy()
```

### Comparing `fse_baro-0.0.9/baro/root_cause_analysis.py` & `fse_baro-0.1.0/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/baro/utility.py` & `fse_baro-0.1.0/baro/utility.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.1.0/fse_baro.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.9
+Version: 0.1.0
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,15 +88,19 @@
 Our datasets are publicly available in Zenodo repository with the following information:
 
 - Dataset DOI: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11046533.svg)](https://doi.org/10.5281/zenodo.11046533)
 - Dataset URL: https://zenodo.org/records/11046533
 
 ## Reproducibility
 
-Check the Jupyter Notebook at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb) to reproduce the performance of BARO.
+To reproduce the performance of our BARO, we have prepared two Google Colab Notebooks as follows,
+1. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/120svKTl53cK8KId1rFSrw0BOqnReMB0j?usp=sharing): This notebook reproduces the RCA performance of BARO (also at [tutorials/reproducibility.ipynb](https://github.com/phamquiluan/baro/blob/main/tutorials/reproducibility.ipynb)).
+2. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TObicUGcP9Z9xqML-iJxDo_Vlttp1Lpm?usp=sharing): This nodebook reproduces the output of the Multivariate BOCPD module. 
+
+
 
 ## Citation
 
 ```
 @inproceedings{pham2024baro,
   title={BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection},
   author={Luan Pham, Huong Ha, and Hongyu Zhang},
```

### Comparing `fse_baro-0.0.9/pyproject.toml` & `fse_baro-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/tests/test.py` & `fse_baro-0.1.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.9/tutorials/reproducibility.ipynb` & `fse_baro-0.1.0/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*


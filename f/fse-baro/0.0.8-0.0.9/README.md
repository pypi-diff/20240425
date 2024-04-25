# Comparing `tmp/fse_baro-0.0.8.tar.gz` & `tmp/fse_baro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.0.8.tar", last modified: Tue Apr 23 13:36:35 2024, max compression
+gzip compressed data, was "fse_baro-0.0.9.tar", last modified: Thu Apr 25 03:48:49 2024, max compression
```

## Comparing `fse_baro-0.0.8.tar` & `fse_baro-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.808563 fse_baro-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.808563 fse_baro-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-23 13:36:30.000000 fse_baro-0.0.8/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-23 13:36:30.000000 fse_baro-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-23 13:36:30.000000 fse_baro-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 13:36:30.000000 fse_baro-0.0.8/ENHANCEMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-23 13:36:30.000000 fse_baro-0.0.8/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 13:36:30.000000 fse_baro-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 13:36:35.812563 fse_baro-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-23 13:36:30.000000 fse_baro-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 13:36:30.000000 fse_baro-0.0.8/REQUIREMENTS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 13:36:30.000000 fse_baro-0.0.8/STATUS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-23 13:36:30.000000 fse_baro-0.0.8/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 13:36:35.000000 fse_baro-0.0.8/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 13:36:30.000000 fse_baro-0.0.8/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-23 13:36:30.000000 fse_baro-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:36:35.812563 fse_baro-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-23 13:36:30.000000 fse_baro-0.0.8/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:36:35.812563 fse_baro-0.0.8/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-23 13:36:30.000000 fse_baro-0.0.8/tutorials/reproducibility.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.149528 fse_baro-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.141528 fse_baro-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-25 03:48:41.000000 fse_baro-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-25 03:48:41.000000 fse_baro-0.0.9/ENHANCEMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-25 03:48:41.000000 fse_baro-0.0.9/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 03:48:41.000000 fse_baro-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-25 03:48:49.145528 fse_baro-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-25 03:48:41.000000 fse_baro-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 03:48:41.000000 fse_baro-0.0.9/REQUIREMENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 03:48:41.000000 fse_baro-0.0.9/STATUS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 03:48:41.000000 fse_baro-0.0.9/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 03:48:49.000000 fse_baro-0.0.9/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 03:48:41.000000 fse_baro-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:48:49.149528 fse_baro-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-25 03:48:41.000000 fse_baro-0.0.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:48:49.145528 fse_baro-0.0.9/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-25 03:48:41.000000 fse_baro-0.0.9/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.0.8/.github/workflows/build-and-test.yml` & `fse_baro-0.0.9/.github/workflows/build-and-test.yml`

 * *Files 13% similar despite different names*

```diff
@@ -6,24 +6,46 @@
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
-  build:
+  build-linux:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v3
+      with:
+        python-version: ${{ matrix.python-version }}
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        python -m pip install .
+    - name: Test with pytest
+      run: |
+        pytest tests/test.py
+
+  build-windows:
+
+    runs-on: windows-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.10", "3.11", "3.12"]
+
+    steps:
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `fse_baro-0.0.8/.github/workflows/python-publish.yml` & `fse_baro-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/.gitignore` & `fse_baro-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/INSTALL.md` & `fse_baro-0.0.9/INSTALL.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Installation
 
-We assume the users already satisfy the [REQUIREMENTS.md](REQUIREMENTS.md). Then, users can install BARO from PyPI ([Section 2](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#2-install-baro-from-pypi)) or build BARO from source ([Section 3](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#3-install-baro-from-source)).
+We assume the users already satisfy the [REQUIREMENTS.md](REQUIREMENTS.md) and have Python 3.10 installed ([Section 1](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#1-install-python310)). Then, users can install BARO from PyPI ([Section 2](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#2-install-baro-from-pypi)) or build BARO from source ([Section 3](https://github.com/phamquiluan/baro/blob/main/INSTALL.md#3-install-baro-from-source)). In addition, users who familiar with Continuous Integration (CI) can take a look at our [build-and-test.yml](https://github.com/phamquiluan/baro/blob/main/.github/workflows/build-and-test.yml) configuration to see how we test our BARO on Linux and Windows machine with Python 3.10, 3.11, and 3.12.
 
 
-## 1. Install Python3.10
+## 1. Install Python 3.10
 
 ```bash
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt update -y
 sudo apt-get install -y python3.10 python3.10-dev python3.10-venv
 ```
```

### Comparing `fse_baro-0.0.8/LICENSE` & `fse_baro-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/PKG-INFO` & `fse_baro-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.8
+Version: 0.0.9
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,51 +33,53 @@
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: pytest
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: matplotlib
 
-# BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
+# 🕵️ BARO: Root Cause Analysis for Microservices 
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
+[![Downloads](https://static.pepy.tech/badge/fse-baro)](https://pepy.tech/project/fse-baro)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/phamquiluan/baro/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/phamquiluan/baro/tree/main)
 [![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
+[![Upload Python Package](https://github.com/phamquiluan/baro/actions/workflows/python-publish.yml/badge.svg)](https://github.com/phamquiluan/baro/actions/workflows/python-publish.yml)
 
-BARO is an end-to-end approach to perform anomaly detection and root cause analysis for microservices's failures. This repository contains the artifact for reproducing the main experimental results in our paper accepted to ESEC/FSE 2024, and reusing purposes.
+**BARO** is an end-to-end anomaly detection and root cause analysis approach for microservices's failures. This repository includes artifacts for reuse and reproduction of experimental results presented in our FSE'24 paper titled _"BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection"_.
 
 
 ## Installation
 
-Install from [PyPI](https://pypi.org/project/fse-baro)
+Install from PyPI
 
 ```bash
 pip install fse-baro
 ```
 
 Or, build from source
 
 ```bash
 git clone https://github.com/phamquiluan/baro.git && cd baro
 pip install -e .
 ```
 
-More details are in [INSTALLATION.md](INSTALLATION.md).
+BARO has been tested on Linux and Windows, with different Python versions. More details are in [INSTALL.md](./INSTALL.md).
 
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
-from baro import BARO
+from baro.anomaly_detection import bocpd
+from baro.root_cause_analysis import robust_scorer
 
-m = BARO()
-
-anomalies = m.detect_anomalies(data)
-root_causes = m.rca(data, anomalies=anomalies)
+anomalies = bocpd(data)  # the data and its visualization are presented in the Google Colab above.
+root_causes = robust_scorer(data, anomalies=anomalies)
 print(root_causes)
 ```
 
 ## Download Paper
 
 TBD
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fse_baro-0.0.8/README.md` & `fse_baro-0.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-# BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
+# 🕵️ BARO: Root Cause Analysis for Microservices 
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
+[![Downloads](https://static.pepy.tech/badge/fse-baro)](https://pepy.tech/project/fse-baro)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/phamquiluan/baro/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/phamquiluan/baro/tree/main)
 [![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
+[![Upload Python Package](https://github.com/phamquiluan/baro/actions/workflows/python-publish.yml/badge.svg)](https://github.com/phamquiluan/baro/actions/workflows/python-publish.yml)
 
-BARO is an end-to-end approach to perform anomaly detection and root cause analysis for microservices's failures. This repository contains the artifact for reproducing the main experimental results in our paper accepted to ESEC/FSE 2024, and reusing purposes.
+**BARO** is an end-to-end anomaly detection and root cause analysis approach for microservices's failures. This repository includes artifacts for reuse and reproduction of experimental results presented in our FSE'24 paper titled _"BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection"_.
 
 
 ## Installation
 
-Install from [PyPI](https://pypi.org/project/fse-baro)
+Install from PyPI
 
 ```bash
 pip install fse-baro
 ```
 
 Or, build from source
 
 ```bash
 git clone https://github.com/phamquiluan/baro.git && cd baro
 pip install -e .
 ```
 
-More details are in [INSTALLATION.md](INSTALLATION.md).
+BARO has been tested on Linux and Windows, with different Python versions. More details are in [INSTALL.md](./INSTALL.md).
 
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
-from baro import BARO
+from baro.anomaly_detection import bocpd
+from baro.root_cause_analysis import robust_scorer
 
-m = BARO()
-
-anomalies = m.detect_anomalies(data)
-root_causes = m.rca(data, anomalies=anomalies)
+anomalies = bocpd(data)  # the data and its visualization are presented in the Google Colab above.
+root_causes = robust_scorer(data, anomalies=anomalies)
 print(root_causes)
 ```
 
 ## Download Paper
 
 TBD
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fse_baro-0.0.8/REQUIREMENTS.md` & `fse_baro-0.0.9/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/STATUS.md` & `fse_baro-0.0.9/STATUS.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 We apply for the Available and Reusable badges.
 We believe our artifact meets the requirements for the two badges in the [artifact submission guideline](https://2024.esec-fse.org/track/fse-2024-artifacts).
 
 * **Available**: Our artifact is "Available" as it is publicly accessible through the following repository.
-  * Github: [https://github.com/phamquiluan/baro/releases/tag/fse2024](https://github.com/phamquiluan/baro/releases/tag/fse2024)
+  * Github: [https://github.com/phamquiluan/baro/releases/tag/0.0.9](https://github.com/phamquiluan/baro/releases/tag/0.0.9)
 
 * **Reusable**: Our artifact is "Reusable" (and also "Functional") as we meet the following five criteria (the first four are the criteria for "Functional" badge) mentioned in the [artifact submission guideline](https://2024.esec-fse.org/track/fse-2024-artifacts).
   * _Documented_: We provide the following documents necessary for using our artifact: (1) README, (2) REQUIREMENTS, (3) STATUS, (4) LICENSE, (5) INSTALL, and (6) a copy of the accepted paper.
   * _Consistent & Complete_: We provide concrete steps for reproducing the main experimental results in the paper.
   * _Exercisable_: We provide scripts and related commands for running experiments.
   * _Reusable for Future Researches_: We provide a PyPI package [fse-baro](https://pypi.org/project/fse-baro/) with a Google Colab Notebook ([![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 ) that provides concrete instructions for running BARO with metrics data. Thus, other researchers can use BARO in their own research.
```

### Comparing `fse_baro-0.0.8/baro/_bocpd.py` & `fse_baro-0.0.9/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/baro/anomaly_detection.py` & `fse_baro-0.0.9/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/baro/root_cause_analysis.py` & `fse_baro-0.0.9/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/baro/utility.py` & `fse_baro-0.0.9/baro/utility.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.0.9/fse_baro.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.8
+Version: 0.0.9
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,51 +33,53 @@
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: pytest
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: matplotlib
 
-# BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
+# 🕵️ BARO: Root Cause Analysis for Microservices 
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
+[![Downloads](https://static.pepy.tech/badge/fse-baro)](https://pepy.tech/project/fse-baro)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/phamquiluan/baro/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/phamquiluan/baro/tree/main)
 [![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
+[![Upload Python Package](https://github.com/phamquiluan/baro/actions/workflows/python-publish.yml/badge.svg)](https://github.com/phamquiluan/baro/actions/workflows/python-publish.yml)
 
-BARO is an end-to-end approach to perform anomaly detection and root cause analysis for microservices's failures. This repository contains the artifact for reproducing the main experimental results in our paper accepted to ESEC/FSE 2024, and reusing purposes.
+**BARO** is an end-to-end anomaly detection and root cause analysis approach for microservices's failures. This repository includes artifacts for reuse and reproduction of experimental results presented in our FSE'24 paper titled _"BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection"_.
 
 
 ## Installation
 
-Install from [PyPI](https://pypi.org/project/fse-baro)
+Install from PyPI
 
 ```bash
 pip install fse-baro
 ```
 
 Or, build from source
 
 ```bash
 git clone https://github.com/phamquiluan/baro.git && cd baro
 pip install -e .
 ```
 
-More details are in [INSTALLATION.md](INSTALLATION.md).
+BARO has been tested on Linux and Windows, with different Python versions. More details are in [INSTALL.md](./INSTALL.md).
 
 ## How-to-use
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
 
 
 ```python
-from baro import BARO
+from baro.anomaly_detection import bocpd
+from baro.root_cause_analysis import robust_scorer
 
-m = BARO()
-
-anomalies = m.detect_anomalies(data)
-root_causes = m.rca(data, anomalies=anomalies)
+anomalies = bocpd(data)  # the data and its visualization are presented in the Google Colab above.
+root_causes = robust_scorer(data, anomalies=anomalies)
 print(root_causes)
 ```
 
 ## Download Paper
 
 TBD
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fse_baro-0.0.8/pyproject.toml` & `fse_baro-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.8/tutorials/reproducibility.ipynb` & `fse_baro-0.0.9/tutorials/reproducibility.ipynb`

 * *Files identical despite different names*


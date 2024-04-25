# Comparing `tmp/cuopt_thin_client-24.3.4.tar.gz` & `tmp/cuopt_thin_client-24.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuopt_thin_client-24.3.4.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "cuopt_thin_client-24.3.5.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cuopt_thin_client-24.3.4.tar` & `cuopt_thin_client-24.3.5.tar`

### file list

```diff
@@ -1,2 +1,2 @@
 -rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
--rw-r--r--   0        0        0     6674 1993-04-05 07:00:00.000000 PKG-INFO
+-rw-r--r--   0        0        0     6705 1993-04-05 07:00:00.000000 PKG-INFO
```

### PKG-INFO

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cuopt_thin_client
-Version: 24.3.4
+Version: 24.3.5
 Summary: A Python client and command-line
 Author: NVIDIA Corporation
 License: MIT
 Project-URL: Homepage, https://docs.nvidia.com/cuopt/overview.html
 Project-URL: Source, https://github.com/rapidsai/cuopt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: License.txt
 Requires-Dist: requests
+Requires-Dist: python-dateutil
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 
 # cuOpt Service Python Thin Client
 cuOpt Service Python Thin Client is a Python interface to enable access to NVIDIA managed cuOpt service.
 
 Install `cuopt-thin-client` via pip
```


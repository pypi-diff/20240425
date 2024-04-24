# Comparing `tmp/brynq_sdk_zoho-1.0.0.tar.gz` & `tmp/brynq_sdk_zoho-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_zoho-1.0.0.tar", last modified: Wed Apr 24 14:21:56 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_zoho-1.0.1.tar", last modified: Wed Apr 24 19:00:27 2024, max compression
```

## Comparing `brynq_sdk_zoho-1.0.0.tar` & `brynq_sdk_zoho-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk/zoho/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-24 14:21:38.000000 brynq_sdk_zoho-1.0.0/brynq_sdk/zoho/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6715 2024-04-24 14:21:38.000000 brynq_sdk_zoho-1.0.0/brynq_sdk/zoho/extract_zoho_desk.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2024-04-24 14:21:38.000000 brynq_sdk_zoho-1.0.0/brynq_sdk/zoho/upload_zoho_desk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/brynq_sdk_zoho.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 14:21:56.000000 brynq_sdk_zoho-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-24 14:21:38.000000 brynq_sdk_zoho-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk/zoho/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-24 19:00:09.000000 brynq_sdk_zoho-1.0.1/brynq_sdk/zoho/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2024-04-24 19:00:09.000000 brynq_sdk_zoho-1.0.1/brynq_sdk/zoho/extract_zoho_desk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2024-04-24 19:00:09.000000 brynq_sdk_zoho-1.0.1/brynq_sdk/zoho/upload_zoho_desk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/brynq_sdk_zoho.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 19:00:27.000000 brynq_sdk_zoho-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-24 19:00:09.000000 brynq_sdk_zoho-1.0.1/setup.py
```

### Comparing `brynq_sdk_zoho-1.0.0/brynq_sdk/zoho/extract_zoho_desk.py` & `brynq_sdk_zoho-1.0.1/brynq_sdk/zoho/extract_zoho_desk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import pandas as pd
 from typing import Union, List
 import requests
 import json
-from brynq_sdk.BrynQ import BrynQ
+from brynq_sdk.brynq import BrynQ
 
 basedir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.append(basedir)
 
 
 class ExtractZohoDesk(BrynQ):
```

### Comparing `brynq_sdk_zoho-1.0.0/brynq_sdk/zoho/upload_zoho_desk.py` & `brynq_sdk_zoho-1.0.1/brynq_sdk/zoho/upload_zoho_desk.py`

 * *Files identical despite different names*


# Comparing `tmp/brynq_sdk_task_scheduler-1.0.0.tar.gz` & `tmp/brynq_sdk_task_scheduler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_task_scheduler-1.0.0.tar", last modified: Wed Apr 17 12:40:49 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_task_scheduler-1.1.0.tar", last modified: Thu Apr 25 10:06:47 2024, max compression
```

## Comparing `brynq_sdk_task_scheduler-1.0.0.tar` & `brynq_sdk_task_scheduler-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-17 12:40:30.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43084 2024-04-17 12:40:30.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/brynq_sdk_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 12:40:49.000000 brynq_sdk_task_scheduler-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-17 12:40:30.000000 brynq_sdk_task_scheduler-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-25 10:06:28.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43079 2024-04-25 10:06:28.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-25 10:06:28.000000 brynq_sdk_task_scheduler-1.1.0/setup.py
```

### Comparing `brynq_sdk_task_scheduler-1.0.0/brynq_sdk/task_scheduler/task_scheduler.py` & `brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/task_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import traceback
 import pandas as pd
 import json
 import requests
 from salure_helpers.mandrill import MailClient
 from brynq_sdk.functions import Functions
 from brynq_sdk.brynq import BrynQ
-from salure_helpers.mysql import MySQL
+from brynq_sdk.brynq import MySQL
 from salure_helpers.elastic import Elastic
 import warnings
 import re
 
 
 class TaskScheduler(BrynQ):
```

### Comparing `brynq_sdk_task_scheduler-1.0.0/setup.py` & `brynq_sdk_task_scheduler-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name='brynq_sdk_task_scheduler',
-    version='1.0.0',
+    version='1.1.0',
     description='Code to execute tasks in BrynQ.com with the task scheduler',
     long_description='Code to execute tasks in the BrynQ.com platform with the task scheduler',
     author='BrynQ',
     author_email='support@brynq.com',
     packages=["brynq_sdk.task_scheduler"],
     license='BrynQ License',
     install_requires=[
         'brynq-sdk-brynq>=1',
         'brynq-sdk-functions>=1',
-        'salure-helpers-mysql>=1',
-        'salure-helpers-mandrill>=0',
-        'salure-helpers-elastic>=1'
+        'brynq-sdk-mysql>=1',
+        'brynq-sdk-mandrill>=1',
+        'brynq-sdk-elastic>=1'
     ],
     zip_safe=False,
 )
```


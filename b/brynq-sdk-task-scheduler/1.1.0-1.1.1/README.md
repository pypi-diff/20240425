# Comparing `tmp/brynq_sdk_task_scheduler-1.1.0.tar.gz` & `tmp/brynq_sdk_task_scheduler-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_task_scheduler-1.1.0.tar", last modified: Thu Apr 25 10:06:47 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_task_scheduler-1.1.1.tar", last modified: Thu Apr 25 10:11:54 2024, max compression
```

## Comparing `brynq_sdk_task_scheduler-1.1.0.tar` & `brynq_sdk_task_scheduler-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-25 10:06:28.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43079 2024-04-25 10:06:28.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/brynq_sdk_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 10:06:47.000000 brynq_sdk_task_scheduler-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-25 10:06:28.000000 brynq_sdk_task_scheduler-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-25 10:11:38.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43069 2024-04-25 10:11:38.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/brynq_sdk_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 10:11:54.000000 brynq_sdk_task_scheduler-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-25 10:11:38.000000 brynq_sdk_task_scheduler-1.1.1/setup.py
```

### Comparing `brynq_sdk_task_scheduler-1.1.0/brynq_sdk/task_scheduler/task_scheduler.py` & `brynq_sdk_task_scheduler-1.1.1/brynq_sdk/task_scheduler/task_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import inspect
 import time
 import typing
 import traceback
 import pandas as pd
 import json
 import requests
-from salure_helpers.mandrill import MailClient
+from brynq_sdk.mandrill import MailClient
 from brynq_sdk.functions import Functions
 from brynq_sdk.brynq import BrynQ
 from brynq_sdk.brynq import MySQL
-from salure_helpers.elastic import Elastic
+from brynq_sdk.elastic import Elastic
 import warnings
 import re
 
 
 class TaskScheduler(BrynQ):
 
     def __init__(self, task_id: int = None, loglevel: str = 'INFO', email_after_errors: bool = False):
```

### Comparing `brynq_sdk_task_scheduler-1.1.0/setup.py` & `brynq_sdk_task_scheduler-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='brynq_sdk_task_scheduler',
-    version='1.1.0',
+    version='1.1.1',
     description='Code to execute tasks in BrynQ.com with the task scheduler',
     long_description='Code to execute tasks in the BrynQ.com platform with the task scheduler',
     author='BrynQ',
     author_email='support@brynq.com',
     packages=["brynq_sdk.task_scheduler"],
     license='BrynQ License',
     install_requires=[
```


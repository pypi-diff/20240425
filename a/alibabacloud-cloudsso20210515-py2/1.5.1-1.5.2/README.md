# Comparing `tmp/alibabacloud_cloudsso20210515_py2-1.5.1.tar.gz` & `tmp/alibabacloud_cloudsso20210515_py2-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudsso20210515_py2-1.5.1.tar", last modified: Mon Apr 22 17:13:39 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudsso20210515_py2-1.5.2.tar", last modified: Thu Apr 25 02:35:26 2024, max compression
```

## Comparing `alibabacloud_cloudsso20210515_py2-1.5.1.tar` & `alibabacloud_cloudsso20210515_py2-1.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/
--rw-r--r--   0 root         (0) root         (0)      917 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   172601 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515/client.py
--rw-r--r--   0 root         (0) root         (0)   557405 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2024-04-22 17:13:39.000000 alibabacloud_cloudsso20210515_py2-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   172601 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515/client.py
+-rw-r--r--   0 root         (0) root         (0)   557405 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 02:35:26.000000 alibabacloud_cloudsso20210515_py2-1.5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-04-25 02:35:25.000000 alibabacloud_cloudsso20210515_py2-1.5.2/setup.py
```

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/ChangeLog.md` & `alibabacloud_cloudsso20210515_py2-1.5.2/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-22 Version: 1.5.1
+- Update API GetDirectoryStatistics: update response param.
+
+
 2024-03-29 Version: 1.5.0
 - Support API GetLoginPreference.
 - Support API GetPasswordPolicy.
 - Support API GetUserId.
 - Support API SetLoginPreference.
 - Support API SetPasswordPolicy.
 - Update API GetUser: update response param.
```

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/LICENSE` & `alibabacloud_cloudsso20210515_py2-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/PKG-INFO` & `alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_cloudsso20210515_py2
-Version: 1.5.1
+Name: alibabacloud-cloudsso20210515-py2
+Version: 1.5.2
 Summary: Alibaba Cloud cloudsso (20210515) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/README-CN.md` & `alibabacloud_cloudsso20210515_py2-1.5.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/README.md` & `alibabacloud_cloudsso20210515_py2-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515/client.py` & `alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515/models.py` & `alibabacloud_cloudsso20210515_py2-1.5.2/alibabacloud_cloudsso20210515/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/alibabacloud_cloudsso20210515_py2.egg-info/PKG-INFO` & `alibabacloud_cloudsso20210515_py2-1.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-cloudsso20210515-py2
-Version: 1.5.1
+Name: alibabacloud_cloudsso20210515_py2
+Version: 1.5.2
 Summary: Alibaba Cloud cloudsso (20210515) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudsso20210515_py2-1.5.1/setup.py` & `alibabacloud_cloudsso20210515_py2-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudsso20210515_py2.
 
-Created on 22/04/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudsso20210515"
 NAME = "alibabacloud_cloudsso20210515_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cloudsso (20210515) SDK Library for Python2"
```


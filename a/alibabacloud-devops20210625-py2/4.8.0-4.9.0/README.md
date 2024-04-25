# Comparing `tmp/alibabacloud_devops20210625_py2-4.8.0.tar.gz` & `tmp/alibabacloud_devops20210625_py2-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_devops20210625_py2-4.8.0.tar", last modified: Fri Jan 19 06:09:01 2024, max compression
+gzip compressed data, was "dist/alibabacloud_devops20210625_py2-4.9.0.tar", last modified: Fri Jan 19 07:25:37 2024, max compression
```

## Comparing `alibabacloud_devops20210625_py2-4.8.0.tar` & `alibabacloud_devops20210625_py2-4.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/
--rw-r--r--   0 root         (0) root         (0)     3079 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625/__init__.py
--rw-r--r--   0 root         (0) root         (0)   330847 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625/client.py
--rw-r--r--   0 root         (0) root         (0)  1736932 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2024-01-19 06:09:01.000000 alibabacloud_devops20210625_py2-4.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/
+-rw-r--r--   0 root         (0) root         (0)     3149 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   330847 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625/client.py
+-rw-r--r--   0 root         (0) root         (0)  1736932 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-01-19 07:25:37.000000 alibabacloud_devops20210625_py2-4.9.0/setup.py
```

### Comparing `alibabacloud_devops20210625_py2-4.8.0/ChangeLog.md` & `alibabacloud_devops20210625_py2-4.9.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-01-19 Version: 4.8.0
+- Generated python2 2021-06-25 for devops.
+
 2024-01-15 Version: 4.7.0
 - Generated python2 2021-06-25 for devops.
 
 2024-01-11 Version: 4.6.1
 - Generated python2 2021-06-25 for devops.
 
 2024-01-05 Version: 4.6.0
```

### Comparing `alibabacloud_devops20210625_py2-4.8.0/LICENSE` & `alibabacloud_devops20210625_py2-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_devops20210625_py2-4.8.0/PKG-INFO` & `alibabacloud_devops20210625_py2-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_devops20210625_py2
-Version: 4.8.0
+Version: 4.9.0
 Summary: Alibaba Cloud devops (20210625) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_devops20210625_py2-4.8.0/README-CN.md` & `alibabacloud_devops20210625_py2-4.9.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_devops20210625_py2-4.8.0/README.md` & `alibabacloud_devops20210625_py2-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625/client.py` & `alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625/models.py` & `alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_devops20210625_py2-4.8.0/alibabacloud_devops20210625_py2.egg-info/PKG-INFO` & `alibabacloud_devops20210625_py2-4.9.0/alibabacloud_devops20210625_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-devops20210625-py2
-Version: 4.8.0
+Version: 4.9.0
 Summary: Alibaba Cloud devops (20210625) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_devops20210625_py2-4.8.0/setup.py` & `alibabacloud_devops20210625_py2-4.9.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0.tar.gz` & `tmp/aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/aws-kinesisfirehose-alpha/dist/python/aws-cdk.aws-kinesisfirehose-alpha-2.", last modified: Wed Sep 27 19:38:47 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/aws-kinesisfirehose-alpha/dist/python/aws-cdk.aws-kinesisfirehose-alpha-2", last modified: Sat Sep 30 10:07:58 2023, max compression
```

## Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0.tar` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    25508 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24491 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1926 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/
--rw-r--r--   0 root         (0) root         (0)   155687 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      457 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73903 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.99.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:36.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25508 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      611 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:38:47.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    25508 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24491 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/
+-rw-r--r--   0 root         (0) root         (0)   155687 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73904 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.99.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:49.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25508 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      611 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:07:58.000000 aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/LICENSE` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: The CDK Construct Library for AWS::KinesisFirehose
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/README.md` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/setup.py` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-kinesisfirehose-alpha",
-    "version": "2.99.0.a0",
+    "version": "2.99.1.a0",
     "description": "The CDK Construct Library for AWS::KinesisFirehose",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_kinesisfirehose_alpha",
         "aws_cdk.aws_kinesisfirehose_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_kinesisfirehose_alpha._jsii": [
-            "aws-kinesisfirehose-alpha@2.99.0-alpha.0.jsii.tgz"
+            "aws-kinesisfirehose-alpha@2.99.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_kinesisfirehose_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.99.0",
+        "aws-cdk-lib==2.99.1",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.88.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: The CDK Construct Library for AWS::KinesisFirehose
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-kinesisfirehose-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-kinesisfirehose-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/requires.txt
 src/aws_cdk.aws_kinesisfirehose_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_kinesisfirehose_alpha/__init__.py
 src/aws_cdk/aws_kinesisfirehose_alpha/py.typed
 src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/__init__.py
-src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.99.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_kinesisfirehose_alpha/_jsii/aws-kinesisfirehose-alpha@2.99.1-alpha.0.jsii.tgz
```


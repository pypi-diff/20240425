# Comparing `tmp/boto3_stubs-1.34.91.tar.gz` & `tmp/boto3_stubs-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3_stubs-1.34.91.tar", last modified: Wed Apr 24 19:19:03 2024, max compression
+gzip compressed data, was "boto3_stubs-1.34.92.tar", last modified: Thu Apr 25 19:32:12 2024, max compression
```

## Comparing `boto3_stubs-1.34.91.tar` & `boto3_stubs-1.34.92.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.275932 boto3_stubs-1.34.91/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:17:44.000000 boto3_stubs-1.34.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-04-24 19:19:03.275932 boto3_stubs-1.34.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    69482 2024-04-24 19:17:44.000000 boto3_stubs-1.34.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.175934 boto3_stubs-1.34.91/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   205730 2024-04-24 19:17:48.000000 boto3_stubs-1.34.91/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/crt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.175934 boto3_stubs-1.34.91/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.175934 boto3_stubs-1.34.91/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.175934 boto3_stubs-1.34.91/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:48.000000 boto3_stubs-1.34.91/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.175934 boto3_stubs-1.34.91/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.175934 boto3_stubs-1.34.91/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/s3/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   232778 2024-04-24 19:17:52.000000 boto3_stubs-1.34.91/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:03.179934 boto3_stubs-1.34.91/boto3_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-04-24 19:19:03.000000 boto3_stubs-1.34.91/boto3_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 19:19:03.000000 boto3_stubs-1.34.91/boto3_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:03.000000 boto3_stubs-1.34.91/boto3_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:03.000000 boto3_stubs-1.34.91/boto3_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-04-24 19:19:03.000000 boto3_stubs-1.34.91/boto3_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 19:19:03.000000 boto3_stubs-1.34.91/boto3_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:03.275932 boto3_stubs-1.34.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    50417 2024-04-24 19:17:43.000000 boto3_stubs-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.559390 boto3_stubs-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:34.000000 boto3_stubs-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-04-25 19:32:12.559390 boto3_stubs-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    69482 2024-04-25 19:31:34.000000 boto3_stubs-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.455389 boto3_stubs-1.34.92/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   205730 2024-04-25 19:31:38.000000 boto3_stubs-1.34.92/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/crt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.455389 boto3_stubs-1.34.92/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.455389 boto3_stubs-1.34.92/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.455389 boto3_stubs-1.34.92/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:38.000000 boto3_stubs-1.34.92/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.459390 boto3_stubs-1.34.92/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.459390 boto3_stubs-1.34.92/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/s3/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   232778 2024-04-25 19:31:42.000000 boto3_stubs-1.34.92/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:12.459390 boto3_stubs-1.34.92/boto3_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-04-25 19:32:12.000000 boto3_stubs-1.34.92/boto3_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 19:32:12.000000 boto3_stubs-1.34.92/boto3_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:12.000000 boto3_stubs-1.34.92/boto3_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:12.000000 boto3_stubs-1.34.92/boto3_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-04-25 19:32:12.000000 boto3_stubs-1.34.92/boto3_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:32:12.000000 boto3_stubs-1.34.92/boto3_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:12.559390 boto3_stubs-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    50417 2024-04-25 19:31:33.000000 boto3_stubs-1.34.92/setup.py
```

### Comparing `boto3_stubs-1.34.91/LICENSE` & `boto3_stubs-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/PKG-INFO` & `boto3_stubs-1.34.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.34.91
-Summary: Type annotations for boto3 1.34.91 generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3 1.34.92 generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -421,16 +421,16 @@
 Requires-Dist: mypy-boto3-dynamodb<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-ec2<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-lambda<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-rds<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-s3<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-sqs<1.35.0,>=1.34.0; extra == "essential"
 Provides-Extra: boto3
-Requires-Dist: boto3==1.34.91; extra == "boto3"
-Requires-Dist: botocore==1.34.91; extra == "boto3"
+Requires-Dist: boto3==1.34.92; extra == "boto3"
+Requires-Dist: botocore==1.34.92; extra == "boto3"
 Provides-Extra: accessanalyzer
 Requires-Dist: mypy-boto3-accessanalyzer<1.35.0,>=1.34.0; extra == "accessanalyzer"
 Provides-Extra: account
 Requires-Dist: mypy-boto3-account<1.35.0,>=1.34.0; extra == "account"
 Provides-Extra: acm
 Requires-Dist: mypy-boto3-acm<1.35.0,>=1.34.0; extra == "acm"
 Provides-Extra: acm-pca
@@ -1202,24 +1202,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/1.34.91/index.html)
+[boto3 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/1.34.92/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -1927,15 +1927,15 @@
 - `boto3-stubs[docdb]` - Type annotations for
   [DocDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
   service.
 - `boto3-stubs[docdb-elastic]` - Type annotations for
   [DocDBElastic](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
   service.
 - `boto3-stubs[drs]` - Type annotations for
-  [drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
+  [Drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
 - `boto3-stubs[ds]` - Type annotations for
   [DirectoryService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
   service.
 - `boto3-stubs[dynamodb]` - Type annotations for
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
   service.
 - `boto3-stubs[dynamodbstreams]` - Type annotations for
@@ -1997,15 +1997,15 @@
 - `boto3-stubs[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
   service.
 - `boto3-stubs[evidently]` - Type annotations for
   [CloudWatchEvidently](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
   service.
 - `boto3-stubs[finspace]` - Type annotations for
-  [finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
+  [Finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
   service.
 - `boto3-stubs[finspace-data]` - Type annotations for
   [FinSpaceData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
   service.
 - `boto3-stubs[firehose]` - Type annotations for
   [Firehose](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
   service.
@@ -2064,24 +2064,24 @@
   service.
 - `boto3-stubs[iam]` - Type annotations for
   [IAM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/) service.
 - `boto3-stubs[identitystore]` - Type annotations for
   [IdentityStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
   service.
 - `boto3-stubs[imagebuilder]` - Type annotations for
-  [imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
+  [Imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
   service.
 - `boto3-stubs[importexport]` - Type annotations for
   [ImportExport](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
   service.
 - `boto3-stubs[inspector]` - Type annotations for
   [Inspector](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
   service.
 - `boto3-stubs[inspector-scan]` - Type annotations for
-  [inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
+  [Inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
   service.
 - `boto3-stubs[inspector2]` - Type annotations for
   [Inspector2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
   service.
 - `boto3-stubs[internetmonitor]` - Type annotations for
   [CloudWatchInternetMonitor](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
   service.
@@ -2131,27 +2131,27 @@
   service.
 - `boto3-stubs[iotwireless]` - Type annotations for
   [IoTWireless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
   service.
 - `boto3-stubs[ivs]` - Type annotations for
   [IVS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/) service.
 - `boto3-stubs[ivs-realtime]` - Type annotations for
-  [ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
+  [Ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
   service.
 - `boto3-stubs[ivschat]` - Type annotations for
-  [ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
+  [Ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
   service.
 - `boto3-stubs[kafka]` - Type annotations for
   [Kafka](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
   service.
 - `boto3-stubs[kafkaconnect]` - Type annotations for
   [KafkaConnect](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
   service.
 - `boto3-stubs[kendra]` - Type annotations for
-  [kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
+  [Kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
   service.
 - `boto3-stubs[kendra-ranking]` - Type annotations for
   [KendraRanking](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
   service.
 - `boto3-stubs[keyspaces]` - Type annotations for
   [Keyspaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
   service.
@@ -2271,15 +2271,15 @@
 - `boto3-stubs[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
 - `boto3-stubs[mediapackagev2]` - Type annotations for
-  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  [Mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
   service.
 - `boto3-stubs[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
@@ -2295,15 +2295,15 @@
 - `boto3-stubs[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
   service.
 - `boto3-stubs[mgh]` - Type annotations for
   [MigrationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
   service.
 - `boto3-stubs[mgn]` - Type annotations for
-  [mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
+  [Mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
 - `boto3-stubs[migration-hub-refactor-spaces]` - Type annotations for
   [MigrationHubRefactorSpaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
   service.
 - `boto3-stubs[migrationhub-config]` - Type annotations for
   [MigrationHubConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
   service.
 - `boto3-stubs[migrationhuborchestrator]` - Type annotations for
@@ -2453,15 +2453,15 @@
 - `boto3-stubs[redshift-serverless]` - Type annotations for
   [RedshiftServerless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
   service.
 - `boto3-stubs[rekognition]` - Type annotations for
   [Rekognition](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
   service.
 - `boto3-stubs[repostspace]` - Type annotations for
-  [rePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
+  [RePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
   service.
 - `boto3-stubs[resiliencehub]` - Type annotations for
   [ResilienceHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
   service.
 - `boto3-stubs[resource-explorer-2]` - Type annotations for
   [ResourceExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
   service.
@@ -2571,15 +2571,15 @@
 - `boto3-stubs[sesv2]` - Type annotations for
   [SESV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
   service.
 - `boto3-stubs[shield]` - Type annotations for
   [Shield](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
   service.
 - `boto3-stubs[signer]` - Type annotations for
-  [signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
+  [Signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
   service.
 - `boto3-stubs[simspaceweaver]` - Type annotations for
   [SimSpaceWeaver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
   service.
 - `boto3-stubs[sms]` - Type annotations for
   [SMS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/) service.
 - `boto3-stubs[sms-voice]` - Type annotations for
```

### Comparing `boto3_stubs-1.34.91/README.md` & `boto3_stubs-1.34.92/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/1.34.91/index.html)
+[boto3 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/1.34.92/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -731,15 +731,15 @@
 - `boto3-stubs[docdb]` - Type annotations for
   [DocDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
   service.
 - `boto3-stubs[docdb-elastic]` - Type annotations for
   [DocDBElastic](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
   service.
 - `boto3-stubs[drs]` - Type annotations for
-  [drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
+  [Drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
 - `boto3-stubs[ds]` - Type annotations for
   [DirectoryService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
   service.
 - `boto3-stubs[dynamodb]` - Type annotations for
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
   service.
 - `boto3-stubs[dynamodbstreams]` - Type annotations for
@@ -801,15 +801,15 @@
 - `boto3-stubs[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
   service.
 - `boto3-stubs[evidently]` - Type annotations for
   [CloudWatchEvidently](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
   service.
 - `boto3-stubs[finspace]` - Type annotations for
-  [finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
+  [Finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
   service.
 - `boto3-stubs[finspace-data]` - Type annotations for
   [FinSpaceData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
   service.
 - `boto3-stubs[firehose]` - Type annotations for
   [Firehose](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
   service.
@@ -868,24 +868,24 @@
   service.
 - `boto3-stubs[iam]` - Type annotations for
   [IAM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/) service.
 - `boto3-stubs[identitystore]` - Type annotations for
   [IdentityStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
   service.
 - `boto3-stubs[imagebuilder]` - Type annotations for
-  [imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
+  [Imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
   service.
 - `boto3-stubs[importexport]` - Type annotations for
   [ImportExport](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
   service.
 - `boto3-stubs[inspector]` - Type annotations for
   [Inspector](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
   service.
 - `boto3-stubs[inspector-scan]` - Type annotations for
-  [inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
+  [Inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
   service.
 - `boto3-stubs[inspector2]` - Type annotations for
   [Inspector2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
   service.
 - `boto3-stubs[internetmonitor]` - Type annotations for
   [CloudWatchInternetMonitor](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
   service.
@@ -935,27 +935,27 @@
   service.
 - `boto3-stubs[iotwireless]` - Type annotations for
   [IoTWireless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
   service.
 - `boto3-stubs[ivs]` - Type annotations for
   [IVS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/) service.
 - `boto3-stubs[ivs-realtime]` - Type annotations for
-  [ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
+  [Ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
   service.
 - `boto3-stubs[ivschat]` - Type annotations for
-  [ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
+  [Ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
   service.
 - `boto3-stubs[kafka]` - Type annotations for
   [Kafka](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
   service.
 - `boto3-stubs[kafkaconnect]` - Type annotations for
   [KafkaConnect](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
   service.
 - `boto3-stubs[kendra]` - Type annotations for
-  [kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
+  [Kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
   service.
 - `boto3-stubs[kendra-ranking]` - Type annotations for
   [KendraRanking](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
   service.
 - `boto3-stubs[keyspaces]` - Type annotations for
   [Keyspaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
   service.
@@ -1075,15 +1075,15 @@
 - `boto3-stubs[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
 - `boto3-stubs[mediapackagev2]` - Type annotations for
-  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  [Mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
   service.
 - `boto3-stubs[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
@@ -1099,15 +1099,15 @@
 - `boto3-stubs[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
   service.
 - `boto3-stubs[mgh]` - Type annotations for
   [MigrationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
   service.
 - `boto3-stubs[mgn]` - Type annotations for
-  [mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
+  [Mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
 - `boto3-stubs[migration-hub-refactor-spaces]` - Type annotations for
   [MigrationHubRefactorSpaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
   service.
 - `boto3-stubs[migrationhub-config]` - Type annotations for
   [MigrationHubConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
   service.
 - `boto3-stubs[migrationhuborchestrator]` - Type annotations for
@@ -1257,15 +1257,15 @@
 - `boto3-stubs[redshift-serverless]` - Type annotations for
   [RedshiftServerless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
   service.
 - `boto3-stubs[rekognition]` - Type annotations for
   [Rekognition](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
   service.
 - `boto3-stubs[repostspace]` - Type annotations for
-  [rePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
+  [RePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
   service.
 - `boto3-stubs[resiliencehub]` - Type annotations for
   [ResilienceHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
   service.
 - `boto3-stubs[resource-explorer-2]` - Type annotations for
   [ResourceExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
   service.
@@ -1375,15 +1375,15 @@
 - `boto3-stubs[sesv2]` - Type annotations for
   [SESV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
   service.
 - `boto3-stubs[shield]` - Type annotations for
   [Shield](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
   service.
 - `boto3-stubs[signer]` - Type annotations for
-  [signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
+  [Signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
   service.
 - `boto3-stubs[simspaceweaver]` - Type annotations for
   [SimSpaceWeaver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
   service.
 - `boto3-stubs[sms]` - Type annotations for
   [SMS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/) service.
 - `boto3-stubs[sms-voice]` - Type annotations for
```

### Comparing `boto3_stubs-1.34.91/boto3-stubs/__init__.pyi` & `boto3_stubs-1.34.92/boto3-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 from mypy_boto3_devops_guru.client import DevOpsGuruClient
 from mypy_boto3_directconnect.client import DirectConnectClient
 from mypy_boto3_discovery.client import ApplicationDiscoveryServiceClient
 from mypy_boto3_dlm.client import DLMClient
 from mypy_boto3_dms.client import DatabaseMigrationServiceClient
 from mypy_boto3_docdb.client import DocDBClient
 from mypy_boto3_docdb_elastic.client import DocDBElasticClient
-from mypy_boto3_drs.client import drsClient
+from mypy_boto3_drs.client import DrsClient
 from mypy_boto3_ds.client import DirectoryServiceClient
 from mypy_boto3_dynamodb.client import DynamoDBClient
 from mypy_boto3_dynamodb.service_resource import DynamoDBServiceResource
 from mypy_boto3_dynamodbstreams.client import DynamoDBStreamsClient
 from mypy_boto3_ebs.client import EBSClient
 from mypy_boto3_ec2.client import EC2Client
 from mypy_boto3_ec2.service_resource import EC2ServiceResource
@@ -144,15 +144,15 @@
 from mypy_boto3_emr.client import EMRClient
 from mypy_boto3_emr_containers.client import EMRContainersClient
 from mypy_boto3_emr_serverless.client import EMRServerlessClient
 from mypy_boto3_entityresolution.client import EntityResolutionClient
 from mypy_boto3_es.client import ElasticsearchServiceClient
 from mypy_boto3_events.client import EventBridgeClient
 from mypy_boto3_evidently.client import CloudWatchEvidentlyClient
-from mypy_boto3_finspace.client import finspaceClient
+from mypy_boto3_finspace.client import FinspaceClient
 from mypy_boto3_finspace_data.client import FinSpaceDataClient
 from mypy_boto3_firehose.client import FirehoseClient
 from mypy_boto3_fis.client import FISClient
 from mypy_boto3_fms.client import FMSClient
 from mypy_boto3_forecast.client import ForecastServiceClient
 from mypy_boto3_forecastquery.client import ForecastQueryServiceClient
 from mypy_boto3_frauddetector.client import FraudDetectorClient
@@ -170,19 +170,19 @@
 from mypy_boto3_guardduty.client import GuardDutyClient
 from mypy_boto3_health.client import HealthClient
 from mypy_boto3_healthlake.client import HealthLakeClient
 from mypy_boto3_honeycode.client import HoneycodeClient
 from mypy_boto3_iam.client import IAMClient
 from mypy_boto3_iam.service_resource import IAMServiceResource
 from mypy_boto3_identitystore.client import IdentityStoreClient
-from mypy_boto3_imagebuilder.client import imagebuilderClient
+from mypy_boto3_imagebuilder.client import ImagebuilderClient
 from mypy_boto3_importexport.client import ImportExportClient
 from mypy_boto3_inspector2.client import Inspector2Client
 from mypy_boto3_inspector.client import InspectorClient
-from mypy_boto3_inspector_scan.client import inspectorscanClient
+from mypy_boto3_inspector_scan.client import InspectorscanClient
 from mypy_boto3_internetmonitor.client import CloudWatchInternetMonitorClient
 from mypy_boto3_iot1click_devices.client import IoT1ClickDevicesServiceClient
 from mypy_boto3_iot1click_projects.client import IoT1ClickProjectsClient
 from mypy_boto3_iot.client import IoTClient
 from mypy_boto3_iot_data.client import IoTDataPlaneClient
 from mypy_boto3_iot_jobs_data.client import IoTJobsDataPlaneClient
 from mypy_boto3_iotanalytics.client import IoTAnalyticsClient
@@ -193,19 +193,19 @@
 from mypy_boto3_iotfleetwise.client import IoTFleetWiseClient
 from mypy_boto3_iotsecuretunneling.client import IoTSecureTunnelingClient
 from mypy_boto3_iotsitewise.client import IoTSiteWiseClient
 from mypy_boto3_iotthingsgraph.client import IoTThingsGraphClient
 from mypy_boto3_iottwinmaker.client import IoTTwinMakerClient
 from mypy_boto3_iotwireless.client import IoTWirelessClient
 from mypy_boto3_ivs.client import IVSClient
-from mypy_boto3_ivs_realtime.client import ivsrealtimeClient
-from mypy_boto3_ivschat.client import ivschatClient
+from mypy_boto3_ivs_realtime.client import IvsrealtimeClient
+from mypy_boto3_ivschat.client import IvschatClient
 from mypy_boto3_kafka.client import KafkaClient
 from mypy_boto3_kafkaconnect.client import KafkaConnectClient
-from mypy_boto3_kendra.client import kendraClient
+from mypy_boto3_kendra.client import KendraClient
 from mypy_boto3_kendra_ranking.client import KendraRankingClient
 from mypy_boto3_keyspaces.client import KeyspacesClient
 from mypy_boto3_kinesis.client import KinesisClient
 from mypy_boto3_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
 from mypy_boto3_kinesis_video_media.client import KinesisVideoMediaClient
 from mypy_boto3_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient
 from mypy_boto3_kinesis_video_webrtc_storage.client import KinesisVideoWebRTCStorageClient
@@ -244,23 +244,23 @@
 from mypy_boto3_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
 from mypy_boto3_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
 from mypy_boto3_mediaconnect.client import MediaConnectClient
 from mypy_boto3_mediaconvert.client import MediaConvertClient
 from mypy_boto3_medialive.client import MediaLiveClient
 from mypy_boto3_mediapackage.client import MediaPackageClient
 from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
-from mypy_boto3_mediapackagev2.client import mediapackagev2Client
+from mypy_boto3_mediapackagev2.client import Mediapackagev2Client
 from mypy_boto3_mediastore.client import MediaStoreClient
 from mypy_boto3_mediastore_data.client import MediaStoreDataClient
 from mypy_boto3_mediatailor.client import MediaTailorClient
 from mypy_boto3_medical_imaging.client import HealthImagingClient
 from mypy_boto3_memorydb.client import MemoryDBClient
 from mypy_boto3_meteringmarketplace.client import MarketplaceMeteringClient
 from mypy_boto3_mgh.client import MigrationHubClient
-from mypy_boto3_mgn.client import mgnClient
+from mypy_boto3_mgn.client import MgnClient
 from mypy_boto3_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
 from mypy_boto3_migrationhub_config.client import MigrationHubConfigClient
 from mypy_boto3_migrationhuborchestrator.client import MigrationHubOrchestratorClient
 from mypy_boto3_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
 from mypy_boto3_mobile.client import MobileClient
 from mypy_boto3_mq.client import MQClient
 from mypy_boto3_mturk.client import MTurkClient
@@ -308,15 +308,15 @@
 from mypy_boto3_rbin.client import RecycleBinClient
 from mypy_boto3_rds.client import RDSClient
 from mypy_boto3_rds_data.client import RDSDataServiceClient
 from mypy_boto3_redshift.client import RedshiftClient
 from mypy_boto3_redshift_data.client import RedshiftDataAPIServiceClient
 from mypy_boto3_redshift_serverless.client import RedshiftServerlessClient
 from mypy_boto3_rekognition.client import RekognitionClient
-from mypy_boto3_repostspace.client import rePostPrivateClient
+from mypy_boto3_repostspace.client import RePostPrivateClient
 from mypy_boto3_resiliencehub.client import ResilienceHubClient
 from mypy_boto3_resource_explorer_2.client import ResourceExplorerClient
 from mypy_boto3_resource_groups.client import ResourceGroupsClient
 from mypy_boto3_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient
 from mypy_boto3_robomaker.client import RoboMakerClient
 from mypy_boto3_rolesanywhere.client import IAMRolesAnywhereClient
 from mypy_boto3_route53.client import Route53Client
@@ -349,15 +349,15 @@
 from mypy_boto3_service_quotas.client import ServiceQuotasClient
 from mypy_boto3_servicecatalog.client import ServiceCatalogClient
 from mypy_boto3_servicecatalog_appregistry.client import AppRegistryClient
 from mypy_boto3_servicediscovery.client import ServiceDiscoveryClient
 from mypy_boto3_ses.client import SESClient
 from mypy_boto3_sesv2.client import SESV2Client
 from mypy_boto3_shield.client import ShieldClient
-from mypy_boto3_signer.client import signerClient
+from mypy_boto3_signer.client import SignerClient
 from mypy_boto3_simspaceweaver.client import SimSpaceWeaverClient
 from mypy_boto3_sms.client import SMSClient
 from mypy_boto3_sms_voice.client import PinpointSMSVoiceClient
 from mypy_boto3_snow_device_management.client import SnowDeviceManagementClient
 from mypy_boto3_snowball.client import SnowballClient
 from mypy_boto3_sns.client import SNSClient
 from mypy_boto3_sns.service_resource import SNSServiceResource
@@ -1894,15 +1894,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> drsClient: ...
+) -> DrsClient: ...
 @overload
 def client(
     service_name: Literal["ds"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -2232,15 +2232,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> finspaceClient: ...
+) -> FinspaceClient: ...
 @overload
 def client(
     service_name: Literal["finspace-data"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -2544,15 +2544,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> imagebuilderClient: ...
+) -> ImagebuilderClient: ...
 @overload
 def client(
     service_name: Literal["importexport"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -2583,15 +2583,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> inspectorscanClient: ...
+) -> InspectorscanClient: ...
 @overload
 def client(
     service_name: Literal["inspector2"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -2843,28 +2843,28 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> ivsrealtimeClient: ...
+) -> IvsrealtimeClient: ...
 @overload
 def client(
     service_name: Literal["ivschat"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> ivschatClient: ...
+) -> IvschatClient: ...
 @overload
 def client(
     service_name: Literal["kafka"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -2895,15 +2895,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> kendraClient: ...
+) -> KendraClient: ...
 @overload
 def client(
     service_name: Literal["kendra-ranking"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -3454,15 +3454,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> mediapackagev2Client: ...
+) -> Mediapackagev2Client: ...
 @overload
 def client(
     service_name: Literal["mediastore"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -3558,15 +3558,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> mgnClient: ...
+) -> MgnClient: ...
 @overload
 def client(
     service_name: Literal["migration-hub-refactor-spaces"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -4273,15 +4273,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> rePostPrivateClient: ...
+) -> RePostPrivateClient: ...
 @overload
 def client(
     service_name: Literal["resiliencehub"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
@@ -4793,15 +4793,15 @@
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
-) -> signerClient: ...
+) -> SignerClient: ...
 @overload
 def client(
     service_name: Literal["simspaceweaver"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
```

### Comparing `boto3_stubs-1.34.91/boto3-stubs/crt.pyi` & `boto3_stubs-1.34.92/boto3-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/docs/utils.pyi` & `boto3_stubs-1.34.92/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/dynamodb/conditions.pyi` & `boto3_stubs-1.34.92/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/dynamodb/table.pyi` & `boto3_stubs-1.34.92/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/dynamodb/transform.pyi` & `boto3_stubs-1.34.92/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/dynamodb/types.pyi` & `boto3_stubs-1.34.92/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/exceptions.pyi` & `boto3_stubs-1.34.92/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/resources/action.pyi` & `boto3_stubs-1.34.92/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/resources/base.pyi` & `boto3_stubs-1.34.92/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/resources/collection.pyi` & `boto3_stubs-1.34.92/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/resources/model.pyi` & `boto3_stubs-1.34.92/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/resources/params.pyi` & `boto3_stubs-1.34.92/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/resources/response.pyi` & `boto3_stubs-1.34.92/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/s3/inject.pyi` & `boto3_stubs-1.34.92/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/s3/transfer.pyi` & `boto3_stubs-1.34.92/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3-stubs/session.pyi` & `boto3_stubs-1.34.92/boto3-stubs/session.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 from mypy_boto3_devops_guru.client import DevOpsGuruClient
 from mypy_boto3_directconnect.client import DirectConnectClient
 from mypy_boto3_discovery.client import ApplicationDiscoveryServiceClient
 from mypy_boto3_dlm.client import DLMClient
 from mypy_boto3_dms.client import DatabaseMigrationServiceClient
 from mypy_boto3_docdb.client import DocDBClient
 from mypy_boto3_docdb_elastic.client import DocDBElasticClient
-from mypy_boto3_drs.client import drsClient
+from mypy_boto3_drs.client import DrsClient
 from mypy_boto3_ds.client import DirectoryServiceClient
 from mypy_boto3_dynamodb.client import DynamoDBClient
 from mypy_boto3_dynamodb.service_resource import DynamoDBServiceResource
 from mypy_boto3_dynamodbstreams.client import DynamoDBStreamsClient
 from mypy_boto3_ebs.client import EBSClient
 from mypy_boto3_ec2.client import EC2Client
 from mypy_boto3_ec2.service_resource import EC2ServiceResource
@@ -150,15 +150,15 @@
 from mypy_boto3_emr.client import EMRClient
 from mypy_boto3_emr_containers.client import EMRContainersClient
 from mypy_boto3_emr_serverless.client import EMRServerlessClient
 from mypy_boto3_entityresolution.client import EntityResolutionClient
 from mypy_boto3_es.client import ElasticsearchServiceClient
 from mypy_boto3_events.client import EventBridgeClient
 from mypy_boto3_evidently.client import CloudWatchEvidentlyClient
-from mypy_boto3_finspace.client import finspaceClient
+from mypy_boto3_finspace.client import FinspaceClient
 from mypy_boto3_finspace_data.client import FinSpaceDataClient
 from mypy_boto3_firehose.client import FirehoseClient
 from mypy_boto3_fis.client import FISClient
 from mypy_boto3_fms.client import FMSClient
 from mypy_boto3_forecast.client import ForecastServiceClient
 from mypy_boto3_forecastquery.client import ForecastQueryServiceClient
 from mypy_boto3_frauddetector.client import FraudDetectorClient
@@ -176,19 +176,19 @@
 from mypy_boto3_guardduty.client import GuardDutyClient
 from mypy_boto3_health.client import HealthClient
 from mypy_boto3_healthlake.client import HealthLakeClient
 from mypy_boto3_honeycode.client import HoneycodeClient
 from mypy_boto3_iam.client import IAMClient
 from mypy_boto3_iam.service_resource import IAMServiceResource
 from mypy_boto3_identitystore.client import IdentityStoreClient
-from mypy_boto3_imagebuilder.client import imagebuilderClient
+from mypy_boto3_imagebuilder.client import ImagebuilderClient
 from mypy_boto3_importexport.client import ImportExportClient
 from mypy_boto3_inspector2.client import Inspector2Client
 from mypy_boto3_inspector.client import InspectorClient
-from mypy_boto3_inspector_scan.client import inspectorscanClient
+from mypy_boto3_inspector_scan.client import InspectorscanClient
 from mypy_boto3_internetmonitor.client import CloudWatchInternetMonitorClient
 from mypy_boto3_iot1click_devices.client import IoT1ClickDevicesServiceClient
 from mypy_boto3_iot1click_projects.client import IoT1ClickProjectsClient
 from mypy_boto3_iot.client import IoTClient
 from mypy_boto3_iot_data.client import IoTDataPlaneClient
 from mypy_boto3_iot_jobs_data.client import IoTJobsDataPlaneClient
 from mypy_boto3_iotanalytics.client import IoTAnalyticsClient
@@ -199,19 +199,19 @@
 from mypy_boto3_iotfleetwise.client import IoTFleetWiseClient
 from mypy_boto3_iotsecuretunneling.client import IoTSecureTunnelingClient
 from mypy_boto3_iotsitewise.client import IoTSiteWiseClient
 from mypy_boto3_iotthingsgraph.client import IoTThingsGraphClient
 from mypy_boto3_iottwinmaker.client import IoTTwinMakerClient
 from mypy_boto3_iotwireless.client import IoTWirelessClient
 from mypy_boto3_ivs.client import IVSClient
-from mypy_boto3_ivs_realtime.client import ivsrealtimeClient
-from mypy_boto3_ivschat.client import ivschatClient
+from mypy_boto3_ivs_realtime.client import IvsrealtimeClient
+from mypy_boto3_ivschat.client import IvschatClient
 from mypy_boto3_kafka.client import KafkaClient
 from mypy_boto3_kafkaconnect.client import KafkaConnectClient
-from mypy_boto3_kendra.client import kendraClient
+from mypy_boto3_kendra.client import KendraClient
 from mypy_boto3_kendra_ranking.client import KendraRankingClient
 from mypy_boto3_keyspaces.client import KeyspacesClient
 from mypy_boto3_kinesis.client import KinesisClient
 from mypy_boto3_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
 from mypy_boto3_kinesis_video_media.client import KinesisVideoMediaClient
 from mypy_boto3_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient
 from mypy_boto3_kinesis_video_webrtc_storage.client import KinesisVideoWebRTCStorageClient
@@ -250,23 +250,23 @@
 from mypy_boto3_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
 from mypy_boto3_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
 from mypy_boto3_mediaconnect.client import MediaConnectClient
 from mypy_boto3_mediaconvert.client import MediaConvertClient
 from mypy_boto3_medialive.client import MediaLiveClient
 from mypy_boto3_mediapackage.client import MediaPackageClient
 from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
-from mypy_boto3_mediapackagev2.client import mediapackagev2Client
+from mypy_boto3_mediapackagev2.client import Mediapackagev2Client
 from mypy_boto3_mediastore.client import MediaStoreClient
 from mypy_boto3_mediastore_data.client import MediaStoreDataClient
 from mypy_boto3_mediatailor.client import MediaTailorClient
 from mypy_boto3_medical_imaging.client import HealthImagingClient
 from mypy_boto3_memorydb.client import MemoryDBClient
 from mypy_boto3_meteringmarketplace.client import MarketplaceMeteringClient
 from mypy_boto3_mgh.client import MigrationHubClient
-from mypy_boto3_mgn.client import mgnClient
+from mypy_boto3_mgn.client import MgnClient
 from mypy_boto3_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
 from mypy_boto3_migrationhub_config.client import MigrationHubConfigClient
 from mypy_boto3_migrationhuborchestrator.client import MigrationHubOrchestratorClient
 from mypy_boto3_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
 from mypy_boto3_mobile.client import MobileClient
 from mypy_boto3_mq.client import MQClient
 from mypy_boto3_mturk.client import MTurkClient
@@ -314,15 +314,15 @@
 from mypy_boto3_rbin.client import RecycleBinClient
 from mypy_boto3_rds.client import RDSClient
 from mypy_boto3_rds_data.client import RDSDataServiceClient
 from mypy_boto3_redshift.client import RedshiftClient
 from mypy_boto3_redshift_data.client import RedshiftDataAPIServiceClient
 from mypy_boto3_redshift_serverless.client import RedshiftServerlessClient
 from mypy_boto3_rekognition.client import RekognitionClient
-from mypy_boto3_repostspace.client import rePostPrivateClient
+from mypy_boto3_repostspace.client import RePostPrivateClient
 from mypy_boto3_resiliencehub.client import ResilienceHubClient
 from mypy_boto3_resource_explorer_2.client import ResourceExplorerClient
 from mypy_boto3_resource_groups.client import ResourceGroupsClient
 from mypy_boto3_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient
 from mypy_boto3_robomaker.client import RoboMakerClient
 from mypy_boto3_rolesanywhere.client import IAMRolesAnywhereClient
 from mypy_boto3_route53.client import Route53Client
@@ -355,15 +355,15 @@
 from mypy_boto3_service_quotas.client import ServiceQuotasClient
 from mypy_boto3_servicecatalog.client import ServiceCatalogClient
 from mypy_boto3_servicecatalog_appregistry.client import AppRegistryClient
 from mypy_boto3_servicediscovery.client import ServiceDiscoveryClient
 from mypy_boto3_ses.client import SESClient
 from mypy_boto3_sesv2.client import SESV2Client
 from mypy_boto3_shield.client import ShieldClient
-from mypy_boto3_signer.client import signerClient
+from mypy_boto3_signer.client import SignerClient
 from mypy_boto3_simspaceweaver.client import SimSpaceWeaverClient
 from mypy_boto3_sms.client import SMSClient
 from mypy_boto3_sms_voice.client import PinpointSMSVoiceClient
 from mypy_boto3_snow_device_management.client import SnowDeviceManagementClient
 from mypy_boto3_snowball.client import SnowballClient
 from mypy_boto3_sns.client import SNSClient
 from mypy_boto3_sns.service_resource import SNSServiceResource
@@ -2028,15 +2028,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> drsClient: ...
+    ) -> DrsClient: ...
     @overload
     def client(
         self,
         service_name: Literal["ds"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -2392,15 +2392,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> finspaceClient: ...
+    ) -> FinspaceClient: ...
     @overload
     def client(
         self,
         service_name: Literal["finspace-data"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -2728,15 +2728,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> imagebuilderClient: ...
+    ) -> ImagebuilderClient: ...
     @overload
     def client(
         self,
         service_name: Literal["importexport"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -2770,15 +2770,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> inspectorscanClient: ...
+    ) -> InspectorscanClient: ...
     @overload
     def client(
         self,
         service_name: Literal["inspector2"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -3050,29 +3050,29 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> ivsrealtimeClient: ...
+    ) -> IvsrealtimeClient: ...
     @overload
     def client(
         self,
         service_name: Literal["ivschat"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> ivschatClient: ...
+    ) -> IvschatClient: ...
     @overload
     def client(
         self,
         service_name: Literal["kafka"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -3106,15 +3106,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> kendraClient: ...
+    ) -> KendraClient: ...
     @overload
     def client(
         self,
         service_name: Literal["kendra-ranking"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -3708,15 +3708,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> mediapackagev2Client: ...
+    ) -> Mediapackagev2Client: ...
     @overload
     def client(
         self,
         service_name: Literal["mediastore"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -3820,15 +3820,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> mgnClient: ...
+    ) -> MgnClient: ...
     @overload
     def client(
         self,
         service_name: Literal["migration-hub-refactor-spaces"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -4590,15 +4590,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> rePostPrivateClient: ...
+    ) -> RePostPrivateClient: ...
     @overload
     def client(
         self,
         service_name: Literal["resiliencehub"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
@@ -5150,15 +5150,15 @@
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
-    ) -> signerClient: ...
+    ) -> SignerClient: ...
     @overload
     def client(
         self,
         service_name: Literal["simspaceweaver"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
```

### Comparing `boto3_stubs-1.34.91/boto3-stubs/utils.pyi` & `boto3_stubs-1.34.92/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3_stubs.egg-info/PKG-INFO` & `boto3_stubs-1.34.92/boto3_stubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.34.91
-Summary: Type annotations for boto3 1.34.91 generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3 1.34.92 generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -421,16 +421,16 @@
 Requires-Dist: mypy-boto3-dynamodb<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-ec2<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-lambda<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-rds<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-s3<1.35.0,>=1.34.0; extra == "essential"
 Requires-Dist: mypy-boto3-sqs<1.35.0,>=1.34.0; extra == "essential"
 Provides-Extra: boto3
-Requires-Dist: boto3==1.34.91; extra == "boto3"
-Requires-Dist: botocore==1.34.91; extra == "boto3"
+Requires-Dist: boto3==1.34.92; extra == "boto3"
+Requires-Dist: botocore==1.34.92; extra == "boto3"
 Provides-Extra: accessanalyzer
 Requires-Dist: mypy-boto3-accessanalyzer<1.35.0,>=1.34.0; extra == "accessanalyzer"
 Provides-Extra: account
 Requires-Dist: mypy-boto3-account<1.35.0,>=1.34.0; extra == "account"
 Provides-Extra: acm
 Requires-Dist: mypy-boto3-acm<1.35.0,>=1.34.0; extra == "acm"
 Provides-Extra: acm-pca
@@ -1202,24 +1202,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/1.34.91/index.html)
+[boto3 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/1.34.92/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -1927,15 +1927,15 @@
 - `boto3-stubs[docdb]` - Type annotations for
   [DocDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
   service.
 - `boto3-stubs[docdb-elastic]` - Type annotations for
   [DocDBElastic](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
   service.
 - `boto3-stubs[drs]` - Type annotations for
-  [drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
+  [Drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
 - `boto3-stubs[ds]` - Type annotations for
   [DirectoryService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
   service.
 - `boto3-stubs[dynamodb]` - Type annotations for
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
   service.
 - `boto3-stubs[dynamodbstreams]` - Type annotations for
@@ -1997,15 +1997,15 @@
 - `boto3-stubs[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
   service.
 - `boto3-stubs[evidently]` - Type annotations for
   [CloudWatchEvidently](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
   service.
 - `boto3-stubs[finspace]` - Type annotations for
-  [finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
+  [Finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
   service.
 - `boto3-stubs[finspace-data]` - Type annotations for
   [FinSpaceData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
   service.
 - `boto3-stubs[firehose]` - Type annotations for
   [Firehose](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
   service.
@@ -2064,24 +2064,24 @@
   service.
 - `boto3-stubs[iam]` - Type annotations for
   [IAM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/) service.
 - `boto3-stubs[identitystore]` - Type annotations for
   [IdentityStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
   service.
 - `boto3-stubs[imagebuilder]` - Type annotations for
-  [imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
+  [Imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
   service.
 - `boto3-stubs[importexport]` - Type annotations for
   [ImportExport](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
   service.
 - `boto3-stubs[inspector]` - Type annotations for
   [Inspector](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
   service.
 - `boto3-stubs[inspector-scan]` - Type annotations for
-  [inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
+  [Inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
   service.
 - `boto3-stubs[inspector2]` - Type annotations for
   [Inspector2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
   service.
 - `boto3-stubs[internetmonitor]` - Type annotations for
   [CloudWatchInternetMonitor](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
   service.
@@ -2131,27 +2131,27 @@
   service.
 - `boto3-stubs[iotwireless]` - Type annotations for
   [IoTWireless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
   service.
 - `boto3-stubs[ivs]` - Type annotations for
   [IVS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/) service.
 - `boto3-stubs[ivs-realtime]` - Type annotations for
-  [ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
+  [Ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
   service.
 - `boto3-stubs[ivschat]` - Type annotations for
-  [ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
+  [Ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
   service.
 - `boto3-stubs[kafka]` - Type annotations for
   [Kafka](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
   service.
 - `boto3-stubs[kafkaconnect]` - Type annotations for
   [KafkaConnect](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
   service.
 - `boto3-stubs[kendra]` - Type annotations for
-  [kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
+  [Kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
   service.
 - `boto3-stubs[kendra-ranking]` - Type annotations for
   [KendraRanking](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
   service.
 - `boto3-stubs[keyspaces]` - Type annotations for
   [Keyspaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
   service.
@@ -2271,15 +2271,15 @@
 - `boto3-stubs[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
 - `boto3-stubs[mediapackagev2]` - Type annotations for
-  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  [Mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
   service.
 - `boto3-stubs[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
@@ -2295,15 +2295,15 @@
 - `boto3-stubs[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
   service.
 - `boto3-stubs[mgh]` - Type annotations for
   [MigrationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
   service.
 - `boto3-stubs[mgn]` - Type annotations for
-  [mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
+  [Mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
 - `boto3-stubs[migration-hub-refactor-spaces]` - Type annotations for
   [MigrationHubRefactorSpaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
   service.
 - `boto3-stubs[migrationhub-config]` - Type annotations for
   [MigrationHubConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
   service.
 - `boto3-stubs[migrationhuborchestrator]` - Type annotations for
@@ -2453,15 +2453,15 @@
 - `boto3-stubs[redshift-serverless]` - Type annotations for
   [RedshiftServerless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
   service.
 - `boto3-stubs[rekognition]` - Type annotations for
   [Rekognition](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
   service.
 - `boto3-stubs[repostspace]` - Type annotations for
-  [rePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
+  [RePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
   service.
 - `boto3-stubs[resiliencehub]` - Type annotations for
   [ResilienceHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
   service.
 - `boto3-stubs[resource-explorer-2]` - Type annotations for
   [ResourceExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
   service.
@@ -2571,15 +2571,15 @@
 - `boto3-stubs[sesv2]` - Type annotations for
   [SESV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
   service.
 - `boto3-stubs[shield]` - Type annotations for
   [Shield](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
   service.
 - `boto3-stubs[signer]` - Type annotations for
-  [signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
+  [Signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
   service.
 - `boto3-stubs[simspaceweaver]` - Type annotations for
   [SimSpaceWeaver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
   service.
 - `boto3-stubs[sms]` - Type annotations for
   [SMS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/) service.
 - `boto3-stubs[sms-voice]` - Type annotations for
```

### Comparing `boto3_stubs-1.34.91/boto3_stubs.egg-info/SOURCES.txt` & `boto3_stubs-1.34.92/boto3_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3_stubs-1.34.91/boto3_stubs.egg-info/requires.txt` & `boto3_stubs-1.34.92/boto3_stubs.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -509,16 +509,16 @@
 [bedrock-runtime]
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 
 [billingconductor]
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 
 [boto3]
-boto3==1.34.91
-botocore==1.34.91
+boto3==1.34.92
+botocore==1.34.92
 
 [braket]
 mypy-boto3-braket<1.35.0,>=1.34.0
 
 [budgets]
 mypy-boto3-budgets<1.35.0,>=1.34.0
```

### Comparing `boto3_stubs-1.34.91/setup.py` & `boto3_stubs-1.34.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs",
-    version="1.34.91",
+    version="1.34.92",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.91 generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3 1.34.92 generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -442,15 +442,15 @@
             "mypy-boto3-dynamodb>=1.34.0, <1.35.0",
             "mypy-boto3-ec2>=1.34.0, <1.35.0",
             "mypy-boto3-lambda>=1.34.0, <1.35.0",
             "mypy-boto3-rds>=1.34.0, <1.35.0",
             "mypy-boto3-s3>=1.34.0, <1.35.0",
             "mypy-boto3-sqs>=1.34.0, <1.35.0",
         ],
-        "boto3": ["boto3==1.34.91", "botocore==1.34.91"],
+        "boto3": ["boto3==1.34.92", "botocore==1.34.92"],
         "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.34.0, <1.35.0"],
         "account": ["mypy-boto3-account>=1.34.0, <1.35.0"],
         "acm": ["mypy-boto3-acm>=1.34.0, <1.35.0"],
         "acm-pca": ["mypy-boto3-acm-pca>=1.34.0, <1.35.0"],
         "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.34.0, <1.35.0"],
         "amp": ["mypy-boto3-amp>=1.34.0, <1.35.0"],
         "amplify": ["mypy-boto3-amplify>=1.34.0, <1.35.0"],
```


# Comparing `tmp/boto3_stubs_lite-1.34.91.tar.gz` & `tmp/boto3_stubs_lite-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3_stubs_lite-1.34.91.tar", last modified: Wed Apr 24 19:19:04 2024, max compression
+gzip compressed data, was "boto3_stubs_lite-1.34.92.tar", last modified: Thu Apr 25 19:32:13 2024, max compression
```

## Comparing `boto3_stubs_lite-1.34.91.tar` & `boto3_stubs_lite-1.34.92.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.375917 boto3_stubs_lite-1.34.91/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:17:54.000000 boto3_stubs_lite-1.34.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   141891 2024-04-24 19:19:04.375917 boto3_stubs_lite-1.34.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    71359 2024-04-24 19:17:54.000000 boto3_stubs_lite-1.34.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.275918 boto3_stubs_lite-1.34.91/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/crt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.275918 boto3_stubs_lite-1.34.91/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.275918 boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.275918 boto3_stubs_lite-1.34.91/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:54.000000 boto3_stubs_lite-1.34.91/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.275918 boto3_stubs_lite-1.34.91/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.279918 boto3_stubs_lite-1.34.91/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/s3/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 19:17:52.000000 boto3_stubs_lite-1.34.91/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.279918 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   141891 2024-04-24 19:19:04.000000 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-24 19:19:04.000000 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:04.000000 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:04.000000 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-04-24 19:19:04.000000 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 19:19:04.000000 boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:04.375917 boto3_stubs_lite-1.34.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-24 19:17:53.000000 boto3_stubs_lite-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.675399 boto3_stubs_lite-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:44.000000 boto3_stubs_lite-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   141891 2024-04-25 19:32:13.675399 boto3_stubs_lite-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    71359 2024-04-25 19:31:44.000000 boto3_stubs_lite-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.571398 boto3_stubs_lite-1.34.92/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/crt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.571398 boto3_stubs_lite-1.34.92/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.571398 boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.571398 boto3_stubs_lite-1.34.92/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:44.000000 boto3_stubs_lite-1.34.92/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.575399 boto3_stubs_lite-1.34.92/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.575399 boto3_stubs_lite-1.34.92/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/s3/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 19:31:42.000000 boto3_stubs_lite-1.34.92/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:13.575399 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   141891 2024-04-25 19:32:13.000000 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 19:32:13.000000 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:13.000000 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:13.000000 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-04-25 19:32:13.000000 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:32:13.000000 boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:13.675399 boto3_stubs_lite-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-25 19:31:43.000000 boto3_stubs_lite-1.34.92/setup.py
```

### Comparing `boto3_stubs_lite-1.34.91/LICENSE` & `boto3_stubs_lite-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/PKG-INFO` & `boto3_stubs_lite-1.34.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs-lite
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
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
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -1923,15 +1923,15 @@
 - `boto3-stubs-lite[docdb]` - Type annotations for
   [DocDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
   service.
 - `boto3-stubs-lite[docdb-elastic]` - Type annotations for
   [DocDBElastic](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
   service.
 - `boto3-stubs-lite[drs]` - Type annotations for
-  [drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
+  [Drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
 - `boto3-stubs-lite[ds]` - Type annotations for
   [DirectoryService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
   service.
 - `boto3-stubs-lite[dynamodb]` - Type annotations for
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
   service.
 - `boto3-stubs-lite[dynamodbstreams]` - Type annotations for
@@ -1993,15 +1993,15 @@
 - `boto3-stubs-lite[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
   service.
 - `boto3-stubs-lite[evidently]` - Type annotations for
   [CloudWatchEvidently](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
   service.
 - `boto3-stubs-lite[finspace]` - Type annotations for
-  [finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
+  [Finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
   service.
 - `boto3-stubs-lite[finspace-data]` - Type annotations for
   [FinSpaceData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
   service.
 - `boto3-stubs-lite[firehose]` - Type annotations for
   [Firehose](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
   service.
@@ -2060,24 +2060,24 @@
   service.
 - `boto3-stubs-lite[iam]` - Type annotations for
   [IAM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/) service.
 - `boto3-stubs-lite[identitystore]` - Type annotations for
   [IdentityStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
   service.
 - `boto3-stubs-lite[imagebuilder]` - Type annotations for
-  [imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
+  [Imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
   service.
 - `boto3-stubs-lite[importexport]` - Type annotations for
   [ImportExport](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
   service.
 - `boto3-stubs-lite[inspector]` - Type annotations for
   [Inspector](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
   service.
 - `boto3-stubs-lite[inspector-scan]` - Type annotations for
-  [inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
+  [Inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
   service.
 - `boto3-stubs-lite[inspector2]` - Type annotations for
   [Inspector2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
   service.
 - `boto3-stubs-lite[internetmonitor]` - Type annotations for
   [CloudWatchInternetMonitor](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
   service.
@@ -2127,27 +2127,27 @@
   service.
 - `boto3-stubs-lite[iotwireless]` - Type annotations for
   [IoTWireless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
   service.
 - `boto3-stubs-lite[ivs]` - Type annotations for
   [IVS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/) service.
 - `boto3-stubs-lite[ivs-realtime]` - Type annotations for
-  [ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
+  [Ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
   service.
 - `boto3-stubs-lite[ivschat]` - Type annotations for
-  [ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
+  [Ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
   service.
 - `boto3-stubs-lite[kafka]` - Type annotations for
   [Kafka](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
   service.
 - `boto3-stubs-lite[kafkaconnect]` - Type annotations for
   [KafkaConnect](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
   service.
 - `boto3-stubs-lite[kendra]` - Type annotations for
-  [kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
+  [Kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
   service.
 - `boto3-stubs-lite[kendra-ranking]` - Type annotations for
   [KendraRanking](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
   service.
 - `boto3-stubs-lite[keyspaces]` - Type annotations for
   [Keyspaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
   service.
@@ -2268,15 +2268,15 @@
 - `boto3-stubs-lite[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs-lite[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
 - `boto3-stubs-lite[mediapackagev2]` - Type annotations for
-  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  [Mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
   service.
 - `boto3-stubs-lite[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs-lite[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
@@ -2292,15 +2292,15 @@
 - `boto3-stubs-lite[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
   service.
 - `boto3-stubs-lite[mgh]` - Type annotations for
   [MigrationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
   service.
 - `boto3-stubs-lite[mgn]` - Type annotations for
-  [mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
+  [Mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
 - `boto3-stubs-lite[migration-hub-refactor-spaces]` - Type annotations for
   [MigrationHubRefactorSpaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
   service.
 - `boto3-stubs-lite[migrationhub-config]` - Type annotations for
   [MigrationHubConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
   service.
 - `boto3-stubs-lite[migrationhuborchestrator]` - Type annotations for
@@ -2450,15 +2450,15 @@
 - `boto3-stubs-lite[redshift-serverless]` - Type annotations for
   [RedshiftServerless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
   service.
 - `boto3-stubs-lite[rekognition]` - Type annotations for
   [Rekognition](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
   service.
 - `boto3-stubs-lite[repostspace]` - Type annotations for
-  [rePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
+  [RePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
   service.
 - `boto3-stubs-lite[resiliencehub]` - Type annotations for
   [ResilienceHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
   service.
 - `boto3-stubs-lite[resource-explorer-2]` - Type annotations for
   [ResourceExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
   service.
@@ -2568,15 +2568,15 @@
 - `boto3-stubs-lite[sesv2]` - Type annotations for
   [SESV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
   service.
 - `boto3-stubs-lite[shield]` - Type annotations for
   [Shield](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
   service.
 - `boto3-stubs-lite[signer]` - Type annotations for
-  [signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
+  [Signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
   service.
 - `boto3-stubs-lite[simspaceweaver]` - Type annotations for
   [SimSpaceWeaver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
   service.
 - `boto3-stubs-lite[sms]` - Type annotations for
   [SMS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/) service.
 - `boto3-stubs-lite[sms-voice]` - Type annotations for
```

### Comparing `boto3_stubs_lite-1.34.91/README.md` & `boto3_stubs_lite-1.34.92/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
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
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -727,15 +727,15 @@
 - `boto3-stubs-lite[docdb]` - Type annotations for
   [DocDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
   service.
 - `boto3-stubs-lite[docdb-elastic]` - Type annotations for
   [DocDBElastic](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
   service.
 - `boto3-stubs-lite[drs]` - Type annotations for
-  [drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
+  [Drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
 - `boto3-stubs-lite[ds]` - Type annotations for
   [DirectoryService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
   service.
 - `boto3-stubs-lite[dynamodb]` - Type annotations for
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
   service.
 - `boto3-stubs-lite[dynamodbstreams]` - Type annotations for
@@ -797,15 +797,15 @@
 - `boto3-stubs-lite[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
   service.
 - `boto3-stubs-lite[evidently]` - Type annotations for
   [CloudWatchEvidently](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
   service.
 - `boto3-stubs-lite[finspace]` - Type annotations for
-  [finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
+  [Finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
   service.
 - `boto3-stubs-lite[finspace-data]` - Type annotations for
   [FinSpaceData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
   service.
 - `boto3-stubs-lite[firehose]` - Type annotations for
   [Firehose](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
   service.
@@ -864,24 +864,24 @@
   service.
 - `boto3-stubs-lite[iam]` - Type annotations for
   [IAM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/) service.
 - `boto3-stubs-lite[identitystore]` - Type annotations for
   [IdentityStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
   service.
 - `boto3-stubs-lite[imagebuilder]` - Type annotations for
-  [imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
+  [Imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
   service.
 - `boto3-stubs-lite[importexport]` - Type annotations for
   [ImportExport](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
   service.
 - `boto3-stubs-lite[inspector]` - Type annotations for
   [Inspector](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
   service.
 - `boto3-stubs-lite[inspector-scan]` - Type annotations for
-  [inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
+  [Inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
   service.
 - `boto3-stubs-lite[inspector2]` - Type annotations for
   [Inspector2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
   service.
 - `boto3-stubs-lite[internetmonitor]` - Type annotations for
   [CloudWatchInternetMonitor](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
   service.
@@ -931,27 +931,27 @@
   service.
 - `boto3-stubs-lite[iotwireless]` - Type annotations for
   [IoTWireless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
   service.
 - `boto3-stubs-lite[ivs]` - Type annotations for
   [IVS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/) service.
 - `boto3-stubs-lite[ivs-realtime]` - Type annotations for
-  [ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
+  [Ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
   service.
 - `boto3-stubs-lite[ivschat]` - Type annotations for
-  [ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
+  [Ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
   service.
 - `boto3-stubs-lite[kafka]` - Type annotations for
   [Kafka](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
   service.
 - `boto3-stubs-lite[kafkaconnect]` - Type annotations for
   [KafkaConnect](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
   service.
 - `boto3-stubs-lite[kendra]` - Type annotations for
-  [kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
+  [Kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
   service.
 - `boto3-stubs-lite[kendra-ranking]` - Type annotations for
   [KendraRanking](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
   service.
 - `boto3-stubs-lite[keyspaces]` - Type annotations for
   [Keyspaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
   service.
@@ -1072,15 +1072,15 @@
 - `boto3-stubs-lite[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs-lite[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
 - `boto3-stubs-lite[mediapackagev2]` - Type annotations for
-  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  [Mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
   service.
 - `boto3-stubs-lite[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs-lite[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
@@ -1096,15 +1096,15 @@
 - `boto3-stubs-lite[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
   service.
 - `boto3-stubs-lite[mgh]` - Type annotations for
   [MigrationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
   service.
 - `boto3-stubs-lite[mgn]` - Type annotations for
-  [mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
+  [Mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
 - `boto3-stubs-lite[migration-hub-refactor-spaces]` - Type annotations for
   [MigrationHubRefactorSpaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
   service.
 - `boto3-stubs-lite[migrationhub-config]` - Type annotations for
   [MigrationHubConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
   service.
 - `boto3-stubs-lite[migrationhuborchestrator]` - Type annotations for
@@ -1254,15 +1254,15 @@
 - `boto3-stubs-lite[redshift-serverless]` - Type annotations for
   [RedshiftServerless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
   service.
 - `boto3-stubs-lite[rekognition]` - Type annotations for
   [Rekognition](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
   service.
 - `boto3-stubs-lite[repostspace]` - Type annotations for
-  [rePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
+  [RePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
   service.
 - `boto3-stubs-lite[resiliencehub]` - Type annotations for
   [ResilienceHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
   service.
 - `boto3-stubs-lite[resource-explorer-2]` - Type annotations for
   [ResourceExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
   service.
@@ -1372,15 +1372,15 @@
 - `boto3-stubs-lite[sesv2]` - Type annotations for
   [SESV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
   service.
 - `boto3-stubs-lite[shield]` - Type annotations for
   [Shield](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
   service.
 - `boto3-stubs-lite[signer]` - Type annotations for
-  [signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
+  [Signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
   service.
 - `boto3-stubs-lite[simspaceweaver]` - Type annotations for
   [SimSpaceWeaver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
   service.
 - `boto3-stubs-lite[sms]` - Type annotations for
   [SMS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/) service.
 - `boto3-stubs-lite[sms-voice]` - Type annotations for
```

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/__init__.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/crt.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/docs/utils.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/conditions.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/table.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/transform.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/dynamodb/types.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/exceptions.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/resources/action.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/resources/base.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/resources/collection.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/resources/model.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/resources/params.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/resources/response.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/s3/inject.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/s3/transfer.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/session.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3-stubs/utils.pyi` & `boto3_stubs_lite-1.34.92/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/PKG-INFO` & `boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs-lite
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
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
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -1923,15 +1923,15 @@
 - `boto3-stubs-lite[docdb]` - Type annotations for
   [DocDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
   service.
 - `boto3-stubs-lite[docdb-elastic]` - Type annotations for
   [DocDBElastic](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
   service.
 - `boto3-stubs-lite[drs]` - Type annotations for
-  [drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
+  [Drs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/) service.
 - `boto3-stubs-lite[ds]` - Type annotations for
   [DirectoryService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
   service.
 - `boto3-stubs-lite[dynamodb]` - Type annotations for
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
   service.
 - `boto3-stubs-lite[dynamodbstreams]` - Type annotations for
@@ -1993,15 +1993,15 @@
 - `boto3-stubs-lite[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
   service.
 - `boto3-stubs-lite[evidently]` - Type annotations for
   [CloudWatchEvidently](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_evidently/)
   service.
 - `boto3-stubs-lite[finspace]` - Type annotations for
-  [finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
+  [Finspace](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
   service.
 - `boto3-stubs-lite[finspace-data]` - Type annotations for
   [FinSpaceData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
   service.
 - `boto3-stubs-lite[firehose]` - Type annotations for
   [Firehose](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
   service.
@@ -2060,24 +2060,24 @@
   service.
 - `boto3-stubs-lite[iam]` - Type annotations for
   [IAM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/) service.
 - `boto3-stubs-lite[identitystore]` - Type annotations for
   [IdentityStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
   service.
 - `boto3-stubs-lite[imagebuilder]` - Type annotations for
-  [imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
+  [Imagebuilder](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
   service.
 - `boto3-stubs-lite[importexport]` - Type annotations for
   [ImportExport](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
   service.
 - `boto3-stubs-lite[inspector]` - Type annotations for
   [Inspector](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
   service.
 - `boto3-stubs-lite[inspector-scan]` - Type annotations for
-  [inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
+  [Inspectorscan](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector_scan/)
   service.
 - `boto3-stubs-lite[inspector2]` - Type annotations for
   [Inspector2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
   service.
 - `boto3-stubs-lite[internetmonitor]` - Type annotations for
   [CloudWatchInternetMonitor](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
   service.
@@ -2127,27 +2127,27 @@
   service.
 - `boto3-stubs-lite[iotwireless]` - Type annotations for
   [IoTWireless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/)
   service.
 - `boto3-stubs-lite[ivs]` - Type annotations for
   [IVS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/) service.
 - `boto3-stubs-lite[ivs-realtime]` - Type annotations for
-  [ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
+  [Ivsrealtime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
   service.
 - `boto3-stubs-lite[ivschat]` - Type annotations for
-  [ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
+  [Ivschat](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
   service.
 - `boto3-stubs-lite[kafka]` - Type annotations for
   [Kafka](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
   service.
 - `boto3-stubs-lite[kafkaconnect]` - Type annotations for
   [KafkaConnect](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
   service.
 - `boto3-stubs-lite[kendra]` - Type annotations for
-  [kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
+  [Kendra](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
   service.
 - `boto3-stubs-lite[kendra-ranking]` - Type annotations for
   [KendraRanking](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra_ranking/)
   service.
 - `boto3-stubs-lite[keyspaces]` - Type annotations for
   [Keyspaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
   service.
@@ -2268,15 +2268,15 @@
 - `boto3-stubs-lite[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs-lite[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
 - `boto3-stubs-lite[mediapackagev2]` - Type annotations for
-  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  [Mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
   service.
 - `boto3-stubs-lite[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs-lite[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
@@ -2292,15 +2292,15 @@
 - `boto3-stubs-lite[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
   service.
 - `boto3-stubs-lite[mgh]` - Type annotations for
   [MigrationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
   service.
 - `boto3-stubs-lite[mgn]` - Type annotations for
-  [mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
+  [Mgn](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/) service.
 - `boto3-stubs-lite[migration-hub-refactor-spaces]` - Type annotations for
   [MigrationHubRefactorSpaces](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
   service.
 - `boto3-stubs-lite[migrationhub-config]` - Type annotations for
   [MigrationHubConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
   service.
 - `boto3-stubs-lite[migrationhuborchestrator]` - Type annotations for
@@ -2450,15 +2450,15 @@
 - `boto3-stubs-lite[redshift-serverless]` - Type annotations for
   [RedshiftServerless](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
   service.
 - `boto3-stubs-lite[rekognition]` - Type annotations for
   [Rekognition](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/)
   service.
 - `boto3-stubs-lite[repostspace]` - Type annotations for
-  [rePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
+  [RePostPrivate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_repostspace/)
   service.
 - `boto3-stubs-lite[resiliencehub]` - Type annotations for
   [ResilienceHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
   service.
 - `boto3-stubs-lite[resource-explorer-2]` - Type annotations for
   [ResourceExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
   service.
@@ -2568,15 +2568,15 @@
 - `boto3-stubs-lite[sesv2]` - Type annotations for
   [SESV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
   service.
 - `boto3-stubs-lite[shield]` - Type annotations for
   [Shield](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
   service.
 - `boto3-stubs-lite[signer]` - Type annotations for
-  [signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
+  [Signer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
   service.
 - `boto3-stubs-lite[simspaceweaver]` - Type annotations for
   [SimSpaceWeaver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
   service.
 - `boto3-stubs-lite[sms]` - Type annotations for
   [SMS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/) service.
 - `boto3-stubs-lite[sms-voice]` - Type annotations for
```

### Comparing `boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/SOURCES.txt` & `boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3_stubs_lite-1.34.91/boto3_stubs_lite.egg-info/requires.txt` & `boto3_stubs_lite-1.34.92/boto3_stubs_lite.egg-info/requires.txt`

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

### Comparing `boto3_stubs_lite-1.34.91/setup.py` & `boto3_stubs_lite-1.34.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs-lite",
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


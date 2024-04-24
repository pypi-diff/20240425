# Comparing `tmp/dynamodump-1.9.0.tar.gz` & `tmp/dynamodump-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamodump-1.9.0.tar", last modified: Thu May 11 07:09:54 2023, max compression
+gzip compressed data, was "dynamodump-1.9.1.tar", last modified: Thu Feb  1 11:47:33 2024, max compression
```

## Comparing `dynamodump-1.9.0.tar` & `dynamodump-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.685798 dynamodump-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 07:09:45.000000 dynamodump-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-11 07:09:54.685798 dynamodump-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-11 07:09:45.000000 dynamodump-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.681798 dynamodump-1.9.0/dynamodump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:45.000000 dynamodump-1.9.0/dynamodump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55221 2023-05-11 07:09:45.000000 dynamodump-1.9.0/dynamodump/dynamodump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.685798 dynamodump-1.9.0/dynamodump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 07:09:54.000000 dynamodump-1.9.0/dynamodump.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 07:09:45.000000 dynamodump-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:09:54.685798 dynamodump-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 07:09:45.000000 dynamodump-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:09:54.685798 dynamodump-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-11 07:09:45.000000 dynamodump-1.9.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:47:33.938123 dynamodump-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-01 11:47:25.000000 dynamodump-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-02-01 11:47:33.938123 dynamodump-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-02-01 11:47:25.000000 dynamodump-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:47:33.938123 dynamodump-1.9.1/dynamodump/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 11:47:25.000000 dynamodump-1.9.1/dynamodump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55221 2024-02-01 11:47:25.000000 dynamodump-1.9.1/dynamodump/dynamodump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:47:33.938123 dynamodump-1.9.1/dynamodump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-02-01 11:47:33.000000 dynamodump-1.9.1/dynamodump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-01 11:47:33.000000 dynamodump-1.9.1/dynamodump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 11:47:33.000000 dynamodump-1.9.1/dynamodump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-01 11:47:33.000000 dynamodump-1.9.1/dynamodump.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-01 11:47:33.000000 dynamodump-1.9.1/dynamodump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-01 11:47:33.000000 dynamodump-1.9.1/dynamodump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-01 11:47:25.000000 dynamodump-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 11:47:33.938123 dynamodump-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-01 11:47:25.000000 dynamodump-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 11:47:33.938123 dynamodump-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-01 11:47:25.000000 dynamodump-1.9.1/tests/test.py
```

### Comparing `dynamodump-1.9.0/LICENSE` & `dynamodump-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamodump-1.9.0/PKG-INFO` & `dynamodump-1.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dynamodump
-Version: 1.9.0
-Summary: Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)
-Home-page: https://github.com/bchew/dynamodump
-Author: Benny Chew
-Author-email: noreply@bennychew.com
-Project-URL: Releases, https://github.com/bchew/dynamodump/releases
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dynamodump
 
 ![Build Status](https://github.com/bchew/dynamodump/actions/workflows/build.yml/badge.svg)
 ![CodeQL Status](https://github.com/bchew/dynamodump/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Docker Status](https://github.com/bchew/dynamodump/actions/workflows/docker.yml/badge.svg)](https://hub.docker.com/r/bchew/dynamodump)
 ![Linting Status](https://github.com/bchew/dynamodump/actions/workflows/linting.yml/badge.svg)
 ![Test Status](https://github.com/bchew/dynamodump/actions/workflows/test.yml/badge.svg)
@@ -113,14 +99,19 @@
 dynamodump container images are also published to Amazon ECR Public and GitHub Packages:
 
 ```
 public.ecr.aws/bchew/dynamodump
 ghcr.io/bchew/dynamodump
 ```
 
+Links to the registries specified:
+- [Docker Hub](https://hub.docker.com/r/bchew/dynamodump)
+- [Amazon ECR Public Gallery](https://gallery.ecr.aws/bchew/dynamodump)
+- [GitHub Packages](https://github.com/bchew/dynamodump/pkgs/container/dynamodump)
+
 ## AWS example
 
 Single table backup/restore:
 
 ```
 dynamodump -m backup -r us-west-1 -s testTable
```

### Comparing `dynamodump-1.9.0/README.md` & `dynamodump-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: dynamodump
+Version: 1.9.1
+Summary: Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)
+Home-page: https://github.com/bchew/dynamodump
+Author: Benny Chew
+Author-email: noreply@bennychew.com
+Project-URL: Releases, https://github.com/bchew/dynamodump/releases
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3==1.34.12
+Requires-Dist: six==1.16.0
+
 # dynamodump
 
 ![Build Status](https://github.com/bchew/dynamodump/actions/workflows/build.yml/badge.svg)
 ![CodeQL Status](https://github.com/bchew/dynamodump/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Docker Status](https://github.com/bchew/dynamodump/actions/workflows/docker.yml/badge.svg)](https://hub.docker.com/r/bchew/dynamodump)
 ![Linting Status](https://github.com/bchew/dynamodump/actions/workflows/linting.yml/badge.svg)
 ![Test Status](https://github.com/bchew/dynamodump/actions/workflows/test.yml/badge.svg)
@@ -99,14 +115,19 @@
 dynamodump container images are also published to Amazon ECR Public and GitHub Packages:
 
 ```
 public.ecr.aws/bchew/dynamodump
 ghcr.io/bchew/dynamodump
 ```
 
+Links to the registries specified:
+- [Docker Hub](https://hub.docker.com/r/bchew/dynamodump)
+- [Amazon ECR Public Gallery](https://gallery.ecr.aws/bchew/dynamodump)
+- [GitHub Packages](https://github.com/bchew/dynamodump/pkgs/container/dynamodump)
+
 ## AWS example
 
 Single table backup/restore:
 
 ```
 dynamodump -m backup -r us-west-1 -s testTable
```

### Comparing `dynamodump-1.9.0/dynamodump/dynamodump.py` & `dynamodump-1.9.1/dynamodump/dynamodump.py`

 * *Files identical despite different names*

### Comparing `dynamodump-1.9.0/dynamodump.egg-info/PKG-INFO` & `dynamodump-1.9.1/dynamodump.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: dynamodump
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)
 Home-page: https://github.com/bchew/dynamodump
 Author: Benny Chew
 Author-email: noreply@bennychew.com
 Project-URL: Releases, https://github.com/bchew/dynamodump/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3==1.34.12
+Requires-Dist: six==1.16.0
 
 # dynamodump
 
 ![Build Status](https://github.com/bchew/dynamodump/actions/workflows/build.yml/badge.svg)
 ![CodeQL Status](https://github.com/bchew/dynamodump/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Docker Status](https://github.com/bchew/dynamodump/actions/workflows/docker.yml/badge.svg)](https://hub.docker.com/r/bchew/dynamodump)
 ![Linting Status](https://github.com/bchew/dynamodump/actions/workflows/linting.yml/badge.svg)
@@ -113,14 +115,19 @@
 dynamodump container images are also published to Amazon ECR Public and GitHub Packages:
 
 ```
 public.ecr.aws/bchew/dynamodump
 ghcr.io/bchew/dynamodump
 ```
 
+Links to the registries specified:
+- [Docker Hub](https://hub.docker.com/r/bchew/dynamodump)
+- [Amazon ECR Public Gallery](https://gallery.ecr.aws/bchew/dynamodump)
+- [GitHub Packages](https://github.com/bchew/dynamodump/pkgs/container/dynamodump)
+
 ## AWS example
 
 Single table backup/restore:
 
 ```
 dynamodump -m backup -r us-west-1 -s testTable
```

### Comparing `dynamodump-1.9.0/setup.py` & `dynamodump-1.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dynamodump",
-    version="1.9.0",
+    version="1.9.1",
     author="Benny Chew",
     author_email="noreply@bennychew.com",
     description="Simple backup and restore for Amazon DynamoDB using AWS SDK for Python (boto3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bchew/dynamodump",
     project_urls={
         "Releases": "https://github.com/bchew/dynamodump/releases",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     packages=["dynamodump"],
-    python_requires=">=3.7",
-    install_requires=["boto3==1.26.132", "six==1.16.0"],
+    python_requires=">=3.8",
+    install_requires=["boto3==1.34.12", "six==1.16.0"],
     entry_points={
         "console_scripts": ["dynamodump=dynamodump.dynamodump:main"],
     },
 )
```

### Comparing `dynamodump-1.9.0/tests/test.py` & `dynamodump-1.9.1/tests/test.py`

 * *Files identical despite different names*


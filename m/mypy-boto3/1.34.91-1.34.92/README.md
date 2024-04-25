# Comparing `tmp/mypy_boto3-1.34.91.tar.gz` & `tmp/mypy_boto3-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3-1.34.91.tar", last modified: Wed Apr 24 19:19:02 2024, max compression
+gzip compressed data, was "mypy_boto3-1.34.92.tar", last modified: Thu Apr 25 19:32:11 2024, max compression
```

## Comparing `mypy_boto3-1.34.91.tar` & `mypy_boto3-1.34.92.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:02.407945 mypy_boto3-1.34.91/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-24 19:19:02.407945 mypy_boto3-1.34.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:02.407945 mypy_boto3-1.34.91/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 19:17:43.000000 mypy_boto3-1.34.91/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-24 19:17:43.000000 mypy_boto3-1.34.91/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   116366 2024-04-24 19:17:43.000000 mypy_boto3-1.34.91/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:02.407945 mypy_boto3-1.34.91/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-24 19:19:02.000000 mypy_boto3-1.34.91/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 19:19:02.000000 mypy_boto3-1.34.91/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:02.000000 mypy_boto3-1.34.91/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:02.000000 mypy_boto3-1.34.91/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 19:19:02.000000 mypy_boto3-1.34.91/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 19:19:02.000000 mypy_boto3-1.34.91/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:02.407945 mypy_boto3-1.34.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-24 19:17:41.000000 mypy_boto3-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:11.655383 mypy_boto3-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-25 19:32:11.655383 mypy_boto3-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:11.655383 mypy_boto3-1.34.92/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 19:31:33.000000 mypy_boto3-1.34.92/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-25 19:31:33.000000 mypy_boto3-1.34.92/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   116366 2024-04-25 19:31:33.000000 mypy_boto3-1.34.92/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:11.655383 mypy_boto3-1.34.92/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-25 19:32:11.000000 mypy_boto3-1.34.92/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-25 19:32:11.000000 mypy_boto3-1.34.92/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:11.000000 mypy_boto3-1.34.92/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:11.000000 mypy_boto3-1.34.92/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 19:32:11.000000 mypy_boto3-1.34.92/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 19:32:11.000000 mypy_boto3-1.34.92/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:11.655383 mypy_boto3-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-25 19:31:31.000000 mypy_boto3-1.34.92/setup.py
```

### Comparing `mypy_boto3-1.34.91/LICENSE` & `mypy_boto3-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.91/PKG-INFO` & `mypy_boto3-1.34.92/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.91
-Summary: Type annotations for boto3 1.34.91 master module generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3 1.34.92 master module generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -40,20 +40,20 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/1.34.91/index.html)
+[boto3 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/1.34.92/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy_boto3-1.34.91/README.md` & `mypy_boto3-1.34.92/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/1.34.91/index.html)
+[boto3 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/1.34.92/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy_boto3-1.34.91/mypy_boto3/boto3_init_stub.py` & `mypy_boto3-1.34.92/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.91/mypy_boto3/boto3_session_stub.py` & `mypy_boto3-1.34.92/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.91/mypy_boto3/literals.py` & `mypy_boto3-1.34.92/mypy_boto3/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.91/mypy_boto3/main.py` & `mypy_boto3-1.34.92/mypy_boto3/main.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3-1.34.91/mypy_boto3/submodules.py` & `mypy_boto3-1.34.92/mypy_boto3/submodules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1156,15 +1156,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_drs",
         import_name="drs",
         boto3_name="drs",
-        class_name="drs",
+        class_name="Drs",
         pypi_name="mypy-boto3-drs",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_ds",
@@ -1416,15 +1416,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_finspace",
         import_name="finspace",
         boto3_name="finspace",
-        class_name="finspace",
+        class_name="Finspace",
         pypi_name="mypy-boto3-finspace",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_finspace_data",
@@ -1656,15 +1656,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_imagebuilder",
         import_name="imagebuilder",
         boto3_name="imagebuilder",
-        class_name="imagebuilder",
+        class_name="Imagebuilder",
         pypi_name="mypy-boto3-imagebuilder",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
         module_name="mypy_boto3_importexport",
@@ -1686,15 +1686,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_inspector_scan",
         import_name="inspector_scan",
         boto3_name="inspector-scan",
-        class_name="inspectorscan",
+        class_name="Inspectorscan",
         pypi_name="mypy-boto3-inspector-scan",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
         module_name="mypy_boto3_inspector2",
@@ -1886,25 +1886,25 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_ivs_realtime",
         import_name="ivs_realtime",
         boto3_name="ivs-realtime",
-        class_name="ivsrealtime",
+        class_name="Ivsrealtime",
         pypi_name="mypy-boto3-ivs-realtime",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
         module_name="mypy_boto3_ivschat",
         import_name="ivschat",
         boto3_name="ivschat",
-        class_name="ivschat",
+        class_name="Ivschat",
         pypi_name="mypy-boto3-ivschat",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
         module_name="mypy_boto3_kafka",
@@ -1926,15 +1926,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_kendra",
         import_name="kendra",
         boto3_name="kendra",
-        class_name="kendra",
+        class_name="Kendra",
         pypi_name="mypy-boto3-kendra",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
         module_name="mypy_boto3_kendra_ranking",
@@ -2356,15 +2356,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_mediapackagev2",
         import_name="mediapackagev2",
         boto3_name="mediapackagev2",
-        class_name="mediapackagev2",
+        class_name="Mediapackagev2",
         pypi_name="mypy-boto3-mediapackagev2",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_mediastore",
@@ -2436,15 +2436,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_mgn",
         import_name="mgn",
         boto3_name="mgn",
-        class_name="mgn",
+        class_name="Mgn",
         pypi_name="mypy-boto3-mgn",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_migration_hub_refactor_spaces",
@@ -2986,15 +2986,15 @@
         has_waiter=True,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_repostspace",
         import_name="repostspace",
         boto3_name="repostspace",
-        class_name="rePostPrivate",
+        class_name="RePostPrivate",
         pypi_name="mypy-boto3-repostspace",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_resiliencehub",
@@ -3386,15 +3386,15 @@
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_signer",
         import_name="signer",
         boto3_name="signer",
-        class_name="signer",
+        class_name="Signer",
         pypi_name="mypy-boto3-signer",
         has_resource=False,
         has_waiter=True,
         has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_simspaceweaver",
```

### Comparing `mypy_boto3-1.34.91/mypy_boto3.egg-info/PKG-INFO` & `mypy_boto3-1.34.92/mypy_boto3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.91
-Summary: Type annotations for boto3 1.34.91 master module generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3 1.34.92 master module generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -40,20 +40,20 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/1.34.91/index.html)
+[boto3 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/1.34.92/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy_boto3-1.34.91/setup.py` & `mypy_boto3-1.34.92/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.34.91",
+    version="1.34.92",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.91 master module generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3 1.34.92 master module generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


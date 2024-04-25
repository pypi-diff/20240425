# Comparing `tmp/mypy-boto3-ivs-realtime-1.34.62.tar.gz` & `tmp/mypy_boto3_ivs_realtime-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-realtime-1.34.62.tar", last modified: Wed Mar 13 19:32:08 2024, max compression
+gzip compressed data, was "mypy_boto3_ivs_realtime-1.34.92.tar", last modified: Thu Apr 25 19:32:15 2024, max compression
```

## Comparing `mypy-boto3-ivs-realtime-1.34.62.tar` & `mypy_boto3_ivs_realtime-1.34.92.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:32:08.960831 mypy-boto3-ivs-realtime-1.34.62/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-03-13 19:32:08.960831 mypy-boto3-ivs-realtime-1.34.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:32:08.956831 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19410 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19407 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21819 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21819 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:32:08.956831 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-03-13 19:32:08.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-13 19:32:08.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:32:08.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:32:08.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-13 19:32:08.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-13 19:32:08.000000 mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 19:32:08.960831 mypy-boto3-ivs-realtime-1.34.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-13 19:31:46.000000 mypy-boto3-ivs-realtime-1.34.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.375413 mypy_boto3_ivs_realtime-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-25 19:32:15.375413 mypy_boto3_ivs_realtime-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.375413 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19418 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19415 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-25 19:31:51.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2024-04-25 19:31:51.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.375413 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-25 19:32:15.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 19:32:15.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:15.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:15.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:15.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 19:32:15.000000 mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:15.375413 mypy_boto3_ivs_realtime-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-25 19:31:50.000000 mypy_boto3_ivs_realtime-1.34.92/setup.py
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/LICENSE` & `mypy_boto3_ivs_realtime-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.34.62/PKG-INFO` & `mypy_boto3_ivs_realtime-1.34.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs-realtime
-Version: 1.34.62
-Summary: Type annotations for boto3.ivsrealtime 1.34.62 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3.Ivsrealtime 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs-realtime)](https://pepy.tech/project/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.34.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.Ivsrealtime 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -96,21 +96,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `ivsrealtime`.
+Click `Modify` and select `boto3 common` and `Ivsrealtime`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `ivsrealtime` service.
+Install `boto3-stubs` for `Ivsrealtime` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[ivs-realtime]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -256,34 +256,34 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`ivsrealtimeClient` provides annotations for `boto3.client("ivs-realtime")`.
+`IvsrealtimeClient` provides annotations for `boto3.client("ivs-realtime")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_ivs_realtime import ivsrealtimeClient
+from mypy_boto3_ivs_realtime import IvsrealtimeClient
 
-client: ivsrealtimeClient = Session().client("ivs-realtime")
+client: IvsrealtimeClient = Session().client("ivs-realtime")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_ivs_realtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
-Full list of `ivsrealtime` Literals can be found in
+Full list of `Ivsrealtime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/literals/).
 
 ```python
 from mypy_boto3_ivs_realtime.literals import CompositionStateType
 
 
 def check_value(value: CompositionStateType) -> bool: ...
@@ -292,15 +292,15 @@
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
-Full list of `ivsrealtime` TypeDefs can be found in
+Full list of `Ivsrealtime` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/type_defs/).
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import ChannelDestinationConfigurationTypeDef
 
 
 def get_value() -> ChannelDestinationConfigurationTypeDef:
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/README.md` & `mypy_boto3_ivs_realtime-1.34.92/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs-realtime)](https://pepy.tech/project/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.34.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.Ivsrealtime 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -63,21 +63,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `ivsrealtime`.
+Click `Modify` and select `boto3 common` and `Ivsrealtime`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `ivsrealtime` service.
+Install `boto3-stubs` for `Ivsrealtime` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[ivs-realtime]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -223,34 +223,34 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`ivsrealtimeClient` provides annotations for `boto3.client("ivs-realtime")`.
+`IvsrealtimeClient` provides annotations for `boto3.client("ivs-realtime")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_ivs_realtime import ivsrealtimeClient
+from mypy_boto3_ivs_realtime import IvsrealtimeClient
 
-client: ivsrealtimeClient = Session().client("ivs-realtime")
+client: IvsrealtimeClient = Session().client("ivs-realtime")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_ivs_realtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
-Full list of `ivsrealtime` Literals can be found in
+Full list of `Ivsrealtime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/literals/).
 
 ```python
 from mypy_boto3_ivs_realtime.literals import CompositionStateType
 
 
 def check_value(value: CompositionStateType) -> bool: ...
@@ -259,15 +259,15 @@
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
-Full list of `ivsrealtime` TypeDefs can be found in
+Full list of `Ivsrealtime` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/type_defs/).
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import ChannelDestinationConfigurationTypeDef
 
 
 def get_value() -> ChannelDestinationConfigurationTypeDef:
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/__main__.py` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivsrealtime 1.34.62\n"
-        "Version:         1.34.62\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.Ivsrealtime 1.34.92\n"
+        "Version:         1.34.92\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime//\n"
-        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.62")
+    print("1.34.92")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/client.py` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/)
 
 Usage::
 
     ```python
     from boto3.session import Session
-    from mypy_boto3_ivs_realtime.client import ivsrealtimeClient
+    from mypy_boto3_ivs_realtime.client import IvsrealtimeClient
 
     session = Session()
-    client: ivsrealtimeClient = session.client("ivs-realtime")
+    client: IvsrealtimeClient = session.client("ivs-realtime")
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ParticipantStateType, ParticipantTokenCapabilityType
 from .type_defs import (
     CreateEncoderConfigurationResponseTypeDef,
     CreateParticipantTokenResponseTypeDef,
     CreateStageResponseTypeDef,
     CreateStorageConfigurationResponseTypeDef,
-    DestinationConfigurationTypeDef,
+    DestinationConfigurationUnionTypeDef,
     GetCompositionResponseTypeDef,
     GetEncoderConfigurationResponseTypeDef,
     GetParticipantResponseTypeDef,
     GetStageResponseTypeDef,
     GetStageSessionResponseTypeDef,
     GetStorageConfigurationResponseTypeDef,
     LayoutConfigurationTypeDef,
@@ -43,15 +43,15 @@
     ParticipantTokenConfigurationTypeDef,
     S3StorageConfigurationTypeDef,
     StartCompositionResponseTypeDef,
     UpdateStageResponseTypeDef,
     VideoTypeDef,
 )
 
-__all__ = ("ivsrealtimeClient",)
+__all__ = ("IvsrealtimeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -65,54 +65,54 @@
     InternalServerException: Type[BotocoreClientError]
     PendingVerification: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
-class ivsrealtimeClient(BaseClient):
+class IvsrealtimeClient(BaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        ivsrealtimeClient exceptions.
+        IvsrealtimeClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#exceptions)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#can_paginate)
         """
 
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#close)
         """
 
     def create_encoder_configuration(
         self, *, name: str = ..., tags: Mapping[str, str] = ..., video: VideoTypeDef = ...
     ) -> CreateEncoderConfigurationResponseTypeDef:
         """
         Creates an EncoderConfiguration object.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_encoder_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_encoder_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_encoder_configuration)
         """
 
     def create_participant_token(
         self,
         *,
         stageArn: str,
@@ -120,139 +120,139 @@
         capabilities: Sequence[ParticipantTokenCapabilityType] = ...,
         duration: int = ...,
         userId: str = ...,
     ) -> CreateParticipantTokenResponseTypeDef:
         """
         Creates an additional token for a specified stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_participant_token)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_participant_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_participant_token)
         """
 
     def create_stage(
         self,
         *,
         name: str = ...,
         participantTokenConfigurations: Sequence[ParticipantTokenConfigurationTypeDef] = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateStageResponseTypeDef:
         """
         Creates a new stage (and optionally participant tokens).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_stage)
         """
 
     def create_storage_configuration(
         self, *, s3: S3StorageConfigurationTypeDef, name: str = ..., tags: Mapping[str, str] = ...
     ) -> CreateStorageConfigurationResponseTypeDef:
         """
         Creates a new storage configuration, used to enable recording to Amazon S3.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_storage_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_storage_configuration)
         """
 
     def delete_encoder_configuration(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes an EncoderConfiguration resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_encoder_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.delete_encoder_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#delete_encoder_configuration)
         """
 
     def delete_stage(self, *, arn: str) -> Dict[str, Any]:
         """
         Shuts down and deletes the specified stage (disconnecting all participants).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.delete_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#delete_stage)
         """
 
     def delete_storage_configuration(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes the storage configuration for the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_storage_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.delete_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#delete_storage_configuration)
         """
 
     def disconnect_participant(
         self, *, participantId: str, stageArn: str, reason: str = ...
     ) -> Dict[str, Any]:
         """
         Disconnects a specified participant and revokes the participant permanently
         from a specified
         stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.disconnect_participant)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.disconnect_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#disconnect_participant)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#generate_presigned_url)
         """
 
     def get_composition(self, *, arn: str) -> GetCompositionResponseTypeDef:
         """
         Get information about the specified Composition resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_composition)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_composition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_composition)
         """
 
     def get_encoder_configuration(self, *, arn: str) -> GetEncoderConfigurationResponseTypeDef:
         """
         Gets information about the specified EncoderConfiguration resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_encoder_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_encoder_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_encoder_configuration)
         """
 
     def get_participant(
         self, *, participantId: str, sessionId: str, stageArn: str
     ) -> GetParticipantResponseTypeDef:
         """
         Gets information about the specified participant token.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_participant)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_participant)
         """
 
     def get_stage(self, *, arn: str) -> GetStageResponseTypeDef:
         """
         Gets information for the specified stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage)
         """
 
     def get_stage_session(self, *, sessionId: str, stageArn: str) -> GetStageSessionResponseTypeDef:
         """
         Gets information for the specified stage session.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage_session)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_stage_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage_session)
         """
 
     def get_storage_configuration(self, *, arn: str) -> GetStorageConfigurationResponseTypeDef:
         """
         Gets the storage configuration for the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_storage_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_storage_configuration)
         """
 
     def list_compositions(
         self,
         *,
         filterByEncoderConfigurationArn: str = ...,
@@ -261,27 +261,27 @@
         nextToken: str = ...,
     ) -> ListCompositionsResponseTypeDef:
         """
         Gets summary information about all Compositions in your account, in the AWS
         region where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_compositions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_compositions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_compositions)
         """
 
     def list_encoder_configurations(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListEncoderConfigurationsResponseTypeDef:
         """
         Gets summary information about all EncoderConfigurations in your account, in
         the AWS region where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_encoder_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_encoder_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_encoder_configurations)
         """
 
     def list_participant_events(
         self,
         *,
         participantId: str,
@@ -290,15 +290,15 @@
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> ListParticipantEventsResponseTypeDef:
         """
         Lists events for a specified participant that occurred during a specified stage
         session.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_participant_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participant_events)
         """
 
     def list_participants(
         self,
         *,
         sessionId: str,
@@ -308,101 +308,101 @@
         filterByUserId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> ListParticipantsResponseTypeDef:
         """
         Lists all participants in a specified stage session.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_participants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participants)
         """
 
     def list_stage_sessions(
         self, *, stageArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListStageSessionsResponseTypeDef:
         """
         Gets all sessions for a specified stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stage_sessions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_stage_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_stage_sessions)
         """
 
     def list_stages(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStagesResponseTypeDef:
         """
         Gets summary information about all stages in your account, in the AWS region
         where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stages)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_stages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_stages)
         """
 
     def list_storage_configurations(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStorageConfigurationsResponseTypeDef:
         """
         Gets summary information about all storage configurations in your account, in
         the AWS region where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_storage_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_storage_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_storage_configurations)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Gets information about AWS tags for the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_tags_for_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_tags_for_resource)
         """
 
     def start_composition(
         self,
         *,
-        destinations: Sequence[DestinationConfigurationTypeDef],
+        destinations: Sequence[DestinationConfigurationUnionTypeDef],
         stageArn: str,
         idempotencyToken: str = ...,
         layout: LayoutConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
     ) -> StartCompositionResponseTypeDef:
         """
         Starts a Composition from a stage based on the configuration provided in the
         request.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.start_composition)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.start_composition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#start_composition)
         """
 
     def stop_composition(self, *, arn: str) -> Dict[str, Any]:
         """
         Stops and deletes a Composition resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.stop_composition)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.stop_composition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#stop_composition)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or updates tags for the AWS resource with the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.tag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the resource with the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.untag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#untag_resource)
         """
 
     def update_stage(self, *, arn: str, name: str = ...) -> UpdateStageResponseTypeDef:
         """
-        Updates a stage’s configuration.
+        Updates a stage's configuration.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.update_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.update_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#update_stage)
         """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/client.pyi` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/)
 
 Usage::
 
     ```python
     from boto3.session import Session
-    from mypy_boto3_ivs_realtime.client import ivsrealtimeClient
+    from mypy_boto3_ivs_realtime.client import IvsrealtimeClient
 
     session = Session()
-    client: ivsrealtimeClient = session.client("ivs-realtime")
+    client: IvsrealtimeClient = session.client("ivs-realtime")
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ParticipantStateType, ParticipantTokenCapabilityType
 from .type_defs import (
     CreateEncoderConfigurationResponseTypeDef,
     CreateParticipantTokenResponseTypeDef,
     CreateStageResponseTypeDef,
     CreateStorageConfigurationResponseTypeDef,
-    DestinationConfigurationTypeDef,
+    DestinationConfigurationUnionTypeDef,
     GetCompositionResponseTypeDef,
     GetEncoderConfigurationResponseTypeDef,
     GetParticipantResponseTypeDef,
     GetStageResponseTypeDef,
     GetStageSessionResponseTypeDef,
     GetStorageConfigurationResponseTypeDef,
     LayoutConfigurationTypeDef,
@@ -43,15 +43,15 @@
     ParticipantTokenConfigurationTypeDef,
     S3StorageConfigurationTypeDef,
     StartCompositionResponseTypeDef,
     UpdateStageResponseTypeDef,
     VideoTypeDef,
 )
 
-__all__ = ("ivsrealtimeClient",)
+__all__ = ("IvsrealtimeClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
@@ -62,54 +62,54 @@
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     PendingVerification: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-class ivsrealtimeClient(BaseClient):
+class IvsrealtimeClient(BaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        ivsrealtimeClient exceptions.
+        IvsrealtimeClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#exceptions)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#can_paginate)
         """
 
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#close)
         """
 
     def create_encoder_configuration(
         self, *, name: str = ..., tags: Mapping[str, str] = ..., video: VideoTypeDef = ...
     ) -> CreateEncoderConfigurationResponseTypeDef:
         """
         Creates an EncoderConfiguration object.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_encoder_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_encoder_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_encoder_configuration)
         """
 
     def create_participant_token(
         self,
         *,
         stageArn: str,
@@ -117,139 +117,139 @@
         capabilities: Sequence[ParticipantTokenCapabilityType] = ...,
         duration: int = ...,
         userId: str = ...,
     ) -> CreateParticipantTokenResponseTypeDef:
         """
         Creates an additional token for a specified stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_participant_token)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_participant_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_participant_token)
         """
 
     def create_stage(
         self,
         *,
         name: str = ...,
         participantTokenConfigurations: Sequence[ParticipantTokenConfigurationTypeDef] = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateStageResponseTypeDef:
         """
         Creates a new stage (and optionally participant tokens).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_stage)
         """
 
     def create_storage_configuration(
         self, *, s3: S3StorageConfigurationTypeDef, name: str = ..., tags: Mapping[str, str] = ...
     ) -> CreateStorageConfigurationResponseTypeDef:
         """
         Creates a new storage configuration, used to enable recording to Amazon S3.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_storage_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.create_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#create_storage_configuration)
         """
 
     def delete_encoder_configuration(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes an EncoderConfiguration resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_encoder_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.delete_encoder_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#delete_encoder_configuration)
         """
 
     def delete_stage(self, *, arn: str) -> Dict[str, Any]:
         """
         Shuts down and deletes the specified stage (disconnecting all participants).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.delete_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#delete_stage)
         """
 
     def delete_storage_configuration(self, *, arn: str) -> Dict[str, Any]:
         """
         Deletes the storage configuration for the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_storage_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.delete_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#delete_storage_configuration)
         """
 
     def disconnect_participant(
         self, *, participantId: str, stageArn: str, reason: str = ...
     ) -> Dict[str, Any]:
         """
         Disconnects a specified participant and revokes the participant permanently
         from a specified
         stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.disconnect_participant)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.disconnect_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#disconnect_participant)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#generate_presigned_url)
         """
 
     def get_composition(self, *, arn: str) -> GetCompositionResponseTypeDef:
         """
         Get information about the specified Composition resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_composition)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_composition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_composition)
         """
 
     def get_encoder_configuration(self, *, arn: str) -> GetEncoderConfigurationResponseTypeDef:
         """
         Gets information about the specified EncoderConfiguration resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_encoder_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_encoder_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_encoder_configuration)
         """
 
     def get_participant(
         self, *, participantId: str, sessionId: str, stageArn: str
     ) -> GetParticipantResponseTypeDef:
         """
         Gets information about the specified participant token.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_participant)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_participant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_participant)
         """
 
     def get_stage(self, *, arn: str) -> GetStageResponseTypeDef:
         """
         Gets information for the specified stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage)
         """
 
     def get_stage_session(self, *, sessionId: str, stageArn: str) -> GetStageSessionResponseTypeDef:
         """
         Gets information for the specified stage session.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage_session)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_stage_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage_session)
         """
 
     def get_storage_configuration(self, *, arn: str) -> GetStorageConfigurationResponseTypeDef:
         """
         Gets the storage configuration for the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_storage_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.get_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_storage_configuration)
         """
 
     def list_compositions(
         self,
         *,
         filterByEncoderConfigurationArn: str = ...,
@@ -258,27 +258,27 @@
         nextToken: str = ...,
     ) -> ListCompositionsResponseTypeDef:
         """
         Gets summary information about all Compositions in your account, in the AWS
         region where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_compositions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_compositions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_compositions)
         """
 
     def list_encoder_configurations(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListEncoderConfigurationsResponseTypeDef:
         """
         Gets summary information about all EncoderConfigurations in your account, in
         the AWS region where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_encoder_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_encoder_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_encoder_configurations)
         """
 
     def list_participant_events(
         self,
         *,
         participantId: str,
@@ -287,15 +287,15 @@
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> ListParticipantEventsResponseTypeDef:
         """
         Lists events for a specified participant that occurred during a specified stage
         session.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_participant_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participant_events)
         """
 
     def list_participants(
         self,
         *,
         sessionId: str,
@@ -305,101 +305,101 @@
         filterByUserId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> ListParticipantsResponseTypeDef:
         """
         Lists all participants in a specified stage session.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_participants)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participants)
         """
 
     def list_stage_sessions(
         self, *, stageArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListStageSessionsResponseTypeDef:
         """
         Gets all sessions for a specified stage.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stage_sessions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_stage_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_stage_sessions)
         """
 
     def list_stages(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStagesResponseTypeDef:
         """
         Gets summary information about all stages in your account, in the AWS region
         where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stages)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_stages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_stages)
         """
 
     def list_storage_configurations(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStorageConfigurationsResponseTypeDef:
         """
         Gets summary information about all storage configurations in your account, in
         the AWS region where the API request is
         processed.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_storage_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_storage_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_storage_configurations)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Gets information about AWS tags for the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_tags_for_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_tags_for_resource)
         """
 
     def start_composition(
         self,
         *,
-        destinations: Sequence[DestinationConfigurationTypeDef],
+        destinations: Sequence[DestinationConfigurationUnionTypeDef],
         stageArn: str,
         idempotencyToken: str = ...,
         layout: LayoutConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
     ) -> StartCompositionResponseTypeDef:
         """
         Starts a Composition from a stage based on the configuration provided in the
         request.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.start_composition)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.start_composition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#start_composition)
         """
 
     def stop_composition(self, *, arn: str) -> Dict[str, Any]:
         """
         Stops and deletes a Composition resource.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.stop_composition)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.stop_composition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#stop_composition)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds or updates tags for the AWS resource with the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.tag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the resource with the specified ARN.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.untag_resource)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#untag_resource)
         """
 
     def update_stage(self, *, arn: str, name: str = ...) -> UpdateStageResponseTypeDef:
         """
-        Updates a stage’s configuration.
+        Updates a stage's configuration.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.update_stage)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client.update_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#update_stage)
         """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/literals.py` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "ParticipantStateType",
     "ParticipantTokenCapabilityType",
     "PipBehaviorType",
     "PipPositionType",
     "RecordingConfigurationFormatType",
     "VideoAspectRatioType",
     "VideoFillModeType",
-    "ivsrealtimeServiceName",
+    "IvsrealtimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 CompositionStateType = Literal["ACTIVE", "FAILED", "STARTING", "STOPPED", "STOPPING"]
 DestinationStateType = Literal[
@@ -56,15 +56,15 @@
 ParticipantStateType = Literal["CONNECTED", "DISCONNECTED"]
 ParticipantTokenCapabilityType = Literal["PUBLISH", "SUBSCRIBE"]
 PipBehaviorType = Literal["DYNAMIC", "STATIC"]
 PipPositionType = Literal["BOTTOM_LEFT", "BOTTOM_RIGHT", "TOP_LEFT", "TOP_RIGHT"]
 RecordingConfigurationFormatType = Literal["HLS"]
 VideoAspectRatioType = Literal["AUTO", "PORTRAIT", "SQUARE", "VIDEO"]
 VideoFillModeType = Literal["CONTAIN", "COVER", "FILL"]
-ivsrealtimeServiceName = Literal["ivs-realtime"]
+IvsrealtimeServiceName = Literal["ivs-realtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
@@ -128,14 +128,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -148,24 +149,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -226,15 +229,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -363,14 +365,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -414,14 +417,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/literals.pyi` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "ParticipantStateType",
     "ParticipantTokenCapabilityType",
     "PipBehaviorType",
     "PipPositionType",
     "RecordingConfigurationFormatType",
     "VideoAspectRatioType",
     "VideoFillModeType",
-    "ivsrealtimeServiceName",
+    "IvsrealtimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 CompositionStateType = Literal["ACTIVE", "FAILED", "STARTING", "STOPPED", "STOPPING"]
 DestinationStateType = Literal[
@@ -56,15 +56,15 @@
 ParticipantStateType = Literal["CONNECTED", "DISCONNECTED"]
 ParticipantTokenCapabilityType = Literal["PUBLISH", "SUBSCRIBE"]
 PipBehaviorType = Literal["DYNAMIC", "STATIC"]
 PipPositionType = Literal["BOTTOM_LEFT", "BOTTOM_RIGHT", "TOP_LEFT", "TOP_RIGHT"]
 RecordingConfigurationFormatType = Literal["HLS"]
 VideoAspectRatioType = Literal["AUTO", "PORTRAIT", "SQUARE", "VIDEO"]
 VideoFillModeType = Literal["CONTAIN", "COVER", "FILL"]
-ivsrealtimeServiceName = Literal["ivs-realtime"]
+IvsrealtimeServiceName = Literal["ivs-realtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
@@ -128,14 +128,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -148,24 +149,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -226,15 +229,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -363,14 +365,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -414,14 +417,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/type_defs.py` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: ChannelDestinationConfigurationTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CompositionStateType,
     DestinationStateType,
     EventErrorCodeType,
     EventNameType,
     ParticipantStateType,
@@ -102,25 +102,28 @@
     "ListParticipantEventsResponseTypeDef",
     "GetParticipantResponseTypeDef",
     "GetStageSessionResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "ListParticipantsResponseTypeDef",
     "ListStageSessionsResponseTypeDef",
     "ListStagesResponseTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
     "ListCompositionsResponseTypeDef",
     "CreateEncoderConfigurationResponseTypeDef",
     "GetEncoderConfigurationResponseTypeDef",
     "ListStorageConfigurationsResponseTypeDef",
     "CreateStorageConfigurationResponseTypeDef",
     "GetStorageConfigurationResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "DestinationTypeDef",
-    "StartCompositionRequestRequestTypeDef",
+    "DestinationConfigurationUnionTypeDef",
     "CompositionTypeDef",
+    "StartCompositionRequestRequestTypeDef",
     "GetCompositionResponseTypeDef",
     "StartCompositionResponseTypeDef",
 )
 
 ChannelDestinationConfigurationTypeDef = TypedDict(
     "ChannelDestinationConfigurationTypeDef",
     {
@@ -631,18 +634,26 @@
     "ListStagesResponseTypeDef",
     {
         "nextToken": str,
         "stages": List[StageSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "encoderConfigurationArns": List[str],
+        "storageConfigurationArn": str,
+        "recordingConfiguration": NotRequired[RecordingConfigurationTypeDef],
+    },
+)
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
-        "encoderConfigurationArns": List[str],
+        "encoderConfigurationArns": Sequence[str],
         "storageConfigurationArn": str,
         "recordingConfiguration": NotRequired[RecordingConfigurationTypeDef],
     },
 )
 ListCompositionsResponseTypeDef = TypedDict(
     "ListCompositionsResponseTypeDef",
     {
@@ -683,56 +694,67 @@
 GetStorageConfigurationResponseTypeDef = TypedDict(
     "GetStorageConfigurationResponseTypeDef",
     {
         "storageConfiguration": StorageConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "channel": NotRequired[ChannelDestinationConfigurationTypeDef],
+        "name": NotRequired[str],
+        "s3": NotRequired[S3DestinationConfigurationOutputTypeDef],
+    },
+)
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "channel": NotRequired[ChannelDestinationConfigurationTypeDef],
         "name": NotRequired[str],
         "s3": NotRequired[S3DestinationConfigurationTypeDef],
     },
 )
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
-        "configuration": DestinationConfigurationTypeDef,
+        "configuration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "state": DestinationStateType,
         "detail": NotRequired[DestinationDetailTypeDef],
         "endTime": NotRequired[datetime],
         "startTime": NotRequired[datetime],
     },
 )
-StartCompositionRequestRequestTypeDef = TypedDict(
-    "StartCompositionRequestRequestTypeDef",
-    {
-        "destinations": Sequence[DestinationConfigurationTypeDef],
-        "stageArn": str,
-        "idempotencyToken": NotRequired[str],
-        "layout": NotRequired[LayoutConfigurationTypeDef],
-        "tags": NotRequired[Mapping[str, str]],
-    },
-)
+DestinationConfigurationUnionTypeDef = Union[
+    DestinationConfigurationTypeDef, DestinationConfigurationOutputTypeDef
+]
 CompositionTypeDef = TypedDict(
     "CompositionTypeDef",
     {
         "arn": str,
         "destinations": List[DestinationTypeDef],
         "layout": LayoutConfigurationTypeDef,
         "stageArn": str,
         "state": CompositionStateType,
         "endTime": NotRequired[datetime],
         "startTime": NotRequired[datetime],
         "tags": NotRequired[Dict[str, str]],
     },
 )
+StartCompositionRequestRequestTypeDef = TypedDict(
+    "StartCompositionRequestRequestTypeDef",
+    {
+        "destinations": Sequence[DestinationConfigurationUnionTypeDef],
+        "stageArn": str,
+        "idempotencyToken": NotRequired[str],
+        "layout": NotRequired[LayoutConfigurationTypeDef],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
 GetCompositionResponseTypeDef = TypedDict(
     "GetCompositionResponseTypeDef",
     {
         "composition": CompositionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime/type_defs.pyi` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: ChannelDestinationConfigurationTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CompositionStateType,
     DestinationStateType,
     EventErrorCodeType,
     EventNameType,
     ParticipantStateType,
@@ -102,25 +102,28 @@
     "ListParticipantEventsResponseTypeDef",
     "GetParticipantResponseTypeDef",
     "GetStageSessionResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "ListParticipantsResponseTypeDef",
     "ListStageSessionsResponseTypeDef",
     "ListStagesResponseTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
     "ListCompositionsResponseTypeDef",
     "CreateEncoderConfigurationResponseTypeDef",
     "GetEncoderConfigurationResponseTypeDef",
     "ListStorageConfigurationsResponseTypeDef",
     "CreateStorageConfigurationResponseTypeDef",
     "GetStorageConfigurationResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "DestinationTypeDef",
-    "StartCompositionRequestRequestTypeDef",
+    "DestinationConfigurationUnionTypeDef",
     "CompositionTypeDef",
+    "StartCompositionRequestRequestTypeDef",
     "GetCompositionResponseTypeDef",
     "StartCompositionResponseTypeDef",
 )
 
 ChannelDestinationConfigurationTypeDef = TypedDict(
     "ChannelDestinationConfigurationTypeDef",
     {
@@ -631,18 +634,26 @@
     "ListStagesResponseTypeDef",
     {
         "nextToken": str,
         "stages": List[StageSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "encoderConfigurationArns": List[str],
+        "storageConfigurationArn": str,
+        "recordingConfiguration": NotRequired[RecordingConfigurationTypeDef],
+    },
+)
 S3DestinationConfigurationTypeDef = TypedDict(
     "S3DestinationConfigurationTypeDef",
     {
-        "encoderConfigurationArns": List[str],
+        "encoderConfigurationArns": Sequence[str],
         "storageConfigurationArn": str,
         "recordingConfiguration": NotRequired[RecordingConfigurationTypeDef],
     },
 )
 ListCompositionsResponseTypeDef = TypedDict(
     "ListCompositionsResponseTypeDef",
     {
@@ -683,56 +694,67 @@
 GetStorageConfigurationResponseTypeDef = TypedDict(
     "GetStorageConfigurationResponseTypeDef",
     {
         "storageConfiguration": StorageConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "channel": NotRequired[ChannelDestinationConfigurationTypeDef],
+        "name": NotRequired[str],
+        "s3": NotRequired[S3DestinationConfigurationOutputTypeDef],
+    },
+)
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "channel": NotRequired[ChannelDestinationConfigurationTypeDef],
         "name": NotRequired[str],
         "s3": NotRequired[S3DestinationConfigurationTypeDef],
     },
 )
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
-        "configuration": DestinationConfigurationTypeDef,
+        "configuration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "state": DestinationStateType,
         "detail": NotRequired[DestinationDetailTypeDef],
         "endTime": NotRequired[datetime],
         "startTime": NotRequired[datetime],
     },
 )
-StartCompositionRequestRequestTypeDef = TypedDict(
-    "StartCompositionRequestRequestTypeDef",
-    {
-        "destinations": Sequence[DestinationConfigurationTypeDef],
-        "stageArn": str,
-        "idempotencyToken": NotRequired[str],
-        "layout": NotRequired[LayoutConfigurationTypeDef],
-        "tags": NotRequired[Mapping[str, str]],
-    },
-)
+DestinationConfigurationUnionTypeDef = Union[
+    DestinationConfigurationTypeDef, DestinationConfigurationOutputTypeDef
+]
 CompositionTypeDef = TypedDict(
     "CompositionTypeDef",
     {
         "arn": str,
         "destinations": List[DestinationTypeDef],
         "layout": LayoutConfigurationTypeDef,
         "stageArn": str,
         "state": CompositionStateType,
         "endTime": NotRequired[datetime],
         "startTime": NotRequired[datetime],
         "tags": NotRequired[Dict[str, str]],
     },
 )
+StartCompositionRequestRequestTypeDef = TypedDict(
+    "StartCompositionRequestRequestTypeDef",
+    {
+        "destinations": Sequence[DestinationConfigurationUnionTypeDef],
+        "stageArn": str,
+        "idempotencyToken": NotRequired[str],
+        "layout": NotRequired[LayoutConfigurationTypeDef],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
 GetCompositionResponseTypeDef = TypedDict(
     "GetCompositionResponseTypeDef",
     {
         "composition": CompositionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/PKG-INFO` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs-realtime
-Version: 1.34.62
-Summary: Type annotations for boto3.ivsrealtime 1.34.62 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3.Ivsrealtime 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs-realtime)](https://pepy.tech/project/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.34.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.Ivsrealtime 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -96,21 +96,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `ivsrealtime`.
+Click `Modify` and select `boto3 common` and `Ivsrealtime`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `ivsrealtime` service.
+Install `boto3-stubs` for `Ivsrealtime` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[ivs-realtime]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -256,34 +256,34 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`ivsrealtimeClient` provides annotations for `boto3.client("ivs-realtime")`.
+`IvsrealtimeClient` provides annotations for `boto3.client("ivs-realtime")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_ivs_realtime import ivsrealtimeClient
+from mypy_boto3_ivs_realtime import IvsrealtimeClient
 
-client: ivsrealtimeClient = Session().client("ivs-realtime")
+client: IvsrealtimeClient = Session().client("ivs-realtime")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_ivs_realtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
-Full list of `ivsrealtime` Literals can be found in
+Full list of `Ivsrealtime` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/literals/).
 
 ```python
 from mypy_boto3_ivs_realtime.literals import CompositionStateType
 
 
 def check_value(value: CompositionStateType) -> bool: ...
@@ -292,15 +292,15 @@
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
-Full list of `ivsrealtime` TypeDefs can be found in
+Full list of `Ivsrealtime` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/type_defs/).
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import ChannelDestinationConfigurationTypeDef
 
 
 def get_value() -> ChannelDestinationConfigurationTypeDef:
```

### Comparing `mypy-boto3-ivs-realtime-1.34.62/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt` & `mypy_boto3_ivs_realtime-1.34.92/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.34.62/setup.py` & `mypy_boto3_ivs_realtime-1.34.92/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs-realtime",
-    version="1.34.62",
+    version="1.34.92",
     packages=["mypy_boto3_ivs_realtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ivsrealtime 1.34.62 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Ivsrealtime 1.34.92 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


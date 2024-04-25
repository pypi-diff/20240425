# Comparing `tmp/mypy-boto3-stepfunctions-1.34.0.tar.gz` & `tmp/mypy_boto3_stepfunctions-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.34.0.tar", last modified: Wed Dec 13 21:23:58 2023, max compression
+gzip compressed data, was "mypy_boto3_stepfunctions-1.34.92.tar", last modified: Thu Apr 25 19:32:16 2024, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.34.0.tar` & `mypy_boto3_stepfunctions-1.34.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:58.543396 mypy-boto3-stepfunctions-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13462 2023-12-13 21:23:58.543396 mypy-boto3-stepfunctions-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:58.539396 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30018 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39339 2023-12-13 21:20:29.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39338 2023-12-13 21:20:29.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:58.543396 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13462 2023-12-13 21:23:58.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 21:23:58.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:58.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:58.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:58.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 21:23:58.000000 mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:58.543396 mypy-boto3-stepfunctions-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-13 21:20:28.000000 mypy-boto3-stepfunctions-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:16.115419 mypy_boto3_stepfunctions-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-04-25 19:32:16.115419 mypy_boto3_stepfunctions-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11916 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:16.115419 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    40933 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40933 2024-04-25 19:32:03.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:16.115419 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-04-25 19:32:16.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-25 19:32:16.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:16.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:16.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:16.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 19:32:16.000000 mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:16.115419 mypy_boto3_stepfunctions-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-25 19:32:02.000000 mypy_boto3_stepfunctions-1.34.92/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/LICENSE` & `mypy_boto3_stepfunctions-1.34.92/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/PKG-INFO` & `mypy_boto3_stepfunctions-1.34.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.34.0
-Summary: Type annotations for boto3.SFN 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.92
+Summary: Type annotations for boto3.SFN 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/README.md` & `mypy_boto3_stepfunctions-1.34.92/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/__init__.py` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListExecutionsPaginator,
     ListMapRunsPaginator,
     ListStateMachinesPaginator,
 )
 
 Client = SFNClient
 
-
 __all__ = (
     "Client",
     "GetExecutionHistoryPaginator",
     "ListActivitiesPaginator",
     "ListExecutionsPaginator",
     "ListMapRunsPaginator",
     "ListStateMachinesPaginator",
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/__init__.pyi` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/__main__.py` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.SFN 1.34.92\n"
+        "Version:         1.34.92\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.92")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/client.py` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,34 +47,34 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RedriveExecutionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TestStateOutputTypeDef,
     TracingConfigurationTypeDef,
     UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
+    ValidateStateMachineDefinitionOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SFNClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -160,33 +160,33 @@
     def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine)
         """
 
     def create_state_machine_alias(
         self,
         *,
         name: str,
         routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
-        description: str = ...
+        description: str = ...,
     ) -> CreateStateMachineAliasOutputTypeDef:
         """
         Creates an
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         for a state machine that points to one or two
         [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-version.html)
         of the same state
@@ -319,15 +319,15 @@
     def get_execution_history(
         self,
         *,
         executionArn: str,
         maxResults: int = ...,
         reverseOrder: bool = ...,
         nextToken: str = ...,
-        includeExecutionData: bool = ...
+        includeExecutionData: bool = ...,
     ) -> GetExecutionHistoryOutputTypeDef:
         """
         Returns the history of the specified execution as a list of events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_execution_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_execution_history)
         """
@@ -346,15 +346,15 @@
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         mapRunArn: str = ...,
-        redriveFilter: ExecutionRedriveFilterType = ...
+        redriveFilter: ExecutionRedriveFilterType = ...,
     ) -> ListExecutionsOutputTypeDef:
         """
         Lists all executions of a state machine or a Map Run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_executions)
         """
@@ -514,15 +514,15 @@
     def test_state(
         self,
         *,
         definition: str,
         roleArn: str,
         input: str = ...,
         inspectionLevel: InspectionLevelType = ...,
-        revealSecrets: bool = ...
+        revealSecrets: bool = ...,
     ) -> TestStateOutputTypeDef:
         """
         Accepts the definition of a single state and executes it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.test_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#test_state)
         """
@@ -538,15 +538,15 @@
 
     def update_map_run(
         self,
         *,
         mapRunArn: str,
         maxConcurrency: int = ...,
         toleratedFailurePercentage: float = ...,
-        toleratedFailureCount: int = ...
+        toleratedFailureCount: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates an in-progress Map Run's configuration to include changes to the
         settings that control maximum concurrency and Map Run
         failure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_map_run)
@@ -555,44 +555,54 @@
 
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine)
         """
 
     def update_state_machine_alias(
         self,
         *,
         stateMachineAliasArn: str,
         description: str = ...,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...,
     ) -> UpdateStateMachineAliasOutputTypeDef:
         """
         Updates the configuration of an existing state machine
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         by modifying its `description` or
         `routingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine_alias)
         """
 
+    def validate_state_machine_definition(
+        self, *, definition: str, type: StateMachineTypeType = ...
+    ) -> ValidateStateMachineDefinitionOutputTypeDef:
+        """
+        Validates the syntax of a state machine definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.validate_state_machine_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#validate_state_machine_definition)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_execution_history"]
     ) -> GetExecutionHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_paginator)
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/client.pyi` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,27 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RedriveExecutionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TestStateOutputTypeDef,
     TracingConfigurationTypeDef,
     UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
+    ValidateStateMachineDefinitionOutputTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -156,33 +157,33 @@
     def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine)
         """
 
     def create_state_machine_alias(
         self,
         *,
         name: str,
         routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
-        description: str = ...
+        description: str = ...,
     ) -> CreateStateMachineAliasOutputTypeDef:
         """
         Creates an
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         for a state machine that points to one or two
         [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-version.html)
         of the same state
@@ -315,15 +316,15 @@
     def get_execution_history(
         self,
         *,
         executionArn: str,
         maxResults: int = ...,
         reverseOrder: bool = ...,
         nextToken: str = ...,
-        includeExecutionData: bool = ...
+        includeExecutionData: bool = ...,
     ) -> GetExecutionHistoryOutputTypeDef:
         """
         Returns the history of the specified execution as a list of events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_execution_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_execution_history)
         """
@@ -342,15 +343,15 @@
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         mapRunArn: str = ...,
-        redriveFilter: ExecutionRedriveFilterType = ...
+        redriveFilter: ExecutionRedriveFilterType = ...,
     ) -> ListExecutionsOutputTypeDef:
         """
         Lists all executions of a state machine or a Map Run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_executions)
         """
@@ -510,15 +511,15 @@
     def test_state(
         self,
         *,
         definition: str,
         roleArn: str,
         input: str = ...,
         inspectionLevel: InspectionLevelType = ...,
-        revealSecrets: bool = ...
+        revealSecrets: bool = ...,
     ) -> TestStateOutputTypeDef:
         """
         Accepts the definition of a single state and executes it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.test_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#test_state)
         """
@@ -534,15 +535,15 @@
 
     def update_map_run(
         self,
         *,
         mapRunArn: str,
         maxConcurrency: int = ...,
         toleratedFailurePercentage: float = ...,
-        toleratedFailureCount: int = ...
+        toleratedFailureCount: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates an in-progress Map Run's configuration to include changes to the
         settings that control maximum concurrency and Map Run
         failure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_map_run)
@@ -551,44 +552,54 @@
 
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine)
         """
 
     def update_state_machine_alias(
         self,
         *,
         stateMachineAliasArn: str,
         description: str = ...,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...,
     ) -> UpdateStateMachineAliasOutputTypeDef:
         """
         Updates the configuration of an existing state machine
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         by modifying its `description` or
         `routingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine_alias)
         """
 
+    def validate_state_machine_definition(
+        self, *, definition: str, type: StateMachineTypeType = ...
+    ) -> ValidateStateMachineDefinitionOutputTypeDef:
+        """
+        Validates the syntax of a state machine definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.validate_state_machine_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#validate_state_machine_definition)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_execution_history"]
     ) -> GetExecutionHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_paginator)
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/literals.py` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ExecutionRedriveFilterType",
     "ExecutionRedriveStatusType",
     "ExecutionStatusType",
     "GetExecutionHistoryPaginatorName",
     "HistoryEventTypeType",
     "InspectionLevelType",
@@ -33,22 +32,23 @@
     "ListStateMachinesPaginatorName",
     "LogLevelType",
     "MapRunStatusType",
     "StateMachineStatusType",
     "StateMachineTypeType",
     "SyncExecutionStatusType",
     "TestExecutionStatusType",
+    "ValidateStateMachineDefinitionResultCodeType",
+    "ValidateStateMachineDefinitionSeverityType",
     "SFNServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ExecutionRedriveFilterType = Literal["NOT_REDRIVEN", "REDRIVEN"]
 ExecutionRedriveStatusType = Literal["NOT_REDRIVABLE", "REDRIVABLE", "REDRIVABLE_BY_MAP_RUN"]
 ExecutionStatusType = Literal[
     "ABORTED", "FAILED", "PENDING_REDRIVE", "RUNNING", "SUCCEEDED", "TIMED_OUT"
 ]
 GetExecutionHistoryPaginatorName = Literal["get_execution_history"]
 HistoryEventTypeType = Literal[
@@ -121,14 +121,16 @@
 ListStateMachinesPaginatorName = Literal["list_state_machines"]
 LogLevelType = Literal["ALL", "ERROR", "FATAL", "OFF"]
 MapRunStatusType = Literal["ABORTED", "FAILED", "RUNNING", "SUCCEEDED"]
 StateMachineStatusType = Literal["ACTIVE", "DELETING"]
 StateMachineTypeType = Literal["EXPRESS", "STANDARD"]
 SyncExecutionStatusType = Literal["FAILED", "SUCCEEDED", "TIMED_OUT"]
 TestExecutionStatusType = Literal["CAUGHT_ERROR", "FAILED", "RETRIABLE", "SUCCEEDED"]
+ValidateStateMachineDefinitionResultCodeType = Literal["FAIL", "OK"]
+ValidateStateMachineDefinitionSeverityType = Literal["ERROR"]
 SFNServiceName = Literal["stepfunctions"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -148,14 +150,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -166,14 +169,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -191,14 +195,15 @@
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
@@ -211,24 +216,26 @@
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
@@ -289,15 +296,14 @@
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
@@ -369,17 +375,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -424,14 +432,15 @@
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
@@ -469,19 +478,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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
@@ -530,14 +541,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/literals.pyi` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     "ListStateMachinesPaginatorName",
     "LogLevelType",
     "MapRunStatusType",
     "StateMachineStatusType",
     "StateMachineTypeType",
     "SyncExecutionStatusType",
     "TestExecutionStatusType",
+    "ValidateStateMachineDefinitionResultCodeType",
+    "ValidateStateMachineDefinitionSeverityType",
     "SFNServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -119,14 +121,16 @@
 ListStateMachinesPaginatorName = Literal["list_state_machines"]
 LogLevelType = Literal["ALL", "ERROR", "FATAL", "OFF"]
 MapRunStatusType = Literal["ABORTED", "FAILED", "RUNNING", "SUCCEEDED"]
 StateMachineStatusType = Literal["ACTIVE", "DELETING"]
 StateMachineTypeType = Literal["EXPRESS", "STANDARD"]
 SyncExecutionStatusType = Literal["FAILED", "SUCCEEDED", "TIMED_OUT"]
 TestExecutionStatusType = Literal["CAUGHT_ERROR", "FAILED", "RETRIABLE", "SUCCEEDED"]
+ValidateStateMachineDefinitionResultCodeType = Literal["FAIL", "OK"]
+ValidateStateMachineDefinitionSeverityType = Literal["ERROR"]
 SFNServiceName = Literal["stepfunctions"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -146,14 +150,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -164,14 +169,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -189,14 +195,15 @@
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
@@ -209,24 +216,26 @@
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
@@ -287,15 +296,14 @@
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
@@ -367,17 +375,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -422,14 +432,15 @@
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
@@ -467,19 +478,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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
@@ -528,14 +541,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/paginator.py` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     "GetExecutionHistoryPaginator",
     "ListActivitiesPaginator",
     "ListExecutionsPaginator",
     "ListMapRunsPaginator",
     "ListStateMachinesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -69,15 +68,15 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 
@@ -105,15 +104,15 @@
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
         redriveFilter: ExecutionRedriveFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listexecutionspaginator)
         """
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/paginator.pyi` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 class ListActivitiesPaginator(Paginator):
@@ -100,15 +100,15 @@
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
         redriveFilter: ExecutionRedriveFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/paginators/#listexecutionspaginator)
         """
 
 class ListMapRunsPaginator(Paginator):
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/type_defs.py` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,40 +10,44 @@
 
     data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ExecutionRedriveFilterType,
     ExecutionRedriveStatusType,
     ExecutionStatusType,
     HistoryEventTypeType,
     InspectionLevelType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
     StateMachineTypeType,
     SyncExecutionStatusType,
     TestExecutionStatusType,
+    ValidateStateMachineDefinitionResultCodeType,
 )
 
 if sys.version_info >= (3, 12):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityFailedEventDetailsTypeDef",
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
@@ -109,14 +113,16 @@
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
     "TestStateInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
+    "ValidateStateMachineDefinitionDiagnosticTypeDef",
+    "ValidateStateMachineDefinitionInputRequestTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
@@ -153,20 +159,23 @@
     "InspectionDataTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
+    "ValidateStateMachineDefinitionOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "TestStateOutputTypeDef",
     "HistoryEventTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -234,18 +243,18 @@
         "value": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 RoutingConfigurationListItemTypeDef = TypedDict(
     "RoutingConfigurationListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "weight": int,
@@ -718,14 +727,30 @@
     {
         "mapRunArn": str,
         "maxConcurrency": NotRequired[int],
         "toleratedFailurePercentage": NotRequired[float],
         "toleratedFailureCount": NotRequired[int],
     },
 )
+ValidateStateMachineDefinitionDiagnosticTypeDef = TypedDict(
+    "ValidateStateMachineDefinitionDiagnosticTypeDef",
+    {
+        "severity": Literal["ERROR"],
+        "code": str,
+        "message": str,
+        "location": NotRequired[str],
+    },
+)
+ValidateStateMachineDefinitionInputRequestTypeDef = TypedDict(
+    "ValidateStateMachineDefinitionInputRequestTypeDef",
+    {
+        "definition": str,
+        "type": NotRequired[StateMachineTypeType],
+    },
+)
 ActivityScheduledEventDetailsTypeDef = TypedDict(
     "ActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
         "input": NotRequired[str],
         "inputDetails": NotRequired[HistoryEventExecutionDataDetailsTypeDef],
         "timeoutInSeconds": NotRequired[int],
@@ -1121,14 +1146,30 @@
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ValidateStateMachineDefinitionOutputTypeDef = TypedDict(
+    "ValidateStateMachineDefinitionOutputTypeDef",
+    {
+        "result": ValidateStateMachineDefinitionResultCodeType,
+        "diagnostics": List[ValidateStateMachineDefinitionDiagnosticTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "level": NotRequired[LogLevelType],
+        "includeExecutionData": NotRequired[bool],
+        "destinations": NotRequired[List[LogDestinationTypeDef]],
+    },
+)
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": NotRequired[LogLevelType],
         "includeExecutionData": NotRequired[bool],
         "destinations": NotRequired[Sequence[LogDestinationTypeDef]],
     },
@@ -1198,37 +1239,23 @@
         "stateEnteredEventDetails": NotRequired[StateEnteredEventDetailsTypeDef],
         "stateExitedEventDetails": NotRequired[StateExitedEventDetailsTypeDef],
         "mapRunStartedEventDetails": NotRequired[MapRunStartedEventDetailsTypeDef],
         "mapRunFailedEventDetails": NotRequired[MapRunFailedEventDetailsTypeDef],
         "mapRunRedrivenEventDetails": NotRequired[MapRunRedrivenEventDetailsTypeDef],
     },
 )
-CreateStateMachineInputRequestTypeDef = TypedDict(
-    "CreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-        "type": NotRequired[StateMachineTypeType],
-        "loggingConfiguration": NotRequired[LoggingConfigurationTypeDef],
-        "tags": NotRequired[Sequence[TagTypeDef]],
-        "tracingConfiguration": NotRequired[TracingConfigurationTypeDef],
-        "publish": NotRequired[bool],
-        "versionDescription": NotRequired[str],
-    },
-)
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1238,22 +1265,39 @@
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateStateMachineInputRequestTypeDef = TypedDict(
+    "CreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+        "type": NotRequired[StateMachineTypeType],
+        "loggingConfiguration": NotRequired[LoggingConfigurationTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+        "tracingConfiguration": NotRequired[TracingConfigurationTypeDef],
+        "publish": NotRequired[bool],
+        "versionDescription": NotRequired[str],
+    },
+)
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 UpdateStateMachineInputRequestTypeDef = TypedDict(
     "UpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "definition": NotRequired[str],
         "roleArn": NotRequired[str],
         "loggingConfiguration": NotRequired[LoggingConfigurationTypeDef],
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,36 @@
 
     data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ExecutionRedriveFilterType,
     ExecutionRedriveStatusType,
     ExecutionStatusType,
     HistoryEventTypeType,
     InspectionLevelType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
     StateMachineTypeType,
     SyncExecutionStatusType,
     TestExecutionStatusType,
+    ValidateStateMachineDefinitionResultCodeType,
 )
 
 if sys.version_info >= (3, 12):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -108,14 +113,16 @@
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
     "TestStateInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
+    "ValidateStateMachineDefinitionDiagnosticTypeDef",
+    "ValidateStateMachineDefinitionInputRequestTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
@@ -152,20 +159,23 @@
     "InspectionDataTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
+    "ValidateStateMachineDefinitionOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "TestStateOutputTypeDef",
     "HistoryEventTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -233,18 +243,18 @@
         "value": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 RoutingConfigurationListItemTypeDef = TypedDict(
     "RoutingConfigurationListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "weight": int,
@@ -717,14 +727,30 @@
     {
         "mapRunArn": str,
         "maxConcurrency": NotRequired[int],
         "toleratedFailurePercentage": NotRequired[float],
         "toleratedFailureCount": NotRequired[int],
     },
 )
+ValidateStateMachineDefinitionDiagnosticTypeDef = TypedDict(
+    "ValidateStateMachineDefinitionDiagnosticTypeDef",
+    {
+        "severity": Literal["ERROR"],
+        "code": str,
+        "message": str,
+        "location": NotRequired[str],
+    },
+)
+ValidateStateMachineDefinitionInputRequestTypeDef = TypedDict(
+    "ValidateStateMachineDefinitionInputRequestTypeDef",
+    {
+        "definition": str,
+        "type": NotRequired[StateMachineTypeType],
+    },
+)
 ActivityScheduledEventDetailsTypeDef = TypedDict(
     "ActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
         "input": NotRequired[str],
         "inputDetails": NotRequired[HistoryEventExecutionDataDetailsTypeDef],
         "timeoutInSeconds": NotRequired[int],
@@ -1120,14 +1146,30 @@
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ValidateStateMachineDefinitionOutputTypeDef = TypedDict(
+    "ValidateStateMachineDefinitionOutputTypeDef",
+    {
+        "result": ValidateStateMachineDefinitionResultCodeType,
+        "diagnostics": List[ValidateStateMachineDefinitionDiagnosticTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "level": NotRequired[LogLevelType],
+        "includeExecutionData": NotRequired[bool],
+        "destinations": NotRequired[List[LogDestinationTypeDef]],
+    },
+)
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": NotRequired[LogLevelType],
         "includeExecutionData": NotRequired[bool],
         "destinations": NotRequired[Sequence[LogDestinationTypeDef]],
     },
@@ -1197,37 +1239,23 @@
         "stateEnteredEventDetails": NotRequired[StateEnteredEventDetailsTypeDef],
         "stateExitedEventDetails": NotRequired[StateExitedEventDetailsTypeDef],
         "mapRunStartedEventDetails": NotRequired[MapRunStartedEventDetailsTypeDef],
         "mapRunFailedEventDetails": NotRequired[MapRunFailedEventDetailsTypeDef],
         "mapRunRedrivenEventDetails": NotRequired[MapRunRedrivenEventDetailsTypeDef],
     },
 )
-CreateStateMachineInputRequestTypeDef = TypedDict(
-    "CreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-        "type": NotRequired[StateMachineTypeType],
-        "loggingConfiguration": NotRequired[LoggingConfigurationTypeDef],
-        "tags": NotRequired[Sequence[TagTypeDef]],
-        "tracingConfiguration": NotRequired[TracingConfigurationTypeDef],
-        "publish": NotRequired[bool],
-        "versionDescription": NotRequired[str],
-    },
-)
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1237,22 +1265,39 @@
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateStateMachineInputRequestTypeDef = TypedDict(
+    "CreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+        "type": NotRequired[StateMachineTypeType],
+        "loggingConfiguration": NotRequired[LoggingConfigurationTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+        "tracingConfiguration": NotRequired[TracingConfigurationTypeDef],
+        "publish": NotRequired[bool],
+        "versionDescription": NotRequired[str],
+    },
+)
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 UpdateStateMachineInputRequestTypeDef = TypedDict(
     "UpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "definition": NotRequired[str],
         "roleArn": NotRequired[str],
         "loggingConfiguration": NotRequired[LoggingConfigurationTypeDef],
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.34.0
-Summary: Type annotations for boto3.SFN 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.92
+Summary: Type annotations for boto3.SFN 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-stepfunctions)](https://pepy.tech/project/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-stepfunctions-1.34.0/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy_boto3_stepfunctions-1.34.92/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.34.0/setup.py` & `mypy_boto3_stepfunctions-1.34.92/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.34.0",
+    version="1.34.92",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.SFN 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.SFN 1.34.92 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 stepfunctions type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_stepfunctions": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```


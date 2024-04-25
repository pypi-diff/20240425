# Comparing `tmp/mypy-boto3-fms-1.34.0.tar.gz` & `tmp/mypy_boto3_fms-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.34.0.tar", last modified: Wed Dec 13 21:22:41 2023, max compression
+gzip compressed data, was "mypy_boto3_fms-1.34.92.tar", last modified: Thu Apr 25 19:32:14 2024, max compression
```

## Comparing `mypy-boto3-fms-1.34.0.tar` & `mypy_boto3_fms-1.34.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:41.187217 mypy-boto3-fms-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2023-12-13 21:22:41.187217 mypy-boto3-fms-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:41.183217 mypy-boto3-fms-1.34.0/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30883 2023-12-13 21:10:30.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30879 2023-12-13 21:10:30.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2023-12-13 21:10:30.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2023-12-13 21:10:30.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2023-12-13 21:10:30.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-12-13 21:10:30.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52836 2023-12-13 21:10:31.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52835 2023-12-13 21:10:31.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:10:29.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:41.187217 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2023-12-13 21:22:41.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-13 21:22:41.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:41.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:41.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:41.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 21:22:41.000000 mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:41.187217 mypy-boto3-fms-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-13 21:10:28.000000 mypy-boto3-fms-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.675407 mypy_boto3_fms-1.34.92/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30934 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30931 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    63196 2024-04-25 19:31:48.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63196 2024-04-25 19:31:48.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:32:14.000000 mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:14.679407 mypy_boto3_fms-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-25 19:31:47.000000 mypy_boto3_fms-1.34.92/setup.py
```

### Comparing `mypy-boto3-fms-1.34.0/LICENSE` & `mypy_boto3_fms-1.34.92/LICENSE`

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

### Comparing `mypy-boto3-fms-1.34.0/PKG-INFO` & `mypy_boto3_fms-1.34.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.34.0
-Summary: Type annotations for boto3.FMS 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.92
+Summary: Type annotations for boto3.FMS 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
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
 
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,18 +343,18 @@
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries and unions for additional type checking.
 
 Full list of `FMS` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/).
 
 ```python
-from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
 
-def get_value() -> AccountScopeTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.34.0/README.md` & `mypy_boto3_fms-1.34.92/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,18 +310,18 @@
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries and unions for additional type checking.
 
 Full list of `FMS` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/).
 
 ```python
-from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
 
-def get_value() -> AccountScopeTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/__init__.py` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 
 Client = FMSClient
 
-
 __all__ = (
     "Client",
     "FMSClient",
     "ListAdminAccountsForOrganizationPaginator",
     "ListAdminsManagingAccountPaginator",
     "ListAppsListsPaginator",
     "ListComplianceStatusPaginator",
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/__init__.pyi` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/__main__.py` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.FMS 1.34.92\n"
+        "Version:         1.34.92\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\n"
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

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/client.py` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeTypeDef,
-    AppsListDataTypeDef,
+    AdminScopeUnionTypeDef,
+    AppsListDataUnionTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -57,31 +57,30 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyTypeDef,
-    ProtocolsListDataTypeDef,
+    PolicyUnionTypeDef,
+    ProtocolsListDataUnionTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetUnionTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FMSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -308,15 +307,15 @@
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS
         attack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_protection_status)
@@ -409,15 +408,15 @@
 
     def list_discovered_resources(
         self,
         *,
         MemberAccountIds: Sequence[str],
         ResourceType: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDiscoveredResourcesResponseTypeDef:
         """
         Returns an array of resources in the organization's accounts that are available
         to be associated with a resource
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_discovered_resources)
@@ -493,25 +492,25 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
     def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
         """
 
     def put_apps_list(
-        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_apps_list)
         """
@@ -525,35 +524,35 @@
         logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_notification_channel)
         """
 
     def put_policy(
-        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_policy)
         """
 
     def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_protocols_list)
         """
 
     def put_resource_set(
-        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_resource_set)
         """
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/client.pyi` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeTypeDef,
-    AppsListDataTypeDef,
+    AdminScopeUnionTypeDef,
+    AppsListDataUnionTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -57,21 +57,21 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyTypeDef,
-    ProtocolsListDataTypeDef,
+    PolicyUnionTypeDef,
+    ProtocolsListDataUnionTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetUnionTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -304,15 +304,15 @@
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS
         attack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_protection_status)
@@ -405,15 +405,15 @@
 
     def list_discovered_resources(
         self,
         *,
         MemberAccountIds: Sequence[str],
         ResourceType: str,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListDiscoveredResourcesResponseTypeDef:
         """
         Returns an array of resources in the organization's accounts that are available
         to be associated with a resource
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_discovered_resources)
@@ -489,25 +489,25 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
     def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_admin_account)
         """
 
     def put_apps_list(
-        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_apps_list)
         """
@@ -521,35 +521,35 @@
         logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_notification_channel)
         """
 
     def put_policy(
-        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_policy)
         """
 
     def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_protocols_list)
         """
 
     def put_resource_set(
-        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#put_resource_set)
         """
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/literals.py` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,34 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountRoleStatusType",
     "CustomerPolicyScopeIdTypeType",
     "CustomerPolicyStatusType",
     "DependentServiceNameType",
     "DestinationTypeType",
+    "EntryTypeType",
+    "EntryViolationReasonType",
     "FailedItemReasonType",
     "FirewallDeploymentModelType",
     "ListAdminAccountsForOrganizationPaginatorName",
     "ListAdminsManagingAccountPaginatorName",
     "ListAppsListsPaginatorName",
     "ListComplianceStatusPaginatorName",
     "ListMemberAccountsPaginatorName",
     "ListPoliciesPaginatorName",
     "ListProtocolsListsPaginatorName",
     "ListThirdPartyFirewallFirewallPoliciesPaginatorName",
     "MarketplaceSubscriptionOnboardingStatusType",
+    "NetworkAclRuleActionType",
     "NetworkFirewallOverrideActionType",
     "OrganizationStatusType",
     "PolicyComplianceStatusTypeType",
     "RemediationActionTypeType",
     "ResourceSetStatusType",
     "RuleOrderType",
     "SecurityServiceTypeType",
@@ -51,20 +53,23 @@
     "FMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountRoleStatusType = Literal["CREATING", "DELETED", "DELETING", "PENDING_DELETION", "READY"]
 CustomerPolicyScopeIdTypeType = Literal["ACCOUNT", "ORG_UNIT"]
 CustomerPolicyStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 DependentServiceNameType = Literal["AWSCONFIG", "AWSSHIELD_ADVANCED", "AWSVPC", "AWSWAF"]
 DestinationTypeType = Literal["IPV4", "IPV6", "PREFIX_LIST"]
+EntryTypeType = Literal["CUSTOM_ENTRY", "FMS_MANAGED_FIRST_ENTRY", "FMS_MANAGED_LAST_ENTRY"]
+EntryViolationReasonType = Literal[
+    "ENTRY_CONFLICT", "INCORRECT_ENTRY_ORDER", "MISSING_EXPECTED_ENTRY"
+]
 FailedItemReasonType = Literal[
     "NOT_VALID_ACCOUNT_ID",
     "NOT_VALID_ARN",
     "NOT_VALID_PARTITION",
     "NOT_VALID_REGION",
     "NOT_VALID_RESOURCE_TYPE",
     "NOT_VALID_SERVICE",
@@ -77,25 +82,27 @@
 ListMemberAccountsPaginatorName = Literal["list_member_accounts"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListProtocolsListsPaginatorName = Literal["list_protocols_lists"]
 ListThirdPartyFirewallFirewallPoliciesPaginatorName = Literal[
     "list_third_party_firewall_firewall_policies"
 ]
 MarketplaceSubscriptionOnboardingStatusType = Literal["COMPLETE", "NOT_COMPLETE", "NO_SUBSCRIPTION"]
+NetworkAclRuleActionType = Literal["allow", "deny"]
 NetworkFirewallOverrideActionType = Literal["DROP_TO_ALERT"]
 OrganizationStatusType = Literal[
     "OFFBOARDING", "OFFBOARDING_COMPLETE", "ONBOARDING", "ONBOARDING_COMPLETE"
 ]
 PolicyComplianceStatusTypeType = Literal["COMPLIANT", "NON_COMPLIANT"]
 RemediationActionTypeType = Literal["MODIFY", "REMOVE"]
 ResourceSetStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 RuleOrderType = Literal["DEFAULT_ACTION_ORDER", "STRICT_ORDER"]
 SecurityServiceTypeType = Literal[
     "DNS_FIREWALL",
     "IMPORT_NETWORK_FIREWALL",
+    "NETWORK_ACL_COMMON",
     "NETWORK_FIREWALL",
     "SECURITY_GROUPS_COMMON",
     "SECURITY_GROUPS_CONTENT_AUDIT",
     "SECURITY_GROUPS_USAGE_AUDIT",
     "SHIELD_ADVANCED",
     "THIRD_PARTY_FIREWALL",
     "WAF",
@@ -122,14 +129,15 @@
     "BLACK_HOLE_ROUTE_DETECTED_IN_FIREWALL_SUBNET",
     "FIREWALL_SUBNET_IS_OUT_OF_SCOPE",
     "FIREWALL_SUBNET_MISSING_EXPECTED_ROUTE",
     "FIREWALL_SUBNET_MISSING_VPCE_ENDPOINT",
     "FMS_CREATED_SECURITY_GROUP_EDITED",
     "INTERNET_GATEWAY_MISSING_EXPECTED_ROUTE",
     "INTERNET_TRAFFIC_NOT_INSPECTED",
+    "INVALID_NETWORK_ACL_ENTRY",
     "INVALID_ROUTE_CONFIGURATION",
     "MISSING_EXPECTED_ROUTE_TABLE",
     "MISSING_FIREWALL",
     "MISSING_FIREWALL_SUBNET_IN_AZ",
     "MISSING_TARGET_GATEWAY",
     "NETWORK_FIREWALL_POLICY_MODIFIED",
     "RESOURCE_INCORRECT_WEB_ACL",
@@ -170,14 +178,15 @@
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
@@ -188,14 +197,15 @@
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
@@ -213,14 +223,15 @@
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
@@ -233,24 +244,26 @@
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
@@ -311,15 +324,14 @@
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
@@ -391,17 +403,19 @@
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
@@ -446,14 +460,15 @@
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
@@ -491,19 +506,21 @@
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
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/literals.pyi` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,28 @@
 
 __all__ = (
     "AccountRoleStatusType",
     "CustomerPolicyScopeIdTypeType",
     "CustomerPolicyStatusType",
     "DependentServiceNameType",
     "DestinationTypeType",
+    "EntryTypeType",
+    "EntryViolationReasonType",
     "FailedItemReasonType",
     "FirewallDeploymentModelType",
     "ListAdminAccountsForOrganizationPaginatorName",
     "ListAdminsManagingAccountPaginatorName",
     "ListAppsListsPaginatorName",
     "ListComplianceStatusPaginatorName",
     "ListMemberAccountsPaginatorName",
     "ListPoliciesPaginatorName",
     "ListProtocolsListsPaginatorName",
     "ListThirdPartyFirewallFirewallPoliciesPaginatorName",
     "MarketplaceSubscriptionOnboardingStatusType",
+    "NetworkAclRuleActionType",
     "NetworkFirewallOverrideActionType",
     "OrganizationStatusType",
     "PolicyComplianceStatusTypeType",
     "RemediationActionTypeType",
     "ResourceSetStatusType",
     "RuleOrderType",
     "SecurityServiceTypeType",
@@ -55,14 +58,18 @@
 )
 
 AccountRoleStatusType = Literal["CREATING", "DELETED", "DELETING", "PENDING_DELETION", "READY"]
 CustomerPolicyScopeIdTypeType = Literal["ACCOUNT", "ORG_UNIT"]
 CustomerPolicyStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 DependentServiceNameType = Literal["AWSCONFIG", "AWSSHIELD_ADVANCED", "AWSVPC", "AWSWAF"]
 DestinationTypeType = Literal["IPV4", "IPV6", "PREFIX_LIST"]
+EntryTypeType = Literal["CUSTOM_ENTRY", "FMS_MANAGED_FIRST_ENTRY", "FMS_MANAGED_LAST_ENTRY"]
+EntryViolationReasonType = Literal[
+    "ENTRY_CONFLICT", "INCORRECT_ENTRY_ORDER", "MISSING_EXPECTED_ENTRY"
+]
 FailedItemReasonType = Literal[
     "NOT_VALID_ACCOUNT_ID",
     "NOT_VALID_ARN",
     "NOT_VALID_PARTITION",
     "NOT_VALID_REGION",
     "NOT_VALID_RESOURCE_TYPE",
     "NOT_VALID_SERVICE",
@@ -75,25 +82,27 @@
 ListMemberAccountsPaginatorName = Literal["list_member_accounts"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListProtocolsListsPaginatorName = Literal["list_protocols_lists"]
 ListThirdPartyFirewallFirewallPoliciesPaginatorName = Literal[
     "list_third_party_firewall_firewall_policies"
 ]
 MarketplaceSubscriptionOnboardingStatusType = Literal["COMPLETE", "NOT_COMPLETE", "NO_SUBSCRIPTION"]
+NetworkAclRuleActionType = Literal["allow", "deny"]
 NetworkFirewallOverrideActionType = Literal["DROP_TO_ALERT"]
 OrganizationStatusType = Literal[
     "OFFBOARDING", "OFFBOARDING_COMPLETE", "ONBOARDING", "ONBOARDING_COMPLETE"
 ]
 PolicyComplianceStatusTypeType = Literal["COMPLIANT", "NON_COMPLIANT"]
 RemediationActionTypeType = Literal["MODIFY", "REMOVE"]
 ResourceSetStatusType = Literal["ACTIVE", "OUT_OF_ADMIN_SCOPE"]
 RuleOrderType = Literal["DEFAULT_ACTION_ORDER", "STRICT_ORDER"]
 SecurityServiceTypeType = Literal[
     "DNS_FIREWALL",
     "IMPORT_NETWORK_FIREWALL",
+    "NETWORK_ACL_COMMON",
     "NETWORK_FIREWALL",
     "SECURITY_GROUPS_COMMON",
     "SECURITY_GROUPS_CONTENT_AUDIT",
     "SECURITY_GROUPS_USAGE_AUDIT",
     "SHIELD_ADVANCED",
     "THIRD_PARTY_FIREWALL",
     "WAF",
@@ -120,14 +129,15 @@
     "BLACK_HOLE_ROUTE_DETECTED_IN_FIREWALL_SUBNET",
     "FIREWALL_SUBNET_IS_OUT_OF_SCOPE",
     "FIREWALL_SUBNET_MISSING_EXPECTED_ROUTE",
     "FIREWALL_SUBNET_MISSING_VPCE_ENDPOINT",
     "FMS_CREATED_SECURITY_GROUP_EDITED",
     "INTERNET_GATEWAY_MISSING_EXPECTED_ROUTE",
     "INTERNET_TRAFFIC_NOT_INSPECTED",
+    "INVALID_NETWORK_ACL_ENTRY",
     "INVALID_ROUTE_CONFIGURATION",
     "MISSING_EXPECTED_ROUTE_TABLE",
     "MISSING_FIREWALL",
     "MISSING_FIREWALL_SUBNET_IN_AZ",
     "MISSING_TARGET_GATEWAY",
     "NETWORK_FIREWALL_POLICY_MODIFIED",
     "RESOURCE_INCORRECT_WEB_ACL",
@@ -168,14 +178,15 @@
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
@@ -186,14 +197,15 @@
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
@@ -211,14 +223,15 @@
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
@@ -231,24 +244,26 @@
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
@@ -309,15 +324,14 @@
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
@@ -389,17 +403,19 @@
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
@@ -444,14 +460,15 @@
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
@@ -489,19 +506,21 @@
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
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/paginator.py` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -184,13 +183,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/paginator.pyi` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,13 +174,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/type_defs.py` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+    from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeTypeDef = ...
+    data: AccountScopeOutputTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
+    EntryTypeType,
+    EntryViolationReasonType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
     MarketplaceSubscriptionOnboardingStatusType,
+    NetworkAclRuleActionType,
     OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
     ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
@@ -46,23 +49,27 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeOutputTypeDef",
+    "PolicyTypeScopeOutputTypeDef",
+    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
+    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
@@ -82,19 +89,18 @@
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "TimestampTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
+    "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetTypeDef",
+    "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
     "ListAppsListsRequestRequestTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
@@ -108,14 +114,16 @@
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
+    "NetworkAclIcmpTypeCodeTypeDef",
+    "NetworkAclPortRangeTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
@@ -124,24 +132,31 @@
     "ResourceTagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateNetworkAclActionTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
+    "ReplaceNetworkAclAssociationActionTypeDef",
+    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
+    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
+    "ProtocolsListDataTypeDef",
+    "ResourceSetTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "DisassociateThirdPartyFirewallResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAdminAccountResponseTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
@@ -151,15 +166,14 @@
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAppsListsRequestListAppsListsPaginateTypeDef",
@@ -169,56 +183,82 @@
     "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
+    "NetworkAclEntryTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
-    "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
-    "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
+    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
-    "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
+    "ListAppsListsResponseTypeDef",
+    "AppsListDataUnionTypeDef",
+    "PutAppsListRequestRequestTypeDef",
+    "ProtocolsListDataUnionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
+    "ResourceSetUnionTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
+    "EntryDescriptionTypeDef",
+    "NetworkAclEntrySetOutputTypeDef",
+    "NetworkAclEntrySetTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
-    "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
-    "RemediationActionWithOrderTypeDef",
+    "CreateNetworkAclEntriesActionTypeDef",
+    "DeleteNetworkAclEntriesActionTypeDef",
+    "EntryViolationTypeDef",
+    "NetworkAclCommonPolicyOutputTypeDef",
+    "NetworkAclCommonPolicyTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
-    "PolicyTypeDef",
+    "RemediationActionTypeDef",
+    "InvalidNetworkAclEntriesViolationTypeDef",
+    "PolicyOptionOutputTypeDef",
+    "PolicyOptionTypeDef",
+    "RemediationActionWithOrderTypeDef",
+    "SecurityServicePolicyDataOutputTypeDef",
+    "SecurityServicePolicyDataTypeDef",
     "PossibleRemediationActionTypeDef",
+    "PolicyOutputTypeDef",
+    "PolicyTypeDef",
+    "PossibleRemediationActionsTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
-    "PossibleRemediationActionsTypeDef",
+    "PolicyUnionTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeOutputTypeDef = TypedDict(
+    "AccountScopeOutputTypeDef",
+    {
+        "Accounts": NotRequired[List[str]],
+        "AllAccountsEnabled": NotRequired[bool],
+        "ExcludeSpecifiedAccounts": NotRequired[bool],
+    },
+)
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": NotRequired[List[str]],
+        "Accounts": NotRequired[Sequence[str]],
         "AllAccountsEnabled": NotRequired[bool],
         "ExcludeSpecifiedAccounts": NotRequired[bool],
     },
 )
 ActionTargetTypeDef = TypedDict(
     "ActionTargetTypeDef",
     {
@@ -230,44 +270,67 @@
     "AdminAccountSummaryTypeDef",
     {
         "AdminAccount": NotRequired[str],
         "DefaultAdmin": NotRequired[bool],
         "Status": NotRequired[OrganizationStatusType],
     },
 )
+OrganizationalUnitScopeOutputTypeDef = TypedDict(
+    "OrganizationalUnitScopeOutputTypeDef",
+    {
+        "OrganizationalUnits": NotRequired[List[str]],
+        "AllOrganizationalUnitsEnabled": NotRequired[bool],
+        "ExcludeSpecifiedOrganizationalUnits": NotRequired[bool],
+    },
+)
+PolicyTypeScopeOutputTypeDef = TypedDict(
+    "PolicyTypeScopeOutputTypeDef",
+    {
+        "PolicyTypes": NotRequired[List[SecurityServiceTypeType]],
+        "AllPolicyTypesEnabled": NotRequired[bool],
+    },
+)
+RegionScopeOutputTypeDef = TypedDict(
+    "RegionScopeOutputTypeDef",
+    {
+        "Regions": NotRequired[List[str]],
+        "AllRegionsEnabled": NotRequired[bool],
+    },
+)
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": NotRequired[List[str]],
+        "OrganizationalUnits": NotRequired[Sequence[str]],
         "AllOrganizationalUnitsEnabled": NotRequired[bool],
         "ExcludeSpecifiedOrganizationalUnits": NotRequired[bool],
     },
 )
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": NotRequired[List[SecurityServiceTypeType]],
+        "PolicyTypes": NotRequired[Sequence[SecurityServiceTypeType]],
         "AllPolicyTypesEnabled": NotRequired[bool],
     },
 )
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": NotRequired[List[str]],
+        "Regions": NotRequired[Sequence[str]],
         "AllRegionsEnabled": NotRequired[bool],
     },
 )
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
+TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
@@ -276,18 +339,18 @@
         "ThirdPartyFirewall": ThirdPartyFirewallType,
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
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "ViolatingSecurityGroups": NotRequired[List[str]],
@@ -462,24 +525,23 @@
 )
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
-TimestampTypeDef = Union[datetime, str]
 GetProtocolsListRequestRequestTypeDef = TypedDict(
     "GetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
         "DefaultList": NotRequired[bool],
     },
 )
-ProtocolsListDataTypeDef = TypedDict(
-    "ProtocolsListDataTypeDef",
+ProtocolsListDataOutputTypeDef = TypedDict(
+    "ProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
         "ListId": NotRequired[str],
         "ListUpdateToken": NotRequired[str],
         "CreateTime": NotRequired[datetime],
         "LastUpdateTime": NotRequired[datetime],
@@ -488,16 +550,16 @@
 )
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
-ResourceSetTypeDef = TypedDict(
-    "ResourceSetTypeDef",
+ResourceSetOutputTypeDef = TypedDict(
+    "ResourceSetOutputTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
         "Id": NotRequired[str],
         "Description": NotRequired[str],
         "UpdateToken": NotRequired[str],
         "LastUpdateTime": NotRequired[datetime],
@@ -666,14 +728,28 @@
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": NotRequired[str],
         "FirewallPolicyName": NotRequired[str],
     },
 )
+NetworkAclIcmpTypeCodeTypeDef = TypedDict(
+    "NetworkAclIcmpTypeCodeTypeDef",
+    {
+        "Code": NotRequired[int],
+        "Type": NotRequired[int],
+    },
+)
+NetworkAclPortRangeTypeDef = TypedDict(
+    "NetworkAclPortRangeTypeDef",
+    {
+        "From": NotRequired[int],
+        "To": NotRequired[int],
+    },
+)
 RouteTypeDef = TypedDict(
     "RouteTypeDef",
     {
         "DestinationType": NotRequired[DestinationTypeType],
         "TargetType": NotRequired[TargetTypeType],
         "Destination": NotRequired[str],
         "Target": NotRequired[str],
@@ -795,14 +871,22 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
+CreateNetworkAclActionTypeDef = TypedDict(
+    "CreateNetworkAclActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "Vpc": NotRequired[ActionTargetTypeDef],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
 EC2AssociateRouteTableActionTypeDef = TypedDict(
     "EC2AssociateRouteTableActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
         "Description": NotRequired[str],
         "SubnetId": NotRequired[ActionTargetTypeDef],
         "GatewayId": NotRequired[ActionTargetTypeDef],
@@ -860,42 +944,107 @@
     "EC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
         "Description": NotRequired[str],
     },
 )
+ReplaceNetworkAclAssociationActionTypeDef = TypedDict(
+    "ReplaceNetworkAclAssociationActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "AssociationId": NotRequired[ActionTargetTypeDef],
+        "NetworkAclId": NotRequired[ActionTargetTypeDef],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
+AdminScopeOutputTypeDef = TypedDict(
+    "AdminScopeOutputTypeDef",
+    {
+        "AccountScope": NotRequired[AccountScopeOutputTypeDef],
+        "OrganizationalUnitScope": NotRequired[OrganizationalUnitScopeOutputTypeDef],
+        "RegionScope": NotRequired[RegionScopeOutputTypeDef],
+        "PolicyTypeScope": NotRequired[PolicyTypeScopeOutputTypeDef],
+    },
+)
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": NotRequired[AccountScopeTypeDef],
         "OrganizationalUnitScope": NotRequired[OrganizationalUnitScopeTypeDef],
         "RegionScope": NotRequired[RegionScopeTypeDef],
         "PolicyTypeScope": NotRequired[PolicyTypeScopeTypeDef],
     },
 )
+AppsListDataOutputTypeDef = TypedDict(
+    "AppsListDataOutputTypeDef",
+    {
+        "ListName": str,
+        "AppsList": List[AppTypeDef],
+        "ListId": NotRequired[str],
+        "ListUpdateToken": NotRequired[str],
+        "CreateTime": NotRequired[datetime],
+        "LastUpdateTime": NotRequired[datetime],
+        "PreviousAppsList": NotRequired[Dict[str, List[AppTypeDef]]],
+    },
+)
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": NotRequired[str],
         "ListId": NotRequired[str],
         "ListName": NotRequired[str],
         "AppsList": NotRequired[List[AppTypeDef]],
     },
 )
 AppsListDataTypeDef = TypedDict(
     "AppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": Sequence[AppTypeDef],
         "ListId": NotRequired[str],
         "ListUpdateToken": NotRequired[str],
-        "CreateTime": NotRequired[datetime],
-        "LastUpdateTime": NotRequired[datetime],
-        "PreviousAppsList": NotRequired[Dict[str, List[AppTypeDef]]],
+        "CreateTime": NotRequired[TimestampTypeDef],
+        "LastUpdateTime": NotRequired[TimestampTypeDef],
+        "PreviousAppsList": NotRequired[Mapping[str, Sequence[AppTypeDef]]],
+    },
+)
+GetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "GetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+        "MemberAccountId": NotRequired[str],
+        "StartTime": NotRequired[TimestampTypeDef],
+        "EndTime": NotRequired[TimestampTypeDef],
+        "NextToken": NotRequired[str],
+        "MaxResults": NotRequired[int],
+    },
+)
+ProtocolsListDataTypeDef = TypedDict(
+    "ProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+        "ListId": NotRequired[str],
+        "ListUpdateToken": NotRequired[str],
+        "CreateTime": NotRequired[TimestampTypeDef],
+        "LastUpdateTime": NotRequired[TimestampTypeDef],
+        "PreviousProtocolsList": NotRequired[Mapping[str, Sequence[str]]],
+    },
+)
+ResourceSetTypeDef = TypedDict(
+    "ResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+        "Id": NotRequired[str],
+        "Description": NotRequired[str],
+        "UpdateToken": NotRequired[str],
+        "LastUpdateTime": NotRequired[TimestampTypeDef],
+        "ResourceSetStatus": NotRequired[ResourceSetStatusType],
     },
 )
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -932,48 +1081,48 @@
 )
 GetProtectionStatusResponseTypeDef = TypedDict(
     "GetProtectionStatusResponseTypeDef",
     {
         "AdminAccountId": str,
         "ServiceType": SecurityServiceTypeType,
         "Data": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationResponseTypeDef",
     {
         "AdminAccounts": List[AdminAccountSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAdminsManagingAccountResponseTypeDef = TypedDict(
     "ListAdminsManagingAccountResponseTypeDef",
     {
         "AdminAccounts": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMemberAccountsResponseTypeDef = TypedDict(
     "ListMemberAccountsResponseTypeDef",
     {
         "MemberAccounts": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "AwsEc2NetworkInterfaceViolations": NotRequired[
@@ -1009,16 +1158,16 @@
         "IssueInfoMap": NotRequired[Dict[DependentServiceNameType, str]],
     },
 )
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": NotRequired[str],
         "PolicyId": NotRequired[str],
@@ -1033,53 +1182,42 @@
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "ExpectedRoutes": NotRequired[List[ExpectedRouteTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
-GetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "GetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-        "MemberAccountId": NotRequired[str],
-        "StartTime": NotRequired[TimestampTypeDef],
-        "EndTime": NotRequired[TimestampTypeDef],
-        "NextToken": NotRequired[str],
-        "MaxResults": NotRequired[int],
-    },
-)
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     {
@@ -1132,76 +1270,74 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProtocolsListsResponseTypeDef = TypedDict(
     "ListProtocolsListsResponseTypeDef",
     {
         "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListResourceSetResourcesResponseTypeDef = TypedDict(
     "ListResourceSetResourcesResponseTypeDef",
     {
         "Items": List[ResourceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "ResourceSets": List[ResourceSetSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutProtocolsListRequestRequestTypeDef = TypedDict(
-    "PutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-        "TagList": NotRequired[Sequence[TagTypeDef]],
-    },
-)
-PutResourceSetRequestRequestTypeDef = TypedDict(
-    "PutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-        "TagList": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+NetworkAclEntryTypeDef = TypedDict(
+    "NetworkAclEntryTypeDef",
+    {
+        "Protocol": str,
+        "RuleAction": NetworkAclRuleActionType,
+        "Egress": bool,
+        "IcmpTypeCode": NotRequired[NetworkAclIcmpTypeCodeTypeDef],
+        "PortRange": NotRequired[NetworkAclPortRangeTypeDef],
+        "CidrBlock": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
     },
 )
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "RouteTableId": NotRequired[str],
@@ -1291,160 +1427,286 @@
     {
         "RuleGroupName": NotRequired[str],
         "ResourceId": NotRequired[str],
         "Priority": NotRequired[int],
         "Override": NotRequired[NetworkFirewallStatefulRuleGroupOverrideTypeDef],
     },
 )
-PolicyOptionTypeDef = TypedDict(
-    "PolicyOptionTypeDef",
-    {
-        "NetworkFirewallPolicy": NotRequired[NetworkFirewallPolicyTypeDef],
-        "ThirdPartyFirewallPolicy": NotRequired[ThirdPartyFirewallPolicyTypeDef],
-    },
-)
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": NotRequired[RemediationActionTypeType],
         "Description": NotRequired[str],
         "RemediationResult": NotRequired[SecurityGroupRuleDescriptionTypeDef],
         "IsDefaultAction": NotRequired[bool],
     },
 )
-RemediationActionTypeDef = TypedDict(
-    "RemediationActionTypeDef",
-    {
-        "Description": NotRequired[str],
-        "EC2CreateRouteAction": NotRequired[EC2CreateRouteActionTypeDef],
-        "EC2ReplaceRouteAction": NotRequired[EC2ReplaceRouteActionTypeDef],
-        "EC2DeleteRouteAction": NotRequired[EC2DeleteRouteActionTypeDef],
-        "EC2CopyRouteTableAction": NotRequired[EC2CopyRouteTableActionTypeDef],
-        "EC2ReplaceRouteTableAssociationAction": NotRequired[
-            EC2ReplaceRouteTableAssociationActionTypeDef
-        ],
-        "EC2AssociateRouteTableAction": NotRequired[EC2AssociateRouteTableActionTypeDef],
-        "EC2CreateRouteTableAction": NotRequired[EC2CreateRouteTableActionTypeDef],
-        "FMSPolicyUpdateFirewallCreationConfigAction": NotRequired[
-            FMSPolicyUpdateFirewallCreationConfigActionTypeDef
-        ],
-    },
-)
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeTypeDef,
+        "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 PutAdminAccountRequestRequestTypeDef = TypedDict(
     "PutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
         "AdminScope": NotRequired[AdminScopeTypeDef],
     },
 )
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
+        "AppsList": AppsListDataOutputTypeDef,
+        "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
+        "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
+    {
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 PutAppsListRequestRequestTypeDef = TypedDict(
     "PutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "TagList": NotRequired[Sequence[TagTypeDef]],
     },
 )
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
+ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
+PutProtocolsListRequestRequestTypeDef = TypedDict(
+    "PutProtocolsListRequestRequestTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
-        "AppsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProtocolsList": ProtocolsListDataTypeDef,
+        "TagList": NotRequired[Sequence[TagTypeDef]],
     },
 )
+PutResourceSetRequestRequestTypeDef = TypedDict(
+    "PutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+        "TagList": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+EntryDescriptionTypeDef = TypedDict(
+    "EntryDescriptionTypeDef",
+    {
+        "EntryDetail": NotRequired[NetworkAclEntryTypeDef],
+        "EntryRuleNumber": NotRequired[int],
+        "EntryType": NotRequired[EntryTypeType],
+    },
+)
+NetworkAclEntrySetOutputTypeDef = TypedDict(
+    "NetworkAclEntrySetOutputTypeDef",
+    {
+        "ForceRemediateForFirstEntries": bool,
+        "ForceRemediateForLastEntries": bool,
+        "FirstEntries": NotRequired[List[NetworkAclEntryTypeDef]],
+        "LastEntries": NotRequired[List[NetworkAclEntryTypeDef]],
+    },
+)
+NetworkAclEntrySetTypeDef = TypedDict(
+    "NetworkAclEntrySetTypeDef",
+    {
+        "ForceRemediateForFirstEntries": bool,
+        "ForceRemediateForLastEntries": bool,
+        "FirstEntries": NotRequired[Sequence[NetworkAclEntryTypeDef]],
+        "LastEntries": NotRequired[Sequence[NetworkAclEntryTypeDef]],
     },
 )
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": NotRequired[List[StatelessRuleGroupTypeDef]],
         "StatelessDefaultActions": NotRequired[List[str]],
         "StatelessFragmentDefaultActions": NotRequired[List[str]],
         "StatelessCustomActions": NotRequired[List[str]],
         "StatefulRuleGroups": NotRequired[List[StatefulRuleGroupTypeDef]],
         "StatefulDefaultActions": NotRequired[List[str]],
         "StatefulEngineOptions": NotRequired[StatefulEngineOptionsTypeDef],
     },
 )
-SecurityServicePolicyDataTypeDef = TypedDict(
-    "SecurityServicePolicyDataTypeDef",
-    {
-        "Type": SecurityServiceTypeType,
-        "ManagedServiceData": NotRequired[str],
-        "PolicyOption": NotRequired[PolicyOptionTypeDef],
-    },
-)
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "ViolationTargetDescription": NotRequired[str],
         "PartialMatches": NotRequired[List[PartialMatchTypeDef]],
         "PossibleSecurityGroupRemediationActions": NotRequired[
             List[SecurityGroupRemediationActionTypeDef]
         ],
     },
 )
-RemediationActionWithOrderTypeDef = TypedDict(
-    "RemediationActionWithOrderTypeDef",
+CreateNetworkAclEntriesActionTypeDef = TypedDict(
+    "CreateNetworkAclEntriesActionTypeDef",
     {
-        "RemediationAction": NotRequired[RemediationActionTypeDef],
-        "Order": NotRequired[int],
+        "Description": NotRequired[str],
+        "NetworkAclId": NotRequired[ActionTargetTypeDef],
+        "NetworkAclEntriesToBeCreated": NotRequired[List[EntryDescriptionTypeDef]],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
+DeleteNetworkAclEntriesActionTypeDef = TypedDict(
+    "DeleteNetworkAclEntriesActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "NetworkAclId": NotRequired[ActionTargetTypeDef],
+        "NetworkAclEntriesToBeDeleted": NotRequired[List[EntryDescriptionTypeDef]],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
+EntryViolationTypeDef = TypedDict(
+    "EntryViolationTypeDef",
+    {
+        "ExpectedEntry": NotRequired[EntryDescriptionTypeDef],
+        "ExpectedEvaluationOrder": NotRequired[str],
+        "ActualEvaluationOrder": NotRequired[str],
+        "EntryAtExpectedEvaluationOrder": NotRequired[EntryDescriptionTypeDef],
+        "EntriesWithConflicts": NotRequired[List[EntryDescriptionTypeDef]],
+        "EntryViolationReasons": NotRequired[List[EntryViolationReasonType]],
+    },
+)
+NetworkAclCommonPolicyOutputTypeDef = TypedDict(
+    "NetworkAclCommonPolicyOutputTypeDef",
+    {
+        "NetworkAclEntrySet": NetworkAclEntrySetOutputTypeDef,
+    },
+)
+NetworkAclCommonPolicyTypeDef = TypedDict(
+    "NetworkAclCommonPolicyTypeDef",
+    {
+        "NetworkAclEntrySet": NetworkAclEntrySetTypeDef,
     },
 )
 NetworkFirewallPolicyModifiedViolationTypeDef = TypedDict(
     "NetworkFirewallPolicyModifiedViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "CurrentPolicyDescription": NotRequired[NetworkFirewallPolicyDescriptionTypeDef],
         "ExpectedPolicyDescription": NotRequired[NetworkFirewallPolicyDescriptionTypeDef],
     },
 )
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
+RemediationActionTypeDef = TypedDict(
+    "RemediationActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "EC2CreateRouteAction": NotRequired[EC2CreateRouteActionTypeDef],
+        "EC2ReplaceRouteAction": NotRequired[EC2ReplaceRouteActionTypeDef],
+        "EC2DeleteRouteAction": NotRequired[EC2DeleteRouteActionTypeDef],
+        "EC2CopyRouteTableAction": NotRequired[EC2CopyRouteTableActionTypeDef],
+        "EC2ReplaceRouteTableAssociationAction": NotRequired[
+            EC2ReplaceRouteTableAssociationActionTypeDef
+        ],
+        "EC2AssociateRouteTableAction": NotRequired[EC2AssociateRouteTableActionTypeDef],
+        "EC2CreateRouteTableAction": NotRequired[EC2CreateRouteTableActionTypeDef],
+        "FMSPolicyUpdateFirewallCreationConfigAction": NotRequired[
+            FMSPolicyUpdateFirewallCreationConfigActionTypeDef
+        ],
+        "CreateNetworkAclAction": NotRequired[CreateNetworkAclActionTypeDef],
+        "ReplaceNetworkAclAssociationAction": NotRequired[
+            ReplaceNetworkAclAssociationActionTypeDef
+        ],
+        "CreateNetworkAclEntriesAction": NotRequired[CreateNetworkAclEntriesActionTypeDef],
+        "DeleteNetworkAclEntriesAction": NotRequired[DeleteNetworkAclEntriesActionTypeDef],
+    },
+)
+InvalidNetworkAclEntriesViolationTypeDef = TypedDict(
+    "InvalidNetworkAclEntriesViolationTypeDef",
+    {
+        "Vpc": NotRequired[str],
+        "Subnet": NotRequired[str],
+        "SubnetAvailabilityZone": NotRequired[str],
+        "CurrentAssociatedNetworkAcl": NotRequired[str],
+        "EntryViolations": NotRequired[List[EntryViolationTypeDef]],
+    },
+)
+PolicyOptionOutputTypeDef = TypedDict(
+    "PolicyOptionOutputTypeDef",
+    {
+        "NetworkFirewallPolicy": NotRequired[NetworkFirewallPolicyTypeDef],
+        "ThirdPartyFirewallPolicy": NotRequired[ThirdPartyFirewallPolicyTypeDef],
+        "NetworkAclCommonPolicy": NotRequired[NetworkAclCommonPolicyOutputTypeDef],
+    },
+)
+PolicyOptionTypeDef = TypedDict(
+    "PolicyOptionTypeDef",
+    {
+        "NetworkFirewallPolicy": NotRequired[NetworkFirewallPolicyTypeDef],
+        "ThirdPartyFirewallPolicy": NotRequired[ThirdPartyFirewallPolicyTypeDef],
+        "NetworkAclCommonPolicy": NotRequired[NetworkAclCommonPolicyTypeDef],
+    },
+)
+RemediationActionWithOrderTypeDef = TypedDict(
+    "RemediationActionWithOrderTypeDef",
+    {
+        "RemediationAction": NotRequired[RemediationActionTypeDef],
+        "Order": NotRequired[int],
+    },
+)
+SecurityServicePolicyDataOutputTypeDef = TypedDict(
+    "SecurityServicePolicyDataOutputTypeDef",
+    {
+        "Type": SecurityServiceTypeType,
+        "ManagedServiceData": NotRequired[str],
+        "PolicyOption": NotRequired[PolicyOptionOutputTypeDef],
+    },
+)
+SecurityServicePolicyDataTypeDef = TypedDict(
+    "SecurityServicePolicyDataTypeDef",
+    {
+        "Type": SecurityServiceTypeType,
+        "ManagedServiceData": NotRequired[str],
+        "PolicyOption": NotRequired[PolicyOptionTypeDef],
+    },
+)
+PossibleRemediationActionTypeDef = TypedDict(
+    "PossibleRemediationActionTypeDef",
+    {
+        "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
+        "Description": NotRequired[str],
+        "IsDefaultAction": NotRequired[bool],
+    },
+)
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
     {
         "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "SecurityServicePolicyData": SecurityServicePolicyDataOutputTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
         "PolicyId": NotRequired[str],
         "PolicyUpdateToken": NotRequired[str],
         "ResourceTypeList": NotRequired[List[str]],
         "ResourceTags": NotRequired[List[ResourceTagTypeDef]],
@@ -1452,50 +1714,63 @@
         "IncludeMap": NotRequired[Dict[CustomerPolicyScopeIdTypeType, List[str]]],
         "ExcludeMap": NotRequired[Dict[CustomerPolicyScopeIdTypeType, List[str]]],
         "ResourceSetIds": NotRequired[List[str]],
         "PolicyDescription": NotRequired[str],
         "PolicyStatus": NotRequired[CustomerPolicyStatusType],
     },
 )
-PossibleRemediationActionTypeDef = TypedDict(
-    "PossibleRemediationActionTypeDef",
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
+    {
+        "PolicyName": str,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "ResourceType": str,
+        "ExcludeResourceTags": bool,
+        "RemediationEnabled": bool,
+        "PolicyId": NotRequired[str],
+        "PolicyUpdateToken": NotRequired[str],
+        "ResourceTypeList": NotRequired[Sequence[str]],
+        "ResourceTags": NotRequired[Sequence[ResourceTagTypeDef]],
+        "DeleteUnusedFMManagedResources": NotRequired[bool],
+        "IncludeMap": NotRequired[Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]]],
+        "ExcludeMap": NotRequired[Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]]],
+        "ResourceSetIds": NotRequired[Sequence[str]],
+        "PolicyDescription": NotRequired[str],
+        "PolicyStatus": NotRequired[CustomerPolicyStatusType],
+    },
+)
+PossibleRemediationActionsTypeDef = TypedDict(
+    "PossibleRemediationActionsTypeDef",
     {
-        "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
         "Description": NotRequired[str],
-        "IsDefaultAction": NotRequired[bool],
+        "Actions": NotRequired[List[PossibleRemediationActionTypeDef]],
     },
 )
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutPolicyRequestRequestTypeDef = TypedDict(
-    "PutPolicyRequestRequestTypeDef",
-    {
-        "Policy": PolicyTypeDef,
-        "TagList": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PossibleRemediationActionsTypeDef = TypedDict(
-    "PossibleRemediationActionsTypeDef",
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
+PutPolicyRequestRequestTypeDef = TypedDict(
+    "PutPolicyRequestRequestTypeDef",
     {
-        "Description": NotRequired[str],
-        "Actions": NotRequired[List[PossibleRemediationActionTypeDef]],
+        "Policy": PolicyTypeDef,
+        "TagList": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ResourceViolationTypeDef = TypedDict(
     "ResourceViolationTypeDef",
     {
         "AwsVPCSecurityGroupViolation": NotRequired[AwsVPCSecurityGroupViolationTypeDef],
         "AwsEc2NetworkInterfaceViolation": NotRequired[AwsEc2NetworkInterfaceViolationTypeDef],
@@ -1533,15 +1808,14 @@
         "DnsRuleGroupPriorityConflictViolation": NotRequired[
             DnsRuleGroupPriorityConflictViolationTypeDef
         ],
         "DnsDuplicateRuleGroupViolation": NotRequired[DnsDuplicateRuleGroupViolationTypeDef],
         "DnsRuleGroupLimitExceededViolation": NotRequired[
             DnsRuleGroupLimitExceededViolationTypeDef
         ],
-        "PossibleRemediationActions": NotRequired[PossibleRemediationActionsTypeDef],
         "FirewallSubnetIsOutOfScopeViolation": NotRequired[
             FirewallSubnetIsOutOfScopeViolationTypeDef
         ],
         "RouteHasOutOfScopeEndpointViolation": NotRequired[
             RouteHasOutOfScopeEndpointViolationTypeDef
         ],
         "ThirdPartyFirewallMissingFirewallViolation": NotRequired[
@@ -1552,14 +1826,16 @@
         ],
         "ThirdPartyFirewallMissingExpectedRouteTableViolation": NotRequired[
             ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef
         ],
         "FirewallSubnetMissingVPCEndpointViolation": NotRequired[
             FirewallSubnetMissingVPCEndpointViolationTypeDef
         ],
+        "InvalidNetworkAclEntriesViolation": NotRequired[InvalidNetworkAclEntriesViolationTypeDef],
+        "PossibleRemediationActions": NotRequired[PossibleRemediationActionsTypeDef],
     },
 )
 ViolationDetailTypeDef = TypedDict(
     "ViolationDetailTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms/type_defs.pyi` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+    from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeTypeDef = ...
+    data: AccountScopeOutputTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
+    EntryTypeType,
+    EntryViolationReasonType,
     FailedItemReasonType,
     FirewallDeploymentModelType,
     MarketplaceSubscriptionOnboardingStatusType,
+    NetworkAclRuleActionType,
     OrganizationStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
     ResourceSetStatusType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
@@ -47,21 +50,26 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeOutputTypeDef",
+    "PolicyTypeScopeOutputTypeDef",
+    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
+    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
@@ -81,19 +89,18 @@
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "TimestampTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
+    "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetTypeDef",
+    "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
     "ListAppsListsRequestRequestTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
@@ -107,14 +114,16 @@
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
+    "NetworkAclIcmpTypeCodeTypeDef",
+    "NetworkAclPortRangeTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
@@ -123,24 +132,31 @@
     "ResourceTagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateNetworkAclActionTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
+    "ReplaceNetworkAclAssociationActionTypeDef",
+    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
+    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
+    "ProtocolsListDataTypeDef",
+    "ResourceSetTypeDef",
     "AssociateThirdPartyFirewallResponseTypeDef",
     "DisassociateThirdPartyFirewallResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAdminAccountResponseTypeDef",
     "GetNotificationChannelResponseTypeDef",
     "GetProtectionStatusResponseTypeDef",
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
@@ -150,15 +166,14 @@
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAppsListsRequestListAppsListsPaginateTypeDef",
@@ -168,56 +183,82 @@
     "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
+    "NetworkAclEntryTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
-    "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
-    "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
+    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
-    "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
+    "ListAppsListsResponseTypeDef",
+    "AppsListDataUnionTypeDef",
+    "PutAppsListRequestRequestTypeDef",
+    "ProtocolsListDataUnionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
+    "ResourceSetUnionTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
+    "EntryDescriptionTypeDef",
+    "NetworkAclEntrySetOutputTypeDef",
+    "NetworkAclEntrySetTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
-    "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
-    "RemediationActionWithOrderTypeDef",
+    "CreateNetworkAclEntriesActionTypeDef",
+    "DeleteNetworkAclEntriesActionTypeDef",
+    "EntryViolationTypeDef",
+    "NetworkAclCommonPolicyOutputTypeDef",
+    "NetworkAclCommonPolicyTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
-    "PolicyTypeDef",
+    "RemediationActionTypeDef",
+    "InvalidNetworkAclEntriesViolationTypeDef",
+    "PolicyOptionOutputTypeDef",
+    "PolicyOptionTypeDef",
+    "RemediationActionWithOrderTypeDef",
+    "SecurityServicePolicyDataOutputTypeDef",
+    "SecurityServicePolicyDataTypeDef",
     "PossibleRemediationActionTypeDef",
+    "PolicyOutputTypeDef",
+    "PolicyTypeDef",
+    "PossibleRemediationActionsTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
-    "PossibleRemediationActionsTypeDef",
+    "PolicyUnionTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeOutputTypeDef = TypedDict(
+    "AccountScopeOutputTypeDef",
+    {
+        "Accounts": NotRequired[List[str]],
+        "AllAccountsEnabled": NotRequired[bool],
+        "ExcludeSpecifiedAccounts": NotRequired[bool],
+    },
+)
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": NotRequired[List[str]],
+        "Accounts": NotRequired[Sequence[str]],
         "AllAccountsEnabled": NotRequired[bool],
         "ExcludeSpecifiedAccounts": NotRequired[bool],
     },
 )
 ActionTargetTypeDef = TypedDict(
     "ActionTargetTypeDef",
     {
@@ -229,44 +270,67 @@
     "AdminAccountSummaryTypeDef",
     {
         "AdminAccount": NotRequired[str],
         "DefaultAdmin": NotRequired[bool],
         "Status": NotRequired[OrganizationStatusType],
     },
 )
+OrganizationalUnitScopeOutputTypeDef = TypedDict(
+    "OrganizationalUnitScopeOutputTypeDef",
+    {
+        "OrganizationalUnits": NotRequired[List[str]],
+        "AllOrganizationalUnitsEnabled": NotRequired[bool],
+        "ExcludeSpecifiedOrganizationalUnits": NotRequired[bool],
+    },
+)
+PolicyTypeScopeOutputTypeDef = TypedDict(
+    "PolicyTypeScopeOutputTypeDef",
+    {
+        "PolicyTypes": NotRequired[List[SecurityServiceTypeType]],
+        "AllPolicyTypesEnabled": NotRequired[bool],
+    },
+)
+RegionScopeOutputTypeDef = TypedDict(
+    "RegionScopeOutputTypeDef",
+    {
+        "Regions": NotRequired[List[str]],
+        "AllRegionsEnabled": NotRequired[bool],
+    },
+)
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": NotRequired[List[str]],
+        "OrganizationalUnits": NotRequired[Sequence[str]],
         "AllOrganizationalUnitsEnabled": NotRequired[bool],
         "ExcludeSpecifiedOrganizationalUnits": NotRequired[bool],
     },
 )
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": NotRequired[List[SecurityServiceTypeType]],
+        "PolicyTypes": NotRequired[Sequence[SecurityServiceTypeType]],
         "AllPolicyTypesEnabled": NotRequired[bool],
     },
 )
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": NotRequired[List[str]],
+        "Regions": NotRequired[Sequence[str]],
         "AllRegionsEnabled": NotRequired[bool],
     },
 )
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
+TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
@@ -275,18 +339,18 @@
         "ThirdPartyFirewall": ThirdPartyFirewallType,
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
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "ViolatingSecurityGroups": NotRequired[List[str]],
@@ -461,24 +525,23 @@
 )
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
-TimestampTypeDef = Union[datetime, str]
 GetProtocolsListRequestRequestTypeDef = TypedDict(
     "GetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
         "DefaultList": NotRequired[bool],
     },
 )
-ProtocolsListDataTypeDef = TypedDict(
-    "ProtocolsListDataTypeDef",
+ProtocolsListDataOutputTypeDef = TypedDict(
+    "ProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
         "ListId": NotRequired[str],
         "ListUpdateToken": NotRequired[str],
         "CreateTime": NotRequired[datetime],
         "LastUpdateTime": NotRequired[datetime],
@@ -487,16 +550,16 @@
 )
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
-ResourceSetTypeDef = TypedDict(
-    "ResourceSetTypeDef",
+ResourceSetOutputTypeDef = TypedDict(
+    "ResourceSetOutputTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
         "Id": NotRequired[str],
         "Description": NotRequired[str],
         "UpdateToken": NotRequired[str],
         "LastUpdateTime": NotRequired[datetime],
@@ -665,14 +728,28 @@
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": NotRequired[str],
         "FirewallPolicyName": NotRequired[str],
     },
 )
+NetworkAclIcmpTypeCodeTypeDef = TypedDict(
+    "NetworkAclIcmpTypeCodeTypeDef",
+    {
+        "Code": NotRequired[int],
+        "Type": NotRequired[int],
+    },
+)
+NetworkAclPortRangeTypeDef = TypedDict(
+    "NetworkAclPortRangeTypeDef",
+    {
+        "From": NotRequired[int],
+        "To": NotRequired[int],
+    },
+)
 RouteTypeDef = TypedDict(
     "RouteTypeDef",
     {
         "DestinationType": NotRequired[DestinationTypeType],
         "TargetType": NotRequired[TargetTypeType],
         "Destination": NotRequired[str],
         "Target": NotRequired[str],
@@ -794,14 +871,22 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
+CreateNetworkAclActionTypeDef = TypedDict(
+    "CreateNetworkAclActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "Vpc": NotRequired[ActionTargetTypeDef],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
 EC2AssociateRouteTableActionTypeDef = TypedDict(
     "EC2AssociateRouteTableActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
         "Description": NotRequired[str],
         "SubnetId": NotRequired[ActionTargetTypeDef],
         "GatewayId": NotRequired[ActionTargetTypeDef],
@@ -859,42 +944,107 @@
     "EC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
         "Description": NotRequired[str],
     },
 )
+ReplaceNetworkAclAssociationActionTypeDef = TypedDict(
+    "ReplaceNetworkAclAssociationActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "AssociationId": NotRequired[ActionTargetTypeDef],
+        "NetworkAclId": NotRequired[ActionTargetTypeDef],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
+AdminScopeOutputTypeDef = TypedDict(
+    "AdminScopeOutputTypeDef",
+    {
+        "AccountScope": NotRequired[AccountScopeOutputTypeDef],
+        "OrganizationalUnitScope": NotRequired[OrganizationalUnitScopeOutputTypeDef],
+        "RegionScope": NotRequired[RegionScopeOutputTypeDef],
+        "PolicyTypeScope": NotRequired[PolicyTypeScopeOutputTypeDef],
+    },
+)
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": NotRequired[AccountScopeTypeDef],
         "OrganizationalUnitScope": NotRequired[OrganizationalUnitScopeTypeDef],
         "RegionScope": NotRequired[RegionScopeTypeDef],
         "PolicyTypeScope": NotRequired[PolicyTypeScopeTypeDef],
     },
 )
+AppsListDataOutputTypeDef = TypedDict(
+    "AppsListDataOutputTypeDef",
+    {
+        "ListName": str,
+        "AppsList": List[AppTypeDef],
+        "ListId": NotRequired[str],
+        "ListUpdateToken": NotRequired[str],
+        "CreateTime": NotRequired[datetime],
+        "LastUpdateTime": NotRequired[datetime],
+        "PreviousAppsList": NotRequired[Dict[str, List[AppTypeDef]]],
+    },
+)
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": NotRequired[str],
         "ListId": NotRequired[str],
         "ListName": NotRequired[str],
         "AppsList": NotRequired[List[AppTypeDef]],
     },
 )
 AppsListDataTypeDef = TypedDict(
     "AppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": Sequence[AppTypeDef],
         "ListId": NotRequired[str],
         "ListUpdateToken": NotRequired[str],
-        "CreateTime": NotRequired[datetime],
-        "LastUpdateTime": NotRequired[datetime],
-        "PreviousAppsList": NotRequired[Dict[str, List[AppTypeDef]]],
+        "CreateTime": NotRequired[TimestampTypeDef],
+        "LastUpdateTime": NotRequired[TimestampTypeDef],
+        "PreviousAppsList": NotRequired[Mapping[str, Sequence[AppTypeDef]]],
+    },
+)
+GetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "GetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+        "MemberAccountId": NotRequired[str],
+        "StartTime": NotRequired[TimestampTypeDef],
+        "EndTime": NotRequired[TimestampTypeDef],
+        "NextToken": NotRequired[str],
+        "MaxResults": NotRequired[int],
+    },
+)
+ProtocolsListDataTypeDef = TypedDict(
+    "ProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+        "ListId": NotRequired[str],
+        "ListUpdateToken": NotRequired[str],
+        "CreateTime": NotRequired[TimestampTypeDef],
+        "LastUpdateTime": NotRequired[TimestampTypeDef],
+        "PreviousProtocolsList": NotRequired[Mapping[str, Sequence[str]]],
+    },
+)
+ResourceSetTypeDef = TypedDict(
+    "ResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+        "Id": NotRequired[str],
+        "Description": NotRequired[str],
+        "UpdateToken": NotRequired[str],
+        "LastUpdateTime": NotRequired[TimestampTypeDef],
+        "ResourceSetStatus": NotRequired[ResourceSetStatusType],
     },
 )
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -931,48 +1081,48 @@
 )
 GetProtectionStatusResponseTypeDef = TypedDict(
     "GetProtectionStatusResponseTypeDef",
     {
         "AdminAccountId": str,
         "ServiceType": SecurityServiceTypeType,
         "Data": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationResponseTypeDef",
     {
         "AdminAccounts": List[AdminAccountSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAdminsManagingAccountResponseTypeDef = TypedDict(
     "ListAdminsManagingAccountResponseTypeDef",
     {
         "AdminAccounts": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMemberAccountsResponseTypeDef = TypedDict(
     "ListMemberAccountsResponseTypeDef",
     {
         "MemberAccounts": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "AwsEc2NetworkInterfaceViolations": NotRequired[
@@ -1008,16 +1158,16 @@
         "IssueInfoMap": NotRequired[Dict[DependentServiceNameType, str]],
     },
 )
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": NotRequired[str],
         "PolicyId": NotRequired[str],
@@ -1032,53 +1182,42 @@
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "ExpectedRoutes": NotRequired[List[ExpectedRouteTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
-GetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "GetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-        "MemberAccountId": NotRequired[str],
-        "StartTime": NotRequired[TimestampTypeDef],
-        "EndTime": NotRequired[TimestampTypeDef],
-        "NextToken": NotRequired[str],
-        "MaxResults": NotRequired[int],
-    },
-)
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     {
@@ -1131,76 +1270,74 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListProtocolsListsResponseTypeDef = TypedDict(
     "ListProtocolsListsResponseTypeDef",
     {
         "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListResourceSetResourcesResponseTypeDef = TypedDict(
     "ListResourceSetResourcesResponseTypeDef",
     {
         "Items": List[ResourceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "ResourceSets": List[ResourceSetSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutProtocolsListRequestRequestTypeDef = TypedDict(
-    "PutProtocolsListRequestRequestTypeDef",
-    {
-        "ProtocolsList": ProtocolsListDataTypeDef,
-        "TagList": NotRequired[Sequence[TagTypeDef]],
-    },
-)
-PutResourceSetRequestRequestTypeDef = TypedDict(
-    "PutResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSet": ResourceSetTypeDef,
-        "TagList": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+NetworkAclEntryTypeDef = TypedDict(
+    "NetworkAclEntryTypeDef",
+    {
+        "Protocol": str,
+        "RuleAction": NetworkAclRuleActionType,
+        "Egress": bool,
+        "IcmpTypeCode": NotRequired[NetworkAclIcmpTypeCodeTypeDef],
+        "PortRange": NotRequired[NetworkAclPortRangeTypeDef],
+        "CidrBlock": NotRequired[str],
+        "Ipv6CidrBlock": NotRequired[str],
     },
 )
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "RouteTableId": NotRequired[str],
@@ -1290,160 +1427,286 @@
     {
         "RuleGroupName": NotRequired[str],
         "ResourceId": NotRequired[str],
         "Priority": NotRequired[int],
         "Override": NotRequired[NetworkFirewallStatefulRuleGroupOverrideTypeDef],
     },
 )
-PolicyOptionTypeDef = TypedDict(
-    "PolicyOptionTypeDef",
-    {
-        "NetworkFirewallPolicy": NotRequired[NetworkFirewallPolicyTypeDef],
-        "ThirdPartyFirewallPolicy": NotRequired[ThirdPartyFirewallPolicyTypeDef],
-    },
-)
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": NotRequired[RemediationActionTypeType],
         "Description": NotRequired[str],
         "RemediationResult": NotRequired[SecurityGroupRuleDescriptionTypeDef],
         "IsDefaultAction": NotRequired[bool],
     },
 )
-RemediationActionTypeDef = TypedDict(
-    "RemediationActionTypeDef",
-    {
-        "Description": NotRequired[str],
-        "EC2CreateRouteAction": NotRequired[EC2CreateRouteActionTypeDef],
-        "EC2ReplaceRouteAction": NotRequired[EC2ReplaceRouteActionTypeDef],
-        "EC2DeleteRouteAction": NotRequired[EC2DeleteRouteActionTypeDef],
-        "EC2CopyRouteTableAction": NotRequired[EC2CopyRouteTableActionTypeDef],
-        "EC2ReplaceRouteTableAssociationAction": NotRequired[
-            EC2ReplaceRouteTableAssociationActionTypeDef
-        ],
-        "EC2AssociateRouteTableAction": NotRequired[EC2AssociateRouteTableActionTypeDef],
-        "EC2CreateRouteTableAction": NotRequired[EC2CreateRouteTableActionTypeDef],
-        "FMSPolicyUpdateFirewallCreationConfigAction": NotRequired[
-            FMSPolicyUpdateFirewallCreationConfigActionTypeDef
-        ],
-    },
-)
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeTypeDef,
+        "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 PutAdminAccountRequestRequestTypeDef = TypedDict(
     "PutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
         "AdminScope": NotRequired[AdminScopeTypeDef],
     },
 )
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
+        "AppsList": AppsListDataOutputTypeDef,
+        "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
+        "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
+    {
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 PutAppsListRequestRequestTypeDef = TypedDict(
     "PutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "TagList": NotRequired[Sequence[TagTypeDef]],
     },
 )
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
+ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
+PutProtocolsListRequestRequestTypeDef = TypedDict(
+    "PutProtocolsListRequestRequestTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
-        "AppsListArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProtocolsList": ProtocolsListDataTypeDef,
+        "TagList": NotRequired[Sequence[TagTypeDef]],
     },
 )
+PutResourceSetRequestRequestTypeDef = TypedDict(
+    "PutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+        "TagList": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+EntryDescriptionTypeDef = TypedDict(
+    "EntryDescriptionTypeDef",
+    {
+        "EntryDetail": NotRequired[NetworkAclEntryTypeDef],
+        "EntryRuleNumber": NotRequired[int],
+        "EntryType": NotRequired[EntryTypeType],
+    },
+)
+NetworkAclEntrySetOutputTypeDef = TypedDict(
+    "NetworkAclEntrySetOutputTypeDef",
+    {
+        "ForceRemediateForFirstEntries": bool,
+        "ForceRemediateForLastEntries": bool,
+        "FirstEntries": NotRequired[List[NetworkAclEntryTypeDef]],
+        "LastEntries": NotRequired[List[NetworkAclEntryTypeDef]],
+    },
+)
+NetworkAclEntrySetTypeDef = TypedDict(
+    "NetworkAclEntrySetTypeDef",
+    {
+        "ForceRemediateForFirstEntries": bool,
+        "ForceRemediateForLastEntries": bool,
+        "FirstEntries": NotRequired[Sequence[NetworkAclEntryTypeDef]],
+        "LastEntries": NotRequired[Sequence[NetworkAclEntryTypeDef]],
     },
 )
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": NotRequired[List[StatelessRuleGroupTypeDef]],
         "StatelessDefaultActions": NotRequired[List[str]],
         "StatelessFragmentDefaultActions": NotRequired[List[str]],
         "StatelessCustomActions": NotRequired[List[str]],
         "StatefulRuleGroups": NotRequired[List[StatefulRuleGroupTypeDef]],
         "StatefulDefaultActions": NotRequired[List[str]],
         "StatefulEngineOptions": NotRequired[StatefulEngineOptionsTypeDef],
     },
 )
-SecurityServicePolicyDataTypeDef = TypedDict(
-    "SecurityServicePolicyDataTypeDef",
-    {
-        "Type": SecurityServiceTypeType,
-        "ManagedServiceData": NotRequired[str],
-        "PolicyOption": NotRequired[PolicyOptionTypeDef],
-    },
-)
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "ViolationTargetDescription": NotRequired[str],
         "PartialMatches": NotRequired[List[PartialMatchTypeDef]],
         "PossibleSecurityGroupRemediationActions": NotRequired[
             List[SecurityGroupRemediationActionTypeDef]
         ],
     },
 )
-RemediationActionWithOrderTypeDef = TypedDict(
-    "RemediationActionWithOrderTypeDef",
+CreateNetworkAclEntriesActionTypeDef = TypedDict(
+    "CreateNetworkAclEntriesActionTypeDef",
     {
-        "RemediationAction": NotRequired[RemediationActionTypeDef],
-        "Order": NotRequired[int],
+        "Description": NotRequired[str],
+        "NetworkAclId": NotRequired[ActionTargetTypeDef],
+        "NetworkAclEntriesToBeCreated": NotRequired[List[EntryDescriptionTypeDef]],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
+DeleteNetworkAclEntriesActionTypeDef = TypedDict(
+    "DeleteNetworkAclEntriesActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "NetworkAclId": NotRequired[ActionTargetTypeDef],
+        "NetworkAclEntriesToBeDeleted": NotRequired[List[EntryDescriptionTypeDef]],
+        "FMSCanRemediate": NotRequired[bool],
+    },
+)
+EntryViolationTypeDef = TypedDict(
+    "EntryViolationTypeDef",
+    {
+        "ExpectedEntry": NotRequired[EntryDescriptionTypeDef],
+        "ExpectedEvaluationOrder": NotRequired[str],
+        "ActualEvaluationOrder": NotRequired[str],
+        "EntryAtExpectedEvaluationOrder": NotRequired[EntryDescriptionTypeDef],
+        "EntriesWithConflicts": NotRequired[List[EntryDescriptionTypeDef]],
+        "EntryViolationReasons": NotRequired[List[EntryViolationReasonType]],
+    },
+)
+NetworkAclCommonPolicyOutputTypeDef = TypedDict(
+    "NetworkAclCommonPolicyOutputTypeDef",
+    {
+        "NetworkAclEntrySet": NetworkAclEntrySetOutputTypeDef,
+    },
+)
+NetworkAclCommonPolicyTypeDef = TypedDict(
+    "NetworkAclCommonPolicyTypeDef",
+    {
+        "NetworkAclEntrySet": NetworkAclEntrySetTypeDef,
     },
 )
 NetworkFirewallPolicyModifiedViolationTypeDef = TypedDict(
     "NetworkFirewallPolicyModifiedViolationTypeDef",
     {
         "ViolationTarget": NotRequired[str],
         "CurrentPolicyDescription": NotRequired[NetworkFirewallPolicyDescriptionTypeDef],
         "ExpectedPolicyDescription": NotRequired[NetworkFirewallPolicyDescriptionTypeDef],
     },
 )
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
+RemediationActionTypeDef = TypedDict(
+    "RemediationActionTypeDef",
+    {
+        "Description": NotRequired[str],
+        "EC2CreateRouteAction": NotRequired[EC2CreateRouteActionTypeDef],
+        "EC2ReplaceRouteAction": NotRequired[EC2ReplaceRouteActionTypeDef],
+        "EC2DeleteRouteAction": NotRequired[EC2DeleteRouteActionTypeDef],
+        "EC2CopyRouteTableAction": NotRequired[EC2CopyRouteTableActionTypeDef],
+        "EC2ReplaceRouteTableAssociationAction": NotRequired[
+            EC2ReplaceRouteTableAssociationActionTypeDef
+        ],
+        "EC2AssociateRouteTableAction": NotRequired[EC2AssociateRouteTableActionTypeDef],
+        "EC2CreateRouteTableAction": NotRequired[EC2CreateRouteTableActionTypeDef],
+        "FMSPolicyUpdateFirewallCreationConfigAction": NotRequired[
+            FMSPolicyUpdateFirewallCreationConfigActionTypeDef
+        ],
+        "CreateNetworkAclAction": NotRequired[CreateNetworkAclActionTypeDef],
+        "ReplaceNetworkAclAssociationAction": NotRequired[
+            ReplaceNetworkAclAssociationActionTypeDef
+        ],
+        "CreateNetworkAclEntriesAction": NotRequired[CreateNetworkAclEntriesActionTypeDef],
+        "DeleteNetworkAclEntriesAction": NotRequired[DeleteNetworkAclEntriesActionTypeDef],
+    },
+)
+InvalidNetworkAclEntriesViolationTypeDef = TypedDict(
+    "InvalidNetworkAclEntriesViolationTypeDef",
+    {
+        "Vpc": NotRequired[str],
+        "Subnet": NotRequired[str],
+        "SubnetAvailabilityZone": NotRequired[str],
+        "CurrentAssociatedNetworkAcl": NotRequired[str],
+        "EntryViolations": NotRequired[List[EntryViolationTypeDef]],
+    },
+)
+PolicyOptionOutputTypeDef = TypedDict(
+    "PolicyOptionOutputTypeDef",
+    {
+        "NetworkFirewallPolicy": NotRequired[NetworkFirewallPolicyTypeDef],
+        "ThirdPartyFirewallPolicy": NotRequired[ThirdPartyFirewallPolicyTypeDef],
+        "NetworkAclCommonPolicy": NotRequired[NetworkAclCommonPolicyOutputTypeDef],
+    },
+)
+PolicyOptionTypeDef = TypedDict(
+    "PolicyOptionTypeDef",
+    {
+        "NetworkFirewallPolicy": NotRequired[NetworkFirewallPolicyTypeDef],
+        "ThirdPartyFirewallPolicy": NotRequired[ThirdPartyFirewallPolicyTypeDef],
+        "NetworkAclCommonPolicy": NotRequired[NetworkAclCommonPolicyTypeDef],
+    },
+)
+RemediationActionWithOrderTypeDef = TypedDict(
+    "RemediationActionWithOrderTypeDef",
+    {
+        "RemediationAction": NotRequired[RemediationActionTypeDef],
+        "Order": NotRequired[int],
+    },
+)
+SecurityServicePolicyDataOutputTypeDef = TypedDict(
+    "SecurityServicePolicyDataOutputTypeDef",
+    {
+        "Type": SecurityServiceTypeType,
+        "ManagedServiceData": NotRequired[str],
+        "PolicyOption": NotRequired[PolicyOptionOutputTypeDef],
+    },
+)
+SecurityServicePolicyDataTypeDef = TypedDict(
+    "SecurityServicePolicyDataTypeDef",
+    {
+        "Type": SecurityServiceTypeType,
+        "ManagedServiceData": NotRequired[str],
+        "PolicyOption": NotRequired[PolicyOptionTypeDef],
+    },
+)
+PossibleRemediationActionTypeDef = TypedDict(
+    "PossibleRemediationActionTypeDef",
+    {
+        "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
+        "Description": NotRequired[str],
+        "IsDefaultAction": NotRequired[bool],
+    },
+)
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
     {
         "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "SecurityServicePolicyData": SecurityServicePolicyDataOutputTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
         "PolicyId": NotRequired[str],
         "PolicyUpdateToken": NotRequired[str],
         "ResourceTypeList": NotRequired[List[str]],
         "ResourceTags": NotRequired[List[ResourceTagTypeDef]],
@@ -1451,50 +1714,63 @@
         "IncludeMap": NotRequired[Dict[CustomerPolicyScopeIdTypeType, List[str]]],
         "ExcludeMap": NotRequired[Dict[CustomerPolicyScopeIdTypeType, List[str]]],
         "ResourceSetIds": NotRequired[List[str]],
         "PolicyDescription": NotRequired[str],
         "PolicyStatus": NotRequired[CustomerPolicyStatusType],
     },
 )
-PossibleRemediationActionTypeDef = TypedDict(
-    "PossibleRemediationActionTypeDef",
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
+    {
+        "PolicyName": str,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "ResourceType": str,
+        "ExcludeResourceTags": bool,
+        "RemediationEnabled": bool,
+        "PolicyId": NotRequired[str],
+        "PolicyUpdateToken": NotRequired[str],
+        "ResourceTypeList": NotRequired[Sequence[str]],
+        "ResourceTags": NotRequired[Sequence[ResourceTagTypeDef]],
+        "DeleteUnusedFMManagedResources": NotRequired[bool],
+        "IncludeMap": NotRequired[Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]]],
+        "ExcludeMap": NotRequired[Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]]],
+        "ResourceSetIds": NotRequired[Sequence[str]],
+        "PolicyDescription": NotRequired[str],
+        "PolicyStatus": NotRequired[CustomerPolicyStatusType],
+    },
+)
+PossibleRemediationActionsTypeDef = TypedDict(
+    "PossibleRemediationActionsTypeDef",
     {
-        "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
         "Description": NotRequired[str],
-        "IsDefaultAction": NotRequired[bool],
+        "Actions": NotRequired[List[PossibleRemediationActionTypeDef]],
     },
 )
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutPolicyRequestRequestTypeDef = TypedDict(
-    "PutPolicyRequestRequestTypeDef",
-    {
-        "Policy": PolicyTypeDef,
-        "TagList": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PossibleRemediationActionsTypeDef = TypedDict(
-    "PossibleRemediationActionsTypeDef",
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
+PutPolicyRequestRequestTypeDef = TypedDict(
+    "PutPolicyRequestRequestTypeDef",
     {
-        "Description": NotRequired[str],
-        "Actions": NotRequired[List[PossibleRemediationActionTypeDef]],
+        "Policy": PolicyTypeDef,
+        "TagList": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ResourceViolationTypeDef = TypedDict(
     "ResourceViolationTypeDef",
     {
         "AwsVPCSecurityGroupViolation": NotRequired[AwsVPCSecurityGroupViolationTypeDef],
         "AwsEc2NetworkInterfaceViolation": NotRequired[AwsEc2NetworkInterfaceViolationTypeDef],
@@ -1532,15 +1808,14 @@
         "DnsRuleGroupPriorityConflictViolation": NotRequired[
             DnsRuleGroupPriorityConflictViolationTypeDef
         ],
         "DnsDuplicateRuleGroupViolation": NotRequired[DnsDuplicateRuleGroupViolationTypeDef],
         "DnsRuleGroupLimitExceededViolation": NotRequired[
             DnsRuleGroupLimitExceededViolationTypeDef
         ],
-        "PossibleRemediationActions": NotRequired[PossibleRemediationActionsTypeDef],
         "FirewallSubnetIsOutOfScopeViolation": NotRequired[
             FirewallSubnetIsOutOfScopeViolationTypeDef
         ],
         "RouteHasOutOfScopeEndpointViolation": NotRequired[
             RouteHasOutOfScopeEndpointViolationTypeDef
         ],
         "ThirdPartyFirewallMissingFirewallViolation": NotRequired[
@@ -1551,14 +1826,16 @@
         ],
         "ThirdPartyFirewallMissingExpectedRouteTableViolation": NotRequired[
             ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef
         ],
         "FirewallSubnetMissingVPCEndpointViolation": NotRequired[
             FirewallSubnetMissingVPCEndpointViolationTypeDef
         ],
+        "InvalidNetworkAclEntriesViolation": NotRequired[InvalidNetworkAclEntriesViolationTypeDef],
+        "PossibleRemediationActions": NotRequired[PossibleRemediationActionsTypeDef],
     },
 )
 ViolationDetailTypeDef = TypedDict(
     "ViolationDetailTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.34.0
-Summary: Type annotations for boto3.FMS 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.92
+Summary: Type annotations for boto3.FMS 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
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
 
 <a id="mypy-boto3-fms"></a>
 
 # mypy-boto3-fms
 
 [![PyPI - mypy-boto3-fms](https://img.shields.io/pypi/v/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,18 +343,18 @@
 `mypy_boto3_fms.type_defs` module contains structures and shapes assembled to
 typed dictionaries and unions for additional type checking.
 
 Full list of `FMS` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/type_defs/).
 
 ```python
-from mypy_boto3_fms.type_defs import AccountScopeTypeDef
+from mypy_boto3_fms.type_defs import AccountScopeOutputTypeDef
 
 
-def get_value() -> AccountScopeTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fms-1.34.0/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy_boto3_fms-1.34.92/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.34.0/setup.py` & `mypy_boto3_fms-1.34.92/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.34.0",
+    version="1.34.92",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.FMS 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.FMS 1.34.92 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 fms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_fms": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```


# Comparing `tmp/mypy-boto3-ivs-1.34.78.tar.gz` & `tmp/mypy_boto3_ivs-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.34.78.tar", last modified: Thu Apr  4 19:33:17 2024, max compression
+gzip compressed data, was "mypy_boto3_ivs-1.34.92.tar", last modified: Thu Apr 25 19:32:15 2024, max compression
```

## Comparing `mypy-boto3-ivs-1.34.78.tar` & `mypy_boto3_ivs-1.34.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.792019 mypy-boto3-ivs-1.34.78/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-04 19:33:17.792019 mypy-boto3-ivs-1.34.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.788019 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26395 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26392 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-04 19:33:03.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.788019 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:17.792019 mypy-boto3-ivs-1.34.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.031410 mypy_boto3_ivs-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-25 19:32:15.031410 mypy_boto3_ivs-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.031410 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-04-25 19:31:49.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26412 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-25 19:31:49.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-25 19:31:49.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-25 19:31:49.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-25 19:31:49.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29202 2024-04-25 19:31:50.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29202 2024-04-25 19:31:50.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:15.031410 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-25 19:32:14.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 19:32:14.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:14.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:32:14.000000 mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:15.031410 mypy_boto3_ivs-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-25 19:31:48.000000 mypy_boto3_ivs-1.34.92/setup.py
```

### Comparing `mypy-boto3-ivs-1.34.78/LICENSE` & `mypy_boto3_ivs-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.78/PKG-INFO` & `mypy_boto3_ivs-1.34.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.34.78
-Summary: Type annotations for boto3.IVS 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3.IVS 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.34.78/README.md` & `mypy_boto3_ivs-1.34.92/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.py` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.pyi` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__main__.py` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.34.78\n"
-        "Version:         1.34.78\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.IVS 1.34.92\n"
+        "Version:         1.34.92\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.78")
+    print("1.34.92")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.py` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
     ListPlaybackKeyPairsResponseTypeDef,
     ListPlaybackRestrictionPoliciesResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    RenditionConfigurationTypeDef,
+    RenditionConfigurationUnionTypeDef,
     StreamFiltersTypeDef,
-    ThumbnailConfigurationTypeDef,
+    ThumbnailConfigurationUnionTypeDef,
     UpdateChannelResponseTypeDef,
     UpdatePlaybackRestrictionPolicyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -192,17 +192,17 @@
 
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
-        renditionConfiguration: RenditionConfigurationTypeDef = ...,
+        renditionConfiguration: RenditionConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...,
+        thumbnailConfiguration: ThumbnailConfigurationUnionTypeDef = ...,
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#create_recording_configuration)
         """
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.pyi` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
     ListPlaybackKeyPairsResponseTypeDef,
     ListPlaybackRestrictionPoliciesResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    RenditionConfigurationTypeDef,
+    RenditionConfigurationUnionTypeDef,
     StreamFiltersTypeDef,
-    ThumbnailConfigurationTypeDef,
+    ThumbnailConfigurationUnionTypeDef,
     UpdateChannelResponseTypeDef,
     UpdatePlaybackRestrictionPolicyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -189,17 +189,17 @@
 
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
-        renditionConfiguration: RenditionConfigurationTypeDef = ...,
+        renditionConfiguration: RenditionConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...,
+        thumbnailConfiguration: ThumbnailConfigurationUnionTypeDef = ...,
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/client/#create_recording_configuration)
         """
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.py` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
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
@@ -363,14 +364,15 @@
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
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.pyi` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
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
@@ -363,14 +364,15 @@
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
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.py` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.pyi` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.py` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AudioConfigurationTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
     RenditionConfigurationRenditionSelectionType,
@@ -84,14 +84,16 @@
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutMetadataRequestRequestTypeDef",
+    "RenditionConfigurationOutputTypeDef",
+    "ThumbnailConfigurationOutputTypeDef",
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdatePlaybackRestrictionPolicyRequestRequestTypeDef",
@@ -119,14 +121,16 @@
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListPlaybackRestrictionPoliciesResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
+    "RenditionConfigurationUnionTypeDef",
+    "ThumbnailConfigurationUnionTypeDef",
     "BatchGetChannelResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
@@ -520,14 +524,30 @@
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
+RenditionConfigurationOutputTypeDef = TypedDict(
+    "RenditionConfigurationOutputTypeDef",
+    {
+        "renditionSelection": NotRequired[RenditionConfigurationRenditionSelectionType],
+        "renditions": NotRequired[List[RenditionConfigurationRenditionType]],
+    },
+)
+ThumbnailConfigurationOutputTypeDef = TypedDict(
+    "ThumbnailConfigurationOutputTypeDef",
+    {
+        "recordingMode": NotRequired[RecordingModeType],
+        "resolution": NotRequired[ThumbnailConfigurationResolutionType],
+        "storage": NotRequired[List[ThumbnailConfigurationStorageType]],
+        "targetIntervalSeconds": NotRequired[int],
+    },
+)
 StartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "StartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
         "viewerSessionVersionsLessThanOrEqualTo": NotRequired[int],
     },
@@ -792,14 +812,20 @@
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RenditionConfigurationUnionTypeDef = Union[
+    RenditionConfigurationTypeDef, RenditionConfigurationOutputTypeDef
+]
+ThumbnailConfigurationUnionTypeDef = Union[
+    ThumbnailConfigurationTypeDef, ThumbnailConfigurationOutputTypeDef
+]
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -851,17 +877,17 @@
     "RecordingConfigurationTypeDef",
     {
         "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "state": RecordingConfigurationStateType,
         "name": NotRequired[str],
         "recordingReconnectWindowSeconds": NotRequired[int],
-        "renditionConfiguration": NotRequired[RenditionConfigurationTypeDef],
+        "renditionConfiguration": NotRequired[RenditionConfigurationOutputTypeDef],
         "tags": NotRequired[Dict[str, str]],
-        "thumbnailConfiguration": NotRequired[ThumbnailConfigurationTypeDef],
+        "thumbnailConfiguration": NotRequired[ThumbnailConfigurationOutputTypeDef],
     },
 )
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.pyi` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AudioConfigurationTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
     RenditionConfigurationRenditionSelectionType,
@@ -84,14 +84,16 @@
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutMetadataRequestRequestTypeDef",
+    "RenditionConfigurationOutputTypeDef",
+    "ThumbnailConfigurationOutputTypeDef",
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdatePlaybackRestrictionPolicyRequestRequestTypeDef",
@@ -119,14 +121,16 @@
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListPlaybackRestrictionPoliciesResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
+    "RenditionConfigurationUnionTypeDef",
+    "ThumbnailConfigurationUnionTypeDef",
     "BatchGetChannelResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
@@ -520,14 +524,30 @@
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
+RenditionConfigurationOutputTypeDef = TypedDict(
+    "RenditionConfigurationOutputTypeDef",
+    {
+        "renditionSelection": NotRequired[RenditionConfigurationRenditionSelectionType],
+        "renditions": NotRequired[List[RenditionConfigurationRenditionType]],
+    },
+)
+ThumbnailConfigurationOutputTypeDef = TypedDict(
+    "ThumbnailConfigurationOutputTypeDef",
+    {
+        "recordingMode": NotRequired[RecordingModeType],
+        "resolution": NotRequired[ThumbnailConfigurationResolutionType],
+        "storage": NotRequired[List[ThumbnailConfigurationStorageType]],
+        "targetIntervalSeconds": NotRequired[int],
+    },
+)
 StartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "StartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
         "viewerSessionVersionsLessThanOrEqualTo": NotRequired[int],
     },
@@ -792,14 +812,20 @@
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RenditionConfigurationUnionTypeDef = Union[
+    RenditionConfigurationTypeDef, RenditionConfigurationOutputTypeDef
+]
+ThumbnailConfigurationUnionTypeDef = Union[
+    ThumbnailConfigurationTypeDef, ThumbnailConfigurationOutputTypeDef
+]
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -851,17 +877,17 @@
     "RecordingConfigurationTypeDef",
     {
         "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "state": RecordingConfigurationStateType,
         "name": NotRequired[str],
         "recordingReconnectWindowSeconds": NotRequired[int],
-        "renditionConfiguration": NotRequired[RenditionConfigurationTypeDef],
+        "renditionConfiguration": NotRequired[RenditionConfigurationOutputTypeDef],
         "tags": NotRequired[Dict[str, str]],
-        "thumbnailConfiguration": NotRequired[ThumbnailConfigurationTypeDef],
+        "thumbnailConfiguration": NotRequired[ThumbnailConfigurationOutputTypeDef],
     },
 )
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.34.78
-Summary: Type annotations for boto3.IVS 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.92
+Summary: Type annotations for boto3.IVS 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy_boto3_ivs-1.34.92/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.78/setup.py` & `mypy_boto3_ivs-1.34.92/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.34.78",
+    version="1.34.92",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.IVS 1.34.78 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.IVS 1.34.92 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


# Comparing `tmp/mypy-boto3-appsync-1.34.49.tar.gz` & `tmp/mypy_boto3_appsync-1.34.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appsync-1.34.49.tar", last modified: Fri Feb 23 20:23:11 2024, max compression
+gzip compressed data, was "mypy_boto3_appsync-1.34.92.tar", last modified: Thu Apr 25 19:32:14 2024, max compression
```

## Comparing `mypy-boto3-appsync-1.34.49.tar` & `mypy_boto3_appsync-1.34.92.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:23:11.427993 mypy-boto3-appsync-1.34.49/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-02-23 20:23:11.427993 mypy-boto3-appsync-1.34.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:23:11.427993 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46977 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46974 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    55088 2024-02-23 20:22:49.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55088 2024-02-23 20:22:48.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:23:11.427993 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-02-23 20:23:11.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-23 20:23:11.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 20:23:11.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 20:23:11.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-23 20:23:11.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-23 20:23:11.000000 mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 20:23:11.427993 mypy-boto3-appsync-1.34.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-23 20:22:47.000000 mypy-boto3-appsync-1.34.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.319404 mypy_boto3_appsync-1.34.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-25 19:32:14.319404 mypy_boto3_appsync-1.34.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.319404 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47001 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46998 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-25 19:31:45.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-25 19:31:45.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-04-25 19:31:45.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-25 19:31:45.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54289 2024-04-25 19:31:46.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54289 2024-04-25 19:31:45.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:14.319404 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-25 19:32:14.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-25 19:32:14.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:32:14.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:14.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 19:32:14.000000 mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:32:14.319404 mypy_boto3_appsync-1.34.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-25 19:31:44.000000 mypy_boto3_appsync-1.34.92/setup.py
```

### Comparing `mypy-boto3-appsync-1.34.49/LICENSE` & `mypy_boto3_appsync-1.34.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.34.49/PKG-INFO` & `mypy_boto3_appsync-1.34.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.34.49
-Summary: Type annotations for boto3.AppSync 1.34.49 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.92
+Summary: Type annotations for boto3.AppSync 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appsync)](https://pepy.tech/project/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.34.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appsync-1.34.49/README.md` & `mypy_boto3_appsync-1.34.92/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appsync)](https://pepy.tech/project/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.34.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/__init__.py` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/__init__.pyi` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/__main__.py` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppSync 1.34.49\n"
-        "Version:         1.34.49\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.AppSync 1.34.92\n"
+        "Version:         1.34.92\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.49")
+    print("1.34.92")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/client.py` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     BlobTypeDef,
-    CachingConfigTypeDef,
+    CachingConfigUnionTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -94,15 +94,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigTypeDef,
+    PipelineConfigUnionTypeDef,
     PutGraphqlApiEnvironmentVariablesResponseTypeDef,
     RdsDataApiConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartDataSourceIntrospectionResponseTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
@@ -343,17 +343,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...,
         metricsConfig: ResolverLevelMetricsConfigType = ...,
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
@@ -897,16 +897,16 @@
         """
 
     def update_graphql_api(
         self,
         *,
         apiId: str,
         name: str,
+        authenticationType: AuthenticationTypeType,
         logConfig: LogConfigTypeDef = ...,
-        authenticationType: AuthenticationTypeType = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
         lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
         mergedApiExecutionRoleArn: str = ...,
         ownerContact: str = ...,
@@ -928,17 +928,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...,
         metricsConfig: ResolverLevelMetricsConfigType = ...,
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/client.pyi` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     BlobTypeDef,
-    CachingConfigTypeDef,
+    CachingConfigUnionTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -94,15 +94,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigTypeDef,
+    PipelineConfigUnionTypeDef,
     PutGraphqlApiEnvironmentVariablesResponseTypeDef,
     RdsDataApiConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartDataSourceIntrospectionResponseTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
@@ -340,17 +340,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...,
         metricsConfig: ResolverLevelMetricsConfigType = ...,
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
@@ -894,16 +894,16 @@
         """
 
     def update_graphql_api(
         self,
         *,
         apiId: str,
         name: str,
+        authenticationType: AuthenticationTypeType,
         logConfig: LogConfigTypeDef = ...,
-        authenticationType: AuthenticationTypeType = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
         lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
         mergedApiExecutionRoleArn: str = ...,
         ownerContact: str = ...,
@@ -925,17 +925,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...,
         metricsConfig: ResolverLevelMetricsConfigType = ...,
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/literals.py` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,15 @@
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
@@ -229,24 +230,26 @@
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
@@ -307,15 +310,14 @@
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
@@ -444,14 +446,15 @@
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
@@ -495,14 +498,15 @@
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

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/literals.pyi` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,15 @@
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
@@ -229,24 +230,26 @@
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
@@ -307,15 +310,14 @@
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
@@ -444,14 +446,15 @@
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
@@ -495,14 +498,15 @@
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

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/paginator.py` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 from .literals import GraphQLApiTypeType, OwnershipType, TypeDefinitionFormatType
 from .type_defs import (
     ListApiKeysResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListGraphqlApisResponseTypeDef,
-    ListResolversByFunctionResponsePaginatorTypeDef,
-    ListResolversResponsePaginatorTypeDef,
+    ListResolversByFunctionResponseTypeDef,
+    ListResolversResponseTypeDef,
     ListTypesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListApiKeysPaginator",
     "ListDataSourcesPaginator",
@@ -136,30 +136,30 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
     """
 
     def paginate(
         self, *, apiId: str, typeName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResolversResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListResolversResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
         """
 
 
 class ListResolversByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
     """
 
     def paginate(
         self, *, apiId: str, functionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResolversByFunctionResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListResolversByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
         """
 
 
 class ListTypesPaginator(Paginator):
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/paginator.pyi` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 from .literals import GraphQLApiTypeType, OwnershipType, TypeDefinitionFormatType
 from .type_defs import (
     ListApiKeysResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListGraphqlApisResponseTypeDef,
-    ListResolversByFunctionResponsePaginatorTypeDef,
-    ListResolversResponsePaginatorTypeDef,
+    ListResolversByFunctionResponseTypeDef,
+    ListResolversResponseTypeDef,
     ListTypesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListApiKeysPaginator",
     "ListDataSourcesPaginator",
@@ -130,29 +130,29 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
     """
 
     def paginate(
         self, *, apiId: str, typeName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResolversResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListResolversResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
         """
 
 class ListResolversByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
     """
 
     def paginate(
         self, *, apiId: str, functionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResolversByFunctionResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListResolversByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
         """
 
 class ListTypesPaginator(Paginator):
     """
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/type_defs.py` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
     "BlobTypeDef",
-    "CachingConfigPaginatorTypeDef",
+    "CachingConfigExtraOutputTypeDef",
+    "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
@@ -132,15 +133,16 @@
     "ListResolversByFunctionRequestRequestTypeDef",
     "ListResolversRequestRequestTypeDef",
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
     "ListTypesRequestRequestTypeDef",
-    "PipelineConfigPaginatorTypeDef",
+    "PipelineConfigExtraOutputTypeDef",
+    "PipelineConfigOutputTypeDef",
     "PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef",
     "RdsDataApiConfigTypeDef",
     "RdsHttpEndpointConfigTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
@@ -169,14 +171,15 @@
     "UpdateApiKeyResponseTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
     "StartSchemaCreationRequestRequestTypeDef",
+    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
@@ -191,14 +194,15 @@
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversRequestListResolversPaginateTypeDef",
     "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
+    "PipelineConfigUnionTypeDef",
     "StartDataSourceIntrospectionRequestRequestTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
@@ -206,15 +210,14 @@
     "UpdateSourceApiAssociationResponseTypeDef",
     "HttpDataSourceConfigTypeDef",
     "EvaluateCodeErrorDetailTypeDef",
     "DataSourceIntrospectionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "CreateResolverRequestRequestTypeDef",
     "FunctionConfigurationTypeDef",
-    "ResolverPaginatorTypeDef",
     "ResolverTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "UpdateResolverRequestRequestTypeDef",
     "CreateGraphqlApiResponseTypeDef",
     "GetGraphqlApiResponseTypeDef",
     "ListGraphqlApisResponseTypeDef",
     "UpdateGraphqlApiResponseTypeDef",
@@ -223,16 +226,14 @@
     "UpdateDataSourceRequestRequestTypeDef",
     "EvaluateCodeResponseTypeDef",
     "GetDataSourceIntrospectionResponseTypeDef",
     "CreateFunctionResponseTypeDef",
     "GetFunctionResponseTypeDef",
     "ListFunctionsResponseTypeDef",
     "UpdateFunctionResponseTypeDef",
-    "ListResolversByFunctionResponsePaginatorTypeDef",
-    "ListResolversResponsePaginatorTypeDef",
     "CreateResolverResponseTypeDef",
     "GetResolverResponseTypeDef",
     "ListResolversByFunctionResponseTypeDef",
     "ListResolversResponseTypeDef",
     "UpdateResolverResponseTypeDef",
     "CreateDataSourceResponseTypeDef",
     "GetDataSourceResponseTypeDef",
@@ -309,18 +310,18 @@
         "apiId": str,
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
 SourceApiAssociationConfigTypeDef = TypedDict(
     "SourceApiAssociationConfigTypeDef",
     {
         "mergeType": NotRequired[MergeTypeType],
     },
@@ -329,16 +330,23 @@
     "AwsIamConfigTypeDef",
     {
         "signingRegion": NotRequired[str],
         "signingServiceName": NotRequired[str],
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-CachingConfigPaginatorTypeDef = TypedDict(
-    "CachingConfigPaginatorTypeDef",
+CachingConfigExtraOutputTypeDef = TypedDict(
+    "CachingConfigExtraOutputTypeDef",
+    {
+        "ttl": int,
+        "cachingKeys": NotRequired[List[str]],
+    },
+)
+CachingConfigOutputTypeDef = TypedDict(
+    "CachingConfigOutputTypeDef",
     {
         "ttl": int,
         "cachingKeys": NotRequired[List[str]],
     },
 )
 CachingConfigTypeDef = TypedDict(
     "CachingConfigTypeDef",
@@ -796,16 +804,22 @@
     {
         "apiId": str,
         "format": TypeDefinitionFormatType,
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
 )
-PipelineConfigPaginatorTypeDef = TypedDict(
-    "PipelineConfigPaginatorTypeDef",
+PipelineConfigExtraOutputTypeDef = TypedDict(
+    "PipelineConfigExtraOutputTypeDef",
+    {
+        "functions": NotRequired[List[str]],
+    },
+)
+PipelineConfigOutputTypeDef = TypedDict(
+    "PipelineConfigOutputTypeDef",
     {
         "functions": NotRequired[List[str]],
     },
 )
 PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef = TypedDict(
     "PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef",
     {
@@ -1088,14 +1102,15 @@
 StartSchemaCreationRequestRequestTypeDef = TypedDict(
     "StartSchemaCreationRequestRequestTypeDef",
     {
         "apiId": str,
         "definition": BlobTypeDef,
     },
 )
+CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigExtraOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": NotRequired[str],
         "value": NotRequired[str],
         "location": NotRequired[CodeErrorLocationTypeDef],
     },
@@ -1260,14 +1275,15 @@
     "ListSourceApiAssociationsResponseTypeDef",
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigExtraOutputTypeDef]
 StartDataSourceIntrospectionRequestRequestTypeDef = TypedDict(
     "StartDataSourceIntrospectionRequestRequestTypeDef",
     {
         "rdsDataApiConfig": NotRequired[RdsDataApiConfigTypeDef],
     },
 )
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
@@ -1332,16 +1348,16 @@
     },
 )
 UpdateGraphqlApiRequestRequestTypeDef = TypedDict(
     "UpdateGraphqlApiRequestRequestTypeDef",
     {
         "apiId": str,
         "name": str,
+        "authenticationType": AuthenticationTypeType,
         "logConfig": NotRequired[LogConfigTypeDef],
-        "authenticationType": NotRequired[AuthenticationTypeType],
         "userPoolConfig": NotRequired[UserPoolConfigTypeDef],
         "openIDConnectConfig": NotRequired[OpenIDConnectConfigTypeDef],
         "additionalAuthenticationProviders": NotRequired[
             Sequence[AdditionalAuthenticationProviderTypeDef]
         ],
         "xrayEnabled": NotRequired[bool],
         "lambdaAuthorizerConfig": NotRequired[LambdaAuthorizerConfigTypeDef],
@@ -1450,46 +1466,27 @@
         "functionVersion": NotRequired[str],
         "syncConfig": NotRequired[SyncConfigTypeDef],
         "maxBatchSize": NotRequired[int],
         "runtime": NotRequired[AppSyncRuntimeTypeDef],
         "code": NotRequired[str],
     },
 )
-ResolverPaginatorTypeDef = TypedDict(
-    "ResolverPaginatorTypeDef",
-    {
-        "typeName": NotRequired[str],
-        "fieldName": NotRequired[str],
-        "dataSourceName": NotRequired[str],
-        "resolverArn": NotRequired[str],
-        "requestMappingTemplate": NotRequired[str],
-        "responseMappingTemplate": NotRequired[str],
-        "kind": NotRequired[ResolverKindType],
-        "pipelineConfig": NotRequired[PipelineConfigPaginatorTypeDef],
-        "syncConfig": NotRequired[SyncConfigTypeDef],
-        "cachingConfig": NotRequired[CachingConfigPaginatorTypeDef],
-        "maxBatchSize": NotRequired[int],
-        "runtime": NotRequired[AppSyncRuntimeTypeDef],
-        "code": NotRequired[str],
-        "metricsConfig": NotRequired[ResolverLevelMetricsConfigType],
-    },
-)
 ResolverTypeDef = TypedDict(
     "ResolverTypeDef",
     {
         "typeName": NotRequired[str],
         "fieldName": NotRequired[str],
         "dataSourceName": NotRequired[str],
         "resolverArn": NotRequired[str],
         "requestMappingTemplate": NotRequired[str],
         "responseMappingTemplate": NotRequired[str],
         "kind": NotRequired[ResolverKindType],
-        "pipelineConfig": NotRequired[PipelineConfigTypeDef],
+        "pipelineConfig": NotRequired[PipelineConfigOutputTypeDef],
         "syncConfig": NotRequired[SyncConfigTypeDef],
-        "cachingConfig": NotRequired[CachingConfigTypeDef],
+        "cachingConfig": NotRequired[CachingConfigOutputTypeDef],
         "maxBatchSize": NotRequired[int],
         "runtime": NotRequired[AppSyncRuntimeTypeDef],
         "code": NotRequired[str],
         "metricsConfig": NotRequired[ResolverLevelMetricsConfigType],
     },
 )
 UpdateFunctionRequestRequestTypeDef = TypedDict(
@@ -1655,30 +1652,14 @@
 UpdateFunctionResponseTypeDef = TypedDict(
     "UpdateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListResolversByFunctionResponsePaginatorTypeDef = TypedDict(
-    "ListResolversByFunctionResponsePaginatorTypeDef",
-    {
-        "resolvers": List[ResolverPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListResolversResponsePaginatorTypeDef = TypedDict(
-    "ListResolversResponsePaginatorTypeDef",
-    {
-        "resolvers": List[ResolverPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateResolverResponseTypeDef = TypedDict(
     "CreateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync/type_defs.pyi` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
     "BlobTypeDef",
-    "CachingConfigPaginatorTypeDef",
+    "CachingConfigExtraOutputTypeDef",
+    "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
@@ -132,15 +133,16 @@
     "ListResolversByFunctionRequestRequestTypeDef",
     "ListResolversRequestRequestTypeDef",
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
     "ListTypesRequestRequestTypeDef",
-    "PipelineConfigPaginatorTypeDef",
+    "PipelineConfigExtraOutputTypeDef",
+    "PipelineConfigOutputTypeDef",
     "PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef",
     "RdsDataApiConfigTypeDef",
     "RdsHttpEndpointConfigTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
@@ -169,14 +171,15 @@
     "UpdateApiKeyResponseTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
     "StartSchemaCreationRequestRequestTypeDef",
+    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
@@ -191,14 +194,15 @@
     "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversRequestListResolversPaginateTypeDef",
     "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
+    "PipelineConfigUnionTypeDef",
     "StartDataSourceIntrospectionRequestRequestTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
@@ -206,15 +210,14 @@
     "UpdateSourceApiAssociationResponseTypeDef",
     "HttpDataSourceConfigTypeDef",
     "EvaluateCodeErrorDetailTypeDef",
     "DataSourceIntrospectionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "CreateResolverRequestRequestTypeDef",
     "FunctionConfigurationTypeDef",
-    "ResolverPaginatorTypeDef",
     "ResolverTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "UpdateResolverRequestRequestTypeDef",
     "CreateGraphqlApiResponseTypeDef",
     "GetGraphqlApiResponseTypeDef",
     "ListGraphqlApisResponseTypeDef",
     "UpdateGraphqlApiResponseTypeDef",
@@ -223,16 +226,14 @@
     "UpdateDataSourceRequestRequestTypeDef",
     "EvaluateCodeResponseTypeDef",
     "GetDataSourceIntrospectionResponseTypeDef",
     "CreateFunctionResponseTypeDef",
     "GetFunctionResponseTypeDef",
     "ListFunctionsResponseTypeDef",
     "UpdateFunctionResponseTypeDef",
-    "ListResolversByFunctionResponsePaginatorTypeDef",
-    "ListResolversResponsePaginatorTypeDef",
     "CreateResolverResponseTypeDef",
     "GetResolverResponseTypeDef",
     "ListResolversByFunctionResponseTypeDef",
     "ListResolversResponseTypeDef",
     "UpdateResolverResponseTypeDef",
     "CreateDataSourceResponseTypeDef",
     "GetDataSourceResponseTypeDef",
@@ -309,18 +310,18 @@
         "apiId": str,
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
 SourceApiAssociationConfigTypeDef = TypedDict(
     "SourceApiAssociationConfigTypeDef",
     {
         "mergeType": NotRequired[MergeTypeType],
     },
@@ -329,16 +330,23 @@
     "AwsIamConfigTypeDef",
     {
         "signingRegion": NotRequired[str],
         "signingServiceName": NotRequired[str],
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-CachingConfigPaginatorTypeDef = TypedDict(
-    "CachingConfigPaginatorTypeDef",
+CachingConfigExtraOutputTypeDef = TypedDict(
+    "CachingConfigExtraOutputTypeDef",
+    {
+        "ttl": int,
+        "cachingKeys": NotRequired[List[str]],
+    },
+)
+CachingConfigOutputTypeDef = TypedDict(
+    "CachingConfigOutputTypeDef",
     {
         "ttl": int,
         "cachingKeys": NotRequired[List[str]],
     },
 )
 CachingConfigTypeDef = TypedDict(
     "CachingConfigTypeDef",
@@ -796,16 +804,22 @@
     {
         "apiId": str,
         "format": TypeDefinitionFormatType,
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
 )
-PipelineConfigPaginatorTypeDef = TypedDict(
-    "PipelineConfigPaginatorTypeDef",
+PipelineConfigExtraOutputTypeDef = TypedDict(
+    "PipelineConfigExtraOutputTypeDef",
+    {
+        "functions": NotRequired[List[str]],
+    },
+)
+PipelineConfigOutputTypeDef = TypedDict(
+    "PipelineConfigOutputTypeDef",
     {
         "functions": NotRequired[List[str]],
     },
 )
 PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef = TypedDict(
     "PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef",
     {
@@ -1088,14 +1102,15 @@
 StartSchemaCreationRequestRequestTypeDef = TypedDict(
     "StartSchemaCreationRequestRequestTypeDef",
     {
         "apiId": str,
         "definition": BlobTypeDef,
     },
 )
+CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigExtraOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": NotRequired[str],
         "value": NotRequired[str],
         "location": NotRequired[CodeErrorLocationTypeDef],
     },
@@ -1260,14 +1275,15 @@
     "ListSourceApiAssociationsResponseTypeDef",
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigExtraOutputTypeDef]
 StartDataSourceIntrospectionRequestRequestTypeDef = TypedDict(
     "StartDataSourceIntrospectionRequestRequestTypeDef",
     {
         "rdsDataApiConfig": NotRequired[RdsDataApiConfigTypeDef],
     },
 )
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
@@ -1332,16 +1348,16 @@
     },
 )
 UpdateGraphqlApiRequestRequestTypeDef = TypedDict(
     "UpdateGraphqlApiRequestRequestTypeDef",
     {
         "apiId": str,
         "name": str,
+        "authenticationType": AuthenticationTypeType,
         "logConfig": NotRequired[LogConfigTypeDef],
-        "authenticationType": NotRequired[AuthenticationTypeType],
         "userPoolConfig": NotRequired[UserPoolConfigTypeDef],
         "openIDConnectConfig": NotRequired[OpenIDConnectConfigTypeDef],
         "additionalAuthenticationProviders": NotRequired[
             Sequence[AdditionalAuthenticationProviderTypeDef]
         ],
         "xrayEnabled": NotRequired[bool],
         "lambdaAuthorizerConfig": NotRequired[LambdaAuthorizerConfigTypeDef],
@@ -1450,46 +1466,27 @@
         "functionVersion": NotRequired[str],
         "syncConfig": NotRequired[SyncConfigTypeDef],
         "maxBatchSize": NotRequired[int],
         "runtime": NotRequired[AppSyncRuntimeTypeDef],
         "code": NotRequired[str],
     },
 )
-ResolverPaginatorTypeDef = TypedDict(
-    "ResolverPaginatorTypeDef",
-    {
-        "typeName": NotRequired[str],
-        "fieldName": NotRequired[str],
-        "dataSourceName": NotRequired[str],
-        "resolverArn": NotRequired[str],
-        "requestMappingTemplate": NotRequired[str],
-        "responseMappingTemplate": NotRequired[str],
-        "kind": NotRequired[ResolverKindType],
-        "pipelineConfig": NotRequired[PipelineConfigPaginatorTypeDef],
-        "syncConfig": NotRequired[SyncConfigTypeDef],
-        "cachingConfig": NotRequired[CachingConfigPaginatorTypeDef],
-        "maxBatchSize": NotRequired[int],
-        "runtime": NotRequired[AppSyncRuntimeTypeDef],
-        "code": NotRequired[str],
-        "metricsConfig": NotRequired[ResolverLevelMetricsConfigType],
-    },
-)
 ResolverTypeDef = TypedDict(
     "ResolverTypeDef",
     {
         "typeName": NotRequired[str],
         "fieldName": NotRequired[str],
         "dataSourceName": NotRequired[str],
         "resolverArn": NotRequired[str],
         "requestMappingTemplate": NotRequired[str],
         "responseMappingTemplate": NotRequired[str],
         "kind": NotRequired[ResolverKindType],
-        "pipelineConfig": NotRequired[PipelineConfigTypeDef],
+        "pipelineConfig": NotRequired[PipelineConfigOutputTypeDef],
         "syncConfig": NotRequired[SyncConfigTypeDef],
-        "cachingConfig": NotRequired[CachingConfigTypeDef],
+        "cachingConfig": NotRequired[CachingConfigOutputTypeDef],
         "maxBatchSize": NotRequired[int],
         "runtime": NotRequired[AppSyncRuntimeTypeDef],
         "code": NotRequired[str],
         "metricsConfig": NotRequired[ResolverLevelMetricsConfigType],
     },
 )
 UpdateFunctionRequestRequestTypeDef = TypedDict(
@@ -1655,30 +1652,14 @@
 UpdateFunctionResponseTypeDef = TypedDict(
     "UpdateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListResolversByFunctionResponsePaginatorTypeDef = TypedDict(
-    "ListResolversByFunctionResponsePaginatorTypeDef",
-    {
-        "resolvers": List[ResolverPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-ListResolversResponsePaginatorTypeDef = TypedDict(
-    "ListResolversResponsePaginatorTypeDef",
-    {
-        "resolvers": List[ResolverPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateResolverResponseTypeDef = TypedDict(
     "CreateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/PKG-INFO` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.34.49
-Summary: Type annotations for boto3.AppSync 1.34.49 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.92
+Summary: Type annotations for boto3.AppSync 1.34.92 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appsync)](https://pepy.tech/project/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.34.49](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.34.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appsync-1.34.49/mypy_boto3_appsync.egg-info/SOURCES.txt` & `mypy_boto3_appsync-1.34.92/mypy_boto3_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.34.49/setup.py` & `mypy_boto3_appsync-1.34.92/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appsync",
-    version="1.34.49",
+    version="1.34.92",
     packages=["mypy_boto3_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.AppSync 1.34.49 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.AppSync 1.34.92 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


# Comparing `tmp/mypy_boto3_rds-1.34.90.tar.gz` & `tmp/mypy_boto3_rds-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_rds-1.34.90.tar", last modified: Tue Apr 23 19:34:21 2024, max compression
+gzip compressed data, was "mypy_boto3_rds-1.34.91.tar", last modified: Thu Apr 25 01:11:55 2024, max compression
```

## Comparing `mypy_boto3_rds-1.34.90.tar` & `mypy_boto3_rds-1.34.91.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/mypy_boto3_rds/
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   164341 2024-04-23 19:34:01.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   164338 2024-04-23 19:34:01.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-04-23 19:34:02.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-23 19:34:07.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-23 19:34:05.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-23 19:34:03.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 19:34:21.000000 mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:21.900581 mypy_boto3_rds-1.34.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-23 19:34:00.000000 mypy_boto3_rds-1.34.90/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21964 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20425 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:55.088525 mypy_boto3_rds-1.34.91/mypy_boto3_rds/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13119 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13119 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      903 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   164366 2024-04-25 01:11:11.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   164363 2024-04-25 01:11:08.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20349 2024-04-25 01:11:13.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20349 2024-04-25 01:11:13.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    51753 2024-04-25 01:11:12.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    51712 2024-04-25 01:11:11.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   207997 2024-04-25 01:11:22.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   207997 2024-04-25 01:11:19.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       62 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13511 2024-04-25 01:11:12.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13500 2024-04-25 01:11:12.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21964 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      655 2024-04-25 01:11:55.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       15 2024-04-25 01:11:54.000000 mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2024-04-25 01:11:55.098525 mypy_boto3_rds-1.34.91/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1946 2024-04-25 01:11:05.000000 mypy_boto3_rds-1.34.91/setup.py
```

### Comparing `mypy_boto3_rds-1.34.90/LICENSE` & `mypy_boto3_rds-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/PKG-INFO` & `mypy_boto3_rds-1.34.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.90
-Summary: Type annotations for boto3.RDS 1.34.90 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.RDS 1.34.91 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [mypy-boto3-rds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_rds-1.34.90/README.md` & `mypy_boto3_rds-1.34.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [mypy-boto3-rds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/__init__.pyi` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/__main__.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDS 1.34.90\n"
-        "Version:         1.34.90\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.RDS 1.34.91\n"
+        "Version:         1.34.91\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.90")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     ModifyGlobalClusterResultTypeDef,
     ModifyOptionGroupResultTypeDef,
     ModifyTenantDatabaseResultTypeDef,
     OptionConfigurationTypeDef,
     OptionGroupOptionsMessageTypeDef,
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
-    ParameterTypeDef,
+    ParameterUnionTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ProcessorFeatureTypeDef,
     PromoteReadReplicaDBClusterResultTypeDef,
     PromoteReadReplicaResultTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     RdsCustomClusterConfigurationTypeDef,
     RebootDBClusterResultTypeDef,
@@ -2289,15 +2289,15 @@
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_endpoint)
         """
 
     def modify_db_cluster_parameter_group(
-        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
+        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_parameter_group)
         """
@@ -2387,15 +2387,15 @@
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_instance)
         """
 
     def modify_db_parameter_group(
-        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
+        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_parameter_group)
         """
@@ -2730,29 +2730,29 @@
         """
 
     def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...,
+        Parameters: Sequence[ParameterUnionTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_cluster_parameter_group)
         """
 
     def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...,
+        Parameters: Sequence[ParameterUnionTypeDef] = ...,
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_parameter_group)
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/client.pyi` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     ModifyGlobalClusterResultTypeDef,
     ModifyOptionGroupResultTypeDef,
     ModifyTenantDatabaseResultTypeDef,
     OptionConfigurationTypeDef,
     OptionGroupOptionsMessageTypeDef,
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
-    ParameterTypeDef,
+    ParameterUnionTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ProcessorFeatureTypeDef,
     PromoteReadReplicaDBClusterResultTypeDef,
     PromoteReadReplicaResultTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     RdsCustomClusterConfigurationTypeDef,
     RebootDBClusterResultTypeDef,
@@ -2286,15 +2286,15 @@
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_endpoint)
         """
 
     def modify_db_cluster_parameter_group(
-        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
+        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_cluster_parameter_group)
         """
@@ -2384,15 +2384,15 @@
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_instance)
         """
 
     def modify_db_parameter_group(
-        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
+        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#modify_db_parameter_group)
         """
@@ -2727,29 +2727,29 @@
         """
 
     def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...,
+        Parameters: Sequence[ParameterUnionTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_cluster_parameter_group)
         """
 
     def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...,
+        Parameters: Sequence[ParameterUnionTypeDef] = ...,
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#reset_db_parameter_group)
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/literals.pyi` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/paginator.pyi` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
     "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "DBClusterStatusInfoTypeDef",
     "DomainMembershipTypeDef",
     "LimitlessDatabaseTypeDef",
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
@@ -182,14 +182,16 @@
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "ModifyIntegrationMessageRequestTypeDef",
     "ModifyTenantDatabaseMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
     "OutpostTypeDef",
+    "ParameterExtraOutputTypeDef",
+    "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
@@ -298,18 +300,14 @@
     "ModifyDBProxyRequestRequestTypeDef",
     "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionResponseTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
@@ -416,14 +414,15 @@
     "IntegrationResponseTypeDef",
     "IntegrationTypeDef",
     "OptionGroupOptionSettingTypeDef",
     "ModifyDBRecommendationMessageRequestTypeDef",
     "OptionConfigurationTypeDef",
     "OptionTypeDef",
     "SubnetTypeDef",
+    "ParameterUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "ValidStorageOptionsTypeDef",
     "ReservedDBInstanceTypeDef",
     "ReservedDBInstancesOfferingTypeDef",
     "ReferenceDetailsTypeDef",
     "SourceRegionMessageTypeDef",
@@ -477,14 +476,18 @@
     "RemoveFromGlobalClusterResultTypeDef",
     "SwitchoverGlobalClusterResultTypeDef",
     "DescribeIntegrationsResponseTypeDef",
     "OptionGroupOptionTypeDef",
     "ModifyOptionGroupMessageRequestTypeDef",
     "OptionGroupTypeDef",
     "DBSubnetGroupTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "MetricQueryTypeDef",
     "ValidDBInstanceModificationsMessageTypeDef",
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     "ReservedDBInstanceMessageTypeDef",
     "ReservedDBInstancesOfferingMessageTypeDef",
@@ -883,16 +886,16 @@
 DBClusterOptionGroupStatusTypeDef = TypedDict(
     "DBClusterOptionGroupStatusTypeDef",
     {
         "DBClusterOptionGroupName": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": NotRequired[str],
         "ParameterValue": NotRequired[str],
         "Description": NotRequired[str],
         "Source": NotRequired[str],
         "ApplyType": NotRequired[str],
         "DataType": NotRequired[str],
@@ -1584,14 +1587,46 @@
 )
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "Arn": NotRequired[str],
     },
 )
+ParameterExtraOutputTypeDef = TypedDict(
+    "ParameterExtraOutputTypeDef",
+    {
+        "ParameterName": NotRequired[str],
+        "ParameterValue": NotRequired[str],
+        "Description": NotRequired[str],
+        "Source": NotRequired[str],
+        "ApplyType": NotRequired[str],
+        "DataType": NotRequired[str],
+        "AllowedValues": NotRequired[str],
+        "IsModifiable": NotRequired[bool],
+        "MinimumEngineVersion": NotRequired[str],
+        "ApplyMethod": NotRequired[ApplyMethodType],
+        "SupportedEngineModes": NotRequired[List[str]],
+    },
+)
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": NotRequired[str],
+        "ParameterValue": NotRequired[str],
+        "Description": NotRequired[str],
+        "Source": NotRequired[str],
+        "ApplyType": NotRequired[str],
+        "DataType": NotRequired[str],
+        "AllowedValues": NotRequired[str],
+        "IsModifiable": NotRequired[bool],
+        "MinimumEngineVersion": NotRequired[str],
+        "ApplyMethod": NotRequired[ApplyMethodType],
+        "SupportedEngineModes": NotRequired[Sequence[str]],
+    },
+)
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": NotRequired[str],
         "AutoAppliedAfterDate": NotRequired[datetime],
         "ForcedApplyDate": NotRequired[datetime],
         "OptInStatus": NotRequired[str],
@@ -3194,63 +3229,33 @@
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": NotRequired[str],
         "Marker": NotRequired[str],
-        "Parameters": NotRequired[List[ParameterTypeDef]],
-    },
-)
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-ResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResetAllParameters": NotRequired[bool],
-        "Parameters": NotRequired[Sequence[ParameterTypeDef]],
-    },
-)
-ResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "ResetAllParameters": NotRequired[bool],
-        "Parameters": NotRequired[Sequence[ParameterTypeDef]],
+        "Parameters": NotRequired[List[ParameterOutputTypeDef]],
     },
 )
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": NotRequired[str],
         "DBClusterSnapshotAttributes": NotRequired[List[DBClusterSnapshotAttributeTypeDef]],
@@ -4532,14 +4537,15 @@
     {
         "SubnetIdentifier": NotRequired[str],
         "SubnetAvailabilityZone": NotRequired[AvailabilityZoneTypeDef],
         "SubnetOutpost": NotRequired[OutpostTypeDef],
         "SubnetStatus": NotRequired[str],
     },
 )
+ParameterUnionTypeDef = Union[ParameterTypeDef, ParameterExtraOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": NotRequired[str],
         "PendingMaintenanceActionDetails": NotRequired[List[PendingMaintenanceActionTypeDef]],
     },
 )
@@ -5121,14 +5127,44 @@
         "VpcId": NotRequired[str],
         "SubnetGroupStatus": NotRequired[str],
         "Subnets": NotRequired[List[SubnetTypeDef]],
         "DBSubnetGroupArn": NotRequired[str],
         "SupportedNetworkTypes": NotRequired[List[str]],
     },
 )
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterUnionTypeDef],
+    },
+)
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterUnionTypeDef],
+    },
+)
+ResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResetAllParameters": NotRequired[bool],
+        "Parameters": NotRequired[Sequence[ParameterUnionTypeDef]],
+    },
+)
+ResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "ResetAllParameters": NotRequired[bool],
+        "Parameters": NotRequired[Sequence[ParameterUnionTypeDef]],
+    },
+)
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/type_defs.pyi` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
     "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "DBClusterStatusInfoTypeDef",
     "DomainMembershipTypeDef",
     "LimitlessDatabaseTypeDef",
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
@@ -182,14 +182,16 @@
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "ModifyIntegrationMessageRequestTypeDef",
     "ModifyTenantDatabaseMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
     "OutpostTypeDef",
+    "ParameterExtraOutputTypeDef",
+    "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
@@ -298,18 +300,14 @@
     "ModifyDBProxyRequestRequestTypeDef",
     "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionResponseTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
@@ -416,14 +414,15 @@
     "IntegrationResponseTypeDef",
     "IntegrationTypeDef",
     "OptionGroupOptionSettingTypeDef",
     "ModifyDBRecommendationMessageRequestTypeDef",
     "OptionConfigurationTypeDef",
     "OptionTypeDef",
     "SubnetTypeDef",
+    "ParameterUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "ValidStorageOptionsTypeDef",
     "ReservedDBInstanceTypeDef",
     "ReservedDBInstancesOfferingTypeDef",
     "ReferenceDetailsTypeDef",
     "SourceRegionMessageTypeDef",
@@ -477,14 +476,18 @@
     "RemoveFromGlobalClusterResultTypeDef",
     "SwitchoverGlobalClusterResultTypeDef",
     "DescribeIntegrationsResponseTypeDef",
     "OptionGroupOptionTypeDef",
     "ModifyOptionGroupMessageRequestTypeDef",
     "OptionGroupTypeDef",
     "DBSubnetGroupTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "MetricQueryTypeDef",
     "ValidDBInstanceModificationsMessageTypeDef",
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     "ReservedDBInstanceMessageTypeDef",
     "ReservedDBInstancesOfferingMessageTypeDef",
@@ -883,16 +886,16 @@
 DBClusterOptionGroupStatusTypeDef = TypedDict(
     "DBClusterOptionGroupStatusTypeDef",
     {
         "DBClusterOptionGroupName": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": NotRequired[str],
         "ParameterValue": NotRequired[str],
         "Description": NotRequired[str],
         "Source": NotRequired[str],
         "ApplyType": NotRequired[str],
         "DataType": NotRequired[str],
@@ -1584,14 +1587,46 @@
 )
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "Arn": NotRequired[str],
     },
 )
+ParameterExtraOutputTypeDef = TypedDict(
+    "ParameterExtraOutputTypeDef",
+    {
+        "ParameterName": NotRequired[str],
+        "ParameterValue": NotRequired[str],
+        "Description": NotRequired[str],
+        "Source": NotRequired[str],
+        "ApplyType": NotRequired[str],
+        "DataType": NotRequired[str],
+        "AllowedValues": NotRequired[str],
+        "IsModifiable": NotRequired[bool],
+        "MinimumEngineVersion": NotRequired[str],
+        "ApplyMethod": NotRequired[ApplyMethodType],
+        "SupportedEngineModes": NotRequired[List[str]],
+    },
+)
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": NotRequired[str],
+        "ParameterValue": NotRequired[str],
+        "Description": NotRequired[str],
+        "Source": NotRequired[str],
+        "ApplyType": NotRequired[str],
+        "DataType": NotRequired[str],
+        "AllowedValues": NotRequired[str],
+        "IsModifiable": NotRequired[bool],
+        "MinimumEngineVersion": NotRequired[str],
+        "ApplyMethod": NotRequired[ApplyMethodType],
+        "SupportedEngineModes": NotRequired[Sequence[str]],
+    },
+)
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": NotRequired[str],
         "AutoAppliedAfterDate": NotRequired[datetime],
         "ForcedApplyDate": NotRequired[datetime],
         "OptInStatus": NotRequired[str],
@@ -3194,63 +3229,33 @@
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": NotRequired[str],
         "Marker": NotRequired[str],
-        "Parameters": NotRequired[List[ParameterTypeDef]],
-    },
-)
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-ResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResetAllParameters": NotRequired[bool],
-        "Parameters": NotRequired[Sequence[ParameterTypeDef]],
-    },
-)
-ResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "ResetAllParameters": NotRequired[bool],
-        "Parameters": NotRequired[Sequence[ParameterTypeDef]],
+        "Parameters": NotRequired[List[ParameterOutputTypeDef]],
     },
 )
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": NotRequired[str],
         "DBClusterSnapshotAttributes": NotRequired[List[DBClusterSnapshotAttributeTypeDef]],
@@ -4532,14 +4537,15 @@
     {
         "SubnetIdentifier": NotRequired[str],
         "SubnetAvailabilityZone": NotRequired[AvailabilityZoneTypeDef],
         "SubnetOutpost": NotRequired[OutpostTypeDef],
         "SubnetStatus": NotRequired[str],
     },
 )
+ParameterUnionTypeDef = Union[ParameterTypeDef, ParameterExtraOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": NotRequired[str],
         "PendingMaintenanceActionDetails": NotRequired[List[PendingMaintenanceActionTypeDef]],
     },
 )
@@ -5121,14 +5127,44 @@
         "VpcId": NotRequired[str],
         "SubnetGroupStatus": NotRequired[str],
         "Subnets": NotRequired[List[SubnetTypeDef]],
         "DBSubnetGroupArn": NotRequired[str],
         "SupportedNetworkTypes": NotRequired[List[str]],
     },
 )
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterUnionTypeDef],
+    },
+)
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterUnionTypeDef],
+    },
+)
+ResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResetAllParameters": NotRequired[bool],
+        "Parameters": NotRequired[Sequence[ParameterUnionTypeDef]],
+    },
+)
+ResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "ResetAllParameters": NotRequired[bool],
+        "Parameters": NotRequired[Sequence[ParameterUnionTypeDef]],
+    },
+)
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.py` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds/waiter.pyi` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/PKG-INFO` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.90
-Summary: Type annotations for boto3.RDS 1.34.90 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.RDS 1.34.91 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
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
 [mypy-boto3-rds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_rds-1.34.90/mypy_boto3_rds.egg-info/SOURCES.txt` & `mypy_boto3_rds-1.34.91/mypy_boto3_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_rds-1.34.90/setup.py` & `mypy_boto3_rds-1.34.91/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds",
-    version="1.34.90",
+    version="1.34.91",
     packages=["mypy_boto3_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.RDS 1.34.90 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.RDS 1.34.91 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


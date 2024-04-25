# Comparing `tmp/hashboard_cli-1.0.9.tar.gz` & `tmp/hashboard_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashboard_cli-1.0.9.tar", last modified: Tue Apr 23 15:13:56 2024, max compression
+gzip compressed data, was "hashboard_cli-1.1.0.tar", last modified: Thu Apr 25 19:09:29 2024, max compression
```

## Comparing `hashboard_cli-1.0.9.tar` & `hashboard_cli-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.975898 hashboard_cli-1.0.9/
--rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 hashboard_cli-1.0.9/LICENSE
--rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-23 15:13:56.975823 hashboard_cli-1.0.9/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      141 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/README.md
--rw-r--r--   0 anixon     (501) staff       (20)      104 2023-08-30 15:47:31.000000 hashboard_cli-1.0.9/pyproject.toml
--rw-r--r--   0 anixon     (501) staff       (20)      878 2024-04-23 15:13:56.976189 hashboard_cli-1.0.9/setup.cfg
--rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 hashboard_cli-1.0.9/setup.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.965875 hashboard_cli-1.0.9/src/
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.968841 hashboard_cli-1.0.9/src/hashboard/
--rw-r--r--   0 anixon     (501) staff       (20)       18 2024-04-23 15:12:51.000000 hashboard_cli-1.0.9/src/hashboard/__init__.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.969251 hashboard_cli-1.0.9/src/hashboard/api/
--rw-r--r--   0 anixon     (501) staff       (20)    14525 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/__init__.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.970374 hashboard_cli-1.0.9/src/hashboard/api/access_keys/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     4227 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/browser_auth.py
--rw-r--r--   0 anixon     (501) staff       (20)     4409 2024-03-18 20:02:56.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/existing_user.py
--rw-r--r--   0 anixon     (501) staff       (20)     2143 2024-03-18 20:02:56.000000 hashboard_cli-1.0.9/src/hashboard/api/access_keys/utils.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.971419 hashboard_cli-1.0.9/src/hashboard/api/analytics/
--rw-r--r--   0 anixon     (501) staff       (20)      900 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/src/hashboard/api/analytics/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     4003 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/src/hashboard/api/analytics/cli_with_tracking.py
--rw-r--r--   0 anixon     (501) staff       (20)       20 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/src/hashboard/api/analytics/events.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.972227 hashboard_cli-1.0.9/src/hashboard/api/datasource/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/datasource/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)    11030 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/datasource/datasource_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     2950 2024-04-22 20:51:24.000000 hashboard_cli-1.0.9/src/hashboard/api/datasource/utils.py
--rw-r--r--   0 anixon     (501) staff       (20)    38873 2024-04-23 14:57:44.000000 hashboard_cli-1.0.9/src/hashboard/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)      346 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/constants.py
--rw-r--r--   0 anixon     (501) staff       (20)     1744 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3843 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/src/hashboard/filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      597 2023-09-29 18:00:46.000000 hashboard_cli-1.0.9/src/hashboard/session.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.973860 hashboard_cli-1.0.9/src/hashboard/utils/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)      665 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1977 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/src/hashboard/utils/config.py
--rw-r--r--   0 anixon     (501) staff       (20)      230 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/env.py
--rw-r--r--   0 anixon     (501) staff       (20)     2922 2023-11-06 18:51:09.000000 hashboard_cli-1.0.9/src/hashboard/utils/grn.py
--rw-r--r--   0 anixon     (501) staff       (20)      941 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/input_validation.py
--rw-r--r--   0 anixon     (501) staff       (20)     1468 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/src/hashboard/utils/resource.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.975391 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/
--rw-r--r--   0 anixon     (501) staff       (20)      924 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)     1224 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anixon     (501) staff       (20)        1 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anixon     (501) staff       (20)       42 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/entry_points.txt
--rw-r--r--   0 anixon     (501) staff       (20)      138 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/requires.txt
--rw-r--r--   0 anixon     (501) staff       (20)       10 2024-04-23 15:13:56.000000 hashboard_cli-1.0.9/src/hashboard_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-04-23 15:13:56.975180 hashboard_cli-1.0.9/tests/
--rw-r--r--   0 anixon     (501) staff       (20)      310 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/tests/test_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1534 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/tests/test_credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3890 2024-04-16 20:21:42.000000 hashboard_cli-1.0.9/tests/test_filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      668 2023-09-19 18:12:31.000000 hashboard_cli-1.0.9/tests/test_hashboard_api.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.845770 hashboard_cli-1.1.0/
+-rw-r--r--   0 elagulsen   (501) staff       (20)    11357 2023-08-14 18:27:21.000000 hashboard_cli-1.1.0/LICENSE
+-rw-r--r--   0 elagulsen   (501) staff       (20)      924 2024-04-25 19:09:29.845704 hashboard_cli-1.1.0/PKG-INFO
+-rw-r--r--   0 elagulsen   (501) staff       (20)      141 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/README.md
+-rw-r--r--   0 elagulsen   (501) staff       (20)      104 2023-08-15 19:32:06.000000 hashboard_cli-1.1.0/pyproject.toml
+-rw-r--r--   0 elagulsen   (501) staff       (20)      878 2024-04-25 19:09:29.846019 hashboard_cli-1.1.0/setup.cfg
+-rw-r--r--   0 elagulsen   (501) staff       (20)       38 2023-08-14 18:27:21.000000 hashboard_cli-1.1.0/setup.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.838716 hashboard_cli-1.1.0/src/
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.841271 hashboard_cli-1.1.0/src/hashboard/
+-rw-r--r--   0 elagulsen   (501) staff       (20)       18 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/__init__.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.841518 hashboard_cli-1.1.0/src/hashboard/api/
+-rw-r--r--   0 elagulsen   (501) staff       (20)    14949 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/api/__init__.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.842143 hashboard_cli-1.1.0/src/hashboard/api/access_keys/
+-rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     4227 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/browser_auth.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     4409 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/existing_user.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     2143 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/access_keys/utils.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.842538 hashboard_cli-1.1.0/src/hashboard/api/analytics/
+-rw-r--r--   0 elagulsen   (501) staff       (20)      900 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/analytics/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     4003 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/api/analytics/cli_with_tracking.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)       20 2024-04-12 14:43:11.000000 hashboard_cli-1.1.0/src/hashboard/api/analytics/events.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.843049 hashboard_cli-1.1.0/src/hashboard/api/datasource/
+-rw-r--r--   0 elagulsen   (501) staff       (20)        0 2024-04-19 17:47:42.000000 hashboard_cli-1.1.0/src/hashboard/api/datasource/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     9994 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/api/datasource/datasource_cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)    10025 2024-04-25 19:09:12.000000 hashboard_cli-1.1.0/src/hashboard/api/datasource/utils.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)    38873 2024-04-25 15:48:11.000000 hashboard_cli-1.1.0/src/hashboard/cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      346 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/constants.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1744 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/credentials.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     3843 2024-04-16 15:20:55.000000 hashboard_cli-1.1.0/src/hashboard/filesystem.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      597 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/session.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.843985 hashboard_cli-1.1.0/src/hashboard/utils/
+-rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      665 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1977 2024-04-16 15:20:55.000000 hashboard_cli-1.1.0/src/hashboard/utils/config.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      230 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/env.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     2922 2024-04-11 15:34:55.000000 hashboard_cli-1.1.0/src/hashboard/utils/grn.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      941 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/input_validation.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1468 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/src/hashboard/utils/resource.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.845394 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/
+-rw-r--r--   0 elagulsen   (501) staff       (20)      924 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1224 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)        1 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)       42 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)      138 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/requires.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)       10 2024-04-25 19:09:29.000000 hashboard_cli-1.1.0/src/hashboard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-25 19:09:29.845217 hashboard_cli-1.1.0/tests/
+-rw-r--r--   0 elagulsen   (501) staff       (20)      310 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/tests/test_cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1534 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/tests/test_credentials.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     3890 2024-04-16 15:20:55.000000 hashboard_cli-1.1.0/tests/test_filesystem.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      668 2023-09-13 19:44:14.000000 hashboard_cli-1.1.0/tests/test_hashboard_api.py
```

### Comparing `hashboard_cli-1.0.9/LICENSE` & `hashboard_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/PKG-INFO` & `hashboard_cli-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.0.9
+Version: 1.1.0
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Click>=8.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.0
 Requires-Dist: ruamel.yaml>=0.17
 Requires-Dist: yaspin>=2.1.0
```

### Comparing `hashboard_cli-1.0.9/setup.cfg` & `hashboard_cli-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	Click >= 8.0
 	pyyaml >= 6.0
 	requests >= 2.0
 	ruamel.yaml >= 0.17
 	yaspin >= 2.1.0
 	semver >= 3.0.1
```

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/__init__.py` & `hashboard_cli-1.1.0/src/hashboard/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -311,14 +311,28 @@
             id
           }
         }
         """,
         {"datasource": datasource},
     )["data"]["addDatasource"]["id"]
 
+def update_data_source(session: Session, datasource: dict) -> dict:
+    # Assumes that error handling occurs a level up
+    return _graphql_query(
+        session,
+        """
+        mutation UpdateDatasource($datasource: DatasourceInput!) {
+          updateDatasource(datasource: $datasource) {
+            id
+          }
+        }
+        """,
+        {"datasource": datasource},
+    )["data"]["updateDatasource"]["id"]
+
 def test_data_source(session: Session, datasource_name: str, project_id: str) -> bool:
     return _graphql_query(
         session,
         """
         query TestDatasourceByName($name: String!, $projectId: String!) {
             testDatasourceByName(name: $name, projectId: $projectId) 
         }
```

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/access_keys/browser_auth.py` & `hashboard_cli-1.1.0/src/hashboard/api/access_keys/browser_auth.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/access_keys/existing_user.py` & `hashboard_cli-1.1.0/src/hashboard/api/access_keys/existing_user.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/access_keys/utils.py` & `hashboard_cli-1.1.0/src/hashboard/api/access_keys/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/analytics/__init__.py` & `hashboard_cli-1.1.0/src/hashboard/api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/analytics/cli_with_tracking.py` & `hashboard_cli-1.1.0/src/hashboard/api/analytics/cli_with_tracking.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/api/datasource/datasource_cli.py` & `hashboard_cli-1.1.0/src/hashboard/api/datasource/datasource_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,15 @@
 import os
 from hashboard.api import get_datasources, login, upload_files_to_hashboard
 from hashboard.api.analytics.cli_with_tracking import CommandWithTracking, GroupWithTracking
-from hashboard.api.datasource.utils import DatabaseTypes, _test, create_datasource_from_subtype
+from hashboard.api.datasource.utils import DatabaseTypes, _test, athena_arguments, bigquery_arguments, clickhouse_arguments, mutate_datasource_from_subtype, databricks_arguments, motherduck_arguments, mysql_arguments, postgres_arguments, snowflake_arguments, data_source_id
 from hashboard.credentials import get_credentials
 from hashboard.session import get_current_session
 import click
 
-# Common fields
-data_source_name = click.option(
-    "--name",
-    type=str,
-    required=True,
-    help="""The user-facing name for the Hashboard data source you are creating.""",
-    prompt=True,
-)
-data_source_user = click.option(
-    "--user",
-    type=str,
-    required=True,
-    help="""The user used to connect to the data source.""",
-    prompt=True,
-)
-data_source_password = click.option(
-    "--password",
-    type=str,
-    required=True,
-    help="""The password used to connect to the data source.""",
-    prompt=True,
-    hide_input=True,
-)
-def data_source_db(required: bool):
-    return click.option(
-    "--database",
-    type=str,
-    required=required,
-    help="""The name of the database to read from.""",
-    prompt=True,
-)
-data_source_schema = click.option(
-    "--schema",
-    type=str,
-    required=False,
-    help="""Specify a schema to limit which tables are available. 
-    Otherwise, Hashboard will make all accessible schemas and tables available.""",
-    prompt=True,
-)
-data_source_host = click.option(
-    "--host",
-    type=str,
-    required=True,
-    help="""The address of your database.""",
-    prompt=True,
-)
-def data_source_port(default_port: str, required: bool):
-    return click.option(
-    "--port",
-    type=str,
-    required=required,
-    help=f"""The port used to connect to your data source. Default port: {default_port}""",
-    prompt=True,
-)
-
-# Bigquery-specific fields
-bigquery_json_key = click.option(
-    "--json_key",
-    required=True,
-    type=click.Path(exists=True, dir_okay=False, allow_dash=True),
-    help="""A path to a JSON file containing the BigQuery service account JSON key.""",
-)
-
-# Snowflake-specific fields
-snowflake_account = click.option(
-    "--account",
-    required=True,
-    type=str,
-    help="""
-    Your snowflake account identifier (opens in a new tab) is provided by Snowflake and
-    included in the start of the URL you use to login to Snowflake: <account_identifier>.snowflakecomputing.com.
-    """,
-    prompt=True,
-)
-
-snowflake_warehouse = click.option(
-    "--warehouse",
-    required=True,
-    type=str,
-    help="""The warehouse to use in Snowflake. Warehouses correspond with compute resources.""",
-    prompt=True,
-)
-snowflake_role = click.option(
-    "--role",
-    required=True,
-    type=str,
-    prompt=True,
-)
-
-# Athena-specific fields
-athena_aws_region = click.option(
-    "--aws_region",
-    type=str,
-    required=True,
-    help="""The AWS region to use to query data.""",
-    prompt=True,
-)
-athena_port = click.option(
-    "--port",
-    type=str,
-    required=False,
-    help="""The port to connect to.""",
-    prompt=True,
-)
-athena_staging_directory = click.option(
-    "--s3_staging_dir",
-    type=str,
-    required=True,
-    help="""The S3 path where Athena will store query results.""",
-    prompt=True,
-)
-athena_aws_access_key_id = click.option(
-    "--aws_access_key_id",
-    type=str,
-    required=True,
-    help="""The IAM user's access key.""",
-    prompt=True,
-)
-athena_aws_secret_access_key = click.option(
-    "--aws_secret_access_key",
-    type=str,
-    required=True,
-    help="""The IAM user's scret access key.""",
-    prompt=True,
-    hide_input=True,
-)
-athena_query_parameters = click.option(
-    "--additional_query_params",
-    type=str,
-    help="""Additional database connection parameters in the format workGroup=value&param=value.""",
-    required=False,
-    prompt=True,
-)
-
-# Motherduck-specific fields
-motherduck_service_token = click.option(
-    "--service_token",
-    type=str,
-    required=True,
-    help="""Your MotherDuck service token.""",
-    hide_input=True,
-    prompt=True,
-)
-
-# Databricks-specific fields
-databricks_http_path = click.option(
-    "--http_path",
-    type=str,
-    required=True,
-    help="""The HTTP path of the SQL warehouse. Can be found in the Connection Details tab of your SQL warehouse.""",
-    prompt=True,
-)
-databricks_access_token = click.option(
-    "--access_token",
-    type=str,
-    required=True,
-    help="""A personal access token generated in Databricks for a user with access to the data you want to query.""",
-    hide_input=True,
-    prompt=True,
-)
-databricks_catalog = click.option(
-    "--catalog",
-    type=str,
-    required=True,
-    help="""The Databricks catalog within the warehouse to connect to.""",
-    prompt=True,
-)
-
 @click.group(cls=GroupWithTracking)
 @click.pass_context
 def datasource(ctx):
     """Commands for managing Hashboard data sources."""
     pass
 
 @datasource.command("ls", cls=CommandWithTracking)
@@ -202,137 +34,204 @@
     context_settings=dict(),
 )
 @click.pass_context
 def create(ctx):
     """Commands for creating Hashboard data sources."""
     pass
 
+@datasource.group(
+    "update",
+    cls=GroupWithTracking,
+    context_settings=dict(),
+)
+@click.pass_context
+def update(ctx):
+    """Commands for updating existing Hashboard data sources."""
+    pass
+
 @create.command("bigquery")
-@data_source_name
-@bigquery_json_key
+@bigquery_arguments
 @click.pass_context
 def create_bigquery(ctx, **kwargs):
     """Create a BigQuery data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/bigquery
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.BIGQUERY.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.BIGQUERY, **kwargs)
+
+
+@update.command("bigquery")
+@data_source_id
+@bigquery_arguments
+@click.pass_context
+def update_bigquery(ctx, **kwargs):
+    """Update a BigQuery data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/bigquery
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.BIGQUERY, is_update=True, **kwargs)
 
 @create.command("snowflake")
-@data_source_name
-@snowflake_account
-@data_source_user
-@data_source_password
-@data_source_db(required=True)
-@data_source_schema
-@snowflake_warehouse
-@snowflake_role
+@snowflake_arguments
 @click.pass_context
 def create_snowflake(ctx, **kwargs):
     """Create a Snowflake data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/snowflake
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.SNOWFLAKE.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.SNOWFLAKE, **kwargs)
+
+@update.command("snowflake")
+@data_source_id
+@snowflake_arguments
+@click.pass_context
+def update_snowflake(ctx, **kwargs):
+    """Update a Snowflake data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/snowflake
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.SNOWFLAKE, is_update=True, **kwargs)
 
 @create.command("postgres")
-@data_source_name
-@data_source_host
-@data_source_port(default_port="5432", required=True)
-@data_source_user
-@data_source_password
-@data_source_db(required=True)
-@data_source_schema
+@postgres_arguments
 @click.pass_context
 def create_postgres(ctx, **kwargs):
     """Create a Postgres data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/postgresql
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.POSTGRES.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.POSTGRES, **kwargs)
+
+@update.command("postgres")
+@data_source_id
+@postgres_arguments
+@click.pass_context
+def update_postgres(ctx, **kwargs):
+    """Update a Postgres data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/postgresql
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.POSTGRES, is_update=True, **kwargs)
 
 @create.command("redshift")
-@data_source_name
-@data_source_host
-@data_source_port(default_port="5432", required=True)
-@data_source_user
-@data_source_password
-@data_source_db(required=True)
-@data_source_schema
+@postgres_arguments
 @click.pass_context
 def create_redshift(ctx, **kwargs):
     """Create a Redshift data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/postgresql
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.REDSHIFT.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.REDSHIFT, **kwargs)
+
+@update.command("redshift")
+@data_source_id
+@postgres_arguments
+@click.pass_context
+def update_redshift(ctx, **kwargs):
+    """Update a Redshift data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/postgresql
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.REDSHIFT, is_update=True, **kwargs)
 
 @create.command("athena")
-@data_source_name
-@athena_aws_region
-@athena_port
-@data_source_schema
-@athena_staging_directory
-@athena_aws_access_key_id
-@athena_aws_secret_access_key
-@athena_query_parameters
+@athena_arguments
 @click.pass_context
 def create_athena(ctx, **kwargs):
     """Create an Athena data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/athena
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.ATHENA.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.ATHENA, **kwargs)
+
+@update.command("athena")
+@data_source_id
+@athena_arguments
+@click.pass_context
+def update_athena(ctx, **kwargs):
+    """Update an Athena data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/athena
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.ATHENA, is_update=True, **kwargs)
 
 @create.command("clickhouse")
-@data_source_name
-@data_source_port(default_port="9440", required=True)
-@data_source_host
-@data_source_user
-@data_source_password
-@data_source_db(required=True)
+@clickhouse_arguments
 @click.pass_context
 def create_clickhouse(ctx, **kwargs):
     """Create a Clickhouse data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/clickhouse
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.CLICKHOUSE.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.CLICKHOUSE, **kwargs)
+
+@update.command("clickhouse")
+@data_source_id
+@clickhouse_arguments
+@click.pass_context
+def update_clickhouse(ctx, **kwargs):
+    """Update a Clickhouse data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/clickhouse
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.CLICKHOUSE, is_update=True, **kwargs)
 
 @create.command("mysql")
-@data_source_name
-@data_source_host
-@data_source_user
-@data_source_password
-@data_source_db(required=False)
+@mysql_arguments
 @click.pass_context
 def create_mysql(ctx, **kwargs):
     """Create a MySql data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/mysql
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.MYSQL.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.MYSQL, **kwargs)
+
+@update.command("mysql")
+@data_source_id
+@mysql_arguments
+@click.pass_context
+def update_mysql(ctx, **kwargs):
+    """Update a MySQL data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/mysql
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.MYSQL, is_update=True, **kwargs)
 
 @create.command("motherduck")
-@data_source_name
-@data_source_db(required=True)
+@motherduck_arguments
 @click.pass_context
 def create_motherduck(ctx, **kwargs):
     """Create a MotherDuck data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/motherduck
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.MOTHERDUCK.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.MOTHERDUCK, **kwargs)
+
+@update.command("motherduck")
+@data_source_id
+@motherduck_arguments
+@click.pass_context
+def update_motherduck(ctx, **kwargs):
+    """Update a MotherDuck data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/motherduck
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.MOTHERDUCK, is_update=True, **kwargs)
 
 @create.command("databricks")
-@data_source_name
-@data_source_host
-@data_source_port(default_port="443", required=False)
-@databricks_http_path
-@databricks_access_token
-@databricks_catalog
-@data_source_schema
+@databricks_arguments
 @click.pass_context
 def create_databricks(ctx, **kwargs):
     """Create a Databricks data connection in your project. 
     More info: https://docs.hashboard.com/docs/database-connections/databricks
     """
-    create_datasource_from_subtype(ctx, DatabaseTypes.DATABRICKS.value, **kwargs)
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.DATABRICKS, **kwargs)
+
+@update.command("databricks")
+@data_source_id
+@databricks_arguments
+@click.pass_context
+def update_databricks(ctx, **kwargs):
+    """Update a Databricks data connection in your project. 
+    The ID of the connection you provide must match the ID of an existing connection.
+    More info: https://docs.hashboard.com/docs/database-connections/databricks
+    """
+    mutate_datasource_from_subtype(ctx, DatabaseTypes.DATABRICKS, is_update=True, **kwargs)
 
 @datasource.command(
     "upload",
     cls=CommandWithTracking,
     context_settings=dict(),
 )
 @click.argument(
@@ -373,8 +272,7 @@
 @click.pass_context
 def test(ctx, name):
     """Test a data connection by its name."""
     s = get_current_session()
     ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
     project_id = login(s, ctx.obj["credentials"])
     _test(s, name, project_id)
-
```

### Comparing `hashboard_cli-1.0.9/src/hashboard/cli.py` & `hashboard_cli-1.1.0/src/hashboard/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/credentials.py` & `hashboard_cli-1.1.0/src/hashboard/credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/filesystem.py` & `hashboard_cli-1.1.0/src/hashboard/filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/session.py` & `hashboard_cli-1.1.0/src/hashboard/session.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/utils/cli.py` & `hashboard_cli-1.1.0/src/hashboard/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/utils/config.py` & `hashboard_cli-1.1.0/src/hashboard/utils/config.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/utils/grn.py` & `hashboard_cli-1.1.0/src/hashboard/utils/grn.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/utils/input_validation.py` & `hashboard_cli-1.1.0/src/hashboard/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard/utils/resource.py` & `hashboard_cli-1.1.0/src/hashboard/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/src/hashboard_cli.egg-info/PKG-INFO` & `hashboard_cli-1.1.0/src/hashboard_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 1.0.9
+Version: 1.1.0
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Click>=8.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.0
 Requires-Dist: ruamel.yaml>=0.17
 Requires-Dist: yaspin>=2.1.0
```

### Comparing `hashboard_cli-1.0.9/src/hashboard_cli.egg-info/SOURCES.txt` & `hashboard_cli-1.1.0/src/hashboard_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/tests/test_credentials.py` & `hashboard_cli-1.1.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/tests/test_filesystem.py` & `hashboard_cli-1.1.0/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-1.0.9/tests/test_hashboard_api.py` & `hashboard_cli-1.1.0/tests/test_hashboard_api.py`

 * *Files identical despite different names*


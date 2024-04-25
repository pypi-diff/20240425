# Comparing `tmp/tinybird-cli-3.9.1.dev1.tar.gz` & `tmp/tinybird-cli-3.9.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.9.1.dev1.tar", last modified: Wed Apr 24 06:19:04 2024, max compression
+gzip compressed data, was "tinybird-cli-3.9.1.dev2.tar", last modified: Thu Apr 25 09:55:11 2024, max compression
```

## Comparing `tinybird-cli-3.9.1.dev1.tar` & `tinybird-cli-3.9.1.dev2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.494391 tinybird-cli-3.9.1.dev1/
--rw-r--r--   0 root         (0) root         (0)    68385 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 06:19:04.494391 tinybird-cli-3.9.1.dev1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.491391 tinybird-cli-3.9.1.dev1/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-24 06:19:03.000000 tinybird-cli-3.9.1.dev1/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.491391 tinybird-cli-3.9.1.dev1/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59114 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41181 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    30927 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    68385 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:11.258899 tinybird-cli-3.9.1.dev2/
+-rw-r--r--   0 root         (0) root         (0)    68441 2024-04-25 09:55:11.258899 tinybird-cli-3.9.1.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 09:55:11.258899 tinybird-cli-3.9.1.dev2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:11.254899 tinybird-cli-3.9.1.dev2/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-25 09:55:10.000000 tinybird-cli-3.9.1.dev2/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:11.254899 tinybird-cli-3.9.1.dev2/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59114 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41381 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:11.256899 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    30927 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:11.256899 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-25 09:55:03.000000 tinybird-cli-3.9.1.dev2/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 09:55:11.258899 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    68441 2024-04-25 09:55:11.000000 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-25 09:55:11.000000 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 09:55:11.000000 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-25 09:55:11.000000 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-25 09:55:11.000000 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-25 09:55:11.000000 tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.9.1.dev1/PKG-INFO` & `tinybird-cli-3.9.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev1
+Version: 3.9.1.dev2
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,14 +14,19 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ---------
 
+3.9.1.dev2
+************
+
+- `Fixed` Support ngram index
+
 3.9.0
 ************
 
 - `Added` Support for connection names when doing `tb connection rm`
 - `Added` New `--policy` option for `create s3_iamrole` command that will generate different hints depending on the case
 - `Fixed` Avoid system vars evaluation when doing `tb fmt`
 - `Fixed` environment variables substitution for Data Source engine parameters.
```

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/ch_utils/constants.py` & `tinybird-cli-3.9.1.dev2/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/ch_utils/engine.py` & `tinybird-cli-3.9.1.dev2/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/check_pypi.py` & `tinybird-cli-3.9.1.dev2/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/client.py` & `tinybird-cli-3.9.1.dev2/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/config.py` & `tinybird-cli-3.9.1.dev2/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/connectors.py` & `tinybird-cli-3.9.1.dev2/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/context.py` & `tinybird-cli-3.9.1.dev2/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/datafile.py` & `tinybird-cli-3.9.1.dev2/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/datatypes.py` & `tinybird-cli-3.9.1.dev2/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/feedback_manager.py` & `tinybird-cli-3.9.1.dev2/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/git_settings.py` & `tinybird-cli-3.9.1.dev2/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/sql.py` & `tinybird-cli-3.9.1.dev2/tinybird/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
     [TableIndex(name='index_name', expr='type', type_full='set(100)', granularity='100'), TableIndex(name='index_name_bf', expr='mapValues(d)', type_full='bloom_filter(0.001)', granularity='16')]
     >>> parse_indexes_structure(["index_name a TYPE set(100) GRANULARITY 100,", "index_name_bf mapValues(d) TYPE bloom_filter(0.001) GRANULARITY 16"])
     [TableIndex(name='index_name', expr='a', type_full='set(100)', granularity='100'), TableIndex(name='index_name_bf', expr='mapValues(d)', type_full='bloom_filter(0.001)', granularity='16')]
     >>> parse_indexes_structure(["index_name a TYPE set(100)", "index_name_bf mapValues(d) TYPE bloom_filter(0.001)"])
     [TableIndex(name='index_name', expr='a', type_full='set(100)', granularity=None), TableIndex(name='index_name_bf', expr='mapValues(d)', type_full='bloom_filter(0.001)', granularity=None)]
     >>> parse_indexes_structure(["index_name u64 * length(s) TYPE set(100)", "index_name_bf mapValues(d) TYPE bloom_filter"])
     [TableIndex(name='index_name', expr='u64 * length(s)', type_full='set(100)', granularity=None), TableIndex(name='index_name_bf', expr='mapValues(d)', type_full='bloom_filter', granularity=None)]
+    >>> parse_indexes_structure(["index_name path TYPE ngrambf_v1(4,1024,1,42) GRANULARITY 1"])
+    [TableIndex(name='index_name', expr='path', type_full='ngrambf_v1(4,1024,1,42)', granularity='1')]
     >>> parse_indexes_structure(["index_name u64 * length(s)"])
     Traceback (most recent call last):
     ...
     ValueError: invalid INDEX format. Usage: `name expr TYPE type_full GRANULARITY granularity`
     >>> parse_indexes_structure(["index_name a TYPE set(100) GRANULARITY 100, index_name_bf mapValues(d) TYPE bloom_filter(0.001) GRANULARITY 16"])
     Traceback (most recent call last):
     ...
@@ -239,15 +241,15 @@
 
     for index in indexes:
         index = index.strip().rstrip(",")
         index = index.lstrip("INDEX").strip()
         if index.count("TYPE") != 1:
             raise ValueError("invalid INDEX format. Usage: `name expr TYPE type_full GRANULARITY granularity`")
 
-        match = re.match(r"(\w+)\s+([\w\s*()]+)\s+TYPE\s+(\w+)(?:\(([\w.]+)\))?(?:\s+GRANULARITY\s+(\d+))?", index)
+        match = re.match(r"(\w+)\s+([\w\s*()]+)\s+TYPE\s+(\w+)(?:\(([\w.,]+)\))?(?:\s+GRANULARITY\s+(\d+))?", index)
         if match:
             index_name, a, index_type, value, granularity = match.groups()
             index_expr = f"{index_type}({value})" if value else index_type
             parsed_indices.append(TableIndex(index_name, a.strip(), f"{index_expr}", granularity))
         else:
             raise ValueError("invalid INDEX format. Usage: `name expr TYPE type_full GRANULARITY granularity`")
     return parsed_indices
```

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/sql_template.py` & `tinybird-cli-3.9.1.dev2/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/sql_template_fmt.py` & `tinybird-cli-3.9.1.dev2/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/sql_toolset.py` & `tinybird-cli-3.9.1.dev2/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/syncasync.py` & `tinybird-cli-3.9.1.dev2/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.9.1.dev2/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird/tornado_template.py` & `tinybird-cli-3.9.1.dev2/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev1
+Version: 3.9.1.dev2
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,14 +14,19 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ---------
 
+3.9.1.dev2
+************
+
+- `Fixed` Support ngram index
+
 3.9.0
 ************
 
 - `Added` Support for connection names when doing `tb connection rm`
 - `Added` New `--policy` option for `create s3_iamrole` command that will generate different hints depending on the case
 - `Fixed` Avoid system vars evaluation when doing `tb fmt`
 - `Fixed` environment variables substitution for Data Source engine parameters.
```

### Comparing `tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.9.1.dev2/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*


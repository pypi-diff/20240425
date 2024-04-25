# Comparing `tmp/maxwelld-0.2.8.tar.gz` & `tmp/maxwelld-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxwelld-0.2.8.tar", last modified: Fri Mar  8 16:49:54 2024, max compression
+gzip compressed data, was "maxwelld-0.2.9.tar", last modified: Sat Mar  9 07:58:42 2024, max compression
```

## Comparing `maxwelld-0.2.8.tar` & `maxwelld-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.828727 maxwelld-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-08 16:49:46.000000 maxwelld-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-08 16:49:54.828727 maxwelld-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-08 16:49:46.000000 maxwelld-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.820727 maxwelld-0.2.8/maxwelld/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.824727 maxwelld-0.2.8/maxwelld/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/client/maxwell_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/client/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.824727 maxwelld-0.2.8/maxwelld/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/core/compose_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/core/compose_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/core/exec_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/core/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16104 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.824727 maxwelld-0.2.8/maxwelld/env_description/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/env_description/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/env_description/env_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/env_description/env_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.824727 maxwelld-0.2.8/maxwelld/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/helpers/bytes_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/helpers/countdown_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/helpers/state_keeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.824727 maxwelld-0.2.8/maxwelld/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/output/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/output/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.824727 maxwelld-0.2.8/maxwelld/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.828727 maxwelld-0.2.8/maxwelld/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/handlers/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/handlers/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/handlers/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/handlers/up.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/server/maxwelld_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.828727 maxwelld-0.2.8/maxwelld/vedro_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/vedro_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/vedro_plugin/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/vedro_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/vedro_plugin/scenario_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/vedro_plugin/scenario_tag_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/vedro_plugin/state_waiting.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/version
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-08 16:49:46.000000 maxwelld-0.2.8/maxwelld/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 16:49:54.828727 maxwelld-0.2.8/maxwelld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-08 16:49:54.000000 maxwelld-0.2.8/maxwelld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-08 16:49:54.000000 maxwelld-0.2.8/maxwelld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 16:49:54.000000 maxwelld-0.2.8/maxwelld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-08 16:49:54.000000 maxwelld-0.2.8/maxwelld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-08 16:49:54.000000 maxwelld-0.2.8/maxwelld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 16:49:54.828727 maxwelld-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-08 16:49:46.000000 maxwelld-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.526072 maxwelld-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-09 07:58:32.000000 maxwelld-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-09 07:58:42.526072 maxwelld-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-09 07:58:32.000000 maxwelld-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.518072 maxwelld-0.2.9/maxwelld/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.518072 maxwelld-0.2.9/maxwelld/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/client/maxwell_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/client/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_files_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/compose_run_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/sequence_run_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/env_description/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/env_description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/env_description/env_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/env_description/env_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/bytes_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/countdown_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/helpers/state_keeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/output/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.522072 maxwelld-0.2.9/maxwelld/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/handlers/up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/server/maxwelld_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.526072 maxwelld-0.2.9/maxwelld/vedro_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/scenario_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/scenario_tag_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/vedro_plugin/state_waiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/version
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-09 07:58:32.000000 maxwelld-0.2.9/maxwelld/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 07:58:42.526072 maxwelld-0.2.9/maxwelld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-09 07:58:42.000000 maxwelld-0.2.9/maxwelld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 07:58:42.526072 maxwelld-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-09 07:58:32.000000 maxwelld-0.2.9/setup.py
```

### Comparing `maxwelld-0.2.8/LICENSE` & `maxwelld-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/PKG-INFO` & `maxwelld-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxwelld
-Version: 0.2.8
+Version: 0.2.9
 Summary: docker compose testing env orchestrator
 Home-page: https://github.com/ko10ok/maxwelld
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `maxwelld-0.2.8/README.md` & `maxwelld-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/__init__.py` & `maxwelld-0.2.9/maxwelld/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from maxwelld.client.maxwell_client import MaxwellDemonClient
-from maxwelld.core.exec_types import ComposeConfig
+from maxwelld.core.sequence_run_types import ComposeConfig
 from maxwelld.core.service import MaxwellDemonService
 from maxwelld.env_description.env_tools import off
 from maxwelld.env_description.env_types import AsIs
 from maxwelld.env_description.env_types import DEFAULT_ENV
 from maxwelld.env_description.env_types import Env
 from maxwelld.env_description.env_types import Environment
 from maxwelld.env_description.env_types import Environments
```

### Comparing `maxwelld-0.2.8/maxwelld/client/maxwell_client.py` & `maxwelld-0.2.9/maxwelld/client/maxwell_client.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/core/compose_data_types.py` & `maxwelld-0.2.9/maxwelld/core/compose_data_types.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/core/compose_interface.py` & `maxwelld-0.2.9/maxwelld/core/compose_interface.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/core/service.py` & `maxwelld-0.2.9/maxwelld/core/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from typing import Union
 
 from rich.text import Text
 
 from maxwelld.client.types import EnvironmentId
 from maxwelld.core.compose_data_types import ServicesComposeState
 from maxwelld.core.compose_interface import dc_state
-from maxwelld.core.exec_types import EMPTY_ID
-from maxwelld.core.exec_types import EnvConfigInstance
-from maxwelld.core.utils import actualize_in_flight
-from maxwelld.core.utils import down_in_flight_envs
-from maxwelld.core.utils import get_new_env_id
-from maxwelld.core.utils import make_debug_bash_env
-from maxwelld.core.utils import make_env_compose_instance_files
-from maxwelld.core.utils import make_env_config_instance
-from maxwelld.core.utils import run_env
-from maxwelld.core.utils import unpack_services_env_template_params
+from maxwelld.core.sequence_run_types import EMPTY_ID
+from maxwelld.core.sequence_run_types import EnvConfigInstance
+from maxwelld.core.compose_run_sequences import actualize_in_flight
+from maxwelld.core.compose_run_sequences import down_in_flight_envs
+from maxwelld.core.compose_run_sequences import get_new_env_id
+from maxwelld.core.compose_run_sequences import make_debug_bash_env
+from maxwelld.core.compose_run_sequences import make_env_compose_instance_files
+from maxwelld.core.compose_run_sequences import make_env_config_instance
+from maxwelld.core.compose_run_sequences import run_env
+from maxwelld.core.compose_run_sequences import unpack_services_env_template_params
 from maxwelld.env_description.env_types import Environment
 from maxwelld.helpers.bytes_pickle import base64_pickled
 from maxwelld.helpers.bytes_pickle import debase64_pickled
 from maxwelld.output.console import CONSOLE
 from maxwelld.output.styles import Style
```

### Comparing `maxwelld-0.2.8/maxwelld/env_description/env_tools.py` & `maxwelld-0.2.9/maxwelld/env_description/env_tools.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/env_description/env_types.py` & `maxwelld-0.2.9/maxwelld/env_description/env_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,20 +26,48 @@
         self.value = value
 
 
 class Env(Dict):
     ...
 
 
-class EventStage(Enum):
-    BEFORE_ALL = auto()
-    BEFORE_SERVICE_START = auto()
-    AFTER_SERVICE_START = auto()
-    AFTER_ALL = auto()
+class StageName(NamedTuple):
+    compose_name: str
+
 
+class EventStage(Enum):
+    BEFORE_ALL = StageName('before_all')
+    BEFORE_SERVICE_START = StageName('before_start')
+    AFTER_SERVICE_START = StageName('after_start')
+    AFTER_ALL = StageName('after_all')
+
+    @classmethod
+    def get_all_stages(cls):
+        return [
+            cls.BEFORE_ALL,
+            cls.AFTER_SERVICE_START,
+            cls.AFTER_ALL,
+            cls.BEFORE_SERVICE_START
+        ]
+
+    @classmethod
+    def get_all_compose_stages(cls):
+        return [
+            cls.BEFORE_ALL.value.compose_name,
+            cls.AFTER_SERVICE_START.value.compose_name,
+            cls.AFTER_ALL.value.compose_name,
+            cls.BEFORE_SERVICE_START.value.compose_name
+        ]
+
+    @classmethod
+    def get_compose_stage(cls, stage_name: str) -> 'EventStage':
+        for stage in cls.get_all_stages():
+            if stage.value.compose_name == stage_name:
+                return stage
+        assert False, 'No such stage: {}'.format(stage_name)
 
 class Handler(NamedTuple):
     stage: EventStage
     cmd: str
     executor: str = None
```

### Comparing `maxwelld-0.2.8/maxwelld/helpers/state_keeper.py` & `maxwelld-0.2.9/maxwelld/helpers/state_keeper.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/server/handlers/env.py` & `maxwelld-0.2.9/maxwelld/server/handlers/env.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/server/handlers/status.py` & `maxwelld-0.2.9/maxwelld/server/handlers/status.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/server/handlers/up.py` & `maxwelld-0.2.9/maxwelld/server/handlers/up.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/server/maxwelld_server.py` & `maxwelld-0.2.9/maxwelld/server/maxwelld_server.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/vedro_plugin/logger.py` & `maxwelld-0.2.9/maxwelld/vedro_plugin/logger.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/vedro_plugin/plugin.py` & `maxwelld-0.2.9/maxwelld/vedro_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from vedro.events import ScenarioRunEvent
 from vedro.events import StartupEvent
 
 from maxwelld.client.maxwell_client import MaxwellDemonClient
 from maxwelld.vedro_plugin.state_waiting import JobResult
 from maxwelld.vedro_plugin.logger import WaitVerbosity
 from maxwelld.vedro_plugin.state_waiting import wait_all_services_up
-from maxwelld.core.exec_types import ComposeConfig
-from maxwelld.core.utils import setup_env_for_tests
+from maxwelld.core.sequence_run_types import ComposeConfig
+from maxwelld.core.compose_run_sequences import setup_env_for_tests
 from maxwelld.env_description.env_types import Environments
 from maxwelld.output.console import CONSOLE
 from maxwelld.output.styles import Style
 from maxwelld.vedro_plugin.scenario_ordering import EnvTagsOrderer
 from maxwelld.vedro_plugin.scenario_tag_processing import extract_scenario_config
 from maxwelld.vedro_plugin.scenario_tag_processing import extract_scenarios_configs_set
```

### Comparing `maxwelld-0.2.8/maxwelld/vedro_plugin/scenario_tag_processing.py` & `maxwelld-0.2.9/maxwelld/vedro_plugin/scenario_tag_processing.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld/vedro_plugin/state_waiting.py` & `maxwelld-0.2.9/maxwelld/vedro_plugin/state_waiting.py`

 * *Files identical despite different names*

### Comparing `maxwelld-0.2.8/maxwelld.egg-info/PKG-INFO` & `maxwelld-0.2.9/maxwelld.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxwelld
-Version: 0.2.8
+Version: 0.2.9
 Summary: docker compose testing env orchestrator
 Home-page: https://github.com/ko10ok/maxwelld
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `maxwelld-0.2.8/maxwelld.egg-info/SOURCES.txt` & `maxwelld-0.2.9/maxwelld.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 maxwelld.egg-info/requires.txt
 maxwelld.egg-info/top_level.txt
 maxwelld/client/__init__.py
 maxwelld/client/maxwell_client.py
 maxwelld/client/types.py
 maxwelld/core/__init__.py
 maxwelld/core/compose_data_types.py
+maxwelld/core/compose_files_utils.py
 maxwelld/core/compose_interface.py
-maxwelld/core/exec_types.py
+maxwelld/core/compose_run_sequences.py
+maxwelld/core/sequence_run_types.py
 maxwelld/core/service.py
-maxwelld/core/utils.py
 maxwelld/env_description/__init__.py
 maxwelld/env_description/env_tools.py
 maxwelld/env_description/env_types.py
 maxwelld/helpers/__init__.py
 maxwelld/helpers/bytes_pickle.py
 maxwelld/helpers/countdown_counter.py
 maxwelld/helpers/state_keeper.py
```

### Comparing `maxwelld-0.2.8/setup.py` & `maxwelld-0.2.9/setup.py`

 * *Files identical despite different names*


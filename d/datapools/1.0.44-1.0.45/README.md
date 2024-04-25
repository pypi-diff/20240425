# Comparing `tmp/datapools-1.0.44.tar.gz` & `tmp/datapools-1.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.44.tar", last modified: Sat Apr 20 18:46:28 2024, max compression
+gzip compressed data, was "datapools-1.0.45.tar", last modified: Thu Apr 25 14:37:49 2024, max compression
```

## Comparing `datapools-1.0.44.tar` & `datapools-1.0.45.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 18:46:18.000000 datapools-1.0.44/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:18.000000 datapools-1.0.44/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-20 18:46:18.000000 datapools-1.0.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-20 18:46:18.000000 datapools-1.0.44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-20 18:46:28.676915 datapools-1.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-20 18:46:18.000000 datapools-1.0.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.664915 datapools-1.0.44/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.664915 datapools-1.0.44/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.668915 datapools-1.0.44/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.672915 datapools-1.0.44/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-20 18:46:18.000000 datapools-1.0.44/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 18:46:28.000000 datapools-1.0.44/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:46:28.676915 datapools-1.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-20 18:46:18.000000 datapools-1.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:28.676915 datapools-1.0.44/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:46:18.000000 datapools-1.0.44/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-20 18:46:18.000000 datapools-1.0.44/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 18:46:18.000000 datapools-1.0.44/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.354473 datapools-1.0.45/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 14:37:36.000000 datapools-1.0.45/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-04-25 14:37:36.000000 datapools-1.0.45/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-25 14:37:36.000000 datapools-1.0.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 14:37:36.000000 datapools-1.0.45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 14:37:49.350473 datapools-1.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 14:37:36.000000 datapools-1.0.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.338473 datapools-1.0.45/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.342473 datapools-1.0.45/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12221 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.346473 datapools-1.0.45/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-04-25 14:37:36.000000 datapools-1.0.45/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 14:37:49.000000 datapools-1.0.45/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:37:49.354473 datapools-1.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 14:37:36.000000 datapools-1.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:49.350473 datapools-1.0.45/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:37:36.000000 datapools-1.0.45/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-25 14:37:36.000000 datapools-1.0.45/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 14:37:36.000000 datapools-1.0.45/tests/test_base.py
```

### Comparing `datapools-1.0.44/LICENSE` & `datapools-1.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.44/PKG-INFO` & `datapools-1.0.45/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.44
+Version: 1.0.45
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.44/README.md` & `datapools-1.0.45/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.44/datapools/api.py` & `datapools-1.0.45/datapools/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,49 @@
-import os
-import json
 import asyncio
-import websockets
+import json
+import os
 import urllib
-
 from typing import Optional
 
+import websockets
+
+from datapools.common.logger import logger
+from datapools.common.types import BaseProducerSettings, SchedulerSettings, WorkerSettings
 from datapools.producer import BaseProducer
 from datapools.scheduler import CrawlerScheduler
 from datapools.worker.worker import CrawlerWorker
-from datapools.common.logger import logger
-
-from datapools.common.types import (
-    BaseProducerSettings,
-    SchedulerSettings,
-    WorkerSettings,
-)
-
 
 """
 In cli mode `plugins` keys are used to define WorkerSettings.USE_ONLY_PLUGINS and ADDITIONAL_PLUGINS fields:
 So only listed plugins will be loaded.
 
 `queue.connection_url` expects Rabbitmq running locally. 
 Run it as `docker run --rm -p 15672:15672 -p 5672:5672 rabbitmq:3.10.7-management` for example
 """
 default_config = {
-    "backend": {
-        "api_url": "https://openlicense.ai/openlicense/api/",
-        "hints_period": 10
-    },
-    "queue": {
-        "connection_url": "amqp://guest:guest@localhost:5672",
-        "size_limit": 1
-    },
-    "redis": {
-        "host": "localhost",
-        "port": 6379
-    },
-    "storage": {
-        "worker": {
-            "path": "/tmp/datapools_storage"
-        },
-        "producer": {
-            "path": None
-        }
-    },
+    "backend": {"api_url": "https://openlicense.ai/openlicense/api/", "hints_period": 10},
+    "queue": {"connection_url": "amqp://guest:guest@localhost:5672", "size_limit": 1},
+    "redis": {"host": "localhost", "port": 6379},
+    "storage": {"worker": {"path": "/tmp/datapools_storage"}, "producer": {"path": None}},
     "plugins": {
-        "s3": {
-            "aws_access_key_id": None,
-            "aws_secret_access_key": None
-        },
-        "google_drive": {
-            "api_key": ""
-        },
-        "imageshack": {
-        }
-    }
+        "s3": {"aws_access_key_id": None, "aws_secret_access_key": None},
+        "google_drive": {"api_key": ""},
+        "imageshack": {},
+    },
 }
 
 # async def crawl( hint_urls: Union[AnyUrl, Set[AnyUrl]], config_file: Optional[str] = None):
 
 
 def crawl(datapool_id: int = 1, config_file: Optional[str] = None):
     async def crawl_async():
 
         # loading config from json or using default one
         if config_file is not None:
-            with open(config_file, 'r') as f:
+            with open(config_file, "r") as f:
                 config = json.load(f)
         else:
             config = default_config
 
         # initializing and starting Scheduler
         s_cfg = SchedulerSettings()
         s_cfg.load(config)
@@ -82,57 +54,55 @@
         # initializing and starting Worker
         w_cfg = WorkerSettings()
         w_cfg.load(config)
         w_cfg.CLI_MODE = True
         if not os.path.exists(w_cfg.STORAGE_PATH):
             os.mkdir(w_cfg.STORAGE_PATH)
 
-        plugins_list = [plugin_name for plugin_name in config['plugins']]
+        plugins_list = [plugin_name for plugin_name in config["plugins"]]
         w_cfg.USE_ONLY_PLUGINS = plugins_list
         w_cfg.ADDITIONAL_PLUGINS = plugins_list
 
         worker = CrawlerWorker(w_cfg)
         worker.run()
 
         # initializing and starting Producer
         p_cfg = BaseProducerSettings()
         p_cfg.load(config)
         p_cfg.CLI_MODE = True
-        if p_cfg.STORAGE_PATH is not None and not os.path.exists(
-                p_cfg.STORAGE_PATH):
+        if p_cfg.STORAGE_PATH is not None and not os.path.exists(p_cfg.STORAGE_PATH):
             os.mkdir(p_cfg.STORAGE_PATH)
 
         producer = BaseProducer(p_cfg)
         producer.run()
 
         # get datapool contents stream from the backend
-        o = urllib.parse.urlparse(
-            f"{config[ 'backend_api_url' ]}get-datapool-stream")
-        if o.scheme == 'http':
-            url = o._replace(scheme='ws').geturl()
-        elif o.scheme == 'https':
-            url = o._replace(scheme='wss').geturl()
-        logger.info(f'connecting backend websocket {url=}')
+        o = urllib.parse.urlparse(f"{config[ 'backend_api_url' ]}get-datapool-stream")
+        if o.scheme == "http":
+            url = o._replace(scheme="ws").geturl()
+        elif o.scheme == "https":
+            url = o._replace(scheme="wss").geturl()
+        logger.info(f"connecting backend websocket {url=}")
 
         async with websockets.connect(url) as ws:
-            logger.info('connected backend websocket')
+            logger.info("connected backend websocket")
             await ws.send(json.dumps({"id": datapool_id}))
-            logger.info('sent stream request')
+            logger.info("sent stream request")
             try:
                 while True:
                     msg = json.loads(await ws.recv())
-                    logger.info(f'{msg=}')
-                    await scheduler.add_download_task(msg['url'], msg['type'])
+                    logger.info(f"{msg=}")
+                    await scheduler.add_download_task(msg["url"], msg["type"])
             except websockets.exceptions.ConnectionClosed:
-                logger.info('connection closed')
+                logger.info("connection closed")
 
-        logger.info('pushing end marker')
+        logger.info("pushing end marker")
         # telling scheduler that this is the end of stream
-        await scheduler.add_download_task('')
+        await scheduler.add_download_task("")
 
         await asyncio.gather(scheduler.wait(), worker.wait(), producer.wait())
-        logger.info('waited all')
+        logger.info("waited all")
 
         await asyncio.gather(scheduler.stop(), worker.stop(), producer.stop())
-        logger.info('stopped all')
+        logger.info("stopped all")
 
-    asyncio.run(crawl_async())
+    asyncio.run(crawl_async())
```

### Comparing `datapools-1.0.44/datapools/cli.py` & `datapools-1.0.45/datapools/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-import asyncio
 import logging
-from typing import List
 
 import click
 
-from datapools.common.logger import logger, setup_logger
 from datapools.api import crawl
+from datapools.common.logger import logger, setup_logger
 
 
 class NotRequiredIf(click.Option):
     def __init__(self, *args, **kwargs):
         self.not_required_if = kwargs.pop("not_required_if")
         assert self.not_required_if, "'not_required_if' parameter required"
         kwargs["help"] = (
-            kwargs.get("help", "")
-            + " NOTE: This argument is mutually exclusive with %s"
-            % self.not_required_if
+            kwargs.get("help", "") + " NOTE: This argument is mutually exclusive with %s" % self.not_required_if
         ).strip()
         super(NotRequiredIf, self).__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         we_are_present = self.name in opts
         other_present = self.not_required_if in opts
 
         if other_present:
             if we_are_present:
                 raise click.UsageError(
-                    "Illegal usage: `%s` is mutually exclusive with `%s`"
-                    % (self.name, self.not_required_if)
+                    "Illegal usage: `%s` is mutually exclusive with `%s`" % (self.name, self.not_required_if)
                 )
             else:
                 self.prompt = None
 
         return super(NotRequiredIf, self).handle_parse_result(ctx, opts, args)
 
 
@@ -43,16 +38,14 @@
         # await crawl( hint_urls, config_file )
         crawl(id, config_file)
         logger.info("crawl done")
     except KeyboardInterrupt as e:
         logger.info("exiting")
 
 
-
-
 @click.group(invoke_without_command=True)
 @click.option(
     "-l",
     "--loglevel",
     type=str,
     default="info",
     help="info, debug, error, warning}}",
@@ -80,12 +73,12 @@
     #             hint_urls = set()
     #             for line in lines:
     #                 line = line.strip()
     #                 if len(line):
     #                     hint_urls.add(line)
     #     else:
     #         raise Exception("Expect --hint-url or --hint-urls-file argument(s)")
-    id = kwargs.get('id')
+    id = kwargs.get("id")
 
-    config_file = kwargs.get('config_file')
+    config_file = kwargs.get("config_file")
     # return (hint_urls, config_file)
     return (id, config_file)
```

### Comparing `datapools-1.0.44/datapools/common/backend_api.py` & `datapools-1.0.45/datapools/common/backend_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import List
-
 import httpx
-from pydantic import BaseModel
 
 from ..common.logger import logger
 from ..common.types import CrawlerHintURLStatus  # , DatapoolRules
 
-
 # class TagDatapool(BaseModel):
 #     id: int
 #     rules: DatapoolRules
 
 #     class Config:
 #         validate_assignment = True
 
 
+class BackendAPIException(Exception):
+    def __str__(self):
+        return f"BackendAPIException: {self.args[0] if self.args else ''}"
+
+
 class BackendAPI:
     def __init__(self, url):
         self.url = url
 
     async def get_hint_urls(self, limit):
         res = await self.get_uri("get-hint-urls", {"limit": limit})
         return res if res is not None else []
 
     async def set_hint_url_status(self, hint_id, status: CrawlerHintURLStatus, session_id=None):
         return await self.get_uri(
             "set-hint-url-status", {"id": hint_id, "status": status.value, "session_id": session_id}
         )
+
     async def notify_session_stopped(self, session_id):
-        return await self.get_uri(
-            f"notify-crawler-session-stopped/{session_id}"
-        )
+        return await self.get_uri(f"notify-crawler-session-stopped/{session_id}")
 
     # async def add_crawler_contents( self, contents: dict ):
     #     return await self.get_uri( 'add-crawler-contents', { 'contents': contents } )
 
     # async def get_crawled_contents(self, limit):
     #     return await self.get_uri( 'get-crawled-contents', { 'limit': limit } )
 
     async def add_crawled_content(self, data):
         return await self.get_uri("add-crawled-content", data)
-    
+
     async def add_demo_user(self, data):
-        return await self.get_uri('add-demo-user', data)
+        return await self.get_uri("add-demo-user", data)
 
     # async def get_tag_datapools(self, tag_id) -> List[TagDatapool]:
     #     res = await self.get_uri(
     #         "get-tag-datapools", {"filter": {"tag_id": tag_id}}
     #     )
     #     # logger.info( f"get_tag_datapools {res=}")
     #     for i in range(len(res)):
@@ -60,10 +60,10 @@
 
             try:
                 r = await client.post(url, json=data)
                 if r.status_code == 200:
                     return r.json()
                 else:
                     logger.error(f"Non 200 http response {r=}")
-                    raise Exception("non 200 response")
+                    raise BackendAPIException("non 200 response")
             except httpx.ConnectError as e:
-                logger.error( f'Failed connect Backend API server: {e}')
+                logger.error(f"Failed connect Backend API server: {e}")
```

### Comparing `datapools-1.0.44/datapools/common/queues/__init__.py` & `datapools-1.0.45/datapools/common/queues/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,27 @@
 
 # from pydantic import AnyUrl, BaseModel
 from ..logger import logger
 from .types import *
 
 
 class GenericQueue:
-    def __init__(
-        self, role: QueueRole, url=None, name=None, size=1, topic=None
-    ):
+    def __init__(self, role: QueueRole, url=None, name=None, size=1, topic=None):
         parsed = urlparse(url)
         if parsed.scheme == "amqp":
             import aio_pika
 
             from .rabbitmq import RabbitmqParams, RabbitmqQueue
 
             params = RabbitmqParams(prefetch_count=size)
             if topic is not None:
                 params.exchange_type = aio_pika.ExchangeType.TOPIC
                 params.routing_key = topic
 
-            logger.info(
-                f"RabbitmqQueue {url=}"
-            )
+            logger.info(f"RabbitmqQueue {url=}")
             self.queue = RabbitmqQueue(role, url, name, params)
         else:
             raise Exception(f"not supported {url=}")
 
     def run(self):
         self.queue.run()
```

### Comparing `datapools-1.0.44/datapools/common/queues/rabbitmq.py` & `datapools-1.0.45/datapools/common/queues/rabbitmq.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
 class RestAPI:
     def __init__(self, connection_url):
         p = urlparse(connection_url)
         # TODO: port should be configurable
         self.url = f"http://{p.username}:{p.password}@{p.hostname}:15672/api/"
 
-        logging.getLogger("httpx").setLevel(
-            logging.WARNING
-        )  # disable verbose logging when global level is INFO
+        logging.getLogger("httpx").setLevel(logging.WARNING)  # disable verbose logging when global level is INFO
 
     async def get_queue(self, queue_name):
         async with AsyncClient() as client:
             r = await client.get(f"{self.url}queues/%2f/{queue_name}")
             q = r.json()
             # print(q)
             return q
@@ -52,17 +50,15 @@
     ):
         super().__init__()
         self.role = role
         self.url = connection_url
         self.params = params
         self.queue_name = queue_name  # rabbitmq router_key
         self.internal_queue = asyncio.Queue()
-        self.ready_state = {
-            self.role: asyncio.Event()
-        }  # dict is for future: may support both server+client
+        self.ready_state = {self.role: asyncio.Event()}  # dict is for future: may support both server+client
         self.is_working = asyncio.Lock()
         self.rest_api = RestAPI(self.url)
 
     def run(self):
         # logger.info( f'{id(self.role)=} {id(QueueRole.Receiver)=} {id(QueueRole.Publisher)=}' )
         if self.role == QueueRole.Publisher:
             self.tasks.append(asyncio.create_task(self.publisher_loop()))
@@ -104,52 +100,48 @@
         last_log = 0
         while True:
             # is internal queue empty?
             if self.internal_queue.empty():
                 # if receiver then is receiver queue empty?
                 if self.role == QueueRole.Receiver:
                     queue = await self.rest_api.get_queue(self.queue_name)
-                    if 'message_stats' in queue:
+                    if "message_stats" in queue:
                         if time.time() - last_log > 5:
                             last_log = time.time()
                             logger.info(
                                 f'=================== receiver queue size {self.queue_name} {self.params} {queue["messages"]=} {queue["messages_unacknowledged"]=} {queue["message_stats"]["publish"]=} {queue["message_stats"]["deliver_get"]=}'
                             )
                         if (
                             queue["messages"] == 0
                             and queue["messages_unacknowledged"] == 0
                             # ensures that at least anything was put into and got out of the queue.
-                            and queue['message_stats']['publish'] > 0
-                            and queue['message_stats']['deliver_get'] >= queue['message_stats']['publish']
+                            and queue["message_stats"]["publish"] > 0
+                            and queue["message_stats"]["deliver_get"] >= queue["message_stats"]["publish"]
                         ):
                             break
-                    elif queue['messages'] == 0 and 'message_stats' not in queue:
+                    elif queue["messages"] == 0 and "message_stats" not in queue:
                         # non touched queue => nothing to wait
                         break
                 elif self.role == QueueRole.Publisher:
                     break
                 else:
                     raise Exception("not implemented")
             await asyncio.sleep(1)
 
     async def mark_done(self, message: aio_pika.IncomingMessage):
         try:
             await message.ack()
         except aio_pika.exceptions.ChannelInvalidStateError:
-            logger.error(
-                f"ack for {message.message_id=} failed with ChannelInvalidStateError"
-            )
+            logger.error(f"ack for {message.message_id=} failed with ChannelInvalidStateError")
 
     async def reject(self, message: aio_pika.IncomingMessage, requeue: bool):
         try:
             await message.reject(requeue)
         except aio_pika.exceptions.ChannelInvalidStateError:
-            logger.error(
-                f"reject for {message.message_id=} failed with ChannelInvalidStateError"
-            )
+            logger.error(f"reject for {message.message_id=} failed with ChannelInvalidStateError")
 
     async def is_ready(self):
         await self.ready_state[self.role].wait()
 
     async def publisher_loop(self):
         try:
             while not await self.is_stopped():
@@ -163,36 +155,26 @@
                 logger.info(f"rabbitmq {connection=} --------------------")
 
                 async with connection:
                     channel = await connection.channel()
                     logger.info(f"rabbitmq {channel=} ----------------------")
 
                     # Declaring queue
-                    self.receiver_queue = await channel.declare_queue(
-                        self.queue_name, durable=True
-                    )
+                    self.receiver_queue = await channel.declare_queue(self.queue_name, durable=True)
 
                     # TODO: can combine those conditions into single declare_exchange() expression
-                    if (
-                        self.params.exchange_type
-                        == aio_pika.ExchangeType.DIRECT
-                    ):
+                    if self.params.exchange_type == aio_pika.ExchangeType.DIRECT:
                         exchange = channel.default_exchange
-                    elif (
-                        self.params.exchange_type
-                        == aio_pika.ExchangeType.TOPIC
-                    ):
+                    elif self.params.exchange_type == aio_pika.ExchangeType.TOPIC:
                         exchange = await channel.declare_exchange(
                             name=self._gen_queue_exchange_name(),
                             type=self.params.exchange_type,
                         )
                     else:
-                        raise Exception(
-                            f"not supported {self.params.exchange_type=}"
-                        )
+                        raise Exception(f"not supported {self.params.exchange_type=}")
 
                     self.ready_state[QueueRole.Publisher].set()
 
                     try:
                         while not await self.is_stopped():
                             # logger.info( f'puslisher {self.queue_name} loop iteration')
                             message = await self.pop(1)
@@ -214,31 +196,27 @@
                                     routing_key=routing_key,
                                 )
                                 # logger.info( f'published into {routing_key=}')
 
                                 self.internal_queue.task_done()
 
                     except Exception as e:
-                        logger.error(
-                            f"!!!!!!!!!!!!!!!!!! exception in RabbitmqQueue::publisher_loop"
-                        )
+                        logger.error(f"!!!!!!!!!!!!!!!!!! exception in RabbitmqQueue::publisher_loop")
                         logger.error(traceback.format_exc())
 
                 self.ready_state[QueueRole.Publisher].clear()
 
         except Exception as e:
             logger.error(f"!!!!!!!!!!!!!!!!!! exception in rabbitmq")
             logger.error(traceback.format_exc())
 
     def _gen_queue_exchange_name(self):
         return f"{self.queue_name}_exchange"
 
-    async def receive_message(
-        self, message: aio_pika.message.IncomingMessage
-    ) -> None:
+    async def receive_message(self, message: aio_pika.message.IncomingMessage) -> None:
         # logger.info(
         #     f"RABBITMQ incoming message {type(message)} {message.message_id=} {message.info()=}"
         # )
         # logger.info(f"{message.channel=}")
         # logger.info(message.body)
         await self.push(message)
 
@@ -248,67 +226,51 @@
                 try:
                     connection = await aio_pika.connect_robust(self.url)
                 except aiormq.exceptions.AMQPConnectionError:
                     logger.info("Failed connect to rabbitmq, waiting..")
                     await asyncio.sleep(5)
                     continue
 
-                logger.info(
-                    f"rabbitmq {self.queue_name} {connection=} -----------------------"
-                )
+                logger.info(f"rabbitmq {self.queue_name} {connection=} -----------------------")
 
                 try:
                     # Creating channel
                     channel = await connection.channel()
-                    logger.info(
-                        f"rabbitmq {self.queue_name} {channel=} ----------------------"
-                    )
+                    logger.info(f"rabbitmq {self.queue_name} {channel=} ----------------------")
 
                     # Maximum message count which will be processing at the same time.
-                    await channel.set_qos(
-                        prefetch_count=self.params.prefetch_count
-                    )
+                    await channel.set_qos(prefetch_count=self.params.prefetch_count)
 
                     # Declaring queue
-                    self.receiver_queue = await channel.declare_queue(
-                        self.queue_name, durable=True
-                    )
+                    self.receiver_queue = await channel.declare_queue(self.queue_name, durable=True)
 
                     # print(self.receiver_queue)
-                    if (
-                        self.params.exchange_type
-                        == aio_pika.ExchangeType.TOPIC
-                    ):
+                    if self.params.exchange_type == aio_pika.ExchangeType.TOPIC:
                         exchange_name = self._gen_queue_exchange_name()
                         await channel.declare_exchange(
                             name=exchange_name,
                             type=aio_pika.ExchangeType.TOPIC,
                         )
-                        rks = self.params.routing_key if isinstance(self.params.routing_key, list) else [
-                            self.params.routing_key]
+                        rks = (
+                            self.params.routing_key
+                            if isinstance(self.params.routing_key, list)
+                            else [self.params.routing_key]
+                        )
                         for rk in rks:
-                            await self.receiver_queue.bind(
-                                exchange_name, routing_key=rk
-                            )
+                            await self.receiver_queue.bind(exchange_name, routing_key=rk)
                     self.ready_state[QueueRole.Receiver].set()
 
-                    logger.info(
-                        f"rabbitmq {self.queue_name} consume start----------------------------"
-                    )
+                    logger.info(f"rabbitmq {self.queue_name} consume start----------------------------")
 
                     await self.receiver_queue.consume(self.receive_message)
                     await self.stop_event.wait()
 
-                    logger.info(
-                        f"rabbitmq {self.queue_name} consume done----------------------------"
-                    )
+                    logger.info(f"rabbitmq {self.queue_name} consume done----------------------------")
 
                 except Exception as e:
-                    logger.error(
-                        f"!!!!!!!!!!!!!!!!!! exception in rabbitmq receiver_loop {e}"
-                    )
+                    logger.error(f"!!!!!!!!!!!!!!!!!! exception in rabbitmq receiver_loop {e}")
                     logger.error(traceback.format_exc())
 
                 self.ready_state[QueueRole.Receiver].clear()
         except Exception as e:
             logger.error(f"!!!!!!!!!!!!!!!!!! exception in rabbitmq {e}")
             logger.error(traceback.format_exc())
```

### Comparing `datapools-1.0.44/datapools/common/queues/types.py` & `datapools-1.0.45/datapools/common/queues/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,16 @@
         return json.dumps(
             {"session_id": self.session_id, "type": self.type.value, "data": json.dumps(self.data)}
         ).encode()
 
     @staticmethod
     def decode(binary):
         j = json.loads(binary.decode())
-        res = QueueMessage( 
-            session_id=j['session_id'],
-            message_type=QueueMessageType(j["type"]), 
-            data=json.loads(j["data"])
+        res = QueueMessage(
+            session_id=j["session_id"], message_type=QueueMessageType(j["type"]), data=json.loads(j["data"])
         )
         return res
 
 
 class QueueTopicMessage:
     def __init__(self, topic, data):
         self.topic = topic.split(".")
```

### Comparing `datapools-1.0.44/datapools/common/stoppable.py` & `datapools-1.0.45/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.44/datapools/common/storage/base_storage.py` & `datapools-1.0.45/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.44/datapools/common/storage/file_storage.py` & `datapools-1.0.45/datapools/common/storage/file_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
             res = f.read()
             return res
 
     async def remove(self, storage_id):
         path = self.get_path(storage_id)
         logger.info(f"unlink {path=}")
         os.unlink(path)
-        
-    async def has( self, storage_id):
+
+    async def has(self, storage_id):
         path = self.get_path(storage_id)
-        return os.path.exists( path )
+        return os.path.exists(path)
 
     def get_path(self, storage_id):
         return os.path.join(self.dst_path, storage_id)
```

### Comparing `datapools-1.0.44/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.45/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.44/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.45/datapools/common/tasks_db/tasks_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 TaskOrNone: TypeAlias = Union[dict, None]
 
 
 class TasksDB:
     def __init__(self):
         pass
 
-    def add(
-        self, task, score=0, ignore_existing=False, ignore_done=False
-    ) -> Union[Hash, Literal[False]]:
+    def add(self, task, score=0, ignore_existing=False, ignore_done=False) -> Union[Hash, Literal[False]]:
         # puts new url to the queue
         # score may define priority of the task
         # should return False if url is already in the queue
         raise TasksDBException("implement add()")
 
     def has(self, task) -> bool:
         # checks if URL is not in the queue already
```

### Comparing `datapools-1.0.44/datapools/common/types.py` & `datapools-1.0.45/datapools/common/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from enum import Enum, IntEnum
-from abc import abstractmethod
 import json
-from typing import Any, List, Optional, Set, Union, NamedTuple, TypeAlias
+from abc import abstractmethod
+from enum import Enum, IntEnum
+from typing import Any, List, NamedTuple, Optional, TypeAlias, Union
 
-from pydantic import BaseModel, AnyUrl, validator, ConfigDict
-from .storage import FileStorage
-from .session_manager import Session
+from pydantic import AnyUrl, BaseModel
 from pydantic_settings import BaseSettings
 
+from .session_manager import Session
+from .storage import FileStorage
+
 DEFAULT_QUEUE_WORKER_TASKS = "worker_tasks"
 DEFAULT_QUEUE_REPORTS = "worker_reports"
 DEFAULT_QUEUE_EVAL_TASKS = "eval_tasks"
 DEFAULT_QUEUE_TOPICS = "topics"
 
 DEFAULT_RABBITMQ_HOST = "rabbitmq.crawler"
 DEFAULT_RABBITMQ_PORT: int = 5672
 DEFAULT_REDIS_HOST = "redis.crawler"
 DEFAULT_REDIS_PORT: int = 6379
 
 DEFAULT_CONNECTION_URL: str = "amqp://guest:guest@{host}:{port}/".format(
-    host=DEFAULT_RABBITMQ_HOST,
-    port=DEFAULT_RABBITMQ_PORT)
+    host=DEFAULT_RABBITMQ_HOST, port=DEFAULT_RABBITMQ_PORT
+)
 
 DEFAULT_BACKEND_API_URL: str = "https://openlicense.ai/internal/"
 DEFAULT_BACKEND_HINTS_PERIOD: int = 10  # seconds
 
 
 class InvalidUsageException(Exception):
     pass
 
+
 class SerializableModel(BaseModel):
-    #model_config = ConfigDict(use_enum_values=True)
+    # model_config = ConfigDict(use_enum_values=True)
     pass
 
 
 class BaseCrawlerSettings(BaseSettings):
     def fload(self, json_path):
         """fills self using json file path"""
-        with open(json_path, 'r') as fp:
+        with open(json_path, "r") as fp:
             config = json.load(fp)  # expects dict output
             self.load(config)
 
     @abstractmethod
     def load(self, config: dict):
         pass
 
@@ -58,37 +60,35 @@
 
     WORKER_TASKS_QUEUE_NAME: str = DEFAULT_QUEUE_WORKER_TASKS
     WORKER_REPORTS_QUEUE_NAME: str = DEFAULT_QUEUE_REPORTS
 
     def load(self, config: dict):
         """fills self with json config"""
         # Queue
-        queue = config.get('queue', {})
-        queue_connection_url = queue.get('connection_url')
+        queue = config.get("queue", {})
+        queue_connection_url = queue.get("connection_url")
         if queue_connection_url is not None:
             self.QUEUE_CONNECTION_URL = queue_connection_url
 
-        self.WORKER_TASKS_QUEUE_NAME = queue.get(
-            'worker_tasks_queue_name', DEFAULT_QUEUE_WORKER_TASKS)
-        self.WORKER_REPORTS_QUEUE_NAME = queue.get(
-            'worker_reports_queue_name', DEFAULT_QUEUE_REPORTS)
+        self.WORKER_TASKS_QUEUE_NAME = queue.get("worker_tasks_queue_name", DEFAULT_QUEUE_WORKER_TASKS)
+        self.WORKER_REPORTS_QUEUE_NAME = queue.get("worker_reports_queue_name", DEFAULT_QUEUE_REPORTS)
 
-        backend = config.get('backend', {})
-        api_url = backend.get('api_url')
+        backend = config.get("backend", {})
+        api_url = backend.get("api_url")
         if api_url is not None:
             self.BACKEND_API_URL = api_url
-        hints_period = backend.get('hints_period')
+        hints_period = backend.get("hints_period")
         if hints_period is not None:
             self.BACKEND_HINTS_PERIOD = hints_period
 
-        redis = config.get('redis', {})
-        redis_host = redis.get('host')
+        redis = config.get("redis", {})
+        redis_host = redis.get("host")
         if redis_host is not None:
             self.REDIS_HOST = redis_host
-        redis_port = redis.get('port')
+        redis_port = redis.get("port")
         if redis_port is not None:
             self.REDIS_PORT = redis_port
 
 
 class WorkerSettings(BaseCrawlerSettings):
     QUEUE_CONNECTION_URL: str = DEFAULT_CONNECTION_URL
     TODO_QUEUE_SIZE: int = 1
@@ -118,55 +118,51 @@
     USE_ONLY_PLUGINS: Optional[List[str]] = None
     ADDITIONAL_PLUGINS: Optional[List[str]] = None
 
     plugins_config: dict = {}
 
     def load(self, config: dict):
         """fills self with json config"""
-        backend = config.get('backend', {})
-        api_url = backend.get('api_url')
+        backend = config.get("backend", {})
+        api_url = backend.get("api_url")
         if api_url is not None:
             self.BACKEND_API_URL = api_url
-        
+
         # Queue
-        queue = config.get('queue', {})
-        queue_connection_url = queue.get('connection_url')
+        queue = config.get("queue", {})
+        queue_connection_url = queue.get("connection_url")
         if queue_connection_url is not None:
             self.QUEUE_CONNECTION_URL = queue_connection_url
-        queue_size_limit = queue.get('size_limit')
+        queue_size_limit = queue.get("size_limit")
         if queue_size_limit is not None:
             self.TODO_QUEUE_SIZE = queue_size_limit
 
-        self.WORKER_TASKS_QUEUE_NAME = queue.get(
-            'worker_tasks_queue_name', DEFAULT_QUEUE_WORKER_TASKS)
-        self.WORKER_REPORTS_QUEUE_NAME = queue.get(
-            'worker_reports_queue_name', DEFAULT_QUEUE_REPORTS)
-        self.EVAL_TASKS_QUEUE_NAME = queue.get(
-            'eval_tasks_queue_name', DEFAULT_QUEUE_EVAL_TASKS)
-        self.TOPICS_QUEUE_NAME = queue.get(
-            'topics_queue_name', DEFAULT_QUEUE_TOPICS)
+        self.WORKER_TASKS_QUEUE_NAME = queue.get("worker_tasks_queue_name", DEFAULT_QUEUE_WORKER_TASKS)
+        self.WORKER_REPORTS_QUEUE_NAME = queue.get("worker_reports_queue_name", DEFAULT_QUEUE_REPORTS)
+        self.EVAL_TASKS_QUEUE_NAME = queue.get("eval_tasks_queue_name", DEFAULT_QUEUE_EVAL_TASKS)
+        self.TOPICS_QUEUE_NAME = queue.get("topics_queue_name", DEFAULT_QUEUE_TOPICS)
 
         # redis
-        redis = config.get('redis', {})
-        redis_host = redis.get('host')
+        redis = config.get("redis", {})
+        redis_host = redis.get("host")
         if redis_host is not None:
             self.REDIS_HOST = redis_host
-        redis_port = redis.get('port')
+        redis_port = redis.get("port")
         if redis_port is not None:
             self.REDIS_PORT = redis_port
 
         # Storage
-        storage = config.get('storage', {})
-        worker_storage = storage.get('worker', {})
-        storage_path = worker_storage.get('path')
+        storage = config.get("storage", {})
+        worker_storage = storage.get("worker", {})
+        storage_path = worker_storage.get("path")
         if storage_path is not None:
             self.STORAGE_PATH = storage_path
 
         # plugins
-        self.plugins_config = config.get('plugins', {})
+        self.plugins_config = config.get("plugins", {})
 
 
 class BaseProducerSettings(BaseCrawlerSettings):
     QUEUE_CONNECTION_URL: str = DEFAULT_CONNECTION_URL
     BACKEND_API_URL: str = DEFAULT_BACKEND_API_URL
     STORAGE_PATH: Optional[str] = None
     WORKER_STORAGE_PATH: str = "/worker_storage/"
@@ -177,47 +173,45 @@
     CLI_MODE: bool = False
 
     EVAL_TASKS_QUEUE_NAME: str = DEFAULT_QUEUE_EVAL_TASKS
     TOPICS_QUEUE_NAME: str = DEFAULT_QUEUE_TOPICS
 
     def load(self, config: dict):
         """fills self with json config"""
-        backend = config.get('backend', {})
-        api_url = backend.get('api_url')
+        backend = config.get("backend", {})
+        api_url = backend.get("api_url")
         if api_url is not None:
             self.BACKEND_API_URL = api_url
-        
+
         # Queue
-        queue = config.get('queue', {})
-        queue_connection_url = queue.get('connection_url')
+        queue = config.get("queue", {})
+        queue_connection_url = queue.get("connection_url")
         if queue_connection_url is not None:
             self.QUEUE_CONNECTION_URL = queue_connection_url
 
-        self.EVAL_TASKS_QUEUE_NAME = queue.get(
-            'eval_tasks_queue_name', DEFAULT_QUEUE_EVAL_TASKS)
-        self.TOPICS_QUEUE_NAME = queue.get(
-            'topics_queue_name', DEFAULT_QUEUE_TOPICS)
+        self.EVAL_TASKS_QUEUE_NAME = queue.get("eval_tasks_queue_name", DEFAULT_QUEUE_EVAL_TASKS)
+        self.TOPICS_QUEUE_NAME = queue.get("topics_queue_name", DEFAULT_QUEUE_TOPICS)
 
         # redis
-        redis = config.get('redis', {})
-        redis_host = redis.get('host')
+        redis = config.get("redis", {})
+        redis_host = redis.get("host")
         if redis_host is not None:
             self.REDIS_HOST = redis_host
-        redis_port = redis.get('port')
+        redis_port = redis.get("port")
         if redis_port is not None:
             self.REDIS_PORT = redis_port
 
         # Storage
-        storage = config.get('storage', {})
-        worker_storage = storage.get('worker', {})
-        storage_path = worker_storage.get('path')
+        storage = config.get("storage", {})
+        worker_storage = storage.get("worker", {})
+        storage_path = worker_storage.get("path")
         if storage_path is not None:
             self.WORKER_STORAGE_PATH = storage_path
-        producer_storage = storage.get('producer', {})
-        storage_path = producer_storage.get('path')
+        producer_storage = storage.get("producer", {})
+        storage_path = producer_storage.get("path")
         if storage_path is not None:
             self.STORAGE_PATH = storage_path
 
 
 class CrawlerHintURLStatus(IntEnum):
     Unprocessed = 0
     Success = 1
@@ -238,60 +232,65 @@
             return 1
         if self.value == DatapoolContentType.Image:
             return 2
         if self.value == DatapoolContentType.Video:
             return 3
         if self.value == DatapoolContentType.Audio:
             return 4
-        raise Exception(
-            f"Not supported DatapoolContentType __hash__ {self.value}"
-        )
+        raise Exception(f"Not supported DatapoolContentType __hash__ {self.value}")
 
 
 class BaseCrawlerResult(BaseModel):
     def to_dict(self):
         res = self.__dict__
         return res
 
 
 class CrawlerContent(BaseCrawlerResult):
     tag_id: Optional[str] = None
+    tag_keepout: Optional[bool] = False
     copyright_tag_id: Optional[str] = None
+    copyright_tag_keepout: Optional[bool] = False
     platform_tag_id: Optional[str] = None
+    platform_tag_keepout: Optional[bool] = False
     type: DatapoolContentType
     storage_id: Any
-    url: str
+    url: Union[str, AnyUrl]
 
     def to_dict(self):
         res = self.__dict__
         res["type"] = res["type"].value
         return res
 
 
 class CrawlerBackTask(BaseCrawlerResult):
     url: str
 
-    
+
 class CrawlerDemoUser(BaseCrawlerResult):
     user_name: str
     short_tag_id: str
     platform: str
 
 
 class CrawlerNop(BaseCrawlerResult):
     pass
 
-PriorityTimestamp : TypeAlias = int
+
+PriorityTimestamp: TypeAlias = int
+
+
 class Evaluation(BaseModel):
     nsfw: bool
     score: float
     weight: float
     embeddings: Optional[List[float]] = None
     priority_timestamp: Optional[PriorityTimestamp] = None
 
+
 class WorkerContext(NamedTuple):
     session: Session
     storage: FileStorage
 
 
 class WorkerTask(NamedTuple):
     url: AnyUrl
```

### Comparing `datapools-1.0.44/datapools/producer/base_producer.py` & `datapools-1.0.45/datapools/producer/base_producer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,41 +6,31 @@
 
 # import sys
 import traceback
 
 # from enum import Enum
 from typing import List, Optional
 
-from ..common.backend_api import BackendAPI  # , TagDatapool
+from ..common.backend_api import BackendAPI, BackendAPIException
 from ..common.logger import logger
-from ..common.queues import (
-    GenericQueue,
-    QueueMessage,
-    QueueMessageType,
-    QueueRole,
-    QueueTopicMessage,
-)
+from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole, QueueTopicMessage
+from ..common.session_manager import SessionManager
 from ..common.stoppable import Stoppable
 from ..common.storage.file_storage import FileStorage
-
-from ..common.types import (
-    BaseProducerSettings,
-    InvalidUsageException,
-)
+from ..common.types import BaseProducerSettings, InvalidUsageException
 from ..worker.utils import get_storage_invalidation_topic
-from ..common.session_manager import SessionManager
+
 # from .rules import DatapoolRulesChecker
 
 
 class BaseProducer(Stoppable):
     def __init__(self, cfg: Optional[BaseProducerSettings] = None):
         super().__init__()
         self.cfg = cfg if cfg is not None else BaseProducerSettings()
-        self.session_manager = SessionManager(
-            self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
+        self.session_manager = SessionManager(self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
 
         if not self.cfg.CLI_MODE:
             self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
 
         # receives tasks from workers
         self.eval_queue = GenericQueue(
             role=QueueRole.Receiver,
@@ -66,26 +56,26 @@
         self.tasks.append(asyncio.create_task(self.router_loop()))
         self.eval_queue.run()
         self.topics_queue.run()
         super().run()
 
     async def wait(self):
         if self.cfg.CLI_MODE is False:
-            logger.error('baseproducer invalid usage')
+            logger.error("baseproducer invalid usage")
             raise InvalidUsageException("not a cli mode")
 
-        logger.info('BaseProducer wait()')
+        logger.info("BaseProducer wait()")
         await self.stop_task_received.wait()
-        logger.info('BaseProducer stop_task_received')
+        logger.info("BaseProducer stop_task_received")
         waiters = (
             self.eval_queue.until_empty(),
             self.topics_queue.until_empty(),
         )
         await asyncio.gather(*waiters)
-        logger.info('BaseProducer wait done')
+        logger.info("BaseProducer wait done")
 
     async def stop(self):
         await self.eval_queue.stop()
         await self.topics_queue.stop()
         await super().stop()
         logger.info("BaseProducer stopped")
 
@@ -93,54 +83,53 @@
         try:
             while not await self.is_stopped():
                 message = await self.eval_queue.pop(timeout=1)
                 if message:
                     qm = QueueMessage.decode(message.body)
                     try:
                         if not self.session_manager.has(qm.session_id):
-                            logger.info( f'session is deleted {qm.session_id=}')
+                            logger.info(f"session is deleted {qm.session_id=}")
                             await self.eval_queue.mark_done(message)
                             continue
-                        
+
                         session = self.session_manager.get(qm.session_id)
                         if session.is_stopped():
-                            logger.info( f'session is stopped {qm.session_id=} {message.message_id}')
+                            logger.info(f"session is stopped {qm.session_id=} {message.message_id}")
                             await self.eval_queue.mark_done(message)
                             continue
-                        
+
                         if qm.type == QueueMessageType.Task:
                             task = qm.data
                             logger.info(f"Producer got: {task}")
 
                             # TODO: this storage must be associated with the worker!
                             #   For example, storage path or url can be formatted accordingly to worker id
-                            worker_storage = FileStorage(
-                                self.cfg.WORKER_STORAGE_PATH
-                            )
+                            worker_storage = FileStorage(self.cfg.WORKER_STORAGE_PATH)
                             raw_data = await worker_storage.get(task["storage_id"])
                             await self.process_content(qm.session_id, raw_data, task)
 
                             if not self.is_shared_storage():
                                 # tell worker that his storage item can be removed
                                 await self.topics_queue.push(
                                     QueueTopicMessage(
-                                        get_storage_invalidation_topic(
-                                            task["worker_id"]
-                                        ),
+                                        get_storage_invalidation_topic(task["worker_id"]),
                                         {"storage_id": task["storage_id"]},
                                     )
                                 )
                         elif qm.type == QueueMessageType.Stop:
-                            logger.info('base_producer: stop task received')
+                            logger.info("base_producer: stop task received")
                             self.stop_task_received.set()
                         else:
-                            raise Exception(
-                                f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}")
+                            raise Exception(f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}")
 
                         await self.eval_queue.mark_done(message)
+                    except BackendAPIException as e:
+                        logger.error(str(e))
+                        await self.eval_queue.reject(message)
+                        await asyncio.sleep(5)
                     except Exception as e:
                         logger.error(f"Catched: {traceback.format_exc()}")
                         logger.error(f"failed evaluate {e}")
                         await self.eval_queue.reject(message)
 
         except Exception as e:
             logger.error(f"Catched: {traceback.format_exc()}")
@@ -150,17 +139,15 @@
         # path = os.path.join(self.cfg.STORAGE_PATH, str(datapool_id))
         if not self.is_shared_storage():
             path = self.cfg.STORAGE_PATH
             if not os.path.exists(path):
                 os.mkdir(path)
             storage = FileStorage(path)
             # put data into persistent storage
-            await storage.put(
-                task["storage_id"], raw_data
-            )
+            await storage.put(task["storage_id"], raw_data)
 
         if self.session_manager.has(session_id):
             session = self.session_manager.get(session_id)
             session.inc_evaluated_content()
 
     def is_shared_storage(self):
         return self.cfg.STORAGE_PATH is None or self.cfg.WORKER_STORAGE_PATH == self.cfg.STORAGE_PATH
```

### Comparing `datapools-1.0.44/datapools/scheduler/scheduler.py` & `datapools-1.0.45/datapools/scheduler/scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,21 @@
 # import json
 # import time
 import traceback
 from typing import Optional
 
 from ..common.backend_api import BackendAPI
 from ..common.logger import logger
-from ..common.queues import (
-    GenericQueue,
-    QueueMessage,
-    QueueMessageType,
-    QueueRole,
-)
-from ..common.stoppable import Stoppable
+from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole
 
 # from .common.tasks_db import Hash
 # from .common.tasks_db.redis import RedisTasksDB
 from ..common.session_manager import SessionManager
-from ..common.types import (
-    DatapoolContentType,
-    CrawlerHintURLStatus,
-    SchedulerSettings,
-    InvalidUsageException,
-)
+from ..common.stoppable import Stoppable
+from ..common.types import CrawlerHintURLStatus, DatapoolContentType, InvalidUsageException, SchedulerSettings
 
 # import httpx
 
 
 class CrawlerScheduler(Stoppable):
     # 1. task:
     #   - get hint urls from the backend, put into tasks_db, status is changed at the backend at once
@@ -49,16 +39,15 @@
         self.cfg = cfg if cfg is not None else SchedulerSettings()
 
         if self.cfg.CLI_MODE is True:
             self.cli_tasks = asyncio.Queue()
         else:
             self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
 
-        self.session_manager = SessionManager(
-            self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
+        self.session_manager = SessionManager(self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
 
         # self.tasks_db = RedisTasksDB(
         #     host=self.cfg.REDIS_HOST, port=self.cfg.REDIS_PORT
         # )
         self.todo_queue = GenericQueue(
             role=QueueRole.Publisher,
             url=self.cfg.QUEUE_CONNECTION_URL,
@@ -70,33 +59,33 @@
             url=self.cfg.QUEUE_CONNECTION_URL,
             name=self.cfg.WORKER_REPORTS_QUEUE_NAME,
         )
         logger.info("created receiver reports")
 
         if self.cfg.CLI_MODE:
             self.cli_session = self.session_manager.create()
-            logger.info(f'created session {self.cli_session.id}')
+            logger.info(f"created session {self.cli_session.id}")
 
             # TODO: this mechanism will not work for multiple workers/producers
             self.stop_task_processed = asyncio.Event()
 
     async def wait(self):
         """for CLI mode usage only"""
         if not self.cfg.CLI_MODE:
-            logger.error('scheduler invalid usage')
+            logger.error("scheduler invalid usage")
             raise InvalidUsageException("not a cli mode")
 
         await self.stop_task_processed.wait()
 
         waiters = (
             self.todo_queue.until_empty(),
             self.reports_queue.until_empty(),
         )
         await asyncio.gather(*waiters)
-        logger.info('scheduler wait done')
+        logger.info("scheduler wait done")
 
     def run(self):
         self.tasks.append(asyncio.create_task(self.hints_loop()))
         self.tasks.append(asyncio.create_task(self.reports_loop()))
         self.todo_queue.run()
         self.reports_queue.run()
         super().run()
@@ -113,145 +102,128 @@
     async def _set_task_status(self, session_id, data):
         # hash, status: CrawlerHintURLStatus, contents
         logger.info(f"set_task_status: {session_id=} {data=}")
 
         session = self.session_manager.get(session_id)
 
         meta = session.get_meta()
-        logger.info(f'{meta=}')
+        logger.info(f"{meta=}")
         if not meta:
             return False
 
         status = CrawlerHintURLStatus(data["status"])
 
-        if status in (
-                CrawlerHintURLStatus.Success, CrawlerHintURLStatus.Failure,
-                CrawlerHintURLStatus.Rejected):
+        if status in (CrawlerHintURLStatus.Success, CrawlerHintURLStatus.Failure, CrawlerHintURLStatus.Rejected):
             if status == CrawlerHintURLStatus.Success:
                 session.inc_complete_urls()
             elif status == CrawlerHintURLStatus.Failure:
                 session.inc_failed_urls()
             else:
                 session.inc_rejected_urls()
 
-            if (meta['total_tasks'] == meta['complete_tasks'] + meta['failed_tasks'] + meta['rejected_tasks'] + 1
+            if (
+                meta["total_tasks"] == meta["complete_tasks"] + meta["failed_tasks"] + meta["rejected_tasks"] + 1
                 # and meta[ 'crawled_content'] == meta[ 'evaluated_content']      <--- this will not work here, because producer will evaluate later than task is complete
-                    and meta['hint_id'] is not None):
+                and meta["hint_id"] is not None
+            ):
                 # this is hint url from server => have to update status on the backend
                 if not self.cfg.CLI_MODE:
                     await self.api.set_hint_url_status(meta["hint_id"], status, session_id)
 
     async def _add_task(self, session_id, task: dict):
         if not self.session_manager.has(session_id):
-            logger.error(f'Session not found: {session_id=}')
+            logger.error(f"Session not found: {session_id=}")
             return False
 
         session = self.session_manager.get(session_id)
         if session.is_stopped():
-            logger.info( f'Session is stopped {session_id=}')
+            logger.info(f"Session is stopped {session_id=}")
             return False
 
-        if 'url' in task:
-            #logger.info( f'{task["url"]=}')
-            if not session.has_url(task['url']):
-                session.add_url(task['url'])
-
-                await self.todo_queue.push(
-                    QueueMessage(session_id, QueueMessageType.Task, data=task)
-                )
+        if "url" in task:
+            # logger.info( f'{task["url"]=}')
+            if not session.has_url(task["url"]):
+                session.add_url(task["url"])
+
+                await self.todo_queue.push(QueueMessage(session_id, QueueMessageType.Task, data=task))
             else:
-                #logger.info('task exists, ignored')
+                # logger.info('task exists, ignored')
                 return False
-        elif 'stop_running' in task:
-            await self.todo_queue.push(
-                QueueMessage(session_id, QueueMessageType.Stop)
-            )
+        elif "stop_running" in task:
+            await self.todo_queue.push(QueueMessage(session_id, QueueMessageType.Stop))
         else:
-            raise Exception(f'unsupported {task=}')
+            raise Exception(f"unsupported {task=}")
 
         # logger.info( 'pushed')
         return True
         # return hash
 
     # return False
 
     async def add_download_task(self, url, content_type: Optional[DatapoolContentType] = None):
         """for cli mode: pushing url to the queue. Scheduler will run until empty string is added"""
         if self.cli_tasks is None:
-            logger.error('scheduler invalid usage')
+            logger.error("scheduler invalid usage")
             raise InvalidUsageException("not a cli mode")
         await self.cli_tasks.put((url, content_type))
 
     async def _get_hints(self):
         hints = None
         if not self.cfg.CLI_MODE:
             # deployment mode
             try:
                 hints = await self.api.get_hint_urls(limit=10)
                 for hint in hints:
-                    session = self.session_manager.create(
-                        hint_id=hint.get('id', 0),
-                        url=hint.get('url', '')
-                    )
-                    hint['session_id'] = session.id
+                    session = self.session_manager.create(hint_id=hint.get("id", 0), url=hint.get("url", ""))
+                    hint["session_id"] = session.id
 
             except Exception as e:
                 logger.error(f"Failed get hints: {e}")
         else:
             # cli mode
             try:
                 (url, content_type) = await asyncio.wait_for(self.cli_tasks.get(), timeout=1)
                 if len(url) > 0:
-                    hints = [{"url": url, "content_type": content_type,
-                              "session_id": self.cli_session.id}]
+                    hints = [{"url": url, "content_type": content_type, "session_id": self.cli_session.id}]
                 else:
-                    hints = [{'stop_running': True,
-                              "session_id": self.cli_session.id}]
+                    hints = [{"stop_running": True, "session_id": self.cli_session.id}]
             except asyncio.TimeoutError:
                 pass
         return hints
 
     async def hints_loop(self):
         # infinitely fetching URL hints by calling backend api
         try:
             while not await self.is_stopped():
                 if self.session_manager.is_ready():
                     hints = await self._get_hints()
                     if hints is not None:
                         for hint in hints:
                             logger.info(f"got hint: {hint}")
 
-                            if await self._add_task(
-                                hint.get('session_id'),
-                                hint
-                            ):
+                            if await self._add_task(hint.get("session_id"), hint):
                                 if "id" in hint:
                                     await self.api.set_hint_url_status(
-                                        hint["id"],
-                                        CrawlerHintURLStatus.Processing,
-                                        hint['session_id']
+                                        hint["id"], CrawlerHintURLStatus.Processing, hint["session_id"]
                                     )
                             else:
-                                logger.error('failed add task, REJECTING')
+                                logger.error("failed add task, REJECTING")
                                 if "id" in hint:
                                     await self.api.set_hint_url_status(
                                         hint["id"],
                                         CrawlerHintURLStatus.Rejected,
                                     )
-                                    self.session_manager.remove(
-                                        hint['session_id'])
+                                    self.session_manager.remove(hint["session_id"])
 
                     if not self.cfg.CLI_MODE:
                         await asyncio.sleep(self.cfg.BACKEND_HINTS_PERIOD)
                 else:
                     await asyncio.sleep(1)
         except Exception as e:
-            logger.error(
-                f"!!!!!!! Exception in CrawlerScheduler::hints_loop() {e}"
-            )
+            logger.error(f"!!!!!!! Exception in CrawlerScheduler::hints_loop() {e}")
             logger.error(traceback.format_exc())
 
     async def reports_loop(self):
         # receive reports from workers
         try:
             while not await self.is_stopped():
                 message = await self.reports_queue.pop(timeout=1)
@@ -261,23 +233,21 @@
                         if qm.type == QueueMessageType.Task:
                             # logger.info("new task from worker")
                             # logger.info(f"{qm=}")
                             await self._add_task(qm.session_id, qm.data)
                         elif qm.type == QueueMessageType.Report:
                             await self._set_task_status(qm.session_id, qm.data)
                         elif qm.type == QueueMessageType.Stop:
-                            logger.info('scheduler: got stop from worker')
+                            logger.info("scheduler: got stop from worker")
                             self.stop_task_processed.set()
                         else:
                             logger.error(f"Unsupported QueueMessage {qm=}")
 
                     except Exception as e:
                         logger.error(f"Failed decode {message.body=} {message=}")
                         logger.error(traceback.format_exc())
 
                     await self.reports_queue.mark_done(message)
 
         except Exception as e:
-            logger.error(
-                f"!!!!!!! Exception in CrawlerScheduler::reports_loop() {e}"
-            )
+            logger.error(f"!!!!!!! Exception in CrawlerScheduler::reports_loop() {e}")
             logger.error(traceback.format_exc())
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.45/datapools/worker/plugins/base_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-import sys
-import json
 import base64
+import io
+import sys
+from abc import ABCMeta, abstractmethod
 from hashlib import md5
-from abc import abstractmethod, ABCMeta
-from typing import AsyncGenerator, Union
-from urllib.parse import urlparse, urljoin
-import dns.resolver
 from time import time
-from PIL import Image
-from PIL.ExifTags import Base as ExifTagsList
-import io
-
-
+from typing import AsyncGenerator, Union, Optional
+from urllib.parse import urljoin, urlparse
 
+import dns.resolver
 import httpx
+from PIL import Image
+from PIL.ExifTags import Base as ExifTagsList
 
 from ...common.logger import logger
 from ...common.storage import BaseStorage
 from ...common.types import (
-    CrawlerBackTask,
     BaseCrawlerResult,
-    DatapoolContentType,
+    CrawlerBackTask,
     CrawlerContent,
     CrawlerNop,
+    DatapoolContentType,
     WorkerContext,
     WorkerTask,
 )
 from ...worker.utils import canonicalize_url
 
 try:
     from bs4 import BeautifulSoup
@@ -40,30 +37,30 @@
 
 
 class BasePluginException(Exception):
     pass
 
 
 class BaseTag:
-    _crawling_allowed = None
-    _tag = None
+    _tag: Optional[str] = None
+    _is_keepout: Optional[bool] = None
 
-    def __init__(self, tag, crawling_allowed=True):
+    def __init__(self, tag, keepout=False):
         self._tag = tag
-        self._crawling_allowed = crawling_allowed
+        self._is_keepout = keepout
 
     def __str__(self):
         return self._tag
 
     def __repr__(self):
-        return f"BaseTag(tag={self._tag}, crawling allowed={self._crawling_allowed})"
+        return f"BaseTag(tag={self._tag}, keepout={self._is_keepout})"
+
+    def is_keepout(self):
+        return self._is_keepout
 
-    def is_crawling_allowed(self):
-        return self._crawling_allowed
-    
     def is_valid(self):
         return type(self._tag) is str
 
 
 class CachedPairs:
     def __init__(self):
         self.data = {}
@@ -98,15 +95,15 @@
 
 
 class BasePlugin(metaclass=ABCMeta):
     license_filename = "LICENSE.txt"
     _busy_count = 0
     _is_busy = False
     _regexps = {
-        re.compile(r"(?:^|.*\s)https://openlicense.ai/(t|n)/(\w+)"): True,
+        re.compile(r"(?:^|.*\s)https://openlicense.ai/(n/|t/|\b)(\w+)(?:$|\s)"): True,
         # re.compile("olai\:(\w+)"): False,
     }
     copyright_tags_cache = CachedPairs()
     platform_tag_cache = Cache()
 
     def __init__(self, ctx: WorkerContext):
         self.ctx = ctx
@@ -131,17 +128,15 @@
             BasePlugin._busy_count -= 1
             logger.info(f"busy count of plugins is {self._busy_count} (decremented)")
 
     async def download(self, url, headers={}, follow_redirects=True, max_redirects=5):
         logger.info(f"BasePlugin.download {url=}")
         try:
             async with httpx.AsyncClient(max_redirects=max_redirects) as client:
-                r = await client.get(
-                    url, follow_redirects=follow_redirects, headers=headers
-                )
+                r = await client.get(url, follow_redirects=follow_redirects, headers=headers)
                 return r.content
 
         except Exception as e:
             logger.error(f"failed get content of {url}: {e}")
 
     async def download_content(self, url, type: DatapoolContentType):
         storage_id = BaseStorage.gen_id(url)
@@ -196,17 +191,15 @@
             # print(i, head_slice, tail_slice)
 
             if head_slice == tail_slice:
                 return head + tail[i:]
         return head + tail
 
     @abstractmethod
-    async def process(
-        self, task: WorkerTask
-    ) -> AsyncGenerator[BaseCrawlerResult, None]:
+    async def process(self, task: WorkerTask) -> AsyncGenerator[BaseCrawlerResult, None]:
         pass
 
     @staticmethod
     def is_imported(module):
         return module in sys.modules
 
     @classmethod
@@ -241,31 +234,32 @@
 
     @classmethod
     def parse_tag_in_str(cls, string) -> Union[BaseTag, None]:
         logger.info(f"parse_tag_in_str {string=}")
         for regexp, deniable in BasePlugin._regexps.items():
             tag = regexp.match(string)
             if tag is not None:
+                logger.info(tag.group(1))
+                logger.info(tag.group(2))
+
                 if deniable is False:
                     return BaseTag(tag.group(1))
                 else:
-                    return BaseTag(tag.group(2), tag.group(1) == 't')
+                    return BaseTag(tag.group(2), tag.group(1) == "n/")
         return None
 
     @classmethod
-    def parse_tag_in_bs_content(
-        cls, content: BeautifulSoup, locator: str
-    ) -> Union[BaseTag, None]:
+    def parse_tag_in_bs_content(cls, content: BeautifulSoup, locator: str) -> Union[BaseTag, None]:
         for regexp, deniable in BasePlugin._regexps.items():
             tag = content.find(locator, attrs={"content": regexp})
             if tag is not None:
                 if deniable is False:
                     return BaseTag(tag.group(1))
                 else:
-                    return BaseTag(tag.group(2), tag.group(1) == 't')
+                    return BaseTag(tag.group(2), tag.group(1) == "n/")
         return None
 
     @classmethod
     async def parse_tag_in(cls, content, locator: str = "") -> Union[BaseTag, None]:
         if type(content) is str:
             return BasePlugin.parse_tag_in_str(content)
         elif BasePlugin.is_imported("bs4") and type(content) is BeautifulSoup:
@@ -305,17 +299,15 @@
 
             if type(cp) is str:
                 return cls.parse_tag_in_str(cp)
         except Exception as e:
             logger.error(f"Failed process image: {e}")
         return None
 
-    async def get_platform_tag(
-        self, domain, content, ttl=3600, meta_name=None
-    ) -> Union[BaseTag, None]:
+    async def get_platform_tag(self, domain, content, ttl=3600, meta_name=None) -> Union[BaseTag, None]:
         # logger.info( f'get_platform_tag {self.platform_tag_cache=}')
         # logger.info(f'now={time()}' )
         # logger.info(f'diff={time() - self.platform_tag_cache.time if self.platform_tag_cache.time is not None else "nan"}')
 
         if not self.platform_tag_cache.is_valid(ttl):
             dns_tag = BasePlugin.parse_dns_tag(domain)
             if dns_tag:
@@ -350,36 +342,33 @@
         return base64.b64decode(b64[len("data:image/png;base64,") :])
 
     # TODO: make this function more generic ( support bs4 too )
     # TODO: or maybe don't use bs4 at all?
     async def parse_links(self, page: Page):
         """gather all links on the page and yield them as subtasks. Only current domain urls are counted"""
         hrefs = await page.locator("a").all()
-        for href in hrefs:
-            href = await href.get_attribute("href")
+        for href_loc in hrefs:
+            href = await href_loc.get_attribute("href")
             if href is not None:
-                #logger.info( f'parse_link {href=} {type(href)=} {page.url} {type(page.url)=}')
+                # logger.info( f'parse_link {href=} {type(href)=} {page.url} {type(page.url)=}')
 
                 full_local_url = BasePlugin.get_local_url(href, page.url)
                 if full_local_url:
                     # strict constraint on urls, else may get endless recursions etc
                     full_local_url = canonicalize_url(full_local_url)
-                    #logger.info(full_local_url)
+                    # logger.info(full_local_url)
 
                     # logger.info( f'---------yielding {video_url=}')
                     yield CrawlerBackTask(url=full_local_url)
                     # logger.info( f'---------yielded {video_url=}')
                 else:
-                    #logger.info(f"non local: {href=} {page.url=}")
+                    # logger.info(f"non local: {href=} {page.url=}")
                     pass
 
     @staticmethod
     def make_text_storage_value(body, header=None, excerpt=None):
-        data = ( (header + '\n' if header else '' ) +
-                ( excerpt + '\n' if excerpt else '' ) +
-                body
-        )
+        data = (header + "\n" if header else "") + (excerpt + "\n" if excerpt else "") + body
         return data
-        
+
     @staticmethod
     def gen_demo_tag(user_name):
-        return 'demo_' + md5(user_name.encode()).hexdigest()[-6:]
+        return "demo_" + md5(user_name.encode()).hexdigest()[-6:]
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.45/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import asyncio
-import json
 import re
 
 # from bs4 import BeautifulSoup
 # from playwright.async_api import Locator, Page
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright, expect
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerNop, DatapoolContentType
 from ..base_plugin import BasePlugin, WorkerTask
 
 # import traceback
 
 
 class DataPhoenixInfoPlugin(BasePlugin):
     def __init__(self, ctx):
@@ -46,30 +40,24 @@
             #     r = await client.get( url )
             #     #logger.info( f'got Response {r}')
             #     r = r.text
             logger.info(f"loading url {task.url}")
             await self.page.goto(str(task.url))  # "https://dataphoenix.info/news/"
 
             # check if <meta/> tag exists with our tag
-            self.header_tag_id = await BasePlugin.parse_meta_tag(
-                self.page, "robots"
-            )
+            self.header_tag_id = await BasePlugin.parse_meta_tag(self.page, "robots")
             logger.info(f"{self.header_tag_id=}")
 
             if not self.header_tag_id:
                 logger.info("No <meta> tag found")
                 return
 
-            if self.header_tag_id.is_crawling_allowed() is False:
-                logger.info("crawling disabled")
-                return
-
             if re.match(
-                "^http(s?)://dataphoenix.info/(news|papers|articles|videos)(?:$|/)",
-                str(task.url),  #linter..
+                r"^http(s?)://dataphoenix.info/(news|papers|articles|videos)(?:$|/)",
+                str(task.url),  # linter..
             ):
                 logger.info("parsing feed")
                 async for yielded in self._process_feed(task.url):
                     yield yielded
             else:
                 logger.info("parsing single page")
                 async for yielded in self._process_single_page(task.url):
@@ -98,21 +86,19 @@
         ps = await self.page.locator("section.c-content > p").all()
         for p in ps:
             body += await p.inner_text() + "\n"
 
         storage_id = BaseStorage.gen_id(url)
         logger.info(f"putting article into {storage_id=}")
 
-        await self.ctx.storage.put(
-            storage_id,
-            BasePlugin.make_text_storage_value(body, header=header, excerpt=excerpt )
-        )
+        await self.ctx.storage.put(storage_id, BasePlugin.make_text_storage_value(body, header=header, excerpt=excerpt))
 
         yield CrawlerContent(
             tag_id=str(self.header_tag_id),
+            tag_keepout=self.header_tag_id.is_keepout(),
             type=DatapoolContentType.Text,
             storage_id=storage_id,
             url=url,
         )
 
     async def _process_feed(self, url):
         total_news = 0
@@ -139,17 +125,15 @@
             logger.info(f"button disabled={disabled}")
             if disabled == "disabled":
                 break
 
             ready = False
             for i in range(0, 2):
                 try:
-                    logger.info(
-                        f"waiting until button is ready for clicks ({i})"
-                    )
+                    logger.info(f"waiting until button is ready for clicks ({i})")
                     await button.click(trial=True, timeout=10000)
                     logger.info("button is ready for clicks")
                     ready = True
                     break
                 except PlaywriteTimeoutError:
                     # logger.info( e )
                     # logger.info( traceback.format_exc() )
@@ -168,17 +152,15 @@
                 # await self.page.screenshot(path="/app/tmp/screenshot.png")
                 break
 
             button = self.page.locator("button.js-load-posts.c-btn--loading")
             await button.wait_for()
             logger.info("button changed to Loading")
 
-            button = self.page.locator(
-                "button.js-load-posts:not(.c-btn--loading)"
-            )
+            button = self.page.locator("button.js-load-posts:not(.c-btn--loading)")
             await button.wait_for()
             logger.info("button changed back to More Posts")
 
             await asyncio.sleep(1)
 
         yield CrawlerNop()
 
@@ -186,17 +168,15 @@
         modal = await self.page.locator("div.hb-modal-content").all()
         if len(modal) == 0:
             logger.info("No modal found")
             return False
 
         logger.info("Modal found")
 
-        close_button = await self.page.locator(
-            'button[aria-label="close"]'
-        ).all()
+        close_button = await self.page.locator('button[aria-label="close"]').all()
         if len(close_button) == 0:
             logger.error("Unexpected: modal without close button")
             return False
 
         logger.info("clicking modal close button")
 
         await close_button[0].click(no_wait_after=True)
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/default/default.py` & `datapools-1.0.45/datapools/worker/plugins/default/default.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,60 @@
 import asyncio
 import traceback
+
 # import time
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright
 
 from ....common.logger import logger
-from ..base_plugin import BasePlugin, WorkerTask
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.types import CrawlerBackTask, CrawlerContent, DatapoolContentType
 from ....worker.utils import canonicalize_url
+from ..base_plugin import BasePlugin, WorkerTask
 
 
 class DefaultPlugin(BasePlugin):
     def __init__(self, ctx):
         super().__init__(ctx)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
-        return u.scheme in ( 'https', 'http' )
+        return u.scheme in ("https", "http")
 
     async def process(self, task: WorkerTask):
         logger.info(f"BasePlugin::process({task.url})")
 
-        if task.content_type in (
-                DatapoolContentType.Image, DatapoolContentType.Video,
-                DatapoolContentType.Audio):
+        if task.content_type in (DatapoolContentType.Image, DatapoolContentType.Video, DatapoolContentType.Audio):
             yield await self.download_content(task.url, task.content_type)
             return
 
         async with async_playwright() as playwright:
             webkit = playwright.chromium
             browser = await webkit.launch()
             viewport_height = 1024
             context = await browser.new_context(viewport={"width": 1920, "height": viewport_height})
 
             page = await context.new_page()
             await page.goto(str(task.url))
 
             real_url = page.url
             session_meta = self.ctx.session.get_meta()
-            if not self.get_local_url(real_url, session_meta['url']):
-                logger.info('redirected to different domain')
+            if not self.get_local_url(real_url, session_meta["url"]):
+                logger.info("redirected to different domain")
                 return
 
             url = real_url
 
             p = BasePlugin.parse_url(url)
             platform_tag = await self.get_platform_tag(p.netloc, page, 3600)
-            if platform_tag and platform_tag.is_crawling_allowed() is False:
-                logger.info("Crawling disabled by tag")
-                return
 
-            bodys = page.locator('body')
+            bodys = page.locator("body")
             body = bodys.nth(0)
-            body_text = ''
+            body_text = ""
             n_images = 0
             n_hrefs = 0
             expect_changes = True
             while expect_changes:
                 expect_changes = False
 
                 # 1. full body
@@ -84,33 +75,31 @@
                     # result=1234567890
                 else:
                     body_text = BasePlugin.merge_head_tail(body_text, new_text)
                 if old_text != body_text:
                     expect_changes = True
 
                 # 2. images
-                images = await page.locator('img').all()
+                images = await page.locator("img").all()
                 new_n_images = len(images)
                 if new_n_images != n_images:
                     expect_changes = True
                 while n_images < new_n_images:
                     try:
                         src = await images[n_images].get_attribute("src", timeout=100)
                         n_images += 1
 
-                        logger.info(f'{src=}')
+                        logger.info(f"{src=}")
                         if src is None:
-                            logger.info(
-                                '--------------------------------------')
+                            logger.info("--------------------------------------")
                             outerHTML = await images[n_images - 1].evaluate("el => el.outerHTML")
-                            logger.info(f'{outerHTML=}')
+                            logger.info(f"{outerHTML=}")
                             continue
 
-                        full_local_url = BasePlugin.get_local_url(
-                            src, session_meta['url'])
+                        full_local_url = BasePlugin.get_local_url(src, session_meta["url"])
                         if full_local_url:
                             logger.info(full_local_url)
                             if await self.is_content_processed(full_local_url):
                                 continue
 
                             storage_id = BaseStorage.gen_id(full_local_url)
 
@@ -118,84 +107,79 @@
                             #   requires image type detection, quality check, crossOrigin understading etc
                             #   So for now let's do not in optimal way
                             content = await self.download(full_local_url)
                             # getting content from browser page instead of downloading it again
                             # content = await BasePlugin.get_webpage_image_bytes(images[n_images-1])
                             if content:
                                 image_tag = BasePlugin.parse_image_tag(content)
-                                if image_tag is not None and image_tag.is_crawling_allowed() is False:
-                                    logger.info(
-                                        f'crawling is disabled by {str(image_tag)}')
-                                    continue
 
                                 # TODO: parse copyright_tag_id somehow?
                                 if image_tag is None and platform_tag is None:
-                                    logger.info('no tag available')
+                                    logger.info("no tag available")
                                     continue
 
                                 try:
-                                    logger.info(f'putting to {storage_id=}')
+                                    logger.info(f"putting to {storage_id=}")
                                     await self.ctx.storage.put(storage_id, content)
 
                                     yield CrawlerContent(
                                         tag_id=str(image_tag) if image_tag is not None else None,
-                                        copyright_tag_id=None,
+                                        tag_keepout=image_tag.is_keepout() if image_tag is not None else False,
                                         platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                                        platform_tag_keepout=(
+                                            platform_tag.is_keepout() if platform_tag is not None else None
+                                        ),
                                         type=DatapoolContentType.Image,
                                         storage_id=storage_id,
                                         url=full_local_url,
                                     )
                                 except Exception as e:
                                     logger.error(f"failed put to storage {e}")
                                     logger.error(traceback.format_exc())
                         else:
-                            logger.info(
-                                f'non local: {src=} {session_meta["url"]=}')
+                            logger.info(f'non local: {src=} {session_meta["url"]=}')
 
                     except PlaywriteTimeoutError as e:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
 
                 # 3. hrefs
-                hrefs = await page.locator('a').all()
+                hrefs = await page.locator("a").all()
                 new_n_hrefs = len(hrefs)
                 if new_n_hrefs != n_hrefs:
                     expect_changes = True
                 while n_hrefs < new_n_hrefs:
                     try:
                         href = await hrefs[n_hrefs].get_attribute("href", timeout=100)
                         n_hrefs += 1
 
-                        full_local_url = BasePlugin.get_local_url(
-                            href, session_meta['url'])
+                        full_local_url = BasePlugin.get_local_url(href, session_meta["url"])
                         if full_local_url:
                             # strict constraint on urls, else may get endless recursions etc
                             full_local_url = canonicalize_url(full_local_url)
                             logger.info(full_local_url)
 
                             # logger.info( f'---------yielding {video_url=}')
                             yield CrawlerBackTask(url=full_local_url)
                             # logger.info( f'---------yielded {video_url=}')
                         else:
-                            logger.info(
-                                f'non local: {href=} {session_meta["url"]=}')
+                            logger.info(f'non local: {href=} {session_meta["url"]=}')
 
                     except PlaywriteTimeoutError as e:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
 
-                scroll_height1 = await page.evaluate('document.body.scrollHeight')
+                scroll_height1 = await page.evaluate("document.body.scrollHeight")
                 await page.mouse.wheel(0, viewport_height * 0.8)
-                scroll_height2 = await page.evaluate('document.body.scrollHeight')
-                logger.info(
-                    f'*********** {scroll_height1=} {scroll_height2=} ****************')
+                scroll_height2 = await page.evaluate("document.body.scrollHeight")
+                logger.info(f"*********** {scroll_height1=} {scroll_height2=} ****************")
                 if scroll_height1 != scroll_height2:
                     expect_changes = True
 
                 await asyncio.sleep(1)
                 # await page.screenshot(path=f'/home/psu/page.png')
 
             # await page.screenshot(path='/home/psu/bottom.png')
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.45/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,112 @@
 import re
-import json
+from urllib.parse import urlparse, urlunparse
+
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
-from urllib.parse import urljoin, urlparse, urlunparse
 
-from ....worker.utils import canonicalize_url
-from ..base_plugin import BasePlugin, BaseTag, WorkerTask
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.types import CrawlerBackTask, CrawlerContent, DatapoolContentType
+from ....worker.utils import canonicalize_url
+from ..base_plugin import BasePlugin, BaseTag, WorkerTask
 
-DOMAIN = "www.dw.com"
+DOMAIN = "www.theguardian.com"
 
-class DeutscheWellePlugin(BasePlugin):
 
-    base_url = f"https://{DOMAIN}/en/"
+class TheGuardianPlugin(BasePlugin):
+
+    base_url = f"https://{DOMAIN}/"
 
     def __init__(self, ctx, demo_tag=None):
         super().__init__(ctx)
-        logger.info(f"{demo_tag=} ***************************************************")
-        self.demo_tag = BaseTag( demo_tag )
+        self.demo_tag = BaseTag(demo_tag)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
-        #logger.info( f'dw.is_supported {url=} {u.netloc=} {DOMAIN=}')
-        return u.netloc == DOMAIN
+        # logger.info( f'dataphoenix.info {u=}')
+        return u.netloc[-16:] == ".theguardian.com"
 
     def is_article(self, url):
         path = urlparse(url).path
-        pattern = "^/en/.+/a-\d+/$"
-        return True  # bool(re.match(pattern, path))
+        pattern = r"^/[\w/-]+/\d+/\w+/\d+/[\w/-]+$"
+        return bool(re.match(pattern, path))
 
     def normalize(self, url):
         parts = list(urlparse(url))
-        parts[5] = ""   # remove fragment
+        parts[5] = ""  # remove fragment
         clean_url = urlunparse(parts)
         return clean_url
-          
+
     def extract(self, soup):
         content = soup.find("article")
         if not content:
-            logger.debug(f"No <article>. Skipped.")
+            logger.debug("No <article>. Skipped.")
             return None
 
-        # remove ads
-        for element in content.find_all("div"):
-            for v in element.attrs.values():
-                if "advertisement" in v:
-                    element.extract()
-                    break
-            if element.attrs.get("data-tracking-name", "") == "content-detail-kicker":
-                element.extract()
-
         filter_list = [
-            dict(string = lambda s: isinstance(s, Comment)),
-            dict(name = "img"), 
-            dict(name = "svg"), 
-            dict(name = "button"), 
-            dict(name = "video"), 
-            dict(name = "picture"), 
-            dict(name = "source"), 
-            dict(name = "small"), 
-            dict(name = "footer"),
+            dict(string=lambda s: isinstance(s, Comment)),
+            dict(name="img"),
+            dict(name="svg"),
+            dict(name="button"),
+            dict(name="video"),
+            dict(name="picture"),
+            dict(name="source"),
+            dict(name="small"),
+            dict(name="footer"),
+            dict(name="gu-island"),
         ]
         for tag_params in filter_list:
             for element in content.find_all(**tag_params):
                 element.extract()
 
         unwrap_tags = ["figure", "figcaption", "form", "span", "a"]
         for tag in unwrap_tags:
             for element in content.find_all(tag):
                 element.unwrap()
-            
+
         for element in content.descendants:
             if element.name:
                 element.attrs = {}
 
-        text_maker = HTML2Text(bodywidth = 80)
+        text_maker = HTML2Text(bodywidth=80)
         text_maker.ignore_links = True
         markdown = text_maker.handle(str(content))
         markdown = re.sub("\n[ \t]+", "\n", markdown)
         markdown = re.sub("\n{2,}", "\n\n", markdown)
-        
+
+        i = markdown.find("Explore more on these topics")
+        if i > 0:
+            markdown = markdown[:i].strip()
+
         snippet = re.sub("\n+", " ", markdown)[:160].strip()
         logger.info(f"Extracted content: {snippet}...")
         return markdown
-    
-    async def process(self, task):
-        url = task.url
+
+    async def process(self, task: WorkerTask):
+        url = str(task.url)
         logger.info(f"{url} - Processing...")
-        
+
         response = requests.get(url)
         if response.url != url:
             logger.info(f"{url} - Redirect to {response.url}")
             url = response.url
-                    
-        soup = BeautifulSoup(response.content, 'html.parser')
-        
+
+        soup = BeautifulSoup(response.content, "html.parser")
+
         if not self.demo_tag.is_valid():
             platform_tag = await self.get_platform_tag(DOMAIN, soup, 3600)
         else:
             platform_tag = self.demo_tag
 
-        if platform_tag and platform_tag.is_crawling_allowed() is False:
-            logger.info("Crawling disabled by tag")
-            return                
-
         logger.debug(f"Adding new links...")
-        for link in soup.find_all('a', href = True):
-            href = link['href']
-            #next_url = urljoin(url, href)
-            #next_url = self.normalize(next_url)
-            
+        for link in soup.find_all("a", href=True):
+            href = link["href"]
             full_local_url = BasePlugin.get_local_url(href, url)
             if full_local_url:
                 full_local_url = canonicalize_url(full_local_url)
                 logger.info(full_local_url)
                 yield CrawlerBackTask(url=full_local_url)
 
         if self.is_article(url):
@@ -130,17 +114,15 @@
             if content:
                 storage_id = BaseStorage.gen_id(url)
                 logger.info(f"putting article into {storage_id=}")
 
                 await self.ctx.storage.put(
                     storage_id,
                     BasePlugin.make_text_storage_value(content),
-                )            
+                )
                 yield CrawlerContent(
-                    tag_id=str(platform_tag) if platform_tag is not None else None,
+                    platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                    platform_tag_keepout=platform_tag.is_keepout() if platform_tag is not None else False,
                     type=DatapoolContentType.Text,
                     storage_id=storage_id,
                     url=url,
                 )
-            else:
-                logger.info( 'NO CONTENT')
-
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.45/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 from google.auth.api_key import Credentials
 
 # from google.auth.transport.requests import Request
 # from google.oauth2.credentials import Credentials
 # from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
-# from googleapiclient.http import MediaIoBaseDownload
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import CrawlerContent, DatapoolContentType
 from ..base_plugin import BasePlugin, BasePluginException, WorkerTask
 
+# from googleapiclient.http import MediaIoBaseDownload
+
+
 # from googleapiclient.errors import HttpError
 
 
 # If modifying these scopes, delete the file token.json.
 # SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly']
 
 
@@ -42,15 +44,15 @@
     async def process(self, task: WorkerTask):
         u = self.parse_url(task.url)
         folder_id = u.path.split("/")[3]
 
         try:
             with build("drive", "v3", credentials=self.creds) as drive:
                 self.tag_id = await self.find_license(folder_id, drive)
-                if self.tag_id and self.tag_id.is_crawling_allowed():
+                if self.tag_id:
                     async for msg in self.scan_folder(folder_id, drive):
                         yield msg
         except Exception as e:
             logger.error(f"GoogleDrivePlugin exception {e}")
             logger.error(traceback.format_exc())
 
     def _get_download_url(self, file_id):
@@ -58,17 +60,22 @@
         return f"https://drive.google.com/uc?id={file_id}"
 
         # return f"https://www.googleapis.com/drive/v3/files/{file_id}?alt=media&key={self.creds.token}"
 
     async def find_license(self, folder_id, drive):
         try:
             license = (
-                drive.files().list(
+                drive.files()
+                .list(
                     q=f"name='{BasePlugin.license_filename}' and '{folder_id}' in parents",
-                    pageSize=1, fields="files(id)",).execute())
+                    pageSize=1,
+                    fields="files(id)",
+                )
+                .execute()
+            )
             file_id = license.get("files")[0]["id"]
 
             url = self._get_download_url(file_id)
             # headers = { "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
             #             "Accept-Encoding":"gzip, deflate, br",
             #             "Accept-Language":"en-US,en;q=0.5",
             #             "Connection":"keep-alive",
@@ -139,23 +146,17 @@
                 logger.info(f"{file['mimeType']=}")
 
                 if file["mimeType"] == "application/vnd.google-apps.folder":
                     async for yielded in self.scan_folder(file_id, drive):
                         yield yielded
                 else:
                     try:
-                        datapool_content_type = (
-                            BasePlugin.get_content_type_by_mime_type(
-                                file["mimeType"]
-                            )
-                        )
+                        datapool_content_type = BasePlugin.get_content_type_by_mime_type(file["mimeType"])
                     except BasePluginException:
-                        logger.error(
-                            f'Not supported mime type {file["mimeType"]}'
-                        )
+                        logger.error(f'Not supported mime type {file["mimeType"]}')
 
                     logger.info(f'downloading file {file_id} {file["name"]}')
                     # TODO: this works too, but is getting blocked  when running from lsrv2
                     # fileRequest = drive.files().get_media(fileId=file_id)
                     # fh = io.BytesIO()
                     # downloader = MediaIoBaseDownload(fh, fileRequest)
                     # done = False
@@ -168,27 +169,25 @@
                     content = await self.download(url)
                     if content is not None:
                         logger.info(f"file size={len(content)}")
 
                         image_tag = None
                         if datapool_content_type == DatapoolContentType.Image:
                             image_tag = BasePlugin.parse_image_tag(content)
-                            if image_tag is not None and image_tag.is_crawling_allowed() is False:
-                                logger.info(
-                                    f'crawling is disabled by image tag: {str(image_tag)}')
-                                continue
 
                         # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
                         obj_url = url
                         storage_id = BaseStorage.gen_id(obj_url)
                         await self.ctx.storage.put(storage_id, content)
 
                         yield CrawlerContent(
                             tag_id=str(image_tag) if image_tag is not None else None,
+                            tag_keepout=image_tag.is_keepout() if image_tag is not None else None,
                             copyright_tag_id=str(self.tag_id),
+                            copyright_tag_keepout=self.tag_id.is_keepout(),
                             type=datapool_content_type,
                             storage_id=storage_id,
                             url=obj_url,
                         )
 
                 # baseImage = cv2.imdecode(np.fromstring(fhContents, dtype=np.uint8), cv2.IMREAD_COLOR)
             if page_token is None:
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.45/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,241 +1,226 @@
 import asyncio
-import json
 import traceback
-from typing import Union, Dict
-
-from playwright.async_api import TimeoutError as PlaywriteTimeoutError
-from playwright.async_api import async_playwright
+from typing import Union
 
 # import httpx
 from bs4 import BeautifulSoup
+from playwright.async_api import TimeoutError as PlaywriteTimeoutError
+from playwright.async_api import async_playwright
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerDemoUser,
-    DatapoolContentType,
-)
-from ..base_plugin import BasePlugin, BaseTag, WorkerTask
+from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerDemoUser, DatapoolContentType
 from ....worker.utils import canonicalize_url
+from ..base_plugin import BasePlugin, BaseTag, WorkerTask
 
 # from typing import List
 
 DOMAIN = "imageshack.com"
 
 
 class ImageshackPlugin(BasePlugin):
     def __init__(self, ctx, demo_tag=None):
         super().__init__(ctx)
-        self.demo_tag = BaseTag( demo_tag )
+        self.demo_tag = BaseTag(demo_tag)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
         # logger.info( f'imageshack {u=}')
         return u.netloc == DOMAIN
 
     async def process(self, task: WorkerTask):
         logger.info(f"imageshack::process({task.url})")
 
         if task.content_type == DatapoolContentType.Image:
-            logger.info('Got content_type => direct download')
+            logger.info("Got content_type => direct download")
             yield await self.download_content(task.url, task.content_type)
             return
 
         logger.info(f"loading url {task.url}")
         r = await self.download(task.url)
         if r is None:
             return
         # logger.info( f'text: {r}')
         logger.info(f"got url content length={len(r)}")
-        
-        
+
         async with async_playwright() as playwright:
             webkit = playwright.chromium
             browser = await webkit.launch()
             viewport_height = 1024
             context = await browser.new_context(viewport={"width": 1920, "height": viewport_height})
 
             page = await context.new_page()
             await page.goto(str(task.url))
-            
+
             if not self.demo_tag.is_valid():
                 platform_tag = await self.get_platform_tag(DOMAIN, page, 3600)
             else:
                 platform_tag = self.demo_tag
-            if platform_tag and platform_tag.is_crawling_allowed() is False:
-                logger.info("Crawling disabled by tag")
-                return
-            
+
             session_meta = self.ctx.session.get_meta()
-            
+
             n_images = 0
             n_hrefs = 0
             expect_changes = True
             while expect_changes:
                 expect_changes = False
-                
+
                 # 1.search for photo LINKS and return them as new tasks
                 hrefs = await page.locator("a.photo, a.hero-wrapper").all()
                 new_n_hrefs = len(hrefs)
                 if new_n_hrefs != n_hrefs:
                     expect_changes = True
-                    
+
                 while n_hrefs < new_n_hrefs:
                     try:
                         href = await hrefs[n_hrefs].get_attribute("href", timeout=100)
                         n_hrefs += 1
 
-                        full_local_url = BasePlugin.get_local_url( href, session_meta['url'])
+                        full_local_url = BasePlugin.get_local_url(href, session_meta["url"])
                         if full_local_url:
                             # strict constraint on urls, else may get endless recursions etc
                             full_local_url = canonicalize_url(full_local_url)
-                            logger.info(f'adding task: {full_local_url}')
+                            logger.info(f"adding task: {full_local_url}")
 
                             # logger.info( f'---------yielding {video_url=}')
                             yield CrawlerBackTask(url=full_local_url)
                             # logger.info( f'---------yielded {video_url=}')
                         else:
-                            logger.info(
-                                f'non local: {href=} {session_meta["url"]=}')
+                            logger.info(f'non local: {href=} {session_meta["url"]=}')
 
                     except PlaywriteTimeoutError as e:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
-                    
+
                 # 2. search for single photo IMAGE
                 images = await page.locator("img#lp-image").all()
                 new_n_images = len(images)
                 if new_n_images > n_images:
                     expect_changes = True
-                
+
                 while n_images < new_n_images:
                     try:
                         src = await images[n_images].get_attribute("src", timeout=100)
                         n_images += 1
 
-                        logger.info(f'{src=}')
+                        logger.info(f"{src=}")
                         if src is None:
-                            logger.info(
-                                '--------------------------------------')
+                            logger.info("--------------------------------------")
                             outerHTML = await images[n_images - 1].evaluate("el => el.outerHTML")
-                            logger.info(f'{outerHTML=}')
+                            logger.info(f"{outerHTML=}")
                             continue
 
-                        full_local_url = BasePlugin.get_local_url(src, session_meta['url'])
+                        full_local_url = BasePlugin.get_local_url(src, session_meta["url"])
                         logger.info(full_local_url)
                         if await self.is_content_processed(full_local_url):
                             continue
 
                         storage_id = BaseStorage.gen_id(full_local_url)
-                        
+
                         copyright_owner_tag = None
 
                         # check for user license on his public profile page
                         profile_link = await page.locator("a.profile-link").all()
                         if len(profile_link):
                             # profile_link['href'] = '/user/sergpsu' test
-                            href = await profile_link[0].get_attribute( 'href' )
+                            href = await profile_link[0].get_attribute("href")
                             if href is not None:
                                 # strict constraint on urls, else may get endless recursions etc
-                                full_profile_url = canonicalize_url(BasePlugin.get_local_url( href, session_meta['url']))
-                                logger.info(f'adding task: {full_profile_url}')
+                                full_profile_url = canonicalize_url(BasePlugin.get_local_url(href, session_meta["url"]))
+                                logger.info(f"adding task: {full_profile_url}")
 
                                 yield CrawlerBackTask(url=full_profile_url)
-                                
+
                                 if not self.demo_tag.is_valid():
                                     copyright_owner_tag = await self.parse_user_profile(href)
                                 else:
                                     # demo functionality for royalties spreadout demo
-                                    user_name = href.split('/')[-1]
+                                    user_name = href.split("/")[-1]
                                     short_tag_id = BasePlugin.gen_demo_tag(user_name)
                                     copyright_owner_tag = BaseTag(short_tag_id)
-                                    yield CrawlerDemoUser( user_name=user_name, short_tag_id=short_tag_id, platform='imageshack.com' )
+                                    yield CrawlerDemoUser(
+                                        user_name=user_name, short_tag_id=short_tag_id, platform="imageshack.com"
+                                    )
 
                         if copyright_owner_tag is not None:
-                            logger.info(f'found {copyright_owner_tag=}')
-                            if copyright_owner_tag.is_crawling_allowed() is False:
-                                logger.info('User disabled crawling')
-                                continue
-
+                            logger.info(f"found {copyright_owner_tag=}")
 
                         # TODO: getting image from browser works somehow but
                         #   requires image type detection, quality check, crossOrigin understading etc
                         #   So for now let's do not in optimal way
                         content = await self.download(full_local_url)
                         # getting content from browser page instead of downloading it again
                         # content = await BasePlugin.get_webpage_image_bytes(images[n_images-1])
                         if content:
                             image_tag = BasePlugin.parse_image_tag(content)
-                            if image_tag is not None and image_tag.is_crawling_allowed() is False:
-                                logger.info(
-                                    f'crawling is disabled by {str(image_tag)}')
-                                continue
+                            if image_tag is not None:
+                                logger.info(f"found image tag {image_tag=}")
 
-                            # TODO: parse copyright_tag_id somehow?
-                            if image_tag is None and platform_tag is None:
-                                logger.info('no tag available')
+                            if image_tag is None and platform_tag is None and copyright_owner_tag is None:
+                                logger.info("no tag available")
                                 continue
 
                             try:
-                                logger.info(f'putting to {storage_id=}')
+                                logger.info(f"putting to {storage_id=}")
                                 await self.ctx.storage.put(storage_id, content)
 
                                 yield CrawlerContent(
                                     tag_id=str(image_tag) if image_tag is not None else None,
-                                    copyright_tag_id=str(copyright_owner_tag) if copyright_owner_tag is not None else None,
+                                    tag_keepout=image_tag.is_keepout() if image_tag is not None else False,
+                                    copyright_tag_id=(
+                                        str(copyright_owner_tag) if copyright_owner_tag is not None else None
+                                    ),
+                                    copyright_tag_keepout=(
+                                        copyright_owner_tag.is_keepout() if copyright_owner_tag is not None else False
+                                    ),
                                     platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                                    platform_tag_keepout=(
+                                        platform_tag.is_keepout() if platform_tag is not None else False
+                                    ),
                                     type=DatapoolContentType.Image,
                                     storage_id=storage_id,
                                     url=full_local_url,
                                 )
-                                
+
                             except Exception as e:
                                 logger.error(f"failed put to storage {e}")
                                 logger.error(traceback.format_exc())
                         else:
                             logger.error("failed download image")
-    
 
-                    except PlaywriteTimeoutError as e:
+                    except PlaywriteTimeoutError:
                         # element may be not ready yet, no problems, will get it on the next iteration
                         # logger.info( 'get_attribute timeout' )
                         expect_changes = True
                         break
 
-
-                scroll_height1 = await page.evaluate('document.body.scrollHeight')
+                scroll_height1 = await page.evaluate("document.body.scrollHeight")
                 await page.mouse.wheel(0, viewport_height * 0.8)
-                scroll_height2 = await page.evaluate('document.body.scrollHeight')
-                logger.info(
-                    f'*********** {scroll_height1=} {scroll_height2=} ****************')
+                scroll_height2 = await page.evaluate("document.body.scrollHeight")
+                logger.info(f"*********** {scroll_height1=} {scroll_height2=} ****************")
                 if scroll_height1 != scroll_height2:
                     expect_changes = True
 
                 await asyncio.sleep(1)
 
-            
-
     async def parse_user_profile(self, href) -> Union[BaseTag, None]:
-        username = href.split('/')[-1]
+        username = href.split("/")[-1]
         if not BasePlugin.copyright_tags_cache.contains(username, 3600):
-            url = f'https://{DOMAIN}/{href}'
+            url = f"https://{DOMAIN}/{href}"
 
             logger.info(f"parsing user profile {url=}")
 
             r = await self.download(url)
             # logger.info( f'text: {r}')
             logger.info(f"got url content length={len(r)}")
 
             soup = BeautifulSoup(r, "html.parser")
-            about = soup.body.find('div', attrs={"class": "bio tall"})
+            about = soup.body.find("div", attrs={"class": "bio tall"})
             if about:
-                BasePlugin.copyright_tags_cache.set(
-                    username, BasePlugin.parse_tag_in_str(about.contents[0]))
+                BasePlugin.copyright_tags_cache.set(username, BasePlugin.parse_tag_in_str(about.contents[0]))
             else:
                 BasePlugin.copyright_tags_cache.set(username, None)
         return BasePlugin.copyright_tags_cache.get(username)
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.45/datapools/worker/plugins/s3/s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,31 +17,25 @@
 
 
 class S3Exception(BasePluginException):
     pass
 
 
 class S3Plugin(BasePlugin):
-    def __init__(
-        self, ctx, aws_access_key_id=None, aws_secret_access_key=None
-    ):
+    def __init__(self, ctx, aws_access_key_id=None, aws_secret_access_key=None):
         super().__init__(ctx)
 
         logger.info(f"{aws_access_key_id=}")
         logger.info(f"{aws_secret_access_key=}")
 
         # empty key means bucket is public
         if aws_access_key_id == "":
             self.is_public_bucket = True
-            self.s3_client = boto3.client(
-                "s3", config=Config(signature_version=UNSIGNED)
-            )
-            self.s3 = boto3.resource(
-                "s3", config=Config(signature_version=UNSIGNED)
-            )
+            self.s3_client = boto3.client("s3", config=Config(signature_version=UNSIGNED))
+            self.s3 = boto3.resource("s3", config=Config(signature_version=UNSIGNED))
         else:
             self.is_public_bucket = False
             self.s3_client = boto3.client(
                 "s3",
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
             )
@@ -75,27 +69,20 @@
 
         bucket = self.s3.Bucket(self.bucket_name)
 
         try:
             copyright_tag_id = self._download(BasePlugin.license_filename)
             copyright_tag = await BasePlugin.parse_tag_in(copyright_tag_id.decode())
             logger.info(f"found license: {copyright_tag_id}")
-            if copyright_tag is not None and copyright_tag.is_crawling_allowed() is False:
-                logger.info('crawling disabled by copyright owner')
-                return
         except S3Exception:
-            logger.error(
-                "bucket does not contain license.txt, cannot process(1)"
-            )
+            logger.error("bucket does not contain license.txt, cannot process(1)")
             logger.error(traceback.format_exc())
             return
         except ClientError:
-            logger.error(
-                "bucket does not contain license.txt, cannot process(2)"
-            )
+            logger.error("bucket does not contain license.txt, cannot process(2)")
             logger.error(traceback.format_exc())
             return
 
         for obj in bucket.objects.all():
             logger.info(f"{obj=}")
 
             if obj.key == BasePlugin.license_filename:
@@ -103,44 +90,38 @@
 
             if self.is_public_bucket is False:
                 # THIS IS PURE API ACCESS URL
                 obj_url = f"https://s3.console.aws.amazon.com/s3/buckets/{self.bucket_name}/{obj.key}"
             else:
                 # THIS IS DIRECT URL ( FOR PUBLIC BUCKETS )
                 # TODO: region?
-                obj_url = (
-                    f"https://{self.bucket_name}.s3.amazonaws.com/{obj.key}"
-                )
+                obj_url = f"https://{self.bucket_name}.s3.amazonaws.com/{obj.key}"
 
             storage_id = BaseStorage.gen_id(obj_url)
 
             content = self._download(obj.key)
 
             try:
-                type = self._get_datapool_content_type(content)
+                content_type = self._get_datapool_content_type(content)
+
+                tag = None
+                if content_type == DatapoolContentType.Image:
+                    tag = BasePlugin.parse_image_tag(content)
 
-                if type == DatapoolContentType.Image:
-                    image_tag = BasePlugin.parse_image_tag(content)
-                    if image_tag is not None:
-                        if image_tag.is_crawling_allowed() is False:
-                            logger.info(
-                                f'crawling is disabled by image tag: {str(image_tag)}')
-                            continue
-                    else:
-                        if copyright_tag is None:
-                            logger.info(
-                                'no image tag, nor copyright tag, skipped')
-                            continue
+                if tag is None and copyright_tag is None:
+                    continue
 
                 await self.ctx.storage.put(storage_id, content)
 
                 yield CrawlerContent(
-                    tag_id=str(image_tag) if image_tag is not None else None,
+                    tag_id=str(tag) if tag is not None else None,
+                    tag_keepout=tag.is_keepout() if tag is not None else False,
                     copyright_tag_id=str(copyright_tag) if copyright_tag is not None else None,
-                    type=type,
+                    copyright_tag_keepout=copyright_tag.is_keepout() if copyright_tag is not None else False,
+                    type=content_type,
                     storage_id=storage_id,
                     url=obj_url,
                 )
             except S3Exception as e:
                 logger.info(f"mime type not supported/detected: {e}")
 
     def _download(self, key):
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.45/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,120 @@
 import re
-import json
+from urllib.parse import urlparse, urlunparse
+
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
-from urllib.parse import urljoin, urlparse, urlunparse
 
-from ....worker.utils import canonicalize_url
-from ..base_plugin import BasePlugin, BaseTag, WorkerTask
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.types import CrawlerBackTask, CrawlerContent, DatapoolContentType
+from ....worker.utils import canonicalize_url
+from ..base_plugin import BasePlugin, BaseTag
+
+DOMAIN = "www.dw.com"
 
-DOMAIN = "www.theguardian.com"
 
-class TheGuardianPlugin(BasePlugin):
+class DeutscheWellePlugin(BasePlugin):
 
-    base_url = f"https://{DOMAIN}/"
+    base_url = f"https://{DOMAIN}/en/"
 
     def __init__(self, ctx, demo_tag=None):
         super().__init__(ctx)
+        logger.info(f"{demo_tag=} ***************************************************")
         self.demo_tag = BaseTag(demo_tag)
-        
+
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
-        # logger.info( f'dataphoenix.info {u=}')
-        return u.netloc[-16:] == '.theguardian.com'
-         
+        # logger.info( f'dw.is_supported {url=} {u.netloc=} {DOMAIN=}')
+        return u.netloc == DOMAIN
 
     def is_article(self, url):
         path = urlparse(url).path
-        pattern = "^/[\w/-]+/\d+/\w+/\d+/[\w/-]+$"
-        return bool(re.match(pattern, path))
+        pattern = "^/en/.+/a-\d+/$"
+        return True  # bool(re.match(pattern, path))
 
     def normalize(self, url):
         parts = list(urlparse(url))
-        parts[5] = ""   # remove fragment
+        parts[5] = ""  # remove fragment
         clean_url = urlunparse(parts)
         return clean_url
-          
+
     def extract(self, soup):
         content = soup.find("article")
         if not content:
             logger.debug(f"No <article>. Skipped.")
             return None
 
+        # remove ads
+        for element in content.find_all("div"):
+            for v in element.attrs.values():
+                if "advertisement" in v:
+                    element.extract()
+                    break
+            if element.attrs.get("data-tracking-name", "") == "content-detail-kicker":
+                element.extract()
+
         filter_list = [
-            dict(string = lambda s: isinstance(s, Comment)),
-            dict(name = "img"), 
-            dict(name = "svg"),
-            dict(name = "button"),
-            dict(name = "video"),
-            dict(name = "picture"),
-            dict(name = "source"),
-            dict(name = "small"),
-            dict(name = "footer"),
-            dict(name = "gu-island")
+            dict(string=lambda s: isinstance(s, Comment)),
+            dict(name="img"),
+            dict(name="svg"),
+            dict(name="button"),
+            dict(name="video"),
+            dict(name="picture"),
+            dict(name="source"),
+            dict(name="small"),
+            dict(name="footer"),
         ]
         for tag_params in filter_list:
             for element in content.find_all(**tag_params):
                 element.extract()
 
         unwrap_tags = ["figure", "figcaption", "form", "span", "a"]
         for tag in unwrap_tags:
             for element in content.find_all(tag):
                 element.unwrap()
-            
+
         for element in content.descendants:
             if element.name:
                 element.attrs = {}
 
-        text_maker = HTML2Text(bodywidth = 80)
+        text_maker = HTML2Text(bodywidth=80)
         text_maker.ignore_links = True
         markdown = text_maker.handle(str(content))
         markdown = re.sub("\n[ \t]+", "\n", markdown)
         markdown = re.sub("\n{2,}", "\n\n", markdown)
 
-        i = markdown.find("Explore more on these topics")
-        if i > 0:
-            markdown = markdown[:i].strip()
-        
         snippet = re.sub("\n+", " ", markdown)[:160].strip()
         logger.info(f"Extracted content: {snippet}...")
         return markdown
-    
-    async def process(self, task:WorkerTask):
+
+    async def process(self, task):
         url = task.url
         logger.info(f"{url} - Processing...")
-        
+
         response = requests.get(url)
         if response.url != url:
             logger.info(f"{url} - Redirect to {response.url}")
             url = response.url
 
-        soup = BeautifulSoup(response.content, 'html.parser')
-        
+        soup = BeautifulSoup(response.content, "html.parser")
+
         if not self.demo_tag.is_valid():
             platform_tag = await self.get_platform_tag(DOMAIN, soup, 3600)
         else:
             platform_tag = self.demo_tag
 
-        if platform_tag and platform_tag.is_crawling_allowed() is False:
-            logger.info("Crawling disabled by tag")
-            return        
-
         logger.debug(f"Adding new links...")
-        for link in soup.find_all('a', href = True):
-            href = link['href']
+        for link in soup.find_all("a", href=True):
+            href = link["href"]
+            # next_url = urljoin(url, href)
+            # next_url = self.normalize(next_url)
+
             full_local_url = BasePlugin.get_local_url(href, url)
             if full_local_url:
                 full_local_url = canonicalize_url(full_local_url)
                 logger.info(full_local_url)
                 yield CrawlerBackTask(url=full_local_url)
 
         if self.is_article(url):
@@ -123,16 +122,17 @@
             if content:
                 storage_id = BaseStorage.gen_id(url)
                 logger.info(f"putting article into {storage_id=}")
 
                 await self.ctx.storage.put(
                     storage_id,
                     BasePlugin.make_text_storage_value(content),
-                )            
+                )
                 yield CrawlerContent(
-                    tag_id=str(platform_tag) if platform_tag is not None else None,
+                    platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                    platform_keepout=platform_tag.is_keepout() if platform_tag is not None else None,
                     type=DatapoolContentType.Text,
                     storage_id=storage_id,
                     url=url,
                 )
-                
-
+            else:
+                logger.info("NO CONTENT")
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.45/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,175 +1,166 @@
 import re
-import json
+from urllib.parse import urlparse, urlunparse
+
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
-from urllib.parse import urljoin, urlparse, urlunparse
 
-from ....worker.utils import canonicalize_url
-from ..base_plugin import BasePlugin, BaseTag, WorkerTask, CachedPairs
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerDemoUser,
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerDemoUser, CrawlerNop, DatapoolContentType
+from ....worker.utils import canonicalize_url
+from ..base_plugin import BasePlugin, BaseTag, CachedPairs, WorkerTask
 
 DOMAIN = "www.washingtonpost.com"
 
 
 class WashingtonPostPlugin(BasePlugin):
 
     base_url = f"https://{DOMAIN}/"
     authors = CachedPairs()
 
     def __init__(self, ctx, demo_tag=None):
         super().__init__(ctx)
-        self.demo_tag = BaseTag( demo_tag )
-        
+        self.demo_tag = BaseTag(demo_tag)
+
     @staticmethod
-    def is_supported( url):
+    def is_supported(url):
         u = BasePlugin.parse_url(url)
         if u.netloc != DOMAIN:
             logger.debug(f"Validation failed - Out of domain: {url}")
             return False
-        if re.match("^/subscribe/.*$", u.path):   # these pages timeout
+        if re.match("^/subscribe/.*$", u.path):  # these pages timeout
             logger.debug(f"Validation failed - Subscription page: {url}")
             return False
-        if re.match("^/people/.*$", u.path):   # there are just too many of them
+        if re.match("^/people/.*$", u.path):  # there are just too many of them
             logger.debug(f"Validation failed - People page: {url}")
             return False
         return True
 
     def is_article(self, url):
         path = urlparse(url).path
-        pattern = "^[\w\-/]{3,}/\d+/\d+/\d+/[\w-]+/$"
+        pattern = r"^[\w\-/]{3,}/\d+/\d+/\d+/[\w-]+/$"
         return bool(re.match(pattern, path))
 
     def normalize(self, url):
         parts = list(urlparse(url))
-        parts[5] = ""   # remove fragment
+        parts[5] = ""  # remove fragment
         clean_url = urlunparse(parts)
         return clean_url
-          
+
     def extract(self, soup):
         content = soup.find("article")
         if not content:
-            logger.debug(f"No <article>, trying <main>...")
-            content = soup.find("main", attrs = {"data-qa": "article-body", "id": "article-body"})
+            logger.debug("No <article>, trying <main>...")
+            content = soup.find("main", attrs={"data-qa": "article-body", "id": "article-body"})
         if not content:
-            logger.debug(f"No <main> either. Skipped.")
+            logger.debug("No <main> either. Skipped.")
             return None
 
         filter_list = [
-            dict(string = lambda s: isinstance(s, Comment)),
-            dict(name = "img"),
-            dict(name = "svg"),
-            dict(name = "button"),
-            dict(name = "div", string = "Advertisement"),
-            dict(name = "div", attrs = {"aria-roledescription": "carousel"}),
-            dict(name = "div", string = "End of carousel"),
+            dict(string=lambda s: isinstance(s, Comment)),
+            dict(name="img"),
+            dict(name="svg"),
+            dict(name="button"),
+            dict(name="div", string="Advertisement"),
+            dict(name="div", attrs={"aria-roledescription": "carousel"}),
+            dict(name="div", string="End of carousel"),
         ]
         for tag_params in filter_list:
             for element in content.find_all(**tag_params):
                 element.extract()
 
         unwrap_tags = ["figure", "figcaption", "form", "span", "a"]
         for tag in unwrap_tags:
             for element in content.find_all(tag):
                 element.unwrap()
-            
+
         for element in content.descendants:
             if element.name:
                 element.attrs = {}
 
-        text_maker = HTML2Text(bodywidth = 80)
+        text_maker = HTML2Text(bodywidth=80)
         text_maker.ignore_links = True
         markdown = text_maker.handle(str(content))
         markdown = re.sub("\n[ \t]+", "\n", markdown)
         markdown = re.sub("\n{2,}", "\n\n", markdown)
-        
+
         snippet = re.sub("\n+", " ", markdown)[:160].strip()
         logger.info(f"Extracted content: {snippet}...")
         return markdown
-    
+
     async def process(self, task: WorkerTask):
-        url = task.url 
+        url = str(task.url)
         logger.info(f"{url} - Processing... ")
         response = requests.get(url)
         if response.url != url:
             logger.info(f"{url} - Redirect to {response.url}")
             url = response.url
-        
-        soup = BeautifulSoup(response.content, 'html.parser')
-        
+
+        soup = BeautifulSoup(response.content, "html.parser")
+
         if not self.demo_tag.is_valid():
             platform_tag = await self.get_platform_tag(DOMAIN, soup, 3600)
         else:
             platform_tag = self.demo_tag
 
-        if platform_tag and platform_tag.is_crawling_allowed() is False:
-            logger.info("Crawling disabled by tag")
-            return        
-
         logger.debug(f"Adding new links...")
-        for link in soup.find_all('a', href = True):
-            href = link['href']
+        for link in soup.find_all("a", href=True):
+            href = link["href"]
             full_local_url = BasePlugin.get_local_url(href, url)
             if full_local_url:
                 full_local_url = canonicalize_url(full_local_url)
-                #logger.info(full_local_url)
+                # logger.info(full_local_url)
                 yield CrawlerBackTask(url=full_local_url)
-            
 
         if self.is_article(url):
             (author_tag, user_name) = self._get_author_tag(soup, url)
-            if author_tag and not author_tag.is_crawling_allowed():
-                logger.info('crawling disabled by author tag')
-                return
-            
-            if self.demo_tag and user_name:
-                yield CrawlerDemoUser(user_name=user_name, short_tag_id=author_tag._tag, platform='washingtonpost.com')
-            
-            content = self.extract(soup)
-            if content:
-                storage_id = BaseStorage.gen_id(url)
-                logger.info(f"putting article into {storage_id=}")
-
-                await self.ctx.storage.put(
-                    storage_id,
-                    BasePlugin.make_text_storage_value(content),
-                )            
-                yield CrawlerContent(
-                    platform_tag_id=str(platform_tag) if platform_tag is not None else None,
-                    tag_id=str(author_tag) if author_tag is not None else None,
-                    type=DatapoolContentType.Text,
-                    storage_id=storage_id,
-                    url=url,
-                )
+
+            if author_tag is not None or platform_tag is not None:
+                if self.demo_tag and user_name and author_tag and author_tag.is_valid():
+                    yield CrawlerDemoUser(
+                        user_name=user_name, short_tag_id=str(author_tag), platform="washingtonpost.com"
+                    )
+
+                content = self.extract(soup)
+                if content:
+                    storage_id = BaseStorage.gen_id(url)
+                    logger.info(f"putting article into {storage_id=}")
+
+                    await self.ctx.storage.put(
+                        storage_id,
+                        BasePlugin.make_text_storage_value(content),
+                    )
+                    yield CrawlerContent(
+                        tag_id=str(author_tag) if author_tag is not None else None,
+                        tag_keepout=author_tag.is_keepout() if author_tag is not None else False,
+                        platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                        platform_tag_keepout=platform_tag.is_keepout() if platform_tag is not None else False,
+                        type=DatapoolContentType.Text,
+                        storage_id=storage_id,
+                        url=url,
+                    )
 
     def _get_author_tag(self, soup, url):
-        author_link = soup.find_all('a', attrs={"data-qa":"author-name"}, href=True)
+        author_link = soup.find_all("a", attrs={"data-qa": "author-name"}, href=True)
         if len(author_link) > 0:
-            logger.info(f'Author link {author_link} {author_link[0].text}')
+            logger.info(f"Author link {author_link} {author_link[0].text}")
             user_name = author_link[0].text
-            logger.info( f'Author name {user_name}')
+            logger.info(f"Author name {user_name}")
             if not self.authors.contains(user_name, 3600):
-                full_author_url = BasePlugin.get_local_url(author_link[0]['href'], url)
-                logger.info( f'{full_author_url=}')
+                full_author_url = BasePlugin.get_local_url(author_link[0]["href"], url)
+                logger.info(f"{full_author_url=}")
                 response = requests.get(full_author_url)
 
-                soup2 = BeautifulSoup(response.content, 'html.parser')
-            
+                soup2 = BeautifulSoup(response.content, "html.parser")
+
                 if self.demo_tag:
                     short_tag_id = BasePlugin.gen_demo_tag(user_name)
                     tag = BaseTag(short_tag_id)
                 else:
                     tag = BasePlugin.parse_tag_in(soup)
-                self.authors.set( user_name, tag )
+                self.authors.set(user_name, tag)
             else:
-                tag = self.authors.get( user_name )
+                tag = self.authors.get(user_name)
             return (tag, user_name)
         return (None, None)
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.45/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-import asyncio
-import json
-import re
-from typing import Dict, Optional, List, Set, Union, Tuple
+from typing import Optional, Tuple
 
 # from bs4 import BeautifulSoup
 # from playwright.async_api import Locator, Page
-from playwright.async_api import TimeoutError as PlaywriteTimeoutError
-from playwright.async_api import async_playwright, expect
+# from playwright.async_api import TimeoutError as PlaywriteTimeoutError
+from playwright.async_api import async_playwright
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerDemoUser,
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
-from ..base_plugin import BasePlugin, WorkerTask, BaseTag, CachedPairs
+from ....common.types import CrawlerContent, CrawlerDemoUser, DatapoolContentType
+from ..base_plugin import BasePlugin, BaseTag, CachedPairs, WorkerTask
 
 # import traceback
 
 
 class WikipediaPlugin(BasePlugin):
     users = CachedPairs()
 
@@ -45,22 +36,19 @@
             self.history_page = await self.context.new_page()
             self.user_page = await self.context.new_page()
 
             logger.info(f"loading url {task.url}")
             await self.page.goto(str(task.url))
 
             p = BasePlugin.parse_url(task.url)
-            
+
             if not self.demo_tag.is_valid():
                 platform_tag = await self.get_platform_tag(p.netloc, self.page, 3600)
             else:
                 platform_tag = self.demo_tag
-            if platform_tag and platform_tag.is_crawling_allowed() is False:
-                logger.info("Crawling disabled by tag")
-                return
 
             # get text of the page as plain text
             bodys = self.page.locator("body")
             body = bodys.nth(0)
             body_text = await body.inner_text()
 
             # locate "History" link
@@ -80,33 +68,31 @@
                 #         storage_id,
                 #         json.dumps(
                 #             {"body": body_text, "users": users}
                 #         ),  # TODO: structure
                 #     )
 
                 # TODO: until shared ownership is not supported, we use creator of the article as the copyright owner
-                ( creator_tag, user_name ) = await self._get_article_creator(history_url)
-                if creator_tag and not creator_tag.is_crawling_allowed():
-                    return
+                (creator_tag, user_name) = await self._get_article_creator(history_url)
                 if creator_tag or platform_tag:
                     storage_id = BaseStorage.gen_id(task.url)
                     logger.info(f"putting article into {storage_id=}")
 
-                    await self.ctx.storage.put(
-                        storage_id, BasePlugin.make_text_storage_value(body_text)
-                    )
-                    
-                    if self.demo_tag and user_name:
-                        yield CrawlerDemoUser(user_name=user_name, short_tag_id=creator_tag._tag, platform='wikipedia.org')
+                    await self.ctx.storage.put(storage_id, BasePlugin.make_text_storage_value(body_text))
+
+                    if self.demo_tag and user_name and creator_tag and creator_tag.is_valid():
+                        yield CrawlerDemoUser(
+                            user_name=user_name, short_tag_id=str(creator_tag), platform="wikipedia.org"
+                        )
 
                     yield CrawlerContent(
-                        platform_tag_id=(
-                            str(platform_tag) if platform_tag is not None else None
-                        ),
+                        platform_tag_id=str(platform_tag) if platform_tag is not None else None,
+                        platform_tag_keepout=platform_tag.is_keepout() if platform_tag is not None else False,
                         tag_id=str(creator_tag) if creator_tag is not None else None,
+                        tag_keepout=creator_tag.is_keepout() if creator_tag is not None else False,
                         type=DatapoolContentType.Text,
                         storage_id=storage_id,
                         url=task.url,
                     )
 
             # parsing links as back tasks
             async for yielded in self.parse_links(self.page):
@@ -119,19 +105,19 @@
         history_url += "&dir=prev"
 
         logger.info(f"loading url {history_url}")
         await self.history_page.goto(history_url)
 
         author_link = self.history_page.locator(".mw-userlink").last
         if await author_link.count() > 0:
-            logger.info( f'got creator link {author_link=}')
+            logger.info(f"got creator link {author_link=}")
             title = await author_link.get_attribute("title")
-            if title and title[0:5] == 'User:':
+            if title and title[0:5] == "User:":
                 username = title[5:]  # title structure is "User:$username"
-                logger.info( f'got {username=}')
+                logger.info(f"got {username=}")
 
                 if not self.users.contains(username, 36000):
                     href = await author_link.get_attribute("href")
                     if not self.demo_tag:
                         user_url = BasePlugin.get_local_url(href, history_url)
                         tag = await self._parse_user_page(user_url)
                     else:
```

### Comparing `datapools-1.0.44/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.45/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 import asyncio
 
-# import json
-# import re
-# import traceback
 import os
 import time
 from http.client import HTTPException
 from threading import Thread
 from typing import Dict, Tuple, TypeAlias
 
-# from bs4 import BeautifulSoup
-# from playwright.async_api import Locator, Page
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright
 from pytube import YouTube
 from pytube.exceptions import AgeRestrictedError as PytubeAgeRestrictedError
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
-from ....common.types import (
-    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.types import CrawlerBackTask, CrawlerContent, CrawlerNop, DatapoolContentType
 from ..base_plugin import BasePlugin, WorkerTask
 
 URL: TypeAlias = str
 TagID: TypeAlias = str
 Timestamp: TypeAlias = float
 
 
@@ -75,21 +65,18 @@
             webkit = playwright.chromium
             browser = await webkit.launch()
             context = await browser.new_context()
 
             page = await context.new_page()
 
             if channel_name is not None:
-                tag_id = await self._get_channel_tag_id(channel_name, page)
+                tag_id = await self._get_channel_tag(channel_name, page)
                 if not tag_id:
                     logger.info("No #description tag found, give up")
                     return
-                if tag_id.is_crawling_allowed() is False:
-                    logger.info("Crawling is now allowed by tag")
-                    return
 
                 logger.info(f"{tag_id=}")
 
                 url = f"https://www.youtube.com/{channel_name}/videos"
 
                 logger.info(f"loading url {url}")
                 await page.goto(url)
@@ -120,24 +107,18 @@
 
     def _download_thread(self, url, storage_id, state: dict):
         logger.info(f"_download_thread: {url=} {storage_id=}")
 
         youtube = YouTube(url)
         state["tmp_path"] = None
         try:
-            video = (
-                youtube.streams.filter(progressive=True, file_extension="mp4")
-                .order_by("resolution")
-                .first()
-            )
+            video = youtube.streams.filter(progressive=True, file_extension="mp4").order_by("resolution").first()
             for i in range(0, 3):
                 try:
-                    state["tmp_path"] = video.download(
-                        output_path="/tmp", filename=storage_id
-                    )
+                    state["tmp_path"] = video.download(output_path="/tmp", filename=storage_id)
                     break
 
                 except HTTPException as e:
                     logger.error(f"HTTPException {e}")
                     # will try to download again after delay
                     time.sleep(5)  # TODO: should be configurable
 
@@ -158,23 +139,24 @@
         channel_uri = page.locator("ytd-channel-name a:visible").filter(
             has_not=page.get_by_role("link", name="ManageEngine", exact=True)
         )
         channel_uri = await channel_uri.get_attribute("href")
         logger.info(f"{channel_uri=}")
 
         page2 = await context.new_page()
-        tag_id = await self._get_channel_tag_id(channel_uri, page2)
+        tag = await self._get_channel_tag(channel_uri, page2)
         await page2.close()
-        if not tag_id or tag_id.is_crawling_allowed() is False:
+        if tag is None:
             return
 
         storage_id = await self.download_video(url)
         if storage_id:
             yield CrawlerContent(
-                tag_id=str(tag_id),
+                tag_id=str(tag),
+                tag_keepout=tag.is_keepout(),
                 type=DatapoolContentType.Video,
                 storage_id=storage_id,
                 url=url,
             )
 
     async def download_video(self, url):
         storage_id = BaseStorage.gen_id(url)
@@ -202,41 +184,41 @@
             # for displaying at openlicense.ai
 
             logger.info(f"put video into storage {storage_id=}")
             os.remove(tmp_path)
 
             return storage_id
 
-    async def _get_channel_tag_id(self, channel_uri, page):
+    async def _get_channel_tag(self, channel_uri, page):
         # init channel_lock per channel_uri
         async with self.channel_cache_lock_protection:
             if channel_uri not in self.channel_cache_lock:
                 self.channel_cache_lock[channel_uri] = asyncio.Lock()
 
         # mutexed access to channel_tag_cache per channel_uri
         async with self.channel_cache_lock[channel_uri]:
             # get from internal cache if exists and TTL is fine
             if channel_uri in self.channel_tag_cache:
                 now = time.time()
-                (then, tag_id) = self.channel_tag_cache[channel_uri]
+                (then, tag) = self.channel_tag_cache[channel_uri]
                 if now - then <= self.CHANNEL_CACHE_TTL:
-                    logger.info(f"cached {tag_id=}")
-                    return tag_id
+                    logger.info(f"cached {tag=}")
+                    return tag
 
             # else parse channel page
-            tag_id = await self._parse_channel_tag_id(channel_uri, page)
+            tag = await self._parse_channel_tag(channel_uri, page)
 
             # add to cache
             now = time.time()
-            self.channel_tag_cache[channel_uri] = (now, tag_id)
+            self.channel_tag_cache[channel_uri] = (now, tag)
 
-            logger.info(f"parsed {tag_id=}")
-            return tag_id
+            logger.info(f"parsed {tag=}")
+            return tag
 
-    async def _parse_channel_tag_id(self, channel_uri, page):
+    async def _parse_channel_tag(self, channel_uri, page):
         url = f"https://www.youtube.com/{channel_uri}/about"
 
         logger.info(f"loading url {url}")
         await page.goto(url)
         logger.info(f"loaded {url=}")
 
         return await BasePlugin.parse_meta_tag(page, "description")
@@ -255,35 +237,27 @@
 
             n = len(videos)
             logger.info(f"videos on page {n=}")
 
             i = total_videos
             while i < n:
                 try:
-                    href = (
-                        await videos[i]
-                        .locator("a#video-title-link")
-                        .get_attribute("href", timeout=100)
-                    )
-                    title = (
-                        await videos[i]
-                        .locator("yt-formatted-string#video-title")
-                        .text_content()
-                    )
+                    href = await videos[i].locator("a#video-title-link").get_attribute("href", timeout=100)
+                    title = await videos[i].locator("yt-formatted-string#video-title").text_content()
 
                     logger.info(f"{i=} {href=} {title=}")
 
                     video_url = "https://www.youtube.com" + href
 
                     # logger.info( f'---------yielding {video_url=}')
                     yield CrawlerBackTask(url=video_url)
                     # logger.info( f'---------yielded {video_url=}')
 
                     i += 1
-                except PlaywriteTimeoutError as e:
+                except PlaywriteTimeoutError:
                     # element may be not ready yet, no problems, will get it on the next iteration
                     # logger.info( 'get_attribute timeout' )
                     break
 
             total_videos = i
 
             # logger.info( 'creating button locator')
@@ -292,16 +266,14 @@
             # scroll to  bottom. (js window.scrollTo etc does not work for some reason..)
             await page.mouse.wheel(0, 600)
 
             # logger.info( 'getting disabled attr')
             spinner_exists = await spinner.count()
 
             # logger.info(f"{spinner_exists=}")
-            if (
-                not spinner_exists and n > 0 and total_videos == n
-            ):  # all videos are processed
+            if not spinner_exists and n > 0 and total_videos == n:  # all videos are processed
                 logger.info("spinner gone, done")
                 break
 
             await asyncio.sleep(1)
 
         yield CrawlerNop()
```

### Comparing `datapools-1.0.44/datapools/worker/worker.py` & `datapools-1.0.45/datapools/worker/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 import asyncio
 import importlib
 import inspect
 import os
-import sys
 import re
+import sys
 
 # import sys
 import traceback
 import uuid
-from typing import Optional, Set
 from copy import deepcopy
+from typing import Optional, Set
 
-from .utils import get_storage_invalidation_topic
-from ..common.logger import logger
-from ..common.queues import (
-    GenericQueue,
-    QueueMessage,
-    QueueMessageType,
-    QueueRole,
-    QueueTopicMessage,
-)
 from ..common.backend_api import BackendAPI
+from ..common.logger import logger
+from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole, QueueTopicMessage
+from ..common.session_manager import Session, SessionManager
 from ..common.stoppable import Stoppable
 from ..common.storage import FileStorage
 from ..common.types import (
-    CrawlerDemoUser,
     CrawlerBackTask,
     CrawlerContent,
+    CrawlerDemoUser,
     CrawlerHintURLStatus,
     CrawlerNop,
     DatapoolContentType,
-    WorkerSettings,
     InvalidUsageException,
     WorkerContext,
-    WorkerTask
+    WorkerSettings,
+    WorkerTask,
 )
-from ..common.session_manager import SessionManager, Session
 from .plugins.base_plugin import BasePlugin
+from .utils import get_storage_invalidation_topic
 
 
 class CrawlerWorker(Stoppable):
+    demo_users: dict[str, dict[str, str]]
+
     def __init__(self, cfg: Optional[WorkerSettings] = None):
         super().__init__()
         self.cfg = cfg if cfg is not None else WorkerSettings()
         self.id = uuid.uuid4().hex
         logger.info(f"worker id={self.id}")
-        
+
         self.demo_users = {}
         self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
 
-        self.session_manager = SessionManager(
-            self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
+        self.session_manager = SessionManager(self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
         self.storage = FileStorage(self.cfg.STORAGE_PATH)
 
         self.todo_tasks: Set[asyncio.Task] = set()
 
         self.init_plugins()
         self.todo_queue = GenericQueue(
             role=QueueRole.Receiver,
@@ -95,34 +90,32 @@
         self.tasks.append(asyncio.create_task(self.worker_loop()))
         self.tasks.append(asyncio.create_task(self.topics_loop()))
         super().run()
 
     async def wait(self):
         """for CLI mode usage only"""
         if self.cfg.CLI_MODE is False:
-            logger.error('worker invalid usage')
+            logger.error("worker invalid usage")
             raise InvalidUsageException("not a cli mode")
-        logger.info('CrawlerWorker wait()')
+        logger.info("CrawlerWorker wait()")
         await self.stop_task_received.wait()
-        logger.info('CrawlerWorker stop_task_received')
+        logger.info("CrawlerWorker stop_task_received")
         waiters = (
             self.todo_queue.until_empty(),
             self.reports_queue.until_empty(),
             self.producer_queue.until_empty(),
             self.topics_queue.until_empty(),
         )
         await asyncio.gather(*waiters)
-        logger.info('CrawlerWorker wait done')
+        logger.info("CrawlerWorker wait done")
 
     async def stop(self):
         await super().stop()
         if len(self.todo_tasks) > 0:
-            await asyncio.wait(
-                self.todo_tasks, return_when=asyncio.ALL_COMPLETED
-            )
+            await asyncio.wait(self.todo_tasks, return_when=asyncio.ALL_COMPLETED)
         await self.todo_queue.stop()
         await self.reports_queue.stop()
         await self.producer_queue.stop()
         await self.topics_queue.stop()
 
         # for plugin_data in self.plugins:
         #     if plugin_data[0] is not None:
@@ -137,31 +130,26 @@
         plugin_names = []
 
         plugins_dir = os.path.join(os.path.dirname(__file__), "plugins")
         logger.info(f"{plugins_dir=}")
 
         internal_plugins = []
         for dir in os.listdir(plugins_dir):
-            if dir != "__pycache__" and os.path.isdir(
-                os.path.join(plugins_dir, dir)
-            ):
+            if dir != "__pycache__" and os.path.isdir(os.path.join(plugins_dir, dir)):
                 internal_plugins.append(dir)
-                if (
-                    self.cfg.USE_ONLY_PLUGINS is None
-                    or dir in self.cfg.USE_ONLY_PLUGINS
-                ):
+                if self.cfg.USE_ONLY_PLUGINS is None or dir in self.cfg.USE_ONLY_PLUGINS:
                     name = f"datapools.worker.plugins.{dir}"
                     plugin_names.append(name)
 
         if self.cfg.ADDITIONAL_PLUGINS is not None:
             for name in self.cfg.ADDITIONAL_PLUGINS:
                 if importlib.util.find_spec(name):
                     plugin_names.append(name)
 
-#        logger.info( f'BEFORE:{sys.modules=}')
+        #        logger.info( f'BEFORE:{sys.modules=}')
         for name in plugin_names:
             if name not in sys.modules:
                 logger.info(f"loading module {name}")
                 module = importlib.import_module(name)
             else:
                 logger.info(f"RE-loading module {name}")
                 module = importlib.reload(sys.modules[name])
@@ -180,67 +168,54 @@
 
     async def topics_loop(self):
         # from Producer.Evaluator - receives storage_id which content can be removed
         try:
             while not await self.is_stopped():
                 message = await self.topics_queue.pop(timeout=1)
                 if message:
-                    qm = QueueTopicMessage.decode(
-                        message.routing_key, message.body
-                    )
+                    qm = QueueTopicMessage.decode(message.routing_key, message.body)
                     expected_routing_key = get_storage_invalidation_topic(self.id)
-                    if (
-                        message.routing_key
-                        == expected_routing_key
-                    ):
-                        logger.info(
-                            f"invalidating storage {qm.data[ 'storage_id' ]}"
-                        )
+                    if message.routing_key == expected_routing_key:
+                        logger.info(f"invalidating storage {qm.data[ 'storage_id' ]}")
                         await self.storage.remove(qm.data["storage_id"])
 
                         await self.topics_queue.mark_done(message)
                     else:
-                        logger.error(
-                            f"!!!!!!!!!!!!!!! BUG: unexpected topic {message=} {qm=} {expected_routing_key=}"
-                        )
+                        logger.error(f"!!!!!!!!!!!!!!! BUG: unexpected topic {message=} {qm=} {expected_routing_key=}")
                         await self.topics_queue.reject(message, requeue=False)
         except Exception as e:
             logger.error(f"!!!!!!!!Exception in topics_loop() {e}")
             logger.error(traceback.format_exc())
 
     async def worker_loop(self):
         # fetches urls one by one from the queue and scans them using available plugins
         try:
             while not await self.is_stopped():
                 message = await self.todo_queue.pop(timeout=1)
                 if message:
-                    task = asyncio.create_task(
-                        self._process_todo_message(message)
-                    )
+                    task = asyncio.create_task(self._process_todo_message(message))
                     self.todo_tasks.add(task)
                     task.add_done_callback(self.todo_tasks.discard)
 
         except Exception as e:
             logger.error(f"!!!!!!!!Exception in worker_loop() {e}")
             logger.error(traceback.format_exc())
 
     async def _process_todo_message(self, message):
         qm = QueueMessage.decode(message.body)
 
         if not self.session_manager.has(qm.session_id):
-            logger.error(f'Session not found {qm.session_id}')
+            logger.error(f"Session not found {qm.session_id}")
             await self.todo_queue.reject(message)
             return
 
         if qm.type == QueueMessageType.Task:
             done = False
 
-            task = WorkerTask(
-                url=qm.data['url'],
-                content_type=qm.data.get('content_type'))
+            task = WorkerTask(url=qm.data["url"], content_type=qm.data.get("content_type"))
             logger.info(f"got {task=} {qm.session_id=}")
 
             logger.info(f"processing {task.url=}")
 
             plugin = self._get_url_plugin(task, qm.session_id)
             logger.info(f"suitable {plugin=}")
 
@@ -251,84 +226,86 @@
             is_stopped = False
             for attempt in range(0, self.cfg.ATTEMPTS_PER_URL):
                 if attempt > 0:
                     logger.info(f"{attempt=}")
 
                 try:
                     session = self.session_manager.get(qm.session_id)
+
                     def deleted_or_stopped(session_id):
                         nonlocal is_stopped, session
                         if self.session_manager.has(session_id):
                             if session.is_stopped():
                                 is_stopped = True
-                                logger.info(f'Session is stopped, breaking. {session_id=}')
+                                logger.info(f"Session is stopped, breaking. {session_id=}")
                                 return True
                         else:
                             is_stopped = True
-                            logger.error( f'Session is deleted, breaking. {session_id=}')
+                            logger.error(f"Session is deleted, breaking. {session_id=}")
                             return True
-                        
+
                     if deleted_or_stopped(qm.session_id):
                         break
 
                     async for content_or_task in plugin.process(task):
                         # logger.info( f'{type( content_or_task )=}')
                         t = type(content_or_task)
                         # logger.info( f'{(t is CrawlerNop)=}')
-                        
+
                         if deleted_or_stopped(qm.session_id):
                             break
-                        
+
                         if t is CrawlerContent:
                             session.inc_crawled_content()
-                            
+
                             # notifying datapool pipeline about new crawled data
                             await self.producer_queue.push(
                                 QueueMessage(
                                     qm.session_id,
                                     QueueMessageType.Task,
                                     {
                                         "parent_url": task.url,
                                         "url": content_or_task.url,
                                         "storage_id": content_or_task.storage_id,
                                         "tag_id": content_or_task.tag_id,
+                                        "tag_keepout": content_or_task.tag_keepout,
                                         "copyright_tag_id": content_or_task.copyright_tag_id,
+                                        "copyright_tag_keepout": content_or_task.copyright_tag_keepout,
                                         "platform_tag_id": content_or_task.platform_tag_id,
-                                        "type": DatapoolContentType(
-                                            content_or_task.type
-                                        ).value,
+                                        "platform_tag_keepout": content_or_task.platform_tag_keepout,
+                                        "type": DatapoolContentType(content_or_task.type).value,
                                         "worker_id": self.id,
                                     },
                                 )
                             )
 
                         elif t is CrawlerBackTask:
                             await self._add_back_task(qm.session_id, content_or_task)
                         elif t is CrawlerDemoUser:
                             ct = content_or_task
                             if ct.platform not in self.demo_users:
                                 self.demo_users[ct.platform] = {}
                             if ct.user_name not in self.demo_users[ct.platform]:
-                                self.demo_users[ct.platform][ct.user_name] = ct.short_tag_id
-                                logger.info(f'============= {dict(ct)} ===========')
+                                logger.info(f"============= {dict(ct)} ===========")
                                 await self.api.add_demo_user(dict(ct))
+                                self.demo_users[ct.platform][ct.user_name] = ct.short_tag_id
                         elif t is CrawlerNop:
                             pass
                         else:
                             raise Exception(f"unknown {content_or_task=}")
 
                         is_stopped = await self.is_stopped()
                         if is_stopped:
                             break
 
                     logger.info("plugin.process done")
                     await self._set_task_status(
                         qm.session_id,
                         task,
-                        CrawlerHintURLStatus.Success if not is_stopped else CrawlerHintURLStatus.Canceled
+                        CrawlerHintURLStatus.Success if not is_stopped else CrawlerHintURLStatus.Canceled,
                     )
 
                     done = True
                     break
                 except Exception as e:
                     logger.error(f"failed get url: {e}")
                     logger.error(traceback.format_exc())
@@ -344,98 +321,79 @@
             else:
                 logger.info(f"sending reject for {message.message_id=}")
                 await self.todo_queue.reject(message, requeue=False)
                 await self._set_task_status(qm.session_id, task, CrawlerHintURLStatus.Failure)
 
         elif qm.type == QueueMessageType.Stop:
             await self.todo_queue.mark_done(message)
-            logger.info('worker: got stop task')
+            logger.info("worker: got stop task")
 
-            await self.producer_queue.push(
-                QueueMessage(
-                    qm.session_id,
-                    QueueMessageType.Stop
-                )
-            )
+            await self.producer_queue.push(QueueMessage(qm.session_id, QueueMessageType.Stop))
             # notifying scheduler that we are done
-            await self.reports_queue.push(
-                QueueMessage(
-                    qm.session_id,
-                    QueueMessageType.Stop
-                )
-            )
+            await self.reports_queue.push(QueueMessage(qm.session_id, QueueMessageType.Stop))
             self.stop_task_received.set()
 
         else:
             logger.error(f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}")
             await self.todo_queue.reject(message)
 
     async def _set_task_status(self, session_id, task, status: CrawlerHintURLStatus):
         await self.reports_queue.push(
-            QueueMessage(
-                session_id, QueueMessageType.Report, {"task": deepcopy(task), "status": status.value}
-            )
+            QueueMessage(session_id, QueueMessageType.Report, {"task": deepcopy(task), "status": status.value})
         )
 
     async def _add_back_task(self, session_id, task: CrawlerBackTask):
-        await self.reports_queue.push(
-            QueueMessage(session_id, QueueMessageType.Task, task.to_dict())
-        )
+        await self.reports_queue.push(QueueMessage(session_id, QueueMessageType.Task, task.to_dict()))
 
     def _get_plugin_object(self, cls, session_id) -> BasePlugin:
-        ctx = WorkerContext(
-            session=self.session_manager.get(session_id),
-            storage=self.storage
-        )
+        ctx = WorkerContext(session=self.session_manager.get(session_id), storage=self.storage)
 
         args = [ctx]
         kwargs = {}
         logger.info(f"_get_plugin_object {cls=}")
 
         # convert class name into config plugins key
         # example: GoogleDrivePlugin => google_drive
         # example: S3Plugin => s3
-        cap_words = re.sub(r'([A-Z])', r' \1', cls[0]).split()
-        #logger.info(f'{cap_words=}')
-        config_key = '_'.join(list(map(lambda x: x.lower(), cap_words[:-1])))
-        #logger.info(f'{config_key=}')
+        cap_words = re.sub(r"([A-Z])", r" \1", cls[0]).split()
+        # logger.info(f'{cap_words=}')
+        config_key = "_".join(list(map(lambda x: x.lower(), cap_words[:-1])))
+        # logger.info(f'{config_key=}')
         plugin_config = self.cfg.plugins_config.get(config_key)
-        #logger.info(f'{plugin_config=}')
+        # logger.info(f'{plugin_config=}')
         if plugin_config is not None:
             # plugin config dict keys must match plugin's class __init__ arguments
             kwargs = plugin_config
 
         return cls[1](*args, **kwargs)
 
     def _get_url_plugin(self, task: WorkerTask, session_id):
         for plugin_data in self.plugins:
             cls = plugin_data[1]
             if cls[0] != "DefaultPlugin":
                 if cls[1].is_supported(task.url):
                     if plugin_data[0] is None:
-                        plugin_data[0] = self._get_plugin_object(
-                            cls, session_id)
+                        plugin_data[0] = self._get_plugin_object(cls, session_id)
 
                     if not plugin_data[0].is_busy:  # type: ignore[union-attr]
-                        plugin_data[0].is_busy = True   # type: ignore[union-attr]
+                        plugin_data[0].is_busy = True  # type: ignore[union-attr]
                         return plugin_data[0]
                     else:
                         new_obj = self._get_plugin_object(cls, session_id)
                         new_obj.is_busy = True
                         return new_obj
 
         # creating/usingexisting default plugin
         for plugin_data in self.plugins:
             cls = plugin_data[1]
             if cls[0] == "DefaultPlugin":
                 if cls[1].is_supported(task.url):
                     if plugin_data[0] is None:
-                        plugin_data[0] = self._get_plugin_object(
-                            cls, session_id)
+                        plugin_data[0] = self._get_plugin_object(cls, session_id)
 
                     if not plugin_data[0].is_busy:  # type: ignore[union-attr]
-                        plugin_data[0].is_busy = True   # type: ignore[union-attr]
+                        plugin_data[0].is_busy = True  # type: ignore[union-attr]
                         return plugin_data[0]
                     else:
                         new_obj = self._get_plugin_object(cls, session_id)
                         new_obj.is_busy = True
                         return new_obj
```

### Comparing `datapools-1.0.44/datapools.egg-info/PKG-INFO` & `datapools-1.0.45/datapools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.44
+Version: 1.0.45
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.44/datapools.egg-info/SOURCES.txt` & `datapools-1.0.45/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.44/setup.py` & `datapools-1.0.45/setup.py`

 * *Files identical despite different names*


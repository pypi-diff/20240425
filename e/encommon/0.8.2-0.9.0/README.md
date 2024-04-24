# Comparing `tmp/encommon-0.8.2.tar.gz` & `tmp/encommon-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encommon-0.8.2.tar", last modified: Sun Apr 14 04:45:34 2024, max compression
+gzip compressed data, was "encommon-0.9.0.tar", last modified: Sun Apr 14 13:45:30 2024, max compression
```

## Comparing `encommon-0.8.2.tar` & `encommon-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.8.2/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.8.2/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2917 2024-04-14 04:45:34.075637 encommon-0.8.2/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2423 2024-04-11 05:09:20.000000 encommon-0.8.2/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.072637 encommon-0.8.2/encommon/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      859 2024-04-07 23:12:30.000000 encommon-0.8.2/encommon/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2099 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4802 2024-04-08 05:21:36.000000 encommon-0.8.2/encommon/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2388 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13488 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1806 2024-04-07 23:12:30.000000 encommon-0.8.2/encommon/config/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2535 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/paths.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1069 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2325 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2240 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5131 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2578 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1810 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/crypts/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      371 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3540 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/crypts/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2651 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/crypts/test/test_crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1125 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/crypts/test/test_hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.8.2/encommon/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/times/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      638 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3635 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10794 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6153 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/parse.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/times/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2059 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4161 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4055 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_parse.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3073 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/test/test_timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1691 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5409 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/test/test_window.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6603 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9696 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-14 03:50:15.000000 encommon-0.8.2/encommon/times/window.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/types/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-07 10:25:51.000000 encommon-0.8.2/encommon/types/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2265 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2739 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      632 2024-04-07 10:25:51.000000 encommon-0.8.2/encommon/types/strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/types/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2678 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/test/test_dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      973 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/types/test/test_empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      406 2024-04-07 10:25:51.000000 encommon-0.8.2/encommon/types/test/test_strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/encommon/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      927 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1355 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2471 2024-04-07 23:12:30.000000 encommon-0.8.2/encommon/utils/match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3545 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3230 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7531 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/stdout.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/encommon/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      681 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1919 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1710 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_stdout.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-14 04:41:22.000000 encommon-0.8.2/encommon/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/encommon.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2917 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1926 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.8.2/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.8.2/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      558 2024-04-14 04:45:34.075637 encommon-0.8.2/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.916325 encommon-0.9.0/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.9.0/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.9.0/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2917 2024-04-14 13:45:30.916325 encommon-0.9.0/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2423 2024-04-11 05:09:20.000000 encommon-0.9.0/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.914325 encommon-0.9.0/encommon/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.914325 encommon-0.9.0/encommon/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      859 2024-04-07 23:12:30.000000 encommon-0.9.0/encommon/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2099 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/config/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4802 2024-04-08 05:21:36.000000 encommon-0.9.0/encommon/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2388 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/config/files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13488 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/config/logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1806 2024-04-07 23:12:30.000000 encommon-0.9.0/encommon/config/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2535 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/config/paths.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.914325 encommon-0.9.0/encommon/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1069 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/config/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2440 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2295 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/config/test/test_files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5188 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/config/test/test_logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2633 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/config/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1810 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.915325 encommon-0.9.0/encommon/crypts/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      371 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/crypts/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3540 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/crypts/crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/crypts/hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/crypts/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.915325 encommon-0.9.0/encommon/crypts/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/crypts/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2706 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/crypts/test/test_crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1180 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/crypts/test/test_hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.9.0/encommon/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.915325 encommon-0.9.0/encommon/times/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      638 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3635 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10794 2024-04-14 04:37:18.000000 encommon-0.9.0/encommon/times/duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6153 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/parse.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.915325 encommon-0.9.0/encommon/times/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2059 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4189 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/times/test/test_duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4055 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/test/test_parse.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3128 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/times/test/test_timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1748 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/times/test/test_times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5464 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/times/test/test_window.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6603 2024-04-14 04:37:18.000000 encommon-0.9.0/encommon/times/timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9696 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/times/times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-14 03:50:15.000000 encommon-0.9.0/encommon/times/window.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.915325 encommon-0.9.0/encommon/types/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      544 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/types/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2265 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/types/dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2739 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/types/empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2175 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/types/strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.916325 encommon-0.9.0/encommon/types/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/types/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2678 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/types/test/test_dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      973 2024-04-14 04:37:18.000000 encommon-0.9.0/encommon/types/test/test_empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1084 2024-04-14 13:42:29.000000 encommon-0.9.0/encommon/types/test/test_strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.916325 encommon-0.9.0/encommon/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      927 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1355 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2471 2024-04-07 23:12:30.000000 encommon-0.9.0/encommon/utils/match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3545 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3230 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7531 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/stdout.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.916325 encommon-0.9.0/encommon/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      681 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/test/test_match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1919 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1710 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/test/test_sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-07 10:21:05.000000 encommon-0.9.0/encommon/utils/test/test_stdout.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-14 13:43:12.000000 encommon-0.9.0/encommon/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 13:45:30.916325 encommon-0.9.0/encommon.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2917 2024-04-14 13:45:30.000000 encommon-0.9.0/encommon.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1926 2024-04-14 13:45:30.000000 encommon-0.9.0/encommon.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-14 13:45:30.000000 encommon-0.9.0/encommon.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-14 13:45:30.000000 encommon-0.9.0/encommon.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-14 13:45:30.000000 encommon-0.9.0/encommon.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.9.0/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.9.0/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      558 2024-04-14 13:45:30.916325 encommon-0.9.0/setup.cfg
```

### Comparing `encommon-0.8.2/LICENSE` & `encommon-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/PKG-INFO` & `encommon-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.8.2
+Version: 0.9.0
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.8.2/README.md` & `encommon-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/__init__.py` & `encommon-0.9.0/encommon/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/__init__.py` & `encommon-0.9.0/encommon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/common.py` & `encommon-0.9.0/encommon/config/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/config.py` & `encommon-0.9.0/encommon/config/config.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/files.py` & `encommon-0.9.0/encommon/config/files.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/logger.py` & `encommon-0.9.0/encommon/config/logger.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/params.py` & `encommon-0.9.0/encommon/config/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/paths.py` & `encommon-0.9.0/encommon/config/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/test/test_common.py` & `encommon-0.9.0/encommon/config/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/config/test/test_config.py` & `encommon-0.9.0/encommon/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,114 +4,81 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from pathlib import Path
-from typing import TYPE_CHECKING
 
-from . import SAMPLES
-from ..logger import Logger
-from ..params import Params
-from ... import ENPYRWS
-from ... import PROJECT
-from ...crypts import Crypts
-from ...utils import load_sample
-from ...utils import prep_sample
+from pytest import fixture
 
-if TYPE_CHECKING:
-    from ..config import Config
+from .config import Config
+from .config.test import SAMPLES
+from .utils import save_text
 
 
 
-def test_Config(
+def config_factory(
     tmp_path: Path,
-    config: 'Config',
-) -> None:
+) -> Config:
     """
-    Perform various tests associated with relevant routines.
+    Construct the instance for use in the downstream tests.
 
     :param tmp_path: pytest object for temporal filesystem.
-    :param config: Primary class instance for configuration.
+    :returns: Newly constructed instance of related class.
     """
 
+    save_text(
+        f'{tmp_path}/config.yml',
+        content=(
+            'enconfig:\n'
+            '  paths:\n'
+            f"    - '{SAMPLES}/stark'\n"
+            f"    - '{SAMPLES}/wayne'\n"
+            'enlogger:\n'
+            '  stdo_level: info\n'
+            'encrypts:\n'
+            '  phrases:\n'
+            '    default: phrase\n'))
+
+    config_log = f'{tmp_path}/config.log'
+
+    cargs = {
+        'enlogger': {
+            'file_path': config_log,
+            'file_level': 'info'}}
+
+    return Config(
+        files=f'{tmp_path}/config.yml',
+        cargs=cargs)
 
-    attrs = list(config.__dict__)
 
-    assert attrs == [
-        '_Config__model',
-        '_Config__files',
-        '_Config__cargs',
-        '_Config__params',
-        '_Config__paths',
-        '_Config__logger',
-        '_Config__crypts']
 
+@fixture
+def config_path(
+    tmp_path: Path,
+) -> Path:
+    """
+    Construct the directory and files needed for the tests.
 
-    assert 1 <= repr(config).find(
-        'config.Config object')
-
-    assert hash(config) > 0
-
-    assert 1 <= str(config).find(
-        'config.Config object')
-
-
-    assert 'ConfigFiles' in str(config.files)
-
-    assert 'ConfigPaths' in str(config.paths)
-
-    assert len(config.cargs) == 1
-
-    assert len(config.config) == 3
-
-    assert config.model is Params
-
-    assert isinstance(config.params, Params)
-
-    assert isinstance(config.logger, Logger)
-
-    assert isinstance(config.crypts, Crypts)
-
-
-    replaces = {
-        'pytemp': tmp_path,
-        'PROJECT': PROJECT}
-
-    sample_path = (
-        f'{SAMPLES}/config.json')
-
-    sample = load_sample(
-        path=sample_path,
-        update=ENPYRWS,
-        content=config.config,
-        replace=replaces)
+    :param tmp_path: pytest object for temporal filesystem.
+    :returns: New resolved filesystem path object instance.
+    """
 
-    expect = prep_sample(
-        content=config.config,
-        replace=replaces)
+    config_factory(tmp_path)
 
-    assert sample == expect
+    return tmp_path.resolve()
 
 
 
-def test_Config_cover(
-    config: 'Config',
-) -> None:
+@fixture
+def config(
+    tmp_path: Path,
+) -> Config:
     """
-    Perform various tests associated with relevant routines.
+    Construct the instance for use in the downstream tests.
 
-    :param config: Primary class instance for configuration.
+    :param tmp_path: pytest object for temporal filesystem.
+    :returns: Newly constructed instance of related class.
     """
 
-
-    logger1 = config.logger
-    logger2 = config.logger
-
-    assert logger1 is logger2
-
-
-    crypts1 = config.crypts
-    crypts2 = config.crypts
-
-    assert crypts1 is crypts2
+    return config_factory(tmp_path)
```

### Comparing `encommon-0.8.2/encommon/config/test/test_files.py` & `encommon-0.9.0/encommon/config/test/test_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from pathlib import Path
 
 from pytest import fixture
 
 from . import SAMPLES
 from ..files import ConfigFile
 from ..files import ConfigFiles
+from ...types import inrepr
+from ...types import instr
 
 
 
 @fixture
 def files(
     config_path: Path,
 ) -> ConfigFiles:
@@ -50,21 +52,23 @@
     attrs = list(file.__dict__)
 
     assert attrs == [
         'path',
         'config']
 
 
-    assert 1 <= repr(file).find(
-        'files.ConfigFile object')
+    assert inrepr(
+        'files.ConfigFile object',
+        file)
 
     assert hash(file) > 0
 
-    assert 1 <= str(file).find(
-        'files.ConfigFile object')
+    assert instr(
+        'files.ConfigFile object',
+        file)
 
 
     assert file.path.name == 'config.yml'
 
     assert len(file.config) == 3
 
 
@@ -83,21 +87,23 @@
 
     assert attrs == [
         'paths',
         'config',
         '_ConfigFiles__merged']
 
 
-    assert 1 <= repr(files).find(
-        'files.ConfigFiles object')
+    assert inrepr(
+        'files.ConfigFiles object',
+        files)
 
     assert hash(files) > 0
 
-    assert 1 <= str(files).find(
-        'files.ConfigFiles object')
+    assert instr(
+        'files.ConfigFiles object',
+        files)
 
 
     assert len(files.paths) == 2
 
     assert len(files.config) == 2
 
     assert files.merged == {
```

### Comparing `encommon-0.8.2/encommon/config/test/test_logger.py` & `encommon-0.9.0/encommon/config/test/test_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from pytest import fixture
 
 from ..logger import Logger
 from ..logger import Message
 from ..params import LoggerParams
 from ...times.common import UNIXMPOCH
 from ...times.common import UNIXSPOCH
+from ...types import inrepr
+from ...types import instr
 from ...utils import strip_ansi
 
 
 
 _CAPLOG = list[tuple[str, int, str]]
 
 
@@ -71,21 +73,23 @@
 
     assert attrs == [
         '_Message__level',
         '_Message__time',
         '_Message__fields']
 
 
-    assert repr(message)[:20] == (
-        'Message(level="info"')
+    assert inrepr(
+        'Message(level="info"',
+        message)
 
     assert hash(message) > 0
 
-    assert str(message)[:20] == (
-        'Message(level="info"')
+    assert instr(
+        'Message(level="info"',
+        message)
 
 
     assert message.level == 'info'
 
     assert message.time == 0
 
     assert len(message.fields) == 8
@@ -142,21 +146,23 @@
         '_Logger__file_level',
         '_Logger__file_path',
         '_Logger__started',
         '_Logger__logr_stdo',
         '_Logger__logr_file']
 
 
-    assert 1 <= repr(logger).find(
-        'logger.Logger object')
+    assert inrepr(
+        'logger.Logger object',
+        logger)
 
     assert hash(logger) > 0
 
-    assert 1 <= str(logger).find(
-        'logger.Logger object')
+    assert instr(
+        'logger.Logger object',
+        logger)
 
 
     assert logger.stdo_level == 'info'
 
     assert logger.file_level == 'info'
 
     assert logger.file_path is not None
```

### Comparing `encommon-0.8.2/encommon/config/test/test_paths.py` & `encommon-0.9.0/encommon/config/test/test_paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pytest import fixture
 
 from . import SAMPLES
 from ..paths import ConfigPath
 from ..paths import ConfigPaths
 from ... import ENPYRWS
 from ... import PROJECT
+from ...types import inrepr
+from ...types import instr
 from ...utils import load_sample
 from ...utils import prep_sample
 
 
 
 @fixture
 def paths(
@@ -53,21 +55,23 @@
     attrs = list(path.__dict__)
 
     assert attrs == [
         'path',
         'config']
 
 
-    assert 1 <= repr(path).find(
-        'paths.ConfigPath object')
+    assert inrepr(
+        'paths.ConfigPath object',
+        path)
 
     assert hash(path) > 0
 
-    assert 1 <= str(path).find(
-        'paths.ConfigPath object')
+    assert instr(
+        'paths.ConfigPath object',
+        path)
 
 
     assert 'test' in path.path.name
 
     assert len(path.config) == 1
 
 
@@ -85,21 +89,23 @@
     attrs = list(paths.__dict__)
 
     assert attrs == [
         'paths', 'config',
         '_ConfigPaths__merged']
 
 
-    assert 1 <= repr(paths).find(
-        'paths.ConfigPaths object')
+    assert inrepr(
+        'paths.ConfigPaths object',
+        paths)
 
     assert hash(paths) > 0
 
-    assert 1 <= str(paths).find(
-        'paths.ConfigPaths object')
+    assert instr(
+        'paths.ConfigPaths object',
+        paths)
 
 
     assert len(paths.paths) == 2
 
     assert len(paths.config) == 2
```

### Comparing `encommon-0.8.2/encommon/crypts/crypts.py` & `encommon-0.9.0/encommon/crypts/crypts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/crypts/hashes.py` & `encommon-0.9.0/encommon/crypts/hashes.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/crypts/params.py` & `encommon-0.9.0/encommon/crypts/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/crypts/test/test_crypts.py` & `encommon-0.9.0/encommon/crypts/test/test_crypts.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from pytest import fixture
 from pytest import mark
 from pytest import raises
 
 from ..crypts import Crypts
 from ..params import CryptsParams
+from ...types import inrepr
+from ...types import instr
 
 
 
 @fixture
 def crypts() -> Crypts:
     """
     Construct the instance for use in the downstream tests.
@@ -47,21 +49,23 @@
 
     attrs = list(crypts.__dict__)
 
     assert attrs == [
         '_Crypts__phrases']
 
 
-    assert 1 <= repr(crypts).find(
-        'crypts.Crypts object')
+    assert inrepr(
+        'crypts.Crypts object',
+        crypts)
 
     assert hash(crypts) > 0
 
-    assert 1 <= str(crypts).find(
-        'crypts.Crypts object')
+    assert instr(
+        'crypts.Crypts object',
+        crypts)
 
 
     assert len(crypts.phrases) == 2
 
     assert len(crypts.keygen()) == 44
```

### Comparing `encommon-0.8.2/encommon/crypts/test/test_hashes.py` & `encommon-0.9.0/encommon/crypts/test/test_hashes.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from ..hashes import Hashes
+from ...types import inrepr
+from ...types import instr
 
 
 
 def test_Hashes() -> None:
     """
     Perform various tests associated with relevant routines.
     """
@@ -21,21 +23,23 @@
 
     attrs = list(hashes.__dict__)
 
     assert attrs == [
         '_Hashes__string']
 
 
-    assert 1 <= repr(hashes).find(
-        'hashes.Hashes object')
+    assert inrepr(
+        'hashes.Hashes object',
+        hashes)
 
     assert hash(hashes) > 0
 
-    assert 1 <= str(hashes).find(
-        'hashes.Hashes object')
+    assert instr(
+        'hashes.Hashes object',
+        hashes)
 
 
     assert hashes.string == 'string'
 
     assert hashes.md5[:3] == 'b45'
     assert hashes.md5[-2:] == '21'
```

### Comparing `encommon-0.8.2/encommon/times/__init__.py` & `encommon-0.9.0/encommon/times/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/common.py` & `encommon-0.9.0/encommon/times/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/duration.py` & `encommon-0.9.0/encommon/times/duration.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/parse.py` & `encommon-0.9.0/encommon/times/parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/test/test_common.py` & `encommon-0.9.0/encommon/times/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/test/test_duration.py` & `encommon-0.9.0/encommon/times/test/test_duration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from ..duration import Duration
+from ...types import inrepr
 from ...types.strings import COMMAS
 
 
 
 def test_Duration() -> None:
     """
     Perform various tests associated with relevant routines.
@@ -24,16 +25,17 @@
 
     assert attrs == [
         '_Duration__source',
         '_Duration__smart',
         '_Duration__groups']
 
 
-    assert repr(durate)[:23] == (
-        'Duration(seconds=95401.')
+    assert inrepr(
+        'Duration(seconds=95401',
+        durate)
 
     assert hash(durate) > 0
 
     assert str(durate) == '1d2h30m'
 
 
     assert int(durate) == 95401
```

### Comparing `encommon-0.8.2/encommon/times/test/test_parse.py` & `encommon-0.9.0/encommon/times/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/test/test_timers.py` & `encommon-0.9.0/encommon/times/test/test_timers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from pathlib import Path
 from time import sleep
 
 from pytest import fixture
 from pytest import raises
 
 from ..timers import Timers
+from ...types import inrepr
+from ...types import instr
 
 
 
 @fixture
 def timers(
     tmp_path: Path,
 ) -> Timers:
@@ -50,21 +52,23 @@
         '_Timers__config',
         '_Timers__sqlite',
         '_Timers__file',
         '_Timers__table',
         '_Timers__cache']
 
 
-    assert 1 <= repr(timers).find(
-        'timers.Timers object')
+    assert inrepr(
+        'timers.Timers object',
+        timers)
 
     assert hash(timers) > 0
 
-    assert 1 <= str(timers).find(
-        'timers.Timers object')
+    assert instr(
+        'timers.Timers object',
+        timers)
 
 
     assert timers.timers == {'one': 1}
 
     assert timers.sqlite is not None
 
     assert timers.file[-8:] == 'cache.db'
```

### Comparing `encommon-0.8.2/encommon/times/test/test_times.py` & `encommon-0.9.0/encommon/times/test/test_times.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 
 from ..common import STAMP_SIMPLE
 from ..common import UNIXEPOCH
 from ..common import UNIXHPOCH
 from ..common import UNIXMPOCH
 from ..times import Times
+from ...types import inrepr
+from ...types import instr
 
 
 
 def test_Times() -> None:
     """
     Perform various tests associated with relevant routines.
     """
@@ -28,21 +30,23 @@
     attrs = list(times.__dict__)
 
     assert attrs == [
         '_Times__source',
         '_Times__hashed']
 
 
-    assert repr(times)[:23] == (
-        "Times('1970-01-01T00:00")
+    assert inrepr(
+        "Times('1970-01-01T00:00",
+        times)
 
     assert hash(times) > 0
 
-    assert str(times)[:23] == (
-        '1970-01-01T00:00:00.000')
+    assert instr(
+        '1970-01-01T00:00:00.000',
+        times)
 
 
     assert int(times) == 0
     assert float(times) == 0.0
 
     assert times + 1 == Times(1)
     assert times - 1 == Times(-1)
```

### Comparing `encommon-0.8.2/encommon/times/test/test_window.py` & `encommon-0.9.0/encommon/times/test/test_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from pytest import fixture
 from pytest import mark
 
 from ..window import Window
 from ..window import window_croniter
 from ..window import window_interval
+from ...types import inrepr
+from ...types import instr
 
 if TYPE_CHECKING:
     from ..common import PARSABLE
 
 
 
 @fixture
@@ -54,21 +56,23 @@
         '_Window__anchor',
         '_Window__delay',
         '_Window__wilast',
         '_Window__winext',
         '_Window__walked']
 
 
-    assert 1 <= repr(window).find(
-        'window.Window object')
+    assert inrepr(
+        'window.Window object',
+        window)
 
     assert hash(window) > 0
 
-    assert 1 <= str(window).find(
-        'window.Window object')
+    assert instr(
+        'window.Window object',
+        window)
 
 
     assert window.schedule == '* * * * *'
 
     assert window.start == '1970-01-01T00:05:30Z'
 
     assert window.stop == '1970-01-01T00:10:30Z'
```

### Comparing `encommon-0.8.2/encommon/times/timers.py` & `encommon-0.9.0/encommon/times/timers.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/times.py` & `encommon-0.9.0/encommon/times/times.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/times/window.py` & `encommon-0.9.0/encommon/times/window.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/types/dicts.py` & `encommon-0.9.0/encommon/types/dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/types/empty.py` & `encommon-0.9.0/encommon/types/empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/types/test/test_dicts.py` & `encommon-0.9.0/encommon/types/test/test_dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/types/test/test_empty.py` & `encommon-0.9.0/encommon/types/test/test_empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/__init__.py` & `encommon-0.9.0/encommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/common.py` & `encommon-0.9.0/encommon/utils/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/match.py` & `encommon-0.9.0/encommon/utils/match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/paths.py` & `encommon-0.9.0/encommon/utils/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/sample.py` & `encommon-0.9.0/encommon/utils/sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/stdout.py` & `encommon-0.9.0/encommon/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/test/test_common.py` & `encommon-0.9.0/encommon/utils/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/test/test_match.py` & `encommon-0.9.0/encommon/utils/test/test_match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/test/test_paths.py` & `encommon-0.9.0/encommon/utils/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/test/test_sample.py` & `encommon-0.9.0/encommon/utils/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon/utils/test/test_stdout.py` & `encommon-0.9.0/encommon/utils/test/test_stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/encommon.egg-info/PKG-INFO` & `encommon-0.9.0/encommon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.8.2
+Version: 0.9.0
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.8.2/encommon.egg-info/SOURCES.txt` & `encommon-0.9.0/encommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/pyproject.toml` & `encommon-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `encommon-0.8.2/setup.cfg` & `encommon-0.9.0/setup.cfg`

 * *Files identical despite different names*


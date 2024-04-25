# Comparing `tmp/enhomie-0.2.0.tar.gz` & `tmp/enhomie-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhomie-0.2.0.tar", last modified: Mon Apr 15 08:50:05 2024, max compression
+gzip compressed data, was "enhomie-0.2.1.tar", last modified: Thu Apr 25 01:50:11 2024, max compression
```

## Comparing `enhomie-0.2.0.tar` & `enhomie-0.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.823818 enhomie-0.2.0/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-14 23:33:41.000000 enhomie-0.2.0/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       31 2024-03-14 23:35:40.000000 enhomie-0.2.0/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3949 2024-04-15 08:50:05.823818 enhomie-0.2.0/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3560 2024-04-15 08:45:40.000000 enhomie-0.2.0/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.821817 enhomie-0.2.0/enhomie/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.821817 enhomie-0.2.0/enhomie/builtins/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      423 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/builtins/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1644 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/builtins/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.821817 enhomie-0.2.0/enhomie/builtins/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/builtins/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      928 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/builtins/test/test_params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1277 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/builtins/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1778 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/builtins/when.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.821817 enhomie-0.2.0/enhomie/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2024 2024-04-08 05:15:33.000000 enhomie-0.2.0/enhomie/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2184 2024-04-14 14:23:52.000000 enhomie-0.2.0/enhomie/config/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.821817 enhomie-0.2.0/enhomie/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1205 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5986 2024-04-15 06:45:34.000000 enhomie-0.2.0/enhomie/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.822818 enhomie-0.2.0/enhomie/homie/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/homie/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6633 2024-04-08 04:57:00.000000 enhomie-0.2.0/enhomie/homie/desire.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5409 2024-04-08 06:47:33.000000 enhomie-0.2.0/enhomie/homie/group.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    15456 2024-04-15 08:35:24.000000 enhomie-0.2.0/enhomie/homie/homie.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3425 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/homie/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6012 2024-04-15 08:01:26.000000 enhomie-0.2.0/enhomie/homie/scene.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.822818 enhomie-0.2.0/enhomie/homie/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/homie/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2633 2024-04-15 08:22:12.000000 enhomie-0.2.0/enhomie/homie/test/test_desire.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2184 2024-04-15 08:22:39.000000 enhomie-0.2.0/enhomie/homie/test/test_group.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4354 2024-04-15 08:23:16.000000 enhomie-0.2.0/enhomie/homie/test/test_homie.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2587 2024-04-15 08:23:41.000000 enhomie-0.2.0/enhomie/homie/test/test_scene.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1303 2024-04-15 08:24:01.000000 enhomie-0.2.0/enhomie/homie/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3251 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/homie/when.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.822818 enhomie-0.2.0/enhomie/philipshue/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:09.000000 enhomie-0.2.0/enhomie/philipshue/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10609 2024-04-15 07:54:55.000000 enhomie-0.2.0/enhomie/philipshue/bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8007 2024-04-08 04:48:39.000000 enhomie-0.2.0/enhomie/philipshue/device.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1826 2024-04-14 14:22:48.000000 enhomie-0.2.0/enhomie/philipshue/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.822818 enhomie-0.2.0/enhomie/philipshue/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      635 2024-04-08 05:44:56.000000 enhomie-0.2.0/enhomie/philipshue/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5063 2024-04-15 08:24:20.000000 enhomie-0.2.0/enhomie/philipshue/test/test_bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3131 2024-04-15 08:24:45.000000 enhomie-0.2.0/enhomie/philipshue/test/test_device.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3263 2024-04-08 04:36:12.000000 enhomie-0.2.0/enhomie/philipshue/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2126 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/philipshue/when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-24 11:17:04.000000 enhomie-0.2.0/enhomie/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.823818 enhomie-0.2.0/enhomie/ubiquiti/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:29.000000 enhomie-0.2.0/enhomie/ubiquiti/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7558 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/ubiquiti/client.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1991 2024-04-14 14:21:10.000000 enhomie-0.2.0/enhomie/ubiquiti/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9397 2024-04-15 06:44:32.000000 enhomie-0.2.0/enhomie/ubiquiti/router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.823818 enhomie-0.2.0/enhomie/ubiquiti/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/ubiquiti/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4146 2024-04-15 08:25:06.000000 enhomie-0.2.0/enhomie/ubiquiti/test/test_client.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3495 2024-04-15 08:25:30.000000 enhomie-0.2.0/enhomie/ubiquiti/test/test_router.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2643 2024-04-08 04:36:08.000000 enhomie-0.2.0/enhomie/ubiquiti/test/test_when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2148 2024-04-08 04:21:22.000000 enhomie-0.2.0/enhomie/ubiquiti/when.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-15 08:48:26.000000 enhomie-0.2.0/enhomie/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-15 08:50:05.823818 enhomie-0.2.0/enhomie.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3949 2024-04-15 08:50:05.000000 enhomie-0.2.0/enhomie.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1568 2024-04-15 08:50:05.000000 enhomie-0.2.0/enhomie.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-15 08:50:05.000000 enhomie-0.2.0/enhomie.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-15 08:50:05.000000 enhomie-0.2.0/enhomie.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        8 2024-04-15 08:50:05.000000 enhomie-0.2.0/enhomie.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      521 2024-04-08 04:22:21.000000 enhomie-0.2.0/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-14 14:15:36.000000 enhomie-0.2.0/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-15 08:50:05.823818 enhomie-0.2.0/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.343197 enhomie-0.2.1/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-14 23:33:41.000000 enhomie-0.2.1/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       31 2024-03-14 23:35:40.000000 enhomie-0.2.1/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3949 2024-04-25 01:50:11.343197 enhomie-0.2.1/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3560 2024-04-15 08:45:40.000000 enhomie-0.2.1/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.341197 enhomie-0.2.1/enhomie/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.341197 enhomie-0.2.1/enhomie/builtins/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      423 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/builtins/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1644 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/builtins/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.341197 enhomie-0.2.1/enhomie/builtins/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/builtins/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      948 2024-04-25 01:47:19.000000 enhomie-0.2.1/enhomie/builtins/test/test_params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1277 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/builtins/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1778 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/builtins/when.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.341197 enhomie-0.2.1/enhomie/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2024 2024-04-08 05:15:33.000000 enhomie-0.2.1/enhomie/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2183 2024-04-23 07:21:16.000000 enhomie-0.2.1/enhomie/config/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.342197 enhomie-0.2.1/enhomie/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1205 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6000 2024-04-23 07:21:16.000000 enhomie-0.2.1/enhomie/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.342197 enhomie-0.2.1/enhomie/homie/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/homie/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6728 2024-04-25 01:47:19.000000 enhomie-0.2.1/enhomie/homie/desire.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5409 2024-04-08 06:47:33.000000 enhomie-0.2.1/enhomie/homie/group.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    15456 2024-04-24 23:58:04.000000 enhomie-0.2.1/enhomie/homie/homie.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3425 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/homie/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6012 2024-04-15 08:01:26.000000 enhomie-0.2.1/enhomie/homie/scene.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.342197 enhomie-0.2.1/enhomie/homie/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/homie/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2633 2024-04-15 08:22:12.000000 enhomie-0.2.1/enhomie/homie/test/test_desire.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2184 2024-04-15 08:22:39.000000 enhomie-0.2.1/enhomie/homie/test/test_group.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4354 2024-04-15 08:23:16.000000 enhomie-0.2.1/enhomie/homie/test/test_homie.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2587 2024-04-15 08:23:41.000000 enhomie-0.2.1/enhomie/homie/test/test_scene.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1303 2024-04-15 08:24:01.000000 enhomie-0.2.1/enhomie/homie/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3251 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/homie/when.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.342197 enhomie-0.2.1/enhomie/philipshue/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:09.000000 enhomie-0.2.1/enhomie/philipshue/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10528 2024-04-25 01:47:19.000000 enhomie-0.2.1/enhomie/philipshue/bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8007 2024-04-08 04:48:39.000000 enhomie-0.2.1/enhomie/philipshue/device.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1826 2024-04-14 14:22:48.000000 enhomie-0.2.1/enhomie/philipshue/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.342197 enhomie-0.2.1/enhomie/philipshue/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      635 2024-04-08 05:44:56.000000 enhomie-0.2.1/enhomie/philipshue/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5062 2024-04-25 01:47:19.000000 enhomie-0.2.1/enhomie/philipshue/test/test_bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3131 2024-04-15 08:24:45.000000 enhomie-0.2.1/enhomie/philipshue/test/test_device.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3263 2024-04-08 04:36:12.000000 enhomie-0.2.1/enhomie/philipshue/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2126 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/philipshue/when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-24 11:17:04.000000 enhomie-0.2.1/enhomie/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.343197 enhomie-0.2.1/enhomie/ubiquiti/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      582 2024-04-14 14:24:29.000000 enhomie-0.2.1/enhomie/ubiquiti/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7558 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/ubiquiti/client.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1991 2024-04-14 14:21:10.000000 enhomie-0.2.1/enhomie/ubiquiti/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9316 2024-04-25 01:47:19.000000 enhomie-0.2.1/enhomie/ubiquiti/router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.343197 enhomie-0.2.1/enhomie/ubiquiti/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/ubiquiti/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4146 2024-04-15 08:25:06.000000 enhomie-0.2.1/enhomie/ubiquiti/test/test_client.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3494 2024-04-25 01:47:19.000000 enhomie-0.2.1/enhomie/ubiquiti/test/test_router.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2643 2024-04-08 04:36:08.000000 enhomie-0.2.1/enhomie/ubiquiti/test/test_when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2148 2024-04-08 04:21:22.000000 enhomie-0.2.1/enhomie/ubiquiti/when.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-25 01:47:44.000000 enhomie-0.2.1/enhomie/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 01:50:11.343197 enhomie-0.2.1/enhomie.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3949 2024-04-25 01:50:11.000000 enhomie-0.2.1/enhomie.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1568 2024-04-25 01:50:11.000000 enhomie-0.2.1/enhomie.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-25 01:50:11.000000 enhomie-0.2.1/enhomie.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-25 01:50:11.000000 enhomie-0.2.1/enhomie.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        8 2024-04-25 01:50:11.000000 enhomie-0.2.1/enhomie.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      521 2024-04-08 04:22:21.000000 enhomie-0.2.1/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       19 2024-04-14 14:15:36.000000 enhomie-0.2.1/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-25 01:50:11.343197 enhomie-0.2.1/setup.cfg
```

### Comparing `enhomie-0.2.0/LICENSE` & `enhomie-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/PKG-INFO` & `enhomie-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhomie
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enasis Network Homie Automate
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `enhomie-0.2.0/README.md` & `enhomie-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/__init__.py` & `enhomie-0.2.1/enhomie/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/builtins/params.py` & `enhomie-0.2.1/enhomie/builtins/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/builtins/test/test_params.py` & `enhomie-0.2.1/enhomie/builtins/test/test_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
     anchor = Times('now')
 
 
     start = anchor.shift('-1h@s')
     stop = anchor.shift('+1h@s')
 
-    when = WhenTimePeriodParams(
+    params = WhenTimePeriodParams(
         start=start,
         stop=stop)
 
-    assert when.start and when.stop
+    assert params.start and params.stop
 
-    assert when.start == start
-    assert when.stop == stop
+    assert params.start == start
+    assert params.stop == stop
 
 
     start = anchor.shift('-1h@s')
     stop = anchor.shift('-2h@s')
 
-    when = WhenTimePeriodParams(
+    params = WhenTimePeriodParams(
         start=start,
         stop=stop)
 
-    assert when.start and when.stop
+    assert params.start and params.stop
 
-    assert when.start == start
-    assert when.stop >= start
+    assert params.start == start
+    assert params.stop >= start
```

### Comparing `enhomie-0.2.0/enhomie/builtins/test/test_when.py` & `enhomie-0.2.1/enhomie/builtins/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/builtins/when.py` & `enhomie-0.2.1/enhomie/builtins/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/config/config.py` & `enhomie-0.2.1/enhomie/config/config.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/config/params.py` & `enhomie-0.2.1/enhomie/config/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 _UBIQ_ROUTERS = dict[str, UbiqRouterParams]
 _UBIQ_CLIENTS = dict[str, UbiqClientParams]
 
 
 
 class Params(_Params, extra='forbid'):
     """
-    Process and validate the Homie configuration parameters.
+    Process and validate the core configuration parameters.
 
     .. note::
        These parameters are in addition to those found in
        :class:`encommon.config.Params`.
 
     :param groups: Dictionary of parameters for the groups.
     :param scenes: Dictionary of parameters for the scenes.
```

### Comparing `enhomie-0.2.0/enhomie/config/test/test_config.py` & `enhomie-0.2.1/enhomie/config/test/test_config.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/conftest.py` & `enhomie-0.2.1/enhomie/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 
 from pytest import fixture
 
 from requests_mock import Mocker
 
 from .config import Config
 from .homie import Homie
-from .homie.test import SAMPLES as CORE_SAMPLES
-from .philipshue.test import SAMPLES as PHUE_SAMPLES
-from .ubiquiti.test import SAMPLES as UBIQ_SAMPLES
+from .homie.test import (
+    SAMPLES as CORE_SAMPLES)
+from .philipshue.test import (
+    SAMPLES as PHUE_SAMPLES)
+from .ubiquiti.test import (
+    SAMPLES as UBIQ_SAMPLES)
 
 
 
 _ANCHOR = Times('-0s@s')
 
 REPLACES = {
 
@@ -130,15 +133,15 @@
        Function has slowly evolved and grown over time, but
        should be refactored and simplified in the future.
 
     :param config: Primary class instance for configuration.
     :returns: Newly constructed instance of related class.
     """
 
-    homie = Homie(config=config)
+    homie = Homie(config)
 
     bridges = homie.phue_bridges
     routers = homie.ubiq_routers
 
 
     phue_paths = [
         ('https://192.168.1.10'
```

### Comparing `enhomie-0.2.0/enhomie/homie/__init__.py` & `enhomie-0.2.1/enhomie/homie/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/desire.py` & `enhomie-0.2.1/enhomie/homie/desire.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 
 from typing import Any
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from encommon.times import Times
+from encommon.times import TimerParams
 
 from .when import HomieWhen
 
 if TYPE_CHECKING:
     from .homie import Homie
     from .params import HomieDesireParams
     from .params import HomieWhenParams
@@ -232,22 +232,27 @@
 
         :returns: Boolean indicating whether desire is delayed.
         """
 
         homie = self.homie
         timers = homie.timers['desire']
 
+        children = timers.children
+
         unique = self.name
         delay = self.delay
 
-        started = Times() - delay
+        if unique not in children:
+
+            params = TimerParams(
+                timer=delay,
+                start=f'-{delay}s')
 
-        if unique not in timers.timers:
             timers.create(
-                unique, delay, started)
+                unique, params)
 
         return not timers.ready(
             unique, update=False)
 
 
     def update_timer(
         self,
```

### Comparing `enhomie-0.2.0/enhomie/homie/group.py` & `enhomie-0.2.1/enhomie/homie/group.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/homie.py` & `enhomie-0.2.1/enhomie/homie/homie.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/params.py` & `enhomie-0.2.1/enhomie/homie/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/scene.py` & `enhomie-0.2.1/enhomie/homie/scene.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/test/test_desire.py` & `enhomie-0.2.1/enhomie/homie/test/test_desire.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/test/test_group.py` & `enhomie-0.2.1/enhomie/homie/test/test_group.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/test/test_homie.py` & `enhomie-0.2.1/enhomie/homie/test/test_homie.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/test/test_scene.py` & `enhomie-0.2.1/enhomie/homie/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/test/test_when.py` & `enhomie-0.2.1/enhomie/homie/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/homie/when.py` & `enhomie-0.2.1/enhomie/homie/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/__init__.py` & `enhomie-0.2.1/enhomie/philipshue/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/bridge.py` & `enhomie-0.2.1/enhomie/philipshue/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 from copy import deepcopy
 from typing import Any
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from encommon.times import Timers
+from encommon.times import Timer
 from encommon.times import Times
 from encommon.types import striplower
 
 from enconnect.philipshue import Bridge
 from enconnect.philipshue import BridgeParams
 
 if TYPE_CHECKING:
@@ -40,15 +40,15 @@
     __homie: 'Homie'
     __params: BridgeParams
     __bridge: Bridge
 
     __name: str
 
     __fetched: Optional[_FETCH]
-    __timers: Timers
+    __timer: Timer
     __merged: Optional[_RAWDEV]
 
 
     def __init__(
         self,
         homie: 'Homie',
         name: str,
@@ -74,22 +74,20 @@
 
 
         self.__homie = homie
         self.__params = params
         self.__bridge = Bridge(params)
         self.__name = name
         self.__fetched = None
-        self.__timers = Timers()
         self.__merged = None
 
 
-        self.__timers.create(
-            unique='fetch',
-            minimum=60,
-            started='-60s')
+        self.__timer = Timer(
+            timer=60,
+            start='-60s')
 
 
         homie.log_d(
             base='philipshue',
             item='PhueBridge',
             name=name,
             status='created')
@@ -167,19 +165,19 @@
         """
         Collect the complete dump of all resources within bridge.
 
         :returns: Complete dump of all resources within bridge.
         """
 
         fetched = self.__fetched
-        timers = self.__timers
+        timer = self.__timer
         bridge = self.__bridge
         request = bridge.request
 
-        ready = timers.ready('fetch')
+        ready = timer.ready(False)
 
         if fetched and not ready:
             return deepcopy(fetched)
 
         runtime = Times()
 
 
@@ -201,15 +199,15 @@
             elapsed=runtime.since,
             status='success')
 
 
         self.__fetched = fetched
         self.__merged = None
 
-        timers.update('fetch')
+        timer.update()
 
         return deepcopy(fetched)
 
 
     @property
     def merged(
         self,
```

### Comparing `enhomie-0.2.0/enhomie/philipshue/device.py` & `enhomie-0.2.1/enhomie/philipshue/device.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/params.py` & `enhomie-0.2.1/enhomie/philipshue/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/test/__init__.py` & `enhomie-0.2.1/enhomie/philipshue/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/test/test_bridge.py` & `enhomie-0.2.1/enhomie/philipshue/test/test_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
     assert attrs == [
         '_PhueBridge__homie',
         '_PhueBridge__params',
         '_PhueBridge__bridge',
         '_PhueBridge__name',
         '_PhueBridge__fetched',
-        '_PhueBridge__timers',
-        '_PhueBridge__merged']
+        '_PhueBridge__merged',
+        '_PhueBridge__timer']
 
 
     assert inrepr(
         'bridge.PhueBridge object',
         bridge)
 
     assert hash(bridge) > 0
```

### Comparing `enhomie-0.2.0/enhomie/philipshue/test/test_device.py` & `enhomie-0.2.1/enhomie/philipshue/test/test_device.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/test/test_when.py` & `enhomie-0.2.1/enhomie/philipshue/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/philipshue/when.py` & `enhomie-0.2.1/enhomie/philipshue/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/__init__.py` & `enhomie-0.2.1/enhomie/ubiquiti/__init__.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/client.py` & `enhomie-0.2.1/enhomie/ubiquiti/client.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/params.py` & `enhomie-0.2.1/enhomie/ubiquiti/params.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/router.py` & `enhomie-0.2.1/enhomie/ubiquiti/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from copy import deepcopy
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from encommon.times import Timers
+from encommon.times import Timer
 from encommon.times import Times
 from encommon.types import merge_dicts
 from encommon.types import striplower
 
 from enconnect.ubiquiti import Router
 from enconnect.ubiquiti import RouterParams
 
@@ -50,15 +50,15 @@
     __homie: 'Homie'
     __params: RouterParams
     __router: Router
 
     __name: str
 
     __fetched: Optional[dict[str, _FETCH]]
-    __timers: Timers
+    __timer: Timer
     __merged: Optional[_RAWDEV]
 
 
     def __init__(
         self,
         homie: 'Homie',
         name: str,
@@ -84,22 +84,20 @@
 
 
         self.__homie = homie
         self.__params = params
         self.__router = Router(params)
         self.__name = name
         self.__fetched = None
-        self.__timers = Timers()
         self.__merged = None
 
 
-        self.__timers.create(
-            unique='fetch',
-            minimum=60,
-            started='-60s')
+        self.__timer = Timer(
+            timer=60,
+            start='-60s')
 
 
         homie.log_d(
             base='ubiquiti',
             item='UbiqRouter',
             name=name,
             status='created')
@@ -177,19 +175,19 @@
         """
         Collect the complete dump of all known clients in router.
 
         :returns: Complete dump of all known clients in router.
         """
 
         fetched = self.__fetched
-        timers = self.__timers
+        timer = self.__timer
         router = self.__router
         request = router.request_proxy
 
-        ready = timers.ready('fetch')
+        ready = timer.ready(False)
 
         if fetched and not ready:
             return deepcopy(fetched)
 
         runtime = Times()
 
 
@@ -222,15 +220,15 @@
             elapsed=runtime.since,
             status='success')
 
 
         self.__fetched = fetched
         self.__merged = None
 
-        timers.update('fetch')
+        timer.update()
 
         return deepcopy(fetched)
 
 
     @property
     def merged(
         self,
```

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/test/test_client.py` & `enhomie-0.2.1/enhomie/ubiquiti/test/test_client.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/test/test_router.py` & `enhomie-0.2.1/enhomie/ubiquiti/test/test_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
     assert attrs == [
         '_UbiqRouter__homie',
         '_UbiqRouter__params',
         '_UbiqRouter__router',
         '_UbiqRouter__name',
         '_UbiqRouter__fetched',
-        '_UbiqRouter__timers',
-        '_UbiqRouter__merged']
+        '_UbiqRouter__merged',
+        '_UbiqRouter__timer']
 
 
     assert inrepr(
         'router.UbiqRouter object',
         router)
 
     assert hash(router) > 0
```

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/test/test_when.py` & `enhomie-0.2.1/enhomie/ubiquiti/test/test_when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie/ubiquiti/when.py` & `enhomie-0.2.1/enhomie/ubiquiti/when.py`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/enhomie.egg-info/PKG-INFO` & `enhomie-0.2.1/enhomie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhomie
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enasis Network Homie Automate
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `enhomie-0.2.0/enhomie.egg-info/SOURCES.txt` & `enhomie-0.2.1/enhomie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enhomie-0.2.0/pyproject.toml` & `enhomie-0.2.1/pyproject.toml`

 * *Files identical despite different names*


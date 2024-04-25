# Comparing `tmp/anycluster-2.4.8.tar.gz` & `tmp/anycluster-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.4.8.tar", last modified: Tue Apr  2 07:55:16 2024, max compression
+gzip compressed data, was "anycluster-2.4.9.tar", last modified: Thu Apr 25 08:01:44 2024, max compression
```

## Comparing `anycluster-2.4.8.tar` & `anycluster-2.4.9.tar`

### file list

```diff
@@ -1,71 +1,54 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.064952 anycluster-2.4.8/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.4.8/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.4.8/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-04-02 07:55:16.064952 anycluster-2.4.8/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.4.8/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.058285 anycluster-2.4.8/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.4.8/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7237 2023-10-17 06:13:56.000000 anycluster-2.4.8/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    41911 2024-04-02 07:54:54.000000 anycluster-2.4.8/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.4.8/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.4.8/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.058285 anycluster-2.4.8/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.058285 anycluster-2.4.8/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.4.8/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.4.8/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     4742 2023-12-06 06:46:23.000000 anycluster-2.4.8/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.4.8/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     8261 2023-12-13 07:45:44.000000 anycluster-2.4.8/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.4.8/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5322 2023-12-06 06:43:43.000000 anycluster-2.4.8/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.058285 anycluster-2.4.8/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.058285 anycluster-2.4.8/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.4.8/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2829 2023-06-13 06:32:28.000000 anycluster-2.4.8/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10311 2023-10-17 05:32:11.000000 anycluster-2.4.8/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.4.8/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15654 2023-10-17 05:32:09.000000 anycluster-2.4.8/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.4.8/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10418 2023-12-13 07:45:43.000000 anycluster-2.4.8/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.4.8/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-10-20 10:21:42.000000 anycluster-2.4.8/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.054952 anycluster-2.4.8/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.054952 anycluster-2.4.8/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.061618 anycluster-2.4.8/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.4.8/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.061618 anycluster-2.4.8/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.064952 anycluster-2.4.8/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1576 2023-10-16 11:03:00.000000 anycluster-2.4.8/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2972 2023-10-16 11:00:34.000000 anycluster-2.4.8/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.4.8/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     6082 2023-10-16 10:29:53.000000 anycluster-2.4.8/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.4.8/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    18469 2023-10-20 14:21:34.000000 anycluster-2.4.8/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2901 2023-10-16 11:02:25.000000 anycluster-2.4.8/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2412 2023-10-16 11:00:30.000000 anycluster-2.4.8/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.4.8/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9985 2023-10-16 10:29:51.000000 anycluster-2.4.8/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    32345 2023-10-20 14:21:31.000000 anycluster-2.4.8/anycluster/tests/test_MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.4.8/anycluster/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-02 07:55:16.064952 anycluster-2.4.8/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-04-02 07:55:16.000000 anycluster-2.4.8/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2211 2024-04-02 07:55:16.000000 anycluster-2.4.8/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-02 07:55:16.000000 anycluster-2.4.8/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-04-02 07:55:16.000000 anycluster-2.4.8/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2024-04-02 07:55:16.000000 anycluster-2.4.8/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-02 07:55:16.064952 anycluster-2.4.8/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2024-04-02 07:53:46.000000 anycluster-2.4.8/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.4.9/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.4.9/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-04-25 08:01:44.769286 anycluster-2.4.9/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.4.9/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.765953 anycluster-2.4.9/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.4.9/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7237 2023-10-17 06:13:56.000000 anycluster-2.4.9/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    41927 2024-04-25 07:18:05.000000 anycluster-2.4.9/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.4.9/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.4.9/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/api/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.4.9/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5396 2024-04-25 07:14:35.000000 anycluster-2.4.9/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/api/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.4.9/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    15654 2023-10-17 05:32:09.000000 anycluster-2.4.9/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.4.9/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10705 2024-04-25 07:52:20.000000 anycluster-2.4.9/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.4.9/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-10-20 10:21:42.000000 anycluster-2.4.9/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.765953 anycluster-2.4.9/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.765953 anycluster-2.4.9/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2901 2023-10-16 11:02:25.000000 anycluster-2.4.9/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2412 2023-10-16 11:00:30.000000 anycluster-2.4.9/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.4.9/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9985 2023-10-16 10:29:51.000000 anycluster-2.4.9/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    32345 2023-10-20 14:21:31.000000 anycluster-2.4.9/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.4.9/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1421 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-25 08:01:44.769286 anycluster-2.4.9/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2024-04-25 07:57:46.000000 anycluster-2.4.9/setup.py
```

### Comparing `anycluster-2.4.8/LICENSE` & `anycluster-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/PKG-INFO` & `anycluster-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.4.8
+Version: 2.4.9
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.4.8/README.md` & `anycluster-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/ClusterCache.py` & `anycluster-2.4.9/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/FilterComposer.py` & `anycluster-2.4.9/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/MapClusterer.py` & `anycluster-2.4.9/anycluster/MapClusterer.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
 
         cluster.transform(self.db_srid)
 
         query_geometry = None
         k = BASE_K
 
         if not self.cluster_cache.geometries:
-            raise ValueError('No cached geometries found')
+            raise ValueError('[MapClusterer]: No cached geometries found')
 
 
         for geometry in self.cluster_cache.geometries:
 
             geos = GEOSGeometry(geometry)
             # cached geometries are always srid==self.db_srid
             # bug: geos.srid is set to 4326 here, which is wrong
```

### Comparing `anycluster-2.4.8/anycluster/MapTools.py` & `anycluster-2.4.9/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/api/json_schemas.py` & `anycluster-2.4.9/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/api/serializers.py` & `anycluster-2.4.9/anycluster/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,19 +129,21 @@
 
 class ClusterContentRequestSerializer(serializers.Serializer):
 
     output_srid = serializers.CharField(default='EPSG:4326', required=False, write_only=True)
     input_srid = serializers.CharField(default='EPSG:4326', required=False, write_only=True)
 
     geometry_type = serializers.ChoiceField(choices=GEOMETRY_TYPES, write_only=True)
+    geojson = serializers.JSONField(write_only=True, required=False)
+    filters = serializers.ListField(required=False, default=[], write_only=True)
 
     ids = serializers.ListField(child=serializers.IntegerField(), write_only=True)
     x = serializers.FloatField(write_only=True)
     y = serializers.FloatField(write_only=True)
-    filters = serializers.ListField(required=False, default=[], write_only=True)
+    
 
     def validate_filters(self, value):
         filters_are_allowed(value)
         return value
```

### Comparing `anycluster-2.4.8/anycluster/api/tests/test_serializers.py` & `anycluster-2.4.9/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/api/tests/test_views.py` & `anycluster-2.4.9/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/api/urls.py` & `anycluster-2.4.9/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/api/views.py` & `anycluster-2.4.9/anycluster/api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,21 @@
 
     def post(self, request, *args, **kwargs):
 
         serializer = ClusterContentRequestSerializer(data=request.data)
 
         if serializer.is_valid():
 
+            # awlays use tha latest cache
+            cache = request.session.get(self.cache_name, {})
+            cached_geometries = cache.get('geometries', [])
+
+            if not cached_geometries:
+                raise ValueError('[GetClusterContent]: No cached geometries found')
+
             geometry_type = serializer.validated_data['geometry_type']
             output_srid = self.parse_srid(serializer.validated_data['output_srid'])
             input_srid = self.parse_srid(serializer.validated_data['input_srid'])
 
             filters = serializer.validated_data['filters']
 
             map_clusterer = self.get_map_clusterer(geometry_type, CLUSTER_TYPE_KMEANS, filters, False, output_srid,
```

### Comparing `anycluster-2.4.8/anycluster/clusters.py` & `anycluster-2.4.9/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/definitions.py` & `anycluster-2.4.9/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/globalmaptiles.py` & `anycluster-2.4.9/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/10.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/100.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/1000.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/10000.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/5.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/50.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.4.9/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/tests/common.py` & `anycluster-2.4.9/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/tests/mixins.py` & `anycluster-2.4.9/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/tests/test_ClusterCache.py` & `anycluster-2.4.9/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/tests/test_FilterComposer.py` & `anycluster-2.4.9/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster/tests/test_MapClusterer.py` & `anycluster-2.4.9/anycluster/tests/test_MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.8/anycluster.egg-info/PKG-INFO` & `anycluster-2.4.9/anycluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.4.8
+Version: 2.4.9
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.4.8/anycluster.egg-info/SOURCES.txt` & `anycluster-2.4.9/anycluster.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -17,24 +17,16 @@
 anycluster.egg-info/dependency_links.txt
 anycluster.egg-info/requires.txt
 anycluster.egg-info/top_level.txt
 anycluster/api/json_schemas.py
 anycluster/api/serializers.py
 anycluster/api/urls.py
 anycluster/api/views.py
-anycluster/api/__pycache__/json_schemas.cpython-38.pyc
-anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
-anycluster/api/__pycache__/serializers.cpython-38.pyc
-anycluster/api/__pycache__/urls.cpython-38.pyc
-anycluster/api/__pycache__/views.cpython-38.pyc
 anycluster/api/tests/test_serializers.py
 anycluster/api/tests/test_views.py
-anycluster/api/tests/__pycache__/common.cpython-38.pyc
-anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
-anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
 anycluster/static/anycluster/images/10.png
 anycluster/static/anycluster/images/100.png
 anycluster/static/anycluster/images/1000.png
 anycluster/static/anycluster/images/10000.png
 anycluster/static/anycluster/images/10000_empty.png
 anycluster/static/anycluster/images/1000_empty.png
 anycluster/static/anycluster/images/100_empty.png
@@ -44,14 +36,8 @@
 anycluster/static/anycluster/images/50_empty.png
 anycluster/static/anycluster/images/5_empty.png
 anycluster/static/anycluster/images/pin_unknown.png
 anycluster/tests/common.py
 anycluster/tests/mixins.py
 anycluster/tests/test_ClusterCache.py
 anycluster/tests/test_FilterComposer.py
-anycluster/tests/test_MapClusterer.py
-anycluster/tests/__pycache__/common.cpython-38.pyc
-anycluster/tests/__pycache__/mixins.cpython-38.pyc
-anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
-anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
-anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
-anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+anycluster/tests/test_MapClusterer.py
```

### Comparing `anycluster-2.4.8/setup.py` & `anycluster-2.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.4.8',
+    version='2.4.9',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```


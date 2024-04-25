# Comparing `tmp/simpleworkspace-1.2.190.tar.gz` & `tmp/simpleworkspace-1.2.192.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.190.tar", last modified: Mon Apr 22 19:25:24 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.192.tar", last modified: Thu Apr 25 17:05:44 2024, max compression
```

## Comparing `simpleworkspace-1.2.190.tar` & `simpleworkspace-1.2.192.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:24.051120 simpleworkspace-1.2.190/
--rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.190/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-04-22 19:25:24.047629 simpleworkspace-1.2.190/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-04-22 19:22:31.000000 simpleworkspace-1.2.190/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 19:25:24.053615 simpleworkspace-1.2.190/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.586462 simpleworkspace-1.2.190/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.664265 simpleworkspace-1.2.190/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.190/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.190/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.190/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.730654 simpleworkspace-1.2.190/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.745669 simpleworkspace-1.2.190/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.593381 simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.747559 simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.804063 simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.831164 simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.844616 simpleworkspace-1.2.190/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.190/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.854995 simpleworkspace-1.2.190/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.190/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.190/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.190/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.866355 simpleworkspace-1.2.190/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.190/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.190/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.887330 simpleworkspace-1.2.190/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/__init__.py
--rw-rw-rw-   0        0        0     9009 2024-02-25 18:43:27.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/archive.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.899040 simpleworkspace-1.2.190/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2962 2024-02-07 20:22:40.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      705 2024-02-23 06:39:35.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6058 2024-02-21 21:38:25.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.914377 simpleworkspace-1.2.190/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      321 2023-12-11 19:38:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.190/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.190/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.190/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.632554 simpleworkspace-1.2.190/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.918359 simpleworkspace-1.2.190/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.619927 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.622172 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.923873 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.930115 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.934212 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.938227 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.959166 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.970285 simpleworkspace-1.2.190/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.190/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.190/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:23.996589 simpleworkspace-1.2.190/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.190/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:24.033888 simpleworkspace-1.2.190/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14495 2024-02-14 19:32:38.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-03-18 16:44:18.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1865 2024-02-07 19:12:33.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.190/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:25:24.033888 simpleworkspace-1.2.190/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-04-22 19:25:23.000000 simpleworkspace-1.2.190/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3464 2024-04-22 19:25:23.000000 simpleworkspace-1.2.190/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 19:25:23.000000 simpleworkspace-1.2.190/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 19:25:23.000000 simpleworkspace-1.2.190/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-22 19:25:23.000000 simpleworkspace-1.2.190/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:44.150591 simpleworkspace-1.2.192/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.192/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-04-25 17:05:44.150591 simpleworkspace-1.2.192/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-25 17:01:21.000000 simpleworkspace-1.2.192/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 17:05:44.150591 simpleworkspace-1.2.192/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.365047 simpleworkspace-1.2.192/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.569539 simpleworkspace-1.2.192/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.192/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.192/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.192/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.727347 simpleworkspace-1.2.192/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.727347 simpleworkspace-1.2.192/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.371973 simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.759016 simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.853190 simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.884461 simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.931818 simpleworkspace-1.2.192/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.192/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.121001 simpleworkspace-1.2.192/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.192/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.192/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.192/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.152475 simpleworkspace-1.2.192/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.192/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.192/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.372470 simpleworkspace-1.2.192/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/__init__.py
+-rw-rw-rw-   0        0        0     9009 2024-02-25 18:43:27.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/archive.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.514191 simpleworkspace-1.2.192/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2962 2024-02-07 20:22:40.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      705 2024-02-23 06:39:35.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6058 2024-02-21 21:38:25.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.577369 simpleworkspace-1.2.192/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      321 2023-12-11 19:38:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.192/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.192/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.192/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.459684 simpleworkspace-1.2.192/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.593012 simpleworkspace-1.2.192/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.391687 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:42.392838 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.624261 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.649402 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.671939 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.671939 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.813329 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.828956 simpleworkspace-1.2.192/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.192/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.192/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:43.955029 simpleworkspace-1.2.192/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.192/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:44.145549 simpleworkspace-1.2.192/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-04-25 16:08:18.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1865 2024-02-07 19:12:33.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.192/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:05:44.147558 simpleworkspace-1.2.192/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-04-25 17:05:42.000000 simpleworkspace-1.2.192/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3464 2024-04-25 17:05:42.000000 simpleworkspace-1.2.192/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 17:05:42.000000 simpleworkspace-1.2.192/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 17:05:42.000000 simpleworkspace-1.2.192/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 17:05:42.000000 simpleworkspace-1.2.192/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/app.py` & `simpleworkspace-1.2.192/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.192/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.192/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.192/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.192/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.192/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/archive.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.192/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.192/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.192/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.192/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.192/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.192/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.192/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.192/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.192/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.192/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/linq.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             return sum(1 for _ in self)
 
         return sum(1 for item in self if predicate(item))
    
     def Sorted(self, descending: bool = False):
         return LINQ(sorted(self, reverse=descending))
    
-    def Batch(self, chunkSize: int = None, totalChunks:int = None):
+    def Batch(self, chunkSize:int|None = None, totalChunks:int|None = None):
         """
         Batches the elements of the iterable into chunks of the specified size. 
         
         Two variant of batching are supported, only one can be choosen (PS. desired chunk dimensions might be smaller if the iterable has fewer items)
         * predetermined chunkSize
         * predetermined totalChunks
```

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.192/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.190/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.192/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*


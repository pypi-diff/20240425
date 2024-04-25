# Comparing `tmp/esanalyzer-1.0.0.tar.gz` & `tmp/esanalyzer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanalyzer-1.0.0.tar", last modified: Thu Apr 25 14:18:08 2024, max compression
+gzip compressed data, was "esanalyzer-1.0.2.tar", last modified: Thu Apr 25 15:19:47 2024, max compression
```

## Comparing `esanalyzer-1.0.0.tar` & `esanalyzer-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:18:08.090206 esanalyzer-1.0.0/
--rw-rw-rw-   0        0        0     1074 2024-04-25 11:23:48.000000 esanalyzer-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      383 2024-04-25 14:18:08.088228 esanalyzer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      494 2024-04-25 14:16:26.000000 esanalyzer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 14:18:08.062071 esanalyzer-1.0.0/esanalyzer/
-drwxrwxrwx   0        0        0        0 2024-04-25 14:18:08.082244 esanalyzer-1.0.0/esanalyzer/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 14:18:08.086232 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.egg-info/
--rw-rw-rw-   0        0        0      383 2024-04-25 14:18:07.000000 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-25 14:18:07.000000 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:18:07.000000 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-04-25 14:18:07.000000 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 14:18:07.000000 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23767 2024-04-25 13:08:05.000000 esanalyzer-1.0.0/esanalyzer/src/esanalyzer.py
--rw-rw-rw-   0        0        0       42 2024-04-25 14:18:08.090206 esanalyzer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      591 2024-04-25 14:14:53.000000 esanalyzer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.310021 esanalyzer-1.0.2/
+-rw-rw-rw-   0        0        0     1074 2024-04-25 11:23:48.000000 esanalyzer-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1071 2024-04-25 15:19:47.308247 esanalyzer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2024-04-25 14:16:26.000000 esanalyzer-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.283762 esanalyzer-1.0.2/esanalyzer/
+drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.301264 esanalyzer-1.0.2/esanalyzer/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 15:19:47.306250 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     1071 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 15:19:47.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23767 2024-04-25 13:08:05.000000 esanalyzer-1.0.2/esanalyzer/src/esanalyzer.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:19:47.310021 esanalyzer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2024-04-25 15:18:54.000000 esanalyzer-1.0.2/setup.py
```

### Comparing `esanalyzer-1.0.0/LICENSE` & `esanalyzer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esanalyzer-1.0.0/esanalyzer/src/esanalyzer.py` & `esanalyzer-1.0.2/esanalyzer/src/esanalyzer.py`

 * *Files identical despite different names*


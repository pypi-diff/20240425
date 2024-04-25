# Comparing `tmp/temalib-3.5.tar.gz` & `tmp/temalib-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temalib-3.5.tar", last modified: Fri Apr 19 17:13:35 2024, max compression
+gzip compressed data, was "temalib-3.6.tar", last modified: Thu Apr 25 12:57:32 2024, max compression
```

## Comparing `temalib-3.5.tar` & `temalib-3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 17:13:35.424825 temalib-3.5/
--rw-rw-rw-   0        0        0     1833 2024-04-19 17:12:43.000000 temalib-3.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2024-01-25 13:27:43.000000 temalib-3.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 temalib-3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      600 2024-04-19 17:13:35.424825 temalib-3.5/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-01-25 13:23:18.000000 temalib-3.5/README.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 17:13:35.424825 temalib-3.5/setup.cfg
--rw-rw-rw-   0        0        0      697 2024-04-19 17:12:57.000000 temalib-3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:13:35.414803 temalib-3.5/temalib/
--rw-rw-rw-   0        0        0     7407 2024-04-19 17:12:23.000000 temalib-3.5/temalib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 17:13:35.422831 temalib-3.5/temalib.egg-info/
--rw-rw-rw-   0        0        0      600 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 12:57:32.166325 temalib-3.6/
+-rw-rw-rw-   0        0        0     1833 2024-04-19 17:12:43.000000 temalib-3.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2024-01-25 13:27:43.000000 temalib-3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 temalib-3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1510 2024-04-25 12:57:32.165327 temalib-3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-01-25 13:23:18.000000 temalib-3.6/README.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:57:32.166325 temalib-3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1683 2024-04-25 12:57:27.000000 temalib-3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:57:32.140781 temalib-3.6/temalib/
+-rw-rw-rw-   0        0        0     5106 2024-04-25 12:40:22.000000 temalib-3.6/temalib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:57:32.162797 temalib-3.6/temalib.egg-info/
+-rw-rw-rw-   0        0        0     1510 2024-04-25 12:57:32.000000 temalib-3.6/temalib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-04-25 12:57:32.000000 temalib-3.6/temalib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:57:32.000000 temalib-3.6/temalib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 12:57:32.000000 temalib-3.6/temalib.egg-info/top_level.txt
```

### Comparing `temalib-3.5/CHANGELOG.txt` & `temalib-3.6/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `temalib-3.5/LICENSE.txt` & `temalib-3.6/LICENSE.txt`

 * *Files identical despite different names*


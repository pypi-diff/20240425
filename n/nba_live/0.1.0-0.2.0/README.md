# Comparing `tmp/nba_live-0.1.0.tar.gz` & `tmp/nba_live-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nba_live-0.1.0.tar", max compression
+gzip compressed data, was "nba_live-0.2.0.tar", max compression
```

## Comparing `nba_live-0.1.0.tar` & `nba_live-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-25 20:54:23.164284 nba_live-0.1.0/nba_live/__init__.py
--rw-r--r--   0        0        0     1481 2024-04-25 20:35:50.718741 nba_live-0.1.0/nba_live/datastream.py
--rw-r--r--   0        0        0      983 2024-04-25 19:58:25.047561 nba_live-0.1.0/nba_live/getboxscore.py
--rw-r--r--   0        0        0     1236 2024-04-25 19:24:29.273126 nba_live-0.1.0/nba_live/getgamedata.py
--rw-r--r--   0        0        0      989 2024-04-25 20:12:01.902503 nba_live-0.1.0/nba_live/nbalive.py
--rw-r--r--   0        0        0      515 2024-04-25 21:03:58.606943 nba_live-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      109 2024-04-25 20:56:32.770220 nba_live-0.1.0/README.md
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 nba_live-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 20:54:23.164284 nba_live-0.2.0/nba_live/__init__.py
+-rw-r--r--   0        0        0     1481 2024-04-25 20:35:50.718741 nba_live-0.2.0/nba_live/datastream.py
+-rw-r--r--   0        0        0      983 2024-04-25 19:58:25.047561 nba_live-0.2.0/nba_live/getboxscore.py
+-rw-r--r--   0        0        0     1236 2024-04-25 19:24:29.273126 nba_live-0.2.0/nba_live/getgamedata.py
+-rw-r--r--   0        0        0      989 2024-04-25 20:12:01.902503 nba_live-0.2.0/nba_live/nbalive.py
+-rw-r--r--   0        0        0      515 2024-04-25 21:15:40.372045 nba_live-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-04-25 20:56:32.770220 nba_live-0.2.0/README.md
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 nba_live-0.2.0/PKG-INFO
```

### Comparing `nba_live-0.1.0/nba_live/datastream.py` & `nba_live-0.2.0/nba_live/datastream.py`

 * *Files identical despite different names*

### Comparing `nba_live-0.1.0/nba_live/getboxscore.py` & `nba_live-0.2.0/nba_live/getboxscore.py`

 * *Files identical despite different names*

### Comparing `nba_live-0.1.0/nba_live/getgamedata.py` & `nba_live-0.2.0/nba_live/getgamedata.py`

 * *Files identical despite different names*

### Comparing `nba_live-0.1.0/nba_live/nbalive.py` & `nba_live-0.2.0/nba_live/nbalive.py`

 * *Files identical despite different names*

### Comparing `nba_live-0.1.0/pyproject.toml` & `nba_live-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "nba-live"
-version = "0.1.0"
+name = "nba_live"
+version = "0.2.0"
 description = "This package allows a user to easily grab data from the live endpoints in the nba_api package"
 authors = ["Donnie Leornas <Donnieleo22@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nba_live"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `nba_live-0.1.0/PKG-INFO` & `nba_live-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nba-live
-Version: 0.1.0
+Name: nba_live
+Version: 0.2.0
 Summary: This package allows a user to easily grab data from the live endpoints in the nba_api package
 Author: Donnie Leornas
 Author-email: Donnieleo22@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nba-api (>=1.4.1,<2.0.0)
```


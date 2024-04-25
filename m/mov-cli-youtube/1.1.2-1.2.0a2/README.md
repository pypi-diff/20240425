# Comparing `tmp/mov-cli-youtube-1.1.2.tar.gz` & `tmp/mov_cli_youtube-1.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-youtube-1.1.2.tar", last modified: Tue Apr  9 23:38:26 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.0a2.tar", last modified: Thu Apr 25 16:24:06 2024, max compression
```

## Comparing `mov-cli-youtube-1.1.2.tar` & `mov_cli_youtube-1.2.0a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:38:26.133646 mov-cli-youtube-1.1.2/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov-cli-youtube-1.1.2/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2956 2024-04-09 23:38:26.133646 mov-cli-youtube-1.1.2/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov-cli-youtube-1.1.2/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:38:26.130312 mov-cli-youtube-1.1.2/mov_cli_youtube/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      329 2024-04-09 22:50:30.000000 mov-cli-youtube-1.1.2/mov_cli_youtube/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2600 2024-04-09 23:37:55.000000 mov-cli-youtube-1.1.2/mov_cli_youtube/youtube.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:38:26.133646 mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2956 2024-04-09 23:38:26.000000 mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      281 2024-04-09 23:38:26.000000 mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:38:26.000000 mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       80 2024-04-09 23:38:26.000000 mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-09 23:38:26.000000 mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1271 2024-04-06 22:28:42.000000 mov-cli-youtube-1.1.2/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:38:26.133646 mov-cli-youtube-1.1.2/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a2/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a2/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/mov_cli_youtube/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      335 2024-04-19 01:30:50.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4456 2024-04-19 00:58:14.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube/youtube.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      281 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-16 20:20:33.000000 mov_cli_youtube-1.2.0a2/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/setup.cfg
```

### Comparing `mov-cli-youtube-1.1.2/LICENSE` & `mov_cli_youtube-1.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-youtube-1.1.2/PKG-INFO` & `mov_cli_youtube-1.2.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.1.2
+Version: 1.2.0a2
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pytube
+Requires-Dist: yt-dlp>=2024.4.9
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-youtube
```

### Comparing `mov-cli-youtube-1.1.2/README.md` & `mov_cli_youtube-1.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `mov-cli-youtube-1.1.2/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.1.2
+Version: 1.2.0a2
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pytube
+Requires-Dist: yt-dlp>=2024.4.9
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-youtube
```

### Comparing `mov-cli-youtube-1.1.2/pyproject.toml` & `mov_cli_youtube-1.2.0a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     'Programming Language :: Python :: 3.10',
 	'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     "requests",
     "importlib-metadata; python_version<'3.8'",
 
-    "pytube"
+    "pytube",
+    "yt-dlp>=2024.4.9"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
```


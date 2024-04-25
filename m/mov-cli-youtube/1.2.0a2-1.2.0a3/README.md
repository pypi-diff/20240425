# Comparing `tmp/mov_cli_youtube-1.2.0a2.tar.gz` & `tmp/mov_cli_youtube-1.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_youtube-1.2.0a2.tar", last modified: Thu Apr 25 16:24:06 2024, max compression
+gzip compressed data, was "mov_cli_youtube-1.2.0a3.tar", last modified: Thu Apr 25 18:01:44 2024, max compression
```

## Comparing `mov_cli_youtube-1.2.0a2.tar` & `mov_cli_youtube-1.2.0a3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a2/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a2/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/mov_cli_youtube/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      335 2024-04-19 01:30:50.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4456 2024-04-19 00:58:14.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube/youtube.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      281 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-25 16:24:06.000000 mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-16 20:20:33.000000 mov_cli_youtube-1.2.0a2/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 16:24:06.211728 mov_cli_youtube-1.2.0a2/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:22:29.000000 mov_cli_youtube-1.2.0a3/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      674 2024-03-21 15:27:20.000000 mov_cli_youtube-1.2.0a3/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/mov_cli_youtube/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      335 2024-04-25 18:01:37.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4403 2024-04-25 18:01:37.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube/youtube.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2990 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      281 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       97 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       16 2024-04-25 18:01:44.000000 mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1295 2024-04-16 20:20:33.000000 mov_cli_youtube-1.2.0a3/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 18:01:44.839696 mov_cli_youtube-1.2.0a3/setup.cfg
```

### Comparing `mov_cli_youtube-1.2.0a2/LICENSE` & `mov_cli_youtube-1.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a2/PKG-INFO` & `mov_cli_youtube-1.2.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.0a2/README.md` & `mov_cli_youtube-1.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli_youtube-1.2.0a2/mov_cli_youtube/youtube.py` & `mov_cli_youtube-1.2.0a3/mov_cli_youtube/youtube.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         super().__init__(config, http_client, options)
 
     def search(self, query: str, limit: Optional[int] = None) -> Generator[Metadata, Any, None]:
         max_videos = 100 if limit is None else limit
 
         yt_options = {
-            "noplaylist":"True", 
+            "noplaylist": "True", 
             "default_search": "ytsearch", 
             "nocheckcertificate": True, 
             "geo_bypass": True, 
             "extract_flat": "in_playlist", 
             "skip_download": True, 
             "quiet": False if self.config.debug else True, 
             "ignoreerrors": True, 
@@ -40,16 +40,15 @@
             info = ydl.extract_info(f"ytsearch{max_videos}:{query}", download = False)
 
             for key in info["entries"]:
 
                 yield Metadata(
                     id = key["url"], 
                     title = f"{key['title']} ~ {key['uploader']}", 
-                    type = MetadataType.SINGLE, 
-                    year = key["release_timestamp"]
+                    type = MetadataType.SINGLE
                 )
 
     def scrape(
         self, 
         metadata: Metadata, 
         _: EpisodeSelector
     ) -> Single:
```

### Comparing `mov_cli_youtube-1.2.0a2/mov_cli_youtube.egg-info/PKG-INFO` & `mov_cli_youtube-1.2.0a3/mov_cli_youtube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-youtube
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: A mov-cli v4 plugin for watching youtube.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov_cli_youtube-1.2.0a2/pyproject.toml` & `mov_cli_youtube-1.2.0a3/pyproject.toml`

 * *Files identical despite different names*


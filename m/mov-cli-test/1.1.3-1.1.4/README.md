# Comparing `tmp/mov-cli-test-1.1.3.tar.gz` & `tmp/mov_cli_test-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-test-1.1.3.tar", last modified: Tue Apr  9 23:33:31 2024, max compression
+gzip compressed data, was "mov_cli_test-1.1.4.tar", last modified: Thu Apr 25 01:49:59 2024, max compression
```

## Comparing `mov-cli-test-1.1.3.tar` & `mov_cli_test-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:33:31.371332 mov-cli-test-1.1.3/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1062 2024-03-02 20:16:40.000000 mov-cli-test-1.1.3/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-09 23:33:31.371332 mov-cli-test-1.1.3/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      532 2024-03-26 18:16:37.000000 mov-cli-test-1.1.3/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:33:31.367998 mov-cli-test-1.1.3/mov_cli_test/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      350 2024-04-09 23:30:30.000000 mov-cli-test-1.1.3/mov_cli_test/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4728 2024-04-09 23:29:47.000000 mov-cli-test-1.1.3/mov_cli_test/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:33:31.367998 mov-cli-test-1.1.3/mov_cli_test.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-09 23:33:31.000000 mov-cli-test-1.1.3/mov_cli_test.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      260 2024-04-09 23:33:31.000000 mov-cli-test-1.1.3/mov_cli_test.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:33:31.000000 mov-cli-test-1.1.3/mov_cli_test.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      114 2024-04-09 23:33:31.000000 mov-cli-test-1.1.3/mov_cli_test.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       13 2024-04-09 23:33:31.000000 mov-cli-test-1.1.3/mov_cli_test.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1395 2024-03-26 17:26:10.000000 mov-cli-test-1.1.3/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:33:31.371332 mov-cli-test-1.1.3/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1062 2024-03-02 20:16:40.000000 mov_cli_test-1.1.4/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      532 2024-03-26 18:16:37.000000 mov_cli_test-1.1.4/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 01:49:59.288010 mov_cli_test-1.1.4/mov_cli_test/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      350 2024-04-25 01:49:27.000000 mov_cli_test-1.1.4/mov_cli_test/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4732 2024-04-25 01:49:23.000000 mov_cli_test-1.1.4/mov_cli_test/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/mov_cli_test.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      260 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      114 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       13 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1395 2024-03-26 17:26:10.000000 mov_cli_test-1.1.4/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/setup.cfg
```

### Comparing `mov-cli-test-1.1.3/LICENSE` & `mov_cli_test-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-test-1.1.3/PKG-INFO` & `mov_cli_test-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.3
+Version: 1.1.4
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-test-1.1.3/README.md` & `mov_cli_test-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mov-cli-test-1.1.3/mov_cli_test/scraper.py` & `mov_cli_test-1.1.4/mov_cli_test/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         for metadata in self.creative_common_films:
 
             # this is basically a poor mans search algorithm.
             if query.lower() in metadata.title.lower():
                 yield metadata # yield the element instead of appending it to a list for better performance and UX.
 
     def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:
-        scrape_stream_url = self.options.get("stream_url", False)
+        scrape_stream_url = self.options.get("use_stream_url", False)
 
         url = metadata.id
 
         if scrape_stream_url is True and "https://youtu.be" in url:
             url = YouTube(url).streams.get_highest_resolution().url
 
         # NOTE: I could have just dropped multi as all the media in my list are
```

### Comparing `mov-cli-test-1.1.3/mov_cli_test.egg-info/PKG-INFO` & `mov_cli_test-1.1.4/mov_cli_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.3
+Version: 1.1.4
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mov-cli-test-1.1.3/pyproject.toml` & `mov_cli_test-1.1.4/pyproject.toml`

 * *Files identical despite different names*


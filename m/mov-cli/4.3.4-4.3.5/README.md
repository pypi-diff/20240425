# Comparing `tmp/mov_cli-4.3.4.tar.gz` & `tmp/mov_cli-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.3.4.tar", last modified: Thu Apr 25 01:37:20 2024, max compression
+gzip compressed data, was "mov_cli-4.3.5.tar", last modified: Thu Apr 25 14:36:41 2024, max compression
```

## Comparing `mov_cli-4.3.4.tar` & `mov_cli-4.3.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.711974 mov_cli-4.3.4/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-04-25 01:36:18.000000 mov_cli-4.3.4/LICENSE
--rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 01:37:20.711974 mov_cli-4.3.4/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)     5336 2024-04-25 01:36:18.000000 mov_cli-4.3.4/README.md
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      131 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/__init__.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/cli/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       17 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     5589 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/__main__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      416 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/auto_select.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2089 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/configuration.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2063 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/episode.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2938 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/play.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1785 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/plugins.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4079 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/scraper.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1248 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/search.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     6423 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/ui.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1320 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/watch_options.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     6436 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/config.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      585 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/config.template.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1032 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/download.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1002 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/errors.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2784 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/http_client.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/iterfzf/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4123 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      229 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/logger.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/media/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       44 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/media/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2914 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/media/media.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1859 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/media/metadata.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/players/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      113 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1100 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/custom_player.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3109 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/mpv.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      551 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/player.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2683 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/syncplay.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3856 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/vlc.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1369 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/plugins.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2093 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/scraper.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/utils/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       99 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      620 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/episode_selector.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2018 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/paths.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      652 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/platform.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.711974 mov_cli-4.3.4/mov_cli/utils/scraper/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       69 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4751 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3383 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/version.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.711974 mov_cli-4.3.4/mov_cli.egg-info/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1136 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       53 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)      215 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/requires.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        8 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1733 2024-04-25 01:36:18.000000 mov_cli-4.3.4/pyproject.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-04-25 01:37:20.711974 mov_cli-4.3.4/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-04-25 14:09:38.000000 mov_cli-4.3.5/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 14:36:41.471548 mov_cli-4.3.5/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     5336 2024-04-25 14:09:38.000000 mov_cli-4.3.5/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      131 2024-04-25 14:34:51.000000 mov_cli-4.3.5/mov_cli/__init__.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/cli/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       17 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     5589 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/__main__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      416 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/auto_select.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2089 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/configuration.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2063 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/episode.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2938 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/play.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1785 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/plugins.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4095 2024-04-25 14:10:28.000000 mov_cli-4.3.5/mov_cli/cli/scraper.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1248 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/search.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     6423 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/ui.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1320 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/watch_options.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     6436 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/config.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      585 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/config.template.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1032 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/download.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1002 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/errors.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2784 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/http_client.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/iterfzf/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4123 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      229 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/logger.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/media/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       44 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/media/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2914 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/media/media.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1859 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/media/metadata.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli/players/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      113 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1100 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/custom_player.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3109 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/mpv.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      551 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/player.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2683 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/syncplay.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3856 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/vlc.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1369 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/plugins.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2093 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli/utils/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       99 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      620 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2018 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/paths.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      652 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/platform.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli/utils/scraper/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       69 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4751 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3383 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/version.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1136 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       53 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      215 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        8 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1733 2024-04-25 14:09:38.000000 mov_cli-4.3.5/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-04-25 14:36:41.471548 mov_cli-4.3.5/setup.cfg
```

### Comparing `mov_cli-4.3.4/LICENSE` & `mov_cli-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/PKG-INFO` & `mov_cli-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.4
+Version: 4.3.5
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.4 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.5 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.4/README.md` & `mov_cli-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/__main__.py` & `mov_cli-4.3.5/mov_cli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/configuration.py` & `mov_cli-4.3.5/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/episode.py` & `mov_cli-4.3.5/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/play.py` & `mov_cli-4.3.5/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/plugins.py` & `mov_cli-4.3.5/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/scraper.py` & `mov_cli-4.3.5/mov_cli/cli/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         "Select a plugin", 
         choices = plugins_data, 
         display = lambda x: f"{Colours.ORANGE.apply(x[0])} [{Colours.PINK_GREY.apply(x[1])}]", 
         fzf_enabled = fzf_enabled
     )
 
     if chosen_plugin is not None:
-        plugin_namespace, _, plugin_data = chosen_plugin
+        plugin_namespace, _, plugin_data, plugin = chosen_plugin
 
         chosen_scraper = prompt(
             "Select a scraper", 
             choices = [scraper for scraper in plugin_data["scrapers"].items()], 
             display = lambda x: Colours.BLUE.apply(x[0].lower()), 
             fzf_enabled = fzf_enabled
         )
@@ -100,15 +100,15 @@
     return dict(
         [(x.replace("--", "").replace("-", "_"), True) for x in scrape_arguments]
     )
 
 def get_scraper(scraper_id: str, plugins_data: List[Tuple[str, str, PluginHookData]]) -> Tuple[str, Type[Scraper] | Tuple[None, List[str]]]:
     available_scrapers = []
 
-    for plugin_namespace, _, plugin_hook_data in plugins_data:
+    for plugin_namespace, _, plugin_hook_data, plugin in plugins_data:
         scrapers = plugin_hook_data["scrapers"]
 
         if scraper_id.lower() == plugin_namespace.lower() and "DEFAULT" in scrapers:
             return f"{plugin_namespace}.DEFAULT", scrapers["DEFAULT"]
 
         for scraper_name, scraper in scrapers.items():
             id = f"{plugin_namespace}.{scraper_name}".lower()
```

### Comparing `mov_cli-4.3.4/mov_cli/cli/search.py` & `mov_cli-4.3.5/mov_cli/cli/search.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/ui.py` & `mov_cli-4.3.5/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/cli/watch_options.py` & `mov_cli-4.3.5/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/config.py` & `mov_cli-4.3.5/mov_cli/config.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/config.template.toml` & `mov_cli-4.3.5/mov_cli/config.template.toml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/download.py` & `mov_cli-4.3.5/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/errors.py` & `mov_cli-4.3.5/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/http_client.py` & `mov_cli-4.3.5/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/iterfzf/__init__.py` & `mov_cli-4.3.5/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/media/media.py` & `mov_cli-4.3.5/mov_cli/media/media.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/media/metadata.py` & `mov_cli-4.3.5/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/players/custom_player.py` & `mov_cli-4.3.5/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/players/mpv.py` & `mov_cli-4.3.5/mov_cli/players/mpv.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/players/player.py` & `mov_cli-4.3.5/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/players/syncplay.py` & `mov_cli-4.3.5/mov_cli/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/players/vlc.py` & `mov_cli-4.3.5/mov_cli/players/vlc.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/plugins.py` & `mov_cli-4.3.5/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/scraper.py` & `mov_cli-4.3.5/mov_cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/utils/episode_selector.py` & `mov_cli-4.3.5/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/utils/paths.py` & `mov_cli-4.3.5/mov_cli/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/utils/platform.py` & `mov_cli-4.3.5/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.3.5/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli/utils/version.py` & `mov_cli-4.3.5/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.3.5/mov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.4
+Version: 4.3.5
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.4 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.5 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.4/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.3.5/mov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.4/pyproject.toml` & `mov_cli-4.3.5/pyproject.toml`

 * *Files identical despite different names*


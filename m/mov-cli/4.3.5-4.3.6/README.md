# Comparing `tmp/mov_cli-4.3.5.tar.gz` & `tmp/mov_cli-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.3.5.tar", last modified: Thu Apr 25 14:36:41 2024, max compression
+gzip compressed data, was "mov_cli-4.3.6.tar", last modified: Thu Apr 25 17:49:20 2024, max compression
```

## Comparing `mov_cli-4.3.5.tar` & `mov_cli-4.3.6.tar`

### file list

```diff
@@ -1,57 +1,74 @@
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-04-25 14:09:38.000000 mov_cli-4.3.5/LICENSE
--rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 14:36:41.471548 mov_cli-4.3.5/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)     5336 2024-04-25 14:09:38.000000 mov_cli-4.3.5/README.md
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      131 2024-04-25 14:34:51.000000 mov_cli-4.3.5/mov_cli/__init__.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/cli/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       17 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     5589 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/__main__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      416 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/auto_select.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2089 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/configuration.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2063 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/episode.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2938 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/play.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1785 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/plugins.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4095 2024-04-25 14:10:28.000000 mov_cli-4.3.5/mov_cli/cli/scraper.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1248 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/search.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     6423 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/ui.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1320 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/cli/watch_options.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     6436 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/config.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      585 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/config.template.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1032 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/download.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1002 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/errors.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2784 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/http_client.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/iterfzf/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4123 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      229 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/logger.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.468215 mov_cli-4.3.5/mov_cli/media/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       44 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/media/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2914 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/media/media.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1859 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/media/metadata.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli/players/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      113 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1100 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/custom_player.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3109 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/mpv.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      551 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/player.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2683 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/syncplay.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3856 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/players/vlc.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1369 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/plugins.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2093 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/scraper.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli/utils/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       99 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      620 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/episode_selector.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2018 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/paths.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      652 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/platform.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli/utils/scraper/
--rw-r--r--   0 ananas    (1000) ananas    (1000)       69 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4751 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3383 2024-04-25 14:09:38.000000 mov_cli-4.3.5/mov_cli/utils/version.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 14:36:41.471548 mov_cli-4.3.5/mov_cli.egg-info/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1136 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       53 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)      215 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/requires.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        8 2024-04-25 14:36:41.000000 mov_cli-4.3.5/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1733 2024-04-25 14:09:38.000000 mov_cli-4.3.5/pyproject.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-04-25 14:36:41.471548 mov_cli-4.3.5/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.073767 mov_cli-4.3.6/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.063768 mov_cli-4.3.6/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.067101 mov_cli-4.3.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.067101 mov_cli-4.3.6/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.3.6/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.6/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.3.6/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 16:37:27.000000 mov_cli-4.3.6/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-25 17:49:20.073767 mov_cli-4.3.6/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-04-19 20:31:56.000000 mov_cli-4.3.6/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.3.6/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.067101 mov_cli-4.3.6/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-25 17:47:09.000000 mov_cli-4.3.6/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.070434 mov_cli-4.3.6/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.3.6/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5588 2024-04-25 17:41:01.000000 mov_cli-4.3.6/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2938 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1785 2024-04-25 15:53:32.000000 mov_cli-4.3.6/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4095 2024-04-25 16:37:16.000000 mov_cli-4.3.6/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1259 2024-04-25 17:24:40.000000 mov_cli-4.3.6/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 17:44:59.000000 mov_cli-4.3.6/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6436 2024-04-25 16:37:16.000000 mov_cli-4.3.6/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      585 2024-04-25 16:37:16.000000 mov_cli-4.3.6/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1002 2024-04-19 20:51:26.000000 mov_cli-4.3.6/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov_cli-4.3.6/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.070434 mov_cli-4.3.6/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.3.6/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.3.6/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.3.6/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.070434 mov_cli-4.3.6/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.3.6/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2914 2024-04-19 20:51:26.000000 mov_cli-4.3.6/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.073767 mov_cli-4.3.6/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      113 2024-04-25 15:53:32.000000 mov_cli-4.3.6/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov_cli-4.3.6/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3109 2024-04-19 20:51:26.000000 mov_cli-4.3.6/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov_cli-4.3.6/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2683 2024-04-25 15:53:32.000000 mov_cli-4.3.6/mov_cli/players/syncplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3856 2024-04-22 23:15:31.000000 mov_cli-4.3.6/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.073767 mov_cli-4.3.6/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.3.6/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.3.6/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.3.6/mov_cli/utils/paths.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.3.6/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.073767 mov_cli-4.3.6/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-19 20:31:56.000000 mov_cli-4.3.6/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.073767 mov_cli-4.3.6/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-25 17:49:20.000000 mov_cli-4.3.6/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1457 2024-04-25 17:49:20.000000 mov_cli-4.3.6/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 17:49:20.000000 mov_cli-4.3.6/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-25 17:49:20.000000 mov_cli-4.3.6/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-25 17:49:20.000000 mov_cli-4.3.6/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-25 17:49:20.000000 mov_cli-4.3.6/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1733 2024-04-19 20:31:56.000000 mov_cli-4.3.6/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.3.6/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 17:49:20.073767 mov_cli-4.3.6/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.3.6/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 17:49:20.073767 mov_cli-4.3.6/setup.cfg
```

### Comparing `mov_cli-4.3.5/LICENSE` & `mov_cli-4.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/PKG-INFO` & `mov_cli-4.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.5
+Version: 4.3.6
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.5 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.6 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.5/README.md` & `mov_cli-4.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/cli/__main__.py` & `mov_cli-4.3.6/mov_cli/cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if list_plugins:
         show_all_plugins(plugins)
         return None
 
     welcome_message = welcome_msg(
         plugins = plugins, 
         check_for_updates = True if query is None and config.skip_update_checker is False else False, 
-        display_hint = True if query is None else False, 
+        display_tip = True if query is None else False, 
         display_version = version
     )
 
     print(welcome_message)
 
     if query is not None:
         scrape_options = steal_scraper_args(query)
```

### Comparing `mov_cli-4.3.5/mov_cli/cli/configuration.py` & `mov_cli-4.3.6/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/cli/episode.py` & `mov_cli-4.3.6/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/cli/play.py` & `mov_cli-4.3.6/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/cli/plugins.py` & `mov_cli-4.3.6/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/cli/scraper.py` & `mov_cli-4.3.6/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/cli/search.py` & `mov_cli-4.3.6/mov_cli/cli/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 
     if auto_select is not None:
         choice = auto_select_choice((choice for choice in search_results), auto_select)
     else:
         choice = prompt(
             "Choose Result", 
             choices = (choice for choice in search_results), 
-            display = lambda x: f"{Colours.CLAY if x.type == MetadataType.MOVIE else Colours.BLUE}{x.title}" \
-                f"{Colours.RESET} ({x.year if x.year is not None else 'N/A'})", 
+            display = lambda x: f"{Colours.BLUE if x.type == MetadataType.SINGLE else Colours.PINK_GREY}{x.title}" \
+                f"{Colours.RESET}" + (f" ({x.year})" if x.year is not None else ""), 
             fzf_enabled = fzf_enabled
         )
 
     return choice
```

### Comparing `mov_cli-4.3.5/mov_cli/cli/ui.py` & `mov_cli-4.3.6/mov_cli/cli/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,23 @@
         Any, Dict, List, Tuple, 
         TypeVar, Literal, Iterable, Callable, Generator
     )
 
     T = TypeVar('T')
 
 import re
+import os
+import json
 import types
 import random
 import logging
 import getpass
 import inquirer
 import itertools
+from pathlib import Path
 from datetime import datetime
 from inquirer.themes import Default
 from devgoldyutils import Colours, LoggerAdapter
 
 import mov_cli
 
 from ..iterfzf import iterfzf
@@ -149,31 +152,46 @@
             greeting = "Good Evening"
         elif i > 8:
             greeting = "Good Night"
 
     return greeting, user_name
 
 # This function below is inspired by animdl: https://github.com/justfoolingaround/animdl
-def welcome_msg(plugins: Dict[str, str], check_for_updates: bool = False, display_hint: bool = False, display_version: bool = False) -> str:
+def welcome_msg(
+    plugins: Dict[str, str], 
+    check_for_updates: bool = False, 
+    display_tip: bool = False, 
+    display_version: bool = False
+) -> str:
     """Returns cli welcome message."""
     now = datetime.now()
     adjective = random.choice(
         ("gorgeous", "wonderful", "beautiful", "magnificent")
     )
 
+    random_tips_path = Path(os.path.split(__file__)[0]).joinpath("random_tips.json")
+
     greeting, user_name = greetings()
 
     text = f"\n{greeting}, {Colours.ORANGE.apply(user_name)}."
     text += now.strftime(
         f"\n    It's {Colours.BLUE}%I:%M %p {Colours.RESET}on a {Colours.PURPLE}{adjective} {Colours.PINK_GREY}%A! {Colours.RESET}"
     )
 
-    if display_hint is True and display_version is False:
-        text += f"\n\n- Hint: {Colours.CLAY}mov-cli {Colours.PINK_GREY}-s films {Colours.ORANGE}mr.robot{Colours.RESET}" \
-            f"\n- Hint: {Colours.CLAY}mov-cli {Colours.PINK_GREY}-s anime {Colours.ORANGE}chuunibyou demo take on me{Colours.RESET}"
+    if display_tip and display_version is False:
+
+        if random.randint(0, 1) == 0:
+            text += f"\n\n- {Colours.BLUE}Hint: {Colours.RESET}mov-cli {Colours.PINK_GREY}-s films {Colours.ORANGE}mr.robot{Colours.RESET}" \
+                f"\n- {Colours.BLUE}Hint: {Colours.RESET}mov-cli {Colours.PINK_GREY}-s anime {Colours.ORANGE}chuunibyou demo take on me{Colours.RESET}"
+
+        else:
+            random_tips_json: List[str] = json.load(random_tips_path.open("r")) # TODO: This should be cached after the caching system is implemented.
+            random_tip = random.choice(random_tips_json)
+
+            text += f"\n\n- {Colours.ORANGE}TIP: {Colours.RESET}{random_tip}"
 
     if display_version is True:
         text += f"\n\n{Colours.CLAY}-> {Colours.RESET}Version: {Colours.BLUE}{mov_cli.__version__}{Colours.RESET}"
 
     if check_for_updates:
 
         if update_available():
```

### Comparing `mov_cli-4.3.5/mov_cli/cli/watch_options.py` & `mov_cli-4.3.6/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/config.py` & `mov_cli-4.3.6/mov_cli/config.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/config.template.toml` & `mov_cli-4.3.6/mov_cli/config.template.toml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/download.py` & `mov_cli-4.3.6/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/errors.py` & `mov_cli-4.3.6/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/http_client.py` & `mov_cli-4.3.6/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/iterfzf/__init__.py` & `mov_cli-4.3.6/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/media/media.py` & `mov_cli-4.3.6/mov_cli/media/media.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/media/metadata.py` & `mov_cli-4.3.6/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/players/custom_player.py` & `mov_cli-4.3.6/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/players/mpv.py` & `mov_cli-4.3.6/mov_cli/players/mpv.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/players/player.py` & `mov_cli-4.3.6/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/players/syncplay.py` & `mov_cli-4.3.6/mov_cli/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/players/vlc.py` & `mov_cli-4.3.6/mov_cli/players/vlc.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/plugins.py` & `mov_cli-4.3.6/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/scraper.py` & `mov_cli-4.3.6/mov_cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/utils/episode_selector.py` & `mov_cli-4.3.6/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/utils/paths.py` & `mov_cli-4.3.6/mov_cli/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/utils/platform.py` & `mov_cli-4.3.6/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.3.6/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli/utils/version.py` & `mov_cli-4.3.6/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.5/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.3.6/mov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.5
+Version: 4.3.6
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.5 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.6 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.5/pyproject.toml` & `mov_cli-4.3.6/pyproject.toml`

 * *Files identical despite different names*


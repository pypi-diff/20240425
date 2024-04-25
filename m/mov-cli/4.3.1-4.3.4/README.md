# Comparing `tmp/mov_cli-4.3.1.tar.gz` & `tmp/mov_cli-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.3.1.tar", last modified: Fri Apr 19 01:33:24 2024, max compression
+gzip compressed data, was "mov_cli-4.3.4.tar", last modified: Thu Apr 25 01:37:20 2024, max compression
```

## Comparing `mov_cli-4.3.1.tar` & `mov_cli-4.3.4.tar`

### file list

```diff
@@ -1,72 +1,57 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.820418 mov_cli-4.3.1/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.820418 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.823751 mov_cli-4.3.1/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.3.1/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.3.1/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      291 2024-04-04 00:43:21.000000 mov_cli-4.3.1/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-19 01:33:24.830417 mov_cli-4.3.1/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-04-19 00:17:22.000000 mov_cli-4.3.1/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-08 22:18:54.000000 mov_cli-4.3.1/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.823751 mov_cli-4.3.1/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-19 01:33:09.000000 mov_cli-4.3.1/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.827084 mov_cli-4.3.1/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5589 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2938 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1926 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4079 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1248 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6423 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6913 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      583 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-08 22:18:54.000000 mov_cli-4.3.1/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      942 2024-04-04 00:48:22.000000 mov_cli-4.3.1/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.827084 mov_cli-4.3.1/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.3.1/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.827084 mov_cli-4.3.1/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2793 2024-04-19 00:26:10.000000 mov_cli-4.3.1/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       89 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2813 2024-04-19 00:37:22.000000 mov_cli-4.3.1/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2519 2024-04-19 01:17:33.000000 mov_cli-4.3.1/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.3.1/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-08 22:18:54.000000 mov_cli-4.3.1/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-08 22:18:54.000000 mov_cli-4.3.1/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1406 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1733 2024-04-08 23:54:10.000000 mov_cli-4.3.1/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.3.1/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.3.1/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-19 01:33:24.830417 mov_cli-4.3.1/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.711974 mov_cli-4.3.4/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-04-25 01:36:18.000000 mov_cli-4.3.4/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 01:37:20.711974 mov_cli-4.3.4/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     5336 2024-04-25 01:36:18.000000 mov_cli-4.3.4/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      131 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/__init__.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/cli/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       17 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     5589 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/__main__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      416 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/auto_select.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2089 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/configuration.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2063 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/episode.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2938 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/play.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1785 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/plugins.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4079 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/scraper.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1248 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/search.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     6423 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/ui.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1320 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/cli/watch_options.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     6436 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/config.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      585 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/config.template.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1032 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/download.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1002 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/errors.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2784 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/http_client.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/iterfzf/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4123 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      229 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/logger.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/media/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       44 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/media/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2914 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/media/media.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1859 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/media/metadata.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/players/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      113 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1100 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/custom_player.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3109 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/mpv.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      551 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/player.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2683 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/syncplay.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3856 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/players/vlc.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1369 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/plugins.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2093 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.708640 mov_cli-4.3.4/mov_cli/utils/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       99 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      620 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2018 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/paths.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      652 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/platform.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.711974 mov_cli-4.3.4/mov_cli/utils/scraper/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       69 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4751 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3383 2024-04-25 01:36:18.000000 mov_cli-4.3.4/mov_cli/utils/version.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-25 01:37:20.711974 mov_cli-4.3.4/mov_cli.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     7990 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1136 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       53 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      215 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        8 2024-04-25 01:37:20.000000 mov_cli-4.3.4/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1733 2024-04-25 01:36:18.000000 mov_cli-4.3.4/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-04-25 01:37:20.711974 mov_cli-4.3.4/setup.cfg
```

### Comparing `mov_cli-4.3.1/LICENSE` & `mov_cli-4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/PKG-INFO` & `mov_cli-4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.1
+Version: 4.3.4
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.1 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.4 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.1/README.md` & `mov_cli-4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/__main__.py` & `mov_cli-4.3.4/mov_cli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/configuration.py` & `mov_cli-4.3.4/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/episode.py` & `mov_cli-4.3.4/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/play.py` & `mov_cli-4.3.4/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/plugins.py` & `mov_cli-4.3.4/mov_cli/cli/plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,22 @@
 
         plugin_data, _ = plugin
 
         if plugin_data is None:
             continue
 
         plugins_data.append(
-            (plugin_namespace, plugin_module_name, plugin_data)
+            (plugin_namespace, plugin_module_name, plugin_data, plugin)
         )
 
     return plugins_data
 
 def show_all_plugins(plugins: Dict[str, str]) -> None:
 
-    for plugin_namespace, plugin_module_name, plugin_hook_data in get_plugins_data(plugins):
-        # TODO: Have 'get_plugins_data' return plugin module so we shouldn't have to load the plugin twice.
-        plugin = load_plugin(plugin_module_name)
+    for plugin_namespace, plugin_module_name, plugin_hook_data, plugin in get_plugins_data(plugins):
 
         if plugin is not None:
             plugin_module = plugin[1]
 
             plugin_version = getattr(plugin_module, "__version__", "N/A")
 
             print(f"- {Colours.PURPLE.apply(plugin_module_name)} ({plugin_namespace}) [{Colours.BLUE.apply(plugin_version)}]")
```

### Comparing `mov_cli-4.3.1/mov_cli/cli/scraper.py` & `mov_cli-4.3.4/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/search.py` & `mov_cli-4.3.4/mov_cli/cli/search.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/ui.py` & `mov_cli-4.3.4/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/cli/watch_options.py` & `mov_cli-4.3.4/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/config.py` & `mov_cli-4.3.4/mov_cli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, TypedDict, final
+from typing_extensions import NotRequired
 
 if TYPE_CHECKING:
     from .players import Player
     from typing import Dict, Union, Literal, Any, Optional
 
     JSON_VALUES = Union[str, bool, int, dict]
     SUPPORTED_PARSERS = Literal["lxml", "html.parser"]
@@ -13,14 +14,15 @@
 import shutil
 from pathlib import Path
 from importlib.util import find_spec
 from devgoldyutils import LoggerAdapter
 
 from . import players, utils
 from .logger import mov_cli_logger
+from .utils import get_appdata_directory
 
 __all__ = ("Config", )
 
 @final
 class ConfigUIData(TypedDict):
     fzf: bool
 
@@ -44,15 +46,23 @@
     parser: SUPPORTED_PARSERS
     ui: ConfigUIData
     http: ConfigHTTPData
     downloads: ConfigDownloadsData
     scrapers: ScrapersData
     plugins: Dict[str, str]
     resolution: int
-    
+
+HttpHeadersData = TypedDict(
+    "HttpHeadersData", 
+    {
+        "User-Agent": NotRequired[str],
+        "Accept-Language": NotRequired[str],
+        "Accept": NotRequired[str]
+    }
+)
 
 logger = LoggerAdapter(mov_cli_logger, prefix = "Config")
 
 class Config():
     """Class that wraps the mov-cli configuration file. Mostly used under the CLI interface."""
     def __init__(self, override_config: ConfigData = None, config_path: Path = None) -> None:
         self.config_path = config_path
@@ -84,14 +94,16 @@
 
         platform = utils.what_platform()
 
         if value.lower() == "mpv":
             return players.MPV(platform, self)
         elif value.lower() == "vlc":
             return players.VLC(platform, self)
+        elif value.lower() == "syncplay":
+            return players.SyncPlay(platform, self)
 
         return players.CustomPlayer(value)
 
     @property
     def plugins(self) -> Dict[str, str]:
         return self.data.get("plugins", {"test": "mov-cli-test"})
 
@@ -151,15 +163,15 @@
                 proxy = f"{scheme}://{ip}:{port}"
 
             return {"all://": proxy}
         else:
             return None
 
     @property
-    def http_headers(self) -> dict:
+    def http_headers(self) -> HttpHeadersData:
         """Returns http headers."""
         default_headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
         }
 
@@ -169,38 +181,17 @@
     def resolution(self) -> int:
         return self.data.get("quality", {}).get("resolution", {})
 
     def __get_config_file(self) -> Path:
         """Function that returns the path to the config file with multi platform support."""
         platform = utils.what_platform()
 
-        appdata_dir = Path("./mov-cli-temp")
-
-        if platform == "Windows":
-            user_profile = Path(os.getenv("USERPROFILE"))
-            appdata_dir = user_profile.joinpath("AppData", "Local")
-
-        elif platform == "Darwin": # NOTE: Path maybe incorrect
-            user_profile = Path.home()
-            appdata_dir = user_profile.joinpath("Library", "Application Support")
-
-        elif platform == "iOS":
-            user_profile = Path(os.getenv("HOME"))
-            appdata_dir = user_profile.joinpath("Library")
-
-            appdata_dir.mkdir(exist_ok = True)
-
-        elif platform == "Linux" or platform == "Android":
-            user_profile = Path(os.getenv("HOME"))
-            appdata_dir = user_profile.joinpath(".config")
- 
-            appdata_dir.mkdir(exist_ok = True) # on android the .config file may not exist.
+        appdata_folder = get_appdata_directory(platform)
 
-        config_path = appdata_dir.joinpath("mov-cli", "config.toml")
-        config_path.parent.mkdir(exist_ok = True)
+        config_path = appdata_folder.joinpath("config.toml")
 
         if not config_path.exists():
             logger.debug("The 'config.toml' file doesn't exist so we're creating it...")
             config_file = open(config_path, "w")
 
             template_config_path = f"{Path(os.path.split(__file__)[0])}{os.sep}config.template.toml"
```

### Comparing `mov_cli-4.3.1/mov_cli/config.template.toml` & `mov_cli-4.3.4/mov_cli/config.template.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 version = 1
 player = "mpv"
 debug = false
 # parser = "lxml"
 # editor = "nano"
 skip_update_checker = false
 
-[mov-cli.ui]
+# [mov-cli.ui]
 # fzf = true
 
 [mov-cli.plugins] # E.g: namespace = "package-name"
 test = "mov-cli-test"
 
 # [mov-cli.scrapers]
 # default = "films"
```

### Comparing `mov_cli-4.3.1/mov_cli/download.py` & `mov_cli-4.3.4/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/errors.py` & `mov_cli-4.3.4/mov_cli/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 if TYPE_CHECKING:
     import logging
     from .players import Player
 
 from devgoldyutils import Colours
 from .logger import mov_cli_logger
 
+__all__ = (
+    "MovCliException", 
+    "PlayerNotFound"
+)
+
 class MovCliException(Exception):
     """Raises whenever there's a known error in mov-cli."""
     def __init__(self, message: str, logger: logging.Logger = None):
         message = Colours.RED.apply_to_string(message)
 
         if logger is None:
             logger = mov_cli_logger
```

### Comparing `mov_cli-4.3.1/mov_cli/http_client.py` & `mov_cli-4.3.4/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/iterfzf/__init__.py` & `mov_cli-4.3.4/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/media/media.py` & `mov_cli-4.3.4/mov_cli/media/media.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 class Media():
     """Represents any piece of media in mov-cli that can be streamed or downloaded."""
     def __init__(
         self, 
         url: str, 
         title: str, 
         audio_url: Optional[str], 
-        referrer: Optional[str]
+        referrer: Optional[str], 
+        subtitles: Optional[str]
     ) -> None:
         self.url = url
         """The stream-able url of the media."""
         self.title = title
         """A title to represent this stream-able media."""
         self.audio_url = audio_url
         """The stream-able url that provides audio for the media if the main url doesn't stream with audio."""
         self.referrer = referrer
         """The required referrer for streaming the media content."""
+        self.subtitles = subtitles
+        """The url or file path to the subtitles."""
 
     @property
     @abstractmethod
     def display_name(self) -> str:
         """The title that should be displayed by the player."""
         ...
 
@@ -44,25 +47,25 @@
     def __init__(
         self, 
         url: str, 
         title: str, 
         episode: EpisodeSelector, 
         audio_url: Optional[str] = None, 
         referrer: Optional[str] = None, 
-        subtitles: Optional[dict] = None
+        subtitles: Optional[str] = None
     ) -> None:
         self.episode = episode
         """The episode and season of this series."""
-        self.subtitles = subtitles
 
         super().__init__(
             url, 
             title = title, 
             audio_url = audio_url, 
-            referrer = referrer
+            referrer = referrer,
+            subtitles = subtitles
         )
 
     @property
     def display_name(self) -> str:
         return f"{self.title} - S{self.episode.season} EP{self.episode.episode}"
 
 class Single(Media):
@@ -70,25 +73,25 @@
     def __init__(
         self, 
         url: str, 
         title: str, 
         audio_url: Optional[str] = None, 
         referrer: Optional[str] = None, 
         year: Optional[str] = None, 
-        subtitles: Optional[dict] = None 
+        subtitles: Optional[str] = None 
     ) -> None:
         self.year = year
         """The year this film was released."""
-        self.subtitles = subtitles
 
         super().__init__(
             url, 
             title = title, 
             audio_url = audio_url, 
-            referrer = referrer
+            referrer = referrer,
+            subtitles = subtitles
         )
 
     @property
     def display_name(self) -> str:
         return f"{self.title} ({self.year})"
 
 # Backwards compatibility for post v4.3.0 extensions.
```

### Comparing `mov_cli-4.3.1/mov_cli/media/metadata.py` & `mov_cli-4.3.4/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/players/custom_player.py` & `mov_cli-4.3.4/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/players/mpv.py` & `mov_cli-4.3.4/mov_cli/players/mpv.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
                 if media.referrer is not None:
                     args.append(f"--referrer={media.referrer}")
 
                 if media.audio_url is not None:
                     args.append(f"--audio-file={media.audio_url}")
 
+                if media.subtitles is not None:
+                    args.append(f"--sub-file={media.subtitles}")
+
                 if self.config.resolution:
                     args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
 
                 return subprocess.Popen(args)
 
             elif self.platform == "Darwin":
                 args = [
@@ -72,17 +75,20 @@
                     media.url,
                     f"--mpv-force-media-title={media.display_name}",
                 ]
 
                 if media.referrer is not None:
                     args.append(f"--mpv-referrer={media.referrer}")
 
-                if media.audio_url is not None:
+                if media.audio_url is not None: # TODO: This will need testing.
                     args.append(f"--mpv-audio-file={media.audio_url}")
 
+                if media.subtitles is not None: # TODO: This will need testing.
+                    args.append(f"--mpv-sub-file={media.subtitles}")
+
                 if self.config.resolution:
                     args.append(f"--mpv-hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
 
                 return subprocess.Popen(args)
 
         except (ModuleNotFoundError, FileNotFoundError):
             raise errors.PlayerNotFound(self)
```

### Comparing `mov_cli-4.3.1/mov_cli/players/player.py` & `mov_cli-4.3.4/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/players/vlc.py` & `mov_cli-4.3.4/mov_cli/players/syncplay.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional
-
     from ..media import Media
     from .. import Config
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import subprocess
 from devgoldyutils import Colours, LoggerAdapter
 
 from .. import errors
 from ..logger import mov_cli_logger
 from .player import Player
 
-__all__ = ("VLC",)
+__all__ = ("SyncPlay",)
 
-logger = LoggerAdapter(mov_cli_logger, prefix = Colours.ORANGE.apply("VLC"))
+logger = LoggerAdapter(mov_cli_logger, prefix = Colours.PURPLE.apply("SyncPlay"))
 
-class VLC(Player):
+class SyncPlay(Player):
     def __init__(self, platform: SUPPORTED_PLATFORMS, config: Config, **kwargs) -> None:
         self.platform = platform
         self.config = config
 
         super().__init__(**kwargs)
 
     def play(self, media: Media) -> Optional[subprocess.Popen]:
-        """Plays this media in the VLC media player."""
+        """Plays this media in SyncPlay."""
+
+        logger.info("Launching SyncPlay...")
 
-        logger.info("Launching VLC Media Player...")
+        try:
 
-        if self.platform == "Android":
-            return subprocess.Popen(
-                [
-                    "am",
-                    "start",
-                    "-n",
-                    "org.videolan.vlc/org.videolan.vlc.gui.video.VideoPlayerActivity",
-                    "-e",
-                    "title",
-                    media.display_name,
+            if self.platform == "Windows" or self.platform == "Linux":
+                args = [
+                    "syncplay",
                     media.url,
+                    "--",
+                    f"--force-media-title={media.display_name}",
                 ]
-            )
 
-        elif self.platform == "iOS":
-            logger.debug("Detected your using iOS. \r\n")
+                if media.referrer is not None:
+                    args.append(f"--referrer={media.referrer}")
+
+                if media.audio_url is not None:
+                    args.append(f"--audio-file={media.audio_url}")
 
-            with open('/dev/clipboard', 'w') as f:
-                f.write(f"vlc://{media.url}")
+                if media.subtitles is not None:
+                    args.append(f"--sub-file={media.subtitles}")
 
-            logger.info("The URL was copied into your clipboard. To play it, open a browser and paste the URL.")
+                if self.config.resolution:
+                    args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: Only M3U8
 
-            return None
+                return subprocess.Popen(args)
 
-        elif self.platform == "Linux" or self.platform == "Windows":
-            try:
+            elif self.platform == "Darwin": # NOTE: Limits you to IINA
                 args = [
-                    "vlc", 
-                    f'--meta-title="{media.display_name}"', 
-                    media.url, 
-                    "--quiet"
+                    "syncplay",
+                    media.url,
+                    "--",
+                    f"--mpv-force-media-title={media.display_name}",
                 ]
 
                 if media.referrer is not None:
-                    args.append(f'--http-referrer="{media.referrer}"')
+                    args.append(f"--mpv-referrer={media.referrer}")
 
-                if media.audio_url is not None:
-                    args.append(f"--input-slave={media.audio_url}") # WHY IS THIS UNDOCUMENTED!!!
+                if media.audio_url is not None: # TODO: This will need testing.
+                    args.append(f"--mpv-audio-file={media.audio_url}")
 
-                if self.config.resolution:
-                    args.append(f"--adaptive-maxwidth={self.config.resolution}") # NOTE: I don't really know if that works ~ Ananas
+                if media.subtitles is not None: # TODO: This will need testing.
+                    args.append(f"--mpv-sub-file={media.subtitles}")
+
+                if self.config.resolution: # TODO: This will need testing.
+                    args.append(f"--mpv-hls-bitrate={self.config.resolution}")
 
                 return subprocess.Popen(args)
 
-            except (ModuleNotFoundError, FileNotFoundError):
-                raise errors.PlayerNotFound(self)
+        except (ModuleNotFoundError, FileNotFoundError):
+            raise errors.PlayerNotFound(self)
 
         return None
```

### Comparing `mov_cli-4.3.1/mov_cli/plugins.py` & `mov_cli-4.3.4/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/scraper.py` & `mov_cli-4.3.4/mov_cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/utils/episode_selector.py` & `mov_cli-4.3.4/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/utils/platform.py` & `mov_cli-4.3.4/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.3.4/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli/utils/version.py` & `mov_cli-4.3.4/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.1/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.3.4/mov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.1
+Version: 4.3.4
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.1 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.4 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.3.1/pyproject.toml` & `mov_cli-4.3.4/pyproject.toml`

 * *Files identical despite different names*


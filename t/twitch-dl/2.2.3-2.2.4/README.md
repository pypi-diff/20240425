# Comparing `tmp/twitch_dl-2.2.3.tar.gz` & `tmp/twitch_dl-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dl-2.2.3.tar", last modified: Wed Apr 24 12:55:04 2024, max compression
+gzip compressed data, was "twitch_dl-2.2.4.tar", last modified: Thu Apr 25 05:35:26 2024, max compression
```

## Comparing `twitch_dl-2.2.3.tar` & `twitch_dl-2.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.621527 twitch_dl-2.2.3/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2022-08-04 08:32:39.000000 twitch_dl-2.2.3/.flake8
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.611527 twitch_dl-2.2.3/.github/
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.613527 twitch_dl-2.2.3/.github/workflows/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 12:52:36.000000 twitch_dl-2.2.3/.github/workflows/test.yml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/.gitignore
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/.vermin
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10180 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/CHANGELOG.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-08-04 08:32:39.000000 twitch_dl-2.2.3/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      954 2024-04-24 06:58:58.000000 twitch_dl-2.2.3/Makefile
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-24 12:55:04.621527 twitch_dl-2.2.3/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2022-11-13 13:02:23.000000 twitch_dl-2.2.3/TODO.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/book.css
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/book.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8507 2024-04-24 12:54:22.000000 twitch_dl-2.2.3/changelog.yaml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.614527 twitch_dl-2.2.3/docs/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/docs/SUMMARY.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/docs/advanced.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10180 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/docs/changelog.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.615527 twitch_dl-2.2.3/docs/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/docs/commands/auth_token.png
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/docs/commands/clips.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/docs/commands/download.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/docs/commands/env.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/docs/commands/info.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-24 12:54:27.000000 twitch_dl-2.2.3/docs/commands/videos.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/docs/environment_variables.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/docs/installation.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/docs/introduction.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/docs/license.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/docs/shell_completion.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2022-08-27 09:42:13.000000 twitch_dl-2.2.3/docs/usage.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1308 2024-04-24 06:19:51.000000 twitch_dl-2.2.3/pyproject.toml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.615527 twitch_dl-2.2.3/scripts/
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2022-11-13 13:02:23.000000 twitch_dl-2.2.3/scripts/generate_changelog
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/scripts/generate_docs
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-10 06:26:52.000000 twitch_dl-2.2.3/scripts/tag_version
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-24 12:55:04.621527 twitch_dl-2.2.3/setup.cfg
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.616527 twitch_dl-2.2.3/tests/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2076 2024-04-24 12:38:54.000000 twitch_dl-2.2.3/tests/test_api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4659 2024-04-24 12:44:22.000000 twitch_dl-2.2.3/tests/test_cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2022-08-04 08:32:39.000000 twitch_dl-2.2.3/tests/test_patterns.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2022-11-13 13:02:23.000000 twitch_dl-2.2.3/tests/test_progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2022-08-04 08:32:39.000000 twitch_dl-2.2.3/tests/test_utils.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2022-08-04 08:32:39.000000 twitch_dl-2.2.3/twitch-dl.1.scd
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.620527 twitch_dl-2.2.3/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-24 12:55:04.000000 twitch_dl-2.2.3/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1240 2024-04-24 12:55:04.000000 twitch_dl-2.2.3/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-24 12:55:04.000000 twitch_dl-2.2.3/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-24 12:55:04.000000 twitch_dl-2.2.3/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      133 2024-04-24 12:55:04.000000 twitch_dl-2.2.3/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-24 12:55:04.000000 twitch_dl-2.2.3/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.619527 twitch_dl-2.2.3/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/twitchdl/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9715 2024-04-24 06:58:58.000000 twitch_dl-2.2.3/twitchdl/cli.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-24 12:55:04.620527 twitch_dl-2.2.3/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-03-29 07:50:11.000000 twitch_dl-2.2.3/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-24 05:25:48.000000 twitch_dl-2.2.3/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11691 2024-04-24 06:58:58.000000 twitch_dl-2.2.3/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3015 2024-04-24 06:11:56.000000 twitch_dl-2.2.3/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2039 2024-04-24 12:30:02.000000 twitch_dl-2.2.3/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-24 05:25:48.000000 twitch_dl-2.2.3/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-24 05:25:48.000000 twitch_dl-2.2.3/twitchdl/entities.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-04 06:27:17.000000 twitch_dl-2.2.3/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-24 12:09:16.000000 twitch_dl-2.2.3/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4577 2024-04-24 05:25:48.000000 twitch_dl-2.2.3/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3676 2024-04-24 06:11:56.000000 twitch_dl-2.2.3/twitchdl/playlists.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-12 07:42:26.000000 twitch_dl-2.2.3/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12422 2024-04-24 12:29:56.000000 twitch_dl-2.2.3/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3099 2024-04-24 05:25:48.000000 twitch_dl-2.2.3/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2023-08-11 10:29:42.000000 twitch_dl-2.2.4/.flake8
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.844946 twitch_dl-2.2.4/.github/
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.845946 twitch_dl-2.2.4/.github/workflows/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/.github/workflows/test.yml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/.vermin
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10336 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/CHANGELOG.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2023-08-11 10:29:42.000000 twitch_dl-2.2.4/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      954 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/TODO.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/book.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/book.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8622 2024-04-25 05:32:53.000000 twitch_dl-2.2.4/changelog.yaml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.846946 twitch_dl-2.2.4/docs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/SUMMARY.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/advanced.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10336 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/changelog.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.847946 twitch_dl-2.2.4/docs/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/commands/auth_token.png
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/clips.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/download.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/env.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/info.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-25 05:33:01.000000 twitch_dl-2.2.4/docs/commands/videos.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/environment_variables.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/installation.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/introduction.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/license.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/docs/shell_completion.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2023-08-11 10:29:47.000000 twitch_dl-2.2.4/docs/usage.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1308 2024-04-24 06:41:19.000000 twitch_dl-2.2.4/pyproject.toml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.847946 twitch_dl-2.2.4/scripts/
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2023-10-08 19:39:41.000000 twitch_dl-2.2.4/scripts/generate_changelog
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/scripts/generate_docs
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/scripts/tag_version
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.847946 twitch_dl-2.2.4/tests/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2076 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/tests/test_api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4659 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/tests/test_cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2518 2024-04-25 05:31:42.000000 twitch_dl-2.2.4/tests/test_patterns.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/tests/test_progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2023-08-11 10:29:32.000000 twitch_dl-2.2.4/tests/test_utils.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2023-08-11 10:29:42.000000 twitch_dl-2.2.4/twitch-dl.1.scd
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1240 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      133 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-25 05:35:26.000000 twitch_dl-2.2.4/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.849946 twitch_dl-2.2.4/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-04-23 15:35:36.000000 twitch_dl-2.2.4/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-04-23 15:35:35.000000 twitch_dl-2.2.4/twitchdl/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9715 2024-04-24 06:43:02.000000 twitch_dl-2.2.4/twitchdl/cli.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-25 05:35:26.850946 twitch_dl-2.2.4/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:07:42.000000 twitch_dl-2.2.4/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-23 15:09:23.000000 twitch_dl-2.2.4/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11691 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3015 2024-04-24 06:41:19.000000 twitch_dl-2.2.4/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2039 2024-04-25 05:30:23.000000 twitch_dl-2.2.4/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-23 15:35:34.000000 twitch_dl-2.2.4/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-23 16:09:59.000000 twitch_dl-2.2.4/twitchdl/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-23 15:35:32.000000 twitch_dl-2.2.4/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-23 15:35:32.000000 twitch_dl-2.2.4/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4577 2024-04-23 16:11:39.000000 twitch_dl-2.2.4/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3676 2024-04-24 06:41:19.000000 twitch_dl-2.2.4/twitchdl/playlists.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-23 15:35:30.000000 twitch_dl-2.2.4/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12422 2024-04-24 15:57:20.000000 twitch_dl-2.2.4/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3113 2024-04-25 05:30:27.000000 twitch_dl-2.2.4/twitchdl/utils.py
```

### Comparing `twitch_dl-2.2.3/.github/workflows/test.yml` & `twitch_dl-2.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/CHANGELOG.md` & `twitch_dl-2.2.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.2.4 (2024-04-25)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.4)
+
+* Add m dot url support to video and clip regexes (thanks @localnerve)
+
 ### [2.2.3 (2024-04-24)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.3)
 
 * Respect --dry-run option when downloading videos
 * Add automated tests on github actions
 
 ### [2.2.2 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.2)
```

### Comparing `twitch_dl-2.2.3/LICENSE` & `twitch_dl-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/Makefile` & `twitch_dl-2.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/PKG-INFO` & `twitch_dl-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.3
+Version: 2.2.4
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch_dl-2.2.3/README.md` & `twitch_dl-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/changelog.yaml` & `twitch_dl-2.2.4/changelog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.2.4:
+  date: 2024-04-25
+  changes:
+    - "Add m dot url support to video and clip regexes (thanks @localnerve)"
+
 2.2.3:
   date: 2024-04-24
   changes:
     - "Respect --dry-run option when downloading videos"
     - "Add automated tests on github actions"
 
 2.2.2:
```

### Comparing `twitch_dl-2.2.3/docs/changelog.md` & `twitch_dl-2.2.4/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.2.4 (2024-04-25)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.4)
+
+* Add m dot url support to video and clip regexes (thanks @localnerve)
+
 ### [2.2.3 (2024-04-24)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.3)
 
 * Respect --dry-run option when downloading videos
 * Add automated tests on github actions
 
 ### [2.2.2 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.2)
```

### Comparing `twitch_dl-2.2.3/docs/commands/auth_token.png` & `twitch_dl-2.2.4/docs/commands/auth_token.png`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/commands/clips.md` & `twitch_dl-2.2.4/docs/commands/clips.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/commands/download.md` & `twitch_dl-2.2.4/docs/commands/download.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/commands/env.md` & `twitch_dl-2.2.4/docs/commands/env.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/commands/info.md` & `twitch_dl-2.2.4/docs/commands/info.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/commands/videos.md` & `twitch_dl-2.2.4/docs/commands/videos.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/installation.md` & `twitch_dl-2.2.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/introduction.md` & `twitch_dl-2.2.4/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/license.md` & `twitch_dl-2.2.4/docs/license.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/shell_completion.md` & `twitch_dl-2.2.4/docs/shell_completion.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/docs/usage.md` & `twitch_dl-2.2.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/pyproject.toml` & `twitch_dl-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/scripts/generate_changelog` & `twitch_dl-2.2.4/scripts/generate_changelog`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/scripts/generate_docs` & `twitch_dl-2.2.4/scripts/generate_docs`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/scripts/tag_version` & `twitch_dl-2.2.4/scripts/tag_version`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/tests/test_api.py` & `twitch_dl-2.2.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/tests/test_cli.py` & `twitch_dl-2.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/tests/test_patterns.py` & `twitch_dl-2.2.4/tests/test_patterns.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import pytest
 
-from twitchdl.utils import parse_video_identifier, parse_clip_identifier
-
+from twitchdl.utils import parse_clip_identifier, parse_video_identifier
 
 TEST_VIDEO_PATTERNS = [
     ("702689313", "702689313"),
     ("702689313", "https://twitch.tv/videos/702689313"),
     ("702689313", "https://www.twitch.tv/videos/702689313"),
+    ("702689313", "https://m.twitch.tv/videos/702689313"),
 ]
 
 TEST_CLIP_PATTERNS = {
     ("AbrasivePlayfulMangoMau5", "AbrasivePlayfulMangoMau5"),
     ("AbrasivePlayfulMangoMau5", "https://clips.twitch.tv/AbrasivePlayfulMangoMau5"),
     ("AbrasivePlayfulMangoMau5", "https://www.twitch.tv/dracul1nx/clip/AbrasivePlayfulMangoMau5"),
+    ("AbrasivePlayfulMangoMau5", "https://m.twitch.tv/dracul1nx/clip/AbrasivePlayfulMangoMau5"),
     ("AbrasivePlayfulMangoMau5", "https://twitch.tv/dracul1nx/clip/AbrasivePlayfulMangoMau5"),
     ("HungryProudRadicchioDoggo", "HungryProudRadicchioDoggo"),
     ("HungryProudRadicchioDoggo", "https://clips.twitch.tv/HungryProudRadicchioDoggo"),
     ("HungryProudRadicchioDoggo", "https://www.twitch.tv/bananasaurus_rex/clip/HungryProudRadicchioDoggo?filter=clips&range=7d&sort=time"),
+    ("HungryProudRadicchioDoggo", "https://m.twitch.tv/bananasaurus_rex/clip/HungryProudRadicchioDoggo?filter=clips&range=7d&sort=time"),
     ("HungryProudRadicchioDoggo", "https://twitch.tv/bananasaurus_rex/clip/HungryProudRadicchioDoggo?filter=clips&range=7d&sort=time"),
     ("GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ", "GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ"),
     ("GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ", "https://twitch.tv/dracul1nx/clip/GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ"),
     ("GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ", "https://twitch.tv/dracul1nx/clip/GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ?filter=clips&range=7d&sort=time"),
     ("GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ", "https://www.twitch.tv/dracul1nx/clip/GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ?filter=clips&range=7d&sort=time"),
+    ("GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ", "https://m.twitch.tv/dracul1nx/clip/GloriousColdbloodedTortoiseRuleFive-E017utJ4DZmHVpfQ?filter=clips&range=7d&sort=time"),
 }
 
 
 @pytest.mark.parametrize("expected,input", TEST_VIDEO_PATTERNS)
-def test_video_patterns(expected, input):
+def test_video_patterns(expected: str, input: str):
     assert parse_video_identifier(input) == expected
 
 
 @pytest.mark.parametrize("expected,input", TEST_CLIP_PATTERNS)
-def test_clip_patterns(expected, input):
+def test_clip_patterns(expected: str, input: str):
     assert parse_clip_identifier(input) == expected
```

### Comparing `twitch_dl-2.2.3/tests/test_progress.py` & `twitch_dl-2.2.4/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitch-dl.1.scd` & `twitch_dl-2.2.4/twitch-dl.1.scd`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitch_dl.egg-info/PKG-INFO` & `twitch_dl-2.2.4/twitch_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.3
+Version: 2.2.4
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch_dl-2.2.3/twitch_dl.egg-info/SOURCES.txt` & `twitch_dl-2.2.4/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/cli.py` & `twitch_dl-2.2.4/twitchdl/cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/commands/clips.py` & `twitch_dl-2.2.4/twitchdl/commands/clips.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/commands/download.py` & `twitch_dl-2.2.4/twitchdl/commands/download.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/commands/info.py` & `twitch_dl-2.2.4/twitchdl/commands/info.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/commands/videos.py` & `twitch_dl-2.2.4/twitchdl/commands/videos.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/download.py` & `twitch_dl-2.2.4/twitchdl/download.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/entities.py` & `twitch_dl-2.2.4/twitchdl/entities.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/http.py` & `twitch_dl-2.2.4/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/output.py` & `twitch_dl-2.2.4/twitchdl/output.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/playlists.py` & `twitch_dl-2.2.4/twitchdl/playlists.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/progress.py` & `twitch_dl-2.2.4/twitchdl/progress.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/twitch.py` & `twitch_dl-2.2.4/twitchdl/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.2.3/twitchdl/utils.py` & `twitch_dl-2.2.4/twitchdl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,21 +80,21 @@
     value = re.sub(r"[^\w\s\[\]().-]", "", value)
     value = re.sub(r"\s+", " ", value)
     return value.strip()
 
 
 VIDEO_PATTERNS = [
     r"^(?P<id>\d+)?$",
-    r"^https://(www.)?twitch.tv/videos/(?P<id>\d+)(\?.+)?$",
+    r"^https://(www\.|m\.)?twitch\.tv/videos/(?P<id>\d+)(\?.+)?$",
 ]
 
 CLIP_PATTERNS = [
     r"^(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)$",
-    r"^https://(www.)?twitch.tv/\w+/clip/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
-    r"^https://clips.twitch.tv/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
+    r"^https://(www\.|m\.)?twitch\.tv/\w+/clip/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
+    r"^https://clips\.twitch\.tv/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
 ]
 
 
 def parse_video_identifier(identifier: str) -> Optional[str]:
     """Given a video ID or URL returns the video ID, or null if not matched"""
     for pattern in VIDEO_PATTERNS:
         match = re.match(pattern, identifier)
```


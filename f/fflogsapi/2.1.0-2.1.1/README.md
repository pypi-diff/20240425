# Comparing `tmp/fflogsapi-2.1.0.tar.gz` & `tmp/fflogsapi-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fflogsapi-2.1.0.tar", last modified: Wed Apr  3 19:56:27 2024, max compression
+gzip compressed data, was "fflogsapi-2.1.1.tar", last modified: Thu Apr 25 18:52:14 2024, max compression
```

## Comparing `fflogsapi-2.1.0.tar` & `fflogsapi-2.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.175485 fflogsapi-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-03 19:56:27.175485 fflogsapi-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.163485 fflogsapi-2.1.0/fflogsapi/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/characters/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/character.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/game/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/guilds/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/prograce/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/prograce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/prograce/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/prograce/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/fight.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/user/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/util/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/gql_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/world/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/encounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:56:27.175485 fflogsapi-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.086902 fflogsapi-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-25 18:52:14.086902 fflogsapi-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.074902 fflogsapi-2.1.1/fflogsapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.078902 fflogsapi-2.1.1/fflogsapi/characters/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/characters/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/characters/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/characters/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.078902 fflogsapi-2.1.1/fflogsapi/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/data/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/data/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/data/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.078902 fflogsapi-2.1.1/fflogsapi/game/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/game/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/game/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/game/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.078902 fflogsapi-2.1.1/fflogsapi/guilds/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/guilds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/guilds/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/guilds/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/guilds/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/guilds/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.078902 fflogsapi-2.1.1/fflogsapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.078902 fflogsapi-2.1.1/fflogsapi/prograce/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/prograce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/prograce/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/prograce/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.082902 fflogsapi-2.1.1/fflogsapi/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/reports/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/reports/fight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/reports/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/reports/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/reports/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.082902 fflogsapi-2.1.1/fflogsapi/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/user/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/user/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/user_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.082902 fflogsapi-2.1.1/fflogsapi/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/util/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/util/gql_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/util/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.082902 fflogsapi-2.1.1/fflogsapi/world/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/fflogsapi/world/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:52:14.082902 fflogsapi-2.1.1/fflogsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-25 18:52:14.000000 fflogsapi-2.1.1/fflogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-25 18:52:14.000000 fflogsapi-2.1.1/fflogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:52:14.000000 fflogsapi-2.1.1/fflogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-25 18:52:14.000000 fflogsapi-2.1.1/fflogsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 18:52:14.000000 fflogsapi-2.1.1/fflogsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-25 18:52:07.000000 fflogsapi-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:52:14.086902 fflogsapi-2.1.1/setup.cfg
```

### Comparing `fflogsapi-2.1.0/LICENSE` & `fflogsapi-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/PKG-INFO` & `fflogsapi-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fflogsapi
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client for the FF Logs v2 API
 Author-email: Markus Wang Halvorsen <mwh@halvorsenfamilien.com>
 Project-URL: Repository, https://github.com/halworsen/fflogsapi
 Keywords: api,client,ffxiv,fflogs,lazy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -75,15 +75,15 @@
 
 from fflogsapi import FFLogsClient
 
 client = FFLogsClient(CLIENT_ID, CLIENT_SECRET)
 report = client.get_report('rGARYmQwTKbahXz9')
 
 for fight in report:
-    print(f'Fight #{fight.fight_id}:', fight.name(), f'- Kill: {fight.is_kill()}')
+    print(f'Fight #{fight.id}:', fight.name(), f'- Kill: {fight.is_kill()}')
     pot_table = fight.table(filters={'sourceAurasPresent': 'Medicated'})
     potted_damage = 0
     for damage in pot_table['damageDone']:
         potted_damage += damage['total']
     print(f'Damage done under pots: {potted_damage}')
     if not fight.is_kill():
         print(f'Percentage reached: {fight.percentage()}')
@@ -113,17 +113,17 @@
 
 ```python
 from config import CLIENT_ID, CLIENT_SECRET
 
 from fflogsapi import FFLogsClient, GQLEnum, FightDifficulty
 
 client = FFLogsClient(CLIENT_ID, CLIENT_SECRET)
-character = fapi.get_character(id=19181640)
+character = client.get_character(id=19181640)
 
-abyssos = fapi.get_zone(id=49)
+abyssos = client.get_zone(id=49)
 partition_628 = next(filter(
     lambda p: '6.28' in p.name,
     abyssos.partitions()
 ))
 
 rankings = character.zone_rankings(filters={
     'specName': 'Reaper',
```

### Comparing `fflogsapi-2.1.0/README.md` & `fflogsapi-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 from fflogsapi import FFLogsClient
 
 client = FFLogsClient(CLIENT_ID, CLIENT_SECRET)
 report = client.get_report('rGARYmQwTKbahXz9')
 
 for fight in report:
-    print(f'Fight #{fight.fight_id}:', fight.name(), f'- Kill: {fight.is_kill()}')
+    print(f'Fight #{fight.id}:', fight.name(), f'- Kill: {fight.is_kill()}')
     pot_table = fight.table(filters={'sourceAurasPresent': 'Medicated'})
     potted_damage = 0
     for damage in pot_table['damageDone']:
         potted_damage += damage['total']
     print(f'Damage done under pots: {potted_damage}')
     if not fight.is_kill():
         print(f'Percentage reached: {fight.percentage()}')
@@ -83,17 +83,17 @@
 
 ```python
 from config import CLIENT_ID, CLIENT_SECRET
 
 from fflogsapi import FFLogsClient, GQLEnum, FightDifficulty
 
 client = FFLogsClient(CLIENT_ID, CLIENT_SECRET)
-character = fapi.get_character(id=19181640)
+character = client.get_character(id=19181640)
 
-abyssos = fapi.get_zone(id=49)
+abyssos = client.get_zone(id=49)
 partition_628 = next(filter(
     lambda p: '6.28' in p.name,
     abyssos.partitions()
 ))
 
 rankings = character.zone_rankings(filters={
     'specName': 'Reaper',
```

### Comparing `fflogsapi-2.1.0/fflogsapi/__init__.py` & `fflogsapi-2.1.1/fflogsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/characters/character.py` & `fflogsapi-2.1.1/fflogsapi/characters/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,18 +173,18 @@
                 best_job=best_job,
                 rank_percent=rank['rankPercent'],
                 rank_total_parses=rank['rankTotalParses'],
                 historical_percent=rank['historicalPercent'],
                 historical_total_parses=rank['historicalTotalParses'],
                 today_percent=rank['todayPercent'],
                 today_total_parses=rank['todayTotalParses'],
-                adps=rank['aDPS'],
-                rdps=rank['rDPS'],
-                ndps=rank['nDPS'],
-                pdps=rank['pDPS'],
+                adps=rank.get('aDPS'),
+                rdps=rank.get('rDPS'),
+                ndps=rank.get('nDPS'),
+                pdps=rank.get('pDPS'),
             ))
 
         from ..world.zone import FFLogsZone
         return FFLogsEncounterRankings(
             zone=FFLogsZone(id=result['zone'], client=self._client),
             difficulty=result['difficulty'],
             metric=result['metric'],
```

### Comparing `fflogsapi-2.1.0/fflogsapi/characters/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/characters/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/client.py` & `fflogsapi-2.1.1/fflogsapi/client.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/constants.py` & `fflogsapi-2.1.1/fflogsapi/constants.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/data/__init__.py` & `fflogsapi-2.1.1/fflogsapi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/data/dataclasses.py` & `fflogsapi-2.1.1/fflogsapi/data/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 
     guild: Optional['FFLogsGuild']
     fight: 'FFLogsFight'
 
     job: 'FFJob'
     best_job: 'FFJob'
 
-    adps: float
-    rdps: float
-    ndps: float
-    pdps: float
+    adps: Optional[float]
+    rdps: Optional[float]
+    ndps: Optional[float]
+    pdps: Optional[float]
 
 
 @dataclass
 class FFLogsEncounterRankings:
     '''
     Ranking information for a character on a specific encounter (boss)
     '''
```

### Comparing `fflogsapi-2.1.0/fflogsapi/data/page.py` & `fflogsapi-2.1.1/fflogsapi/data/page.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/game/__init__.py` & `fflogsapi-2.1.1/fflogsapi/game/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/game/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/game/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/game/pages.py` & `fflogsapi-2.1.1/fflogsapi/game/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/game/queries.py` & `fflogsapi-2.1.1/fflogsapi/game/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/guilds/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/guilds/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/guilds/guild.py` & `fflogsapi-2.1.1/fflogsapi/guilds/guild.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/guilds/pages.py` & `fflogsapi-2.1.1/fflogsapi/guilds/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/guilds/queries.py` & `fflogsapi-2.1.1/fflogsapi/guilds/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/prograce/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/prograce/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/reports/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/reports/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/reports/fight.py` & `fflogsapi-2.1.1/fflogsapi/reports/fight.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/reports/pages.py` & `fflogsapi-2.1.1/fflogsapi/reports/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/reports/queries.py` & `fflogsapi-2.1.1/fflogsapi/reports/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/reports/report.py` & `fflogsapi-2.1.1/fflogsapi/reports/report.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/user/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/user/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/user/user.py` & `fflogsapi-2.1.1/fflogsapi/user/user.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/user_auth.py` & `fflogsapi-2.1.1/fflogsapi/user_auth.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/util/decorators.py` & `fflogsapi-2.1.1/fflogsapi/util/decorators.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/util/filters.py` & `fflogsapi-2.1.1/fflogsapi/util/filters.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/__init__.py` & `fflogsapi-2.1.1/fflogsapi/world/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/client_extensions.py` & `fflogsapi-2.1.1/fflogsapi/world/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/encounter.py` & `fflogsapi-2.1.1/fflogsapi/world/encounter.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/expansion.py` & `fflogsapi-2.1.1/fflogsapi/world/expansion.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/pages.py` & `fflogsapi-2.1.1/fflogsapi/world/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/queries.py` & `fflogsapi-2.1.1/fflogsapi/world/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/region.py` & `fflogsapi-2.1.1/fflogsapi/world/region.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/server.py` & `fflogsapi-2.1.1/fflogsapi/world/server.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi/world/zone.py` & `fflogsapi-2.1.1/fflogsapi/world/zone.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/fflogsapi.egg-info/PKG-INFO` & `fflogsapi-2.1.1/fflogsapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fflogsapi
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client for the FF Logs v2 API
 Author-email: Markus Wang Halvorsen <mwh@halvorsenfamilien.com>
 Project-URL: Repository, https://github.com/halworsen/fflogsapi
 Keywords: api,client,ffxiv,fflogs,lazy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -75,15 +75,15 @@
 
 from fflogsapi import FFLogsClient
 
 client = FFLogsClient(CLIENT_ID, CLIENT_SECRET)
 report = client.get_report('rGARYmQwTKbahXz9')
 
 for fight in report:
-    print(f'Fight #{fight.fight_id}:', fight.name(), f'- Kill: {fight.is_kill()}')
+    print(f'Fight #{fight.id}:', fight.name(), f'- Kill: {fight.is_kill()}')
     pot_table = fight.table(filters={'sourceAurasPresent': 'Medicated'})
     potted_damage = 0
     for damage in pot_table['damageDone']:
         potted_damage += damage['total']
     print(f'Damage done under pots: {potted_damage}')
     if not fight.is_kill():
         print(f'Percentage reached: {fight.percentage()}')
@@ -113,17 +113,17 @@
 
 ```python
 from config import CLIENT_ID, CLIENT_SECRET
 
 from fflogsapi import FFLogsClient, GQLEnum, FightDifficulty
 
 client = FFLogsClient(CLIENT_ID, CLIENT_SECRET)
-character = fapi.get_character(id=19181640)
+character = client.get_character(id=19181640)
 
-abyssos = fapi.get_zone(id=49)
+abyssos = client.get_zone(id=49)
 partition_628 = next(filter(
     lambda p: '6.28' in p.name,
     abyssos.partitions()
 ))
 
 rankings = character.zone_rankings(filters={
     'specName': 'Reaper',
```

### Comparing `fflogsapi-2.1.0/fflogsapi.egg-info/SOURCES.txt` & `fflogsapi-2.1.1/fflogsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.1.0/pyproject.toml` & `fflogsapi-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'fflogsapi'
-version = '2.1.0'
+version = '2.1.1'
 description = 'Python client for the FF Logs v2 API'
 readme = 'README.md'
 authors = [
     { name = 'Markus Wang Halvorsen', email = 'mwh@halvorsenfamilien.com' },
 ]
 keywords = ['api', 'client', 'ffxiv', 'fflogs', 'lazy']
 classifiers = [
```


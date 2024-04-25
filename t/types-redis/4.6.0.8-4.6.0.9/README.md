# Comparing `tmp/types-redis-4.6.0.8.tar.gz` & `tmp/types-redis-4.6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-redis-4.6.0.8.tar", last modified: Fri Oct 27 02:14:04 2023, max compression
+gzip compressed data, was "types-redis-4.6.0.9.tar", last modified: Fri Nov  3 02:16:08 2023, max compression
```

## Comparing `types-redis-4.6.0.8.tar` & `types-redis-4.6.0.9.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2023-10-27 02:14:03.000000 types-redis-4.6.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-27 02:14:03.000000 types-redis-4.6.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.327611 types-redis-4.6.0.8/redis-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-27 02:14:03.000000 types-redis-4.6.0.8/redis-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.327611 types-redis-4.6.0.8/redis-stubs/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    51907 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/asyncio/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/backoff.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    41584 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/cluster.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.327611 types-redis-4.6.0.8/redis-stubs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.327611 types-redis-4.6.0.8/redis-stubs/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/bf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/bf/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/bf/info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    72645 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/redis-stubs/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/edge.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/node.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/path.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/graph/query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/redis-stubs/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/json/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/json/decoders.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/json/path.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/redismodules.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/redis-stubs/commands/search/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/search/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/search/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/search/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/search/result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/sentinel.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/redis-stubs/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/timeseries/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/timeseries/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/timeseries/info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/commands/timeseries/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/ocsp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-10-27 02:13:24.000000 types-redis-4.6.0.8/redis-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2023-10-27 02:14:03.000000 types-redis-4.6.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 02:14:04.331611 types-redis-4.6.0.8/types_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-10-27 02:14:04.000000 types-redis-4.6.0.8/types_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-10-27 02:14:04.000000 types-redis-4.6.0.8/types_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 02:14:04.000000 types-redis-4.6.0.8/types_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-27 02:14:04.000000 types-redis-4.6.0.8/types_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-27 02:14:04.000000 types-redis-4.6.0.8/types_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.956371 types-redis-4.6.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    13787 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-11-03 02:16:08.956371 types-redis-4.6.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.948371 types-redis-4.6.0.9/redis-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/redis-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.952371 types-redis-4.6.0.9/redis-stubs/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51907 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/asyncio/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/backoff.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    41708 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/cluster.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.952371 types-redis-4.6.0.9/redis-stubs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.952371 types-redis-4.6.0.9/redis-stubs/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/bf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/bf/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/bf/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    72645 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.952371 types-redis-4.6.0.9/redis-stubs/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/edge.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/graph/query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.952371 types-redis-4.6.0.9/redis-stubs/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/json/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/json/decoders.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/json/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/redismodules.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.952371 types-redis-4.6.0.9/redis-stubs/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/search/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/search/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/search/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/search/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/sentinel.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.956371 types-redis-4.6.0.9/redis-stubs/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/timeseries/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/timeseries/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/timeseries/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/commands/timeseries/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/ocsp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/redis-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2023-11-03 02:15:39.000000 types-redis-4.6.0.9/redis-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 02:16:08.956371 types-redis-4.6.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 02:16:08.956371 types-redis-4.6.0.9/types_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/types_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/types_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/types_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/types_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-03 02:16:08.000000 types-redis-4.6.0.9/types_redis.egg-info/top_level.txt
```

### Comparing `types-redis-4.6.0.8/CHANGELOG.md` & `types-redis-4.6.0.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.6.0.9 (2023-11-03)
+
+Add retry_on_error params for redis stub (#10961)
+
 ## 4.6.0.8 (2023-10-27)
 
 Remove many redundant inheritances from `Generic[]` (#10933)
 
 ## 4.6.0.7 (2023-09-23)
 
 Add overloads to redis.asyncio.Redis (#10742)
```

### Comparing `types-redis-4.6.0.8/PKG-INFO` & `types-redis-4.6.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.6.0.8
+Version: 4.6.0.9
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Note: Redis-py 5.0.0 added a py.typed file, but the inline annotations are incomplete. Continuing to use `types-redis` for the time being may lead to superior results.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1c184fea33d50ba430410cf1b25d4aea2df2981e` and was tested
-with mypy 1.6.1, pyright 1.1.332, and
+This package was generated from typeshed commit `19650767da0bcd01b8e9dc98b4b873522edbf6f9` and was tested
+with mypy 1.6.1, pyright 1.1.334, and
 pytype 2023.10.17.
```

### Comparing `types-redis-4.6.0.8/redis-stubs/METADATA.toml` & `types-redis-4.6.0.9/redis-stubs/METADATA.toml`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/client.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/cluster.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/connection.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/lock.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/retry.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/sentinel.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/asyncio/utils.pyi` & `types-redis-4.6.0.9/redis-stubs/asyncio/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/backoff.pyi` & `types-redis-4.6.0.9/redis-stubs/backoff.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/client.pyi` & `types-redis-4.6.0.9/redis-stubs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         charset: str | None = None,
         errors: str | None = None,
         *,
         decode_responses: Literal[True],
         retry_on_timeout: bool = False,
+        retry_on_error: list[type[RedisError]] | None = None,
         ssl: bool = False,
         ssl_keyfile: str | None = None,
         ssl_certfile: str | None = None,
         ssl_cert_reqs: str | int | None = "required",
         ssl_ca_certs: str | None = None,
         ssl_ca_data: Incomplete | None = None,
         ssl_check_hostname: bool = False,
@@ -249,14 +250,15 @@
         unix_socket_path: str | None = None,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         charset: str | None = None,
         errors: str | None = None,
         decode_responses: Literal[False] = False,
         retry_on_timeout: bool = False,
+        retry_on_error: list[type[RedisError]] | None = None,
         ssl: bool = False,
         ssl_keyfile: str | None = None,
         ssl_certfile: str | None = None,
         ssl_cert_reqs: str | int | None = "required",
         ssl_ca_certs: str | None = None,
         ssl_ca_data: Incomplete | None = None,
         ssl_check_hostname: bool = False,
```

### Comparing `types-redis-4.6.0.8/redis-stubs/cluster.pyi` & `types-redis-4.6.0.9/redis-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/bf/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/bf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/bf/commands.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/bf/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/bf/info.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/bf/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/cluster.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/core.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/core.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/graph/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/graph/commands.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/graph/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/graph/query_result.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/graph/query_result.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/json/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/json/commands.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/json/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/search/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/search/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/search/aggregation.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/search/aggregation.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/search/commands.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/search/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/search/query.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/search/query.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/sentinel.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/timeseries/__init__.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/timeseries/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/timeseries/commands.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/timeseries/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/commands/timeseries/info.pyi` & `types-redis-4.6.0.9/redis-stubs/commands/timeseries/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/connection.pyi` & `types-redis-4.6.0.9/redis-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/exceptions.pyi` & `types-redis-4.6.0.9/redis-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/lock.pyi` & `types-redis-4.6.0.9/redis-stubs/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/ocsp.pyi` & `types-redis-4.6.0.9/redis-stubs/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/sentinel.pyi` & `types-redis-4.6.0.9/redis-stubs/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/typing.pyi` & `types-redis-4.6.0.9/redis-stubs/typing.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/redis-stubs/utils.pyi` & `types-redis-4.6.0.9/redis-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.6.0.8/setup.py` & `types-redis-4.6.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 Note: Redis-py 5.0.0 added a py.typed file, but the inline annotations are incomplete. Continuing to use `types-redis` for the time being may lead to superior results.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1c184fea33d50ba430410cf1b25d4aea2df2981e` and was tested
-with mypy 1.6.1, pyright 1.1.332, and
+This package was generated from typeshed commit `19650767da0bcd01b8e9dc98b4b873522edbf6f9` and was tested
+with mypy 1.6.1, pyright 1.1.334, and
 pytype 2023.10.17.
 '''.lstrip()
 
 setup(name=name,
-      version="4.6.0.8",
+      version="4.6.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md",
```

### Comparing `types-redis-4.6.0.8/types_redis.egg-info/PKG-INFO` & `types-redis-4.6.0.9/types_redis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.6.0.8
+Version: 4.6.0.9
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Note: Redis-py 5.0.0 added a py.typed file, but the inline annotations are incomplete. Continuing to use `types-redis` for the time being may lead to superior results.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1c184fea33d50ba430410cf1b25d4aea2df2981e` and was tested
-with mypy 1.6.1, pyright 1.1.332, and
+This package was generated from typeshed commit `19650767da0bcd01b8e9dc98b4b873522edbf6f9` and was tested
+with mypy 1.6.1, pyright 1.1.334, and
 pytype 2023.10.17.
```

### Comparing `types-redis-4.6.0.8/types_redis.egg-info/SOURCES.txt` & `types-redis-4.6.0.9/types_redis.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 redis-stubs/cluster.pyi
 redis-stubs/connection.pyi
 redis-stubs/crc.pyi
 redis-stubs/credentials.pyi
 redis-stubs/exceptions.pyi
 redis-stubs/lock.pyi
 redis-stubs/ocsp.pyi
+redis-stubs/py.typed
 redis-stubs/retry.pyi
 redis-stubs/sentinel.pyi
 redis-stubs/typing.pyi
 redis-stubs/utils.pyi
 redis-stubs/asyncio/__init__.pyi
 redis-stubs/asyncio/client.pyi
 redis-stubs/asyncio/cluster.pyi
```


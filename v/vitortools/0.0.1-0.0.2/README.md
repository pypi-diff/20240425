# Comparing `tmp/vitortools-0.0.1.tar.gz` & `tmp/vitortools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitortools-0.0.1.tar", last modified: Thu Apr 25 01:00:28 2024, max compression
+gzip compressed data, was "vitortools-0.0.2.tar", last modified: Thu Apr 25 01:10:19 2024, max compression
```

## Comparing `vitortools-0.0.1.tar` & `vitortools-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:00:28.518632 vitortools-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-25 01:00:28.517631 vitortools-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 01:00:28.518632 vitortools-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:00:28.516631 vitortools-0.0.1/vitortools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:00:28.516631 vitortools-0.0.1/vitortools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:00:28.517631 vitortools-0.0.1/vitortools/src/vitortools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-25 01:00:28.000000 vitortools-0.0.1/vitortools/src/vitortools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2024-04-25 01:00:28.000000 vitortools-0.0.1/vitortools/src/vitortools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 01:00:28.000000 vitortools-0.0.1/vitortools/src/vitortools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 01:00:28.000000 vitortools-0.0.1/vitortools/src/vitortools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:10:19.152089 vitortools-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-25 01:10:19.152089 vitortools-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 01:10:19.152089 vitortools-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:10:19.148089 vitortools-0.0.2/vitortools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:10:19.148089 vitortools-0.0.2/vitortools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:10:19.149089 vitortools-0.0.2/vitortools/src/vitortools/
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-25 01:10:17.000000 vitortools-0.0.2/vitortools/src/vitortools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-25 01:10:15.000000 vitortools-0.0.2/vitortools/src/vitortools/vitortools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:10:19.151089 vitortools-0.0.2/vitortools/src/vitortools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-25 01:10:19.000000 vitortools-0.0.2/vitortools/src/vitortools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      285 2024-04-25 01:10:19.000000 vitortools-0.0.2/vitortools/src/vitortools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 01:10:19.000000 vitortools-0.0.2/vitortools/src/vitortools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-25 01:10:19.000000 vitortools-0.0.2/vitortools/src/vitortools.egg-info/top_level.txt
```


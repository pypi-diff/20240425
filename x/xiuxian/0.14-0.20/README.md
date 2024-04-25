# Comparing `tmp/xiuxian-0.14.tar.gz` & `tmp/xiuxian-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuxian-0.14.tar", last modified: Fri Apr 12 14:29:25 2024, max compression
+gzip compressed data, was "xiuxian-0.20.tar", last modified: Thu Apr 25 01:37:41 2024, max compression
```

## Comparing `xiuxian-0.14.tar` & `xiuxian-0.20.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:25.895202 xiuxian-0.14/
--rw-rw-rw-   0        0        0      212 2024-04-12 14:29:25.893966 xiuxian-0.14/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-12 14:29:25.895202 xiuxian-0.14/setup.cfg
--rw-rw-rw-   0        0        0      446 2024-04-12 14:29:23.000000 xiuxian-0.14/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:29:25.893966 xiuxian-0.14/xiuxian.egg-info/
--rw-rw-rw-   0        0        0      212 2024-04-12 14:29:25.000000 xiuxian-0.14/xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2024-04-12 14:29:25.000000 xiuxian-0.14/xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:29:25.000000 xiuxian-0.14/xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 14:29:25.000000 xiuxian-0.14/xiuxian.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 01:37:41.640719 xiuxian-0.20/
+-rw-rw-rw-   0        0        0      246 2024-04-25 01:37:41.639727 xiuxian-0.20/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-25 01:37:41.640719 xiuxian-0.20/setup.cfg
+-rw-rw-rw-   0        0        0      480 2024-04-25 01:34:25.000000 xiuxian-0.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:37:41.639727 xiuxian-0.20/xiuxian.egg-info/
+-rw-rw-rw-   0        0        0      246 2024-04-25 01:37:41.000000 xiuxian-0.20/xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2024-04-25 01:37:41.000000 xiuxian-0.20/xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 01:37:41.000000 xiuxian-0.20/xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 01:37:41.000000 xiuxian-0.20/xiuxian.egg-info/top_level.txt
```


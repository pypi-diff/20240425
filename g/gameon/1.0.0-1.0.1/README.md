# Comparing `tmp/gameon-1.0.0.tar.gz` & `tmp/gameon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameon-1.0.0.tar", last modified: Thu Apr 25 14:52:06 2024, max compression
+gzip compressed data, was "gameon-1.0.1.tar", last modified: Thu Apr 25 15:07:12 2024, max compression
```

## Comparing `gameon-1.0.0.tar` & `gameon-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:52:06.621647 gameon-1.0.0/
--rw-rw-rw-   0        0        0       81 2024-04-25 14:51:36.000000 gameon-1.0.0/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 14:52:06.609327 gameon-1.0.0/GameOn/
--rw-rw-rw-   0        0        0     9674 2024-04-25 13:41:52.000000 gameon-1.0.0/GameOn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:52:06.619354 gameon-1.0.0/GameOn.egg-info/
--rw-rw-rw-   0        0        0      262 2024-04-25 14:52:06.000000 gameon-1.0.0/GameOn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-25 14:52:06.000000 gameon-1.0.0/GameOn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:52:06.000000 gameon-1.0.0/GameOn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-25 14:52:06.000000 gameon-1.0.0/GameOn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 14:52:06.000000 gameon-1.0.0/GameOn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.0/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      262 2024-04-25 14:52:06.620644 gameon-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.0/README.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 14:52:06.621647 gameon-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-04-25 14:50:13.000000 gameon-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:07:12.488386 gameon-1.0.1/
+-rw-rw-rw-   0        0        0      144 2024-04-25 15:06:57.000000 gameon-1.0.1/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 15:07:12.475555 gameon-1.0.1/GameOn/
+-rw-rw-rw-   0        0        0     9674 2024-04-25 13:41:52.000000 gameon-1.0.1/GameOn/__init__.py
+-rw-rw-rw-   0        0        0     9674 2024-04-25 13:43:15.000000 gameon-1.0.1/GameOn/__init__.txt
+-rw-rw-rw-   0        0        0      857 2024-04-25 13:42:42.000000 gameon-1.0.1/GameOn/engine.txt
+-rw-rw-rw-   0        0        0        0 2024-04-25 14:48:28.000000 gameon-1.0.1/GameOn/game.py
+-rw-rw-rw-   0        0        0     1060 2022-07-06 14:58:58.000000 gameon-1.0.1/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2022-07-06 14:59:00.000000 gameon-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2024-04-25 15:07:12.487383 gameon-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2022-07-06 14:47:52.000000 gameon-1.0.1/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 15:07:12.486085 gameon-1.0.1/gameon.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-25 15:07:12.000000 gameon-1.0.1/gameon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-25 15:07:12.000000 gameon-1.0.1/gameon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:07:12.000000 gameon-1.0.1/gameon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-25 15:07:12.000000 gameon-1.0.1/gameon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 15:07:12.000000 gameon-1.0.1/gameon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:07:12.488386 gameon-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-04-25 15:06:37.000000 gameon-1.0.1/setup.py
```

### Comparing `gameon-1.0.0/GameOn/__init__.py` & `gameon-1.0.1/GameOn/__init__.py`

 * *Files identical despite different names*

### Comparing `gameon-1.0.0/LICENCE.txt` & `gameon-1.0.1/LICENCE.txt`

 * *Files identical despite different names*


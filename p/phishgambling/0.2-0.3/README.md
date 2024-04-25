# Comparing `tmp/phishgambling-0.2.tar.gz` & `tmp/phishgambling-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phishgambling-0.2.tar", last modified: Tue Apr 23 20:32:10 2024, max compression
+gzip compressed data, was "phishgambling-0.3.tar", last modified: Thu Apr 25 15:11:19 2024, max compression
```

## Comparing `phishgambling-0.2.tar` & `phishgambling-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 20:32:10.554886 phishgambling-0.2/
--rw-rw-rw-   0        0        0      128 2024-04-23 20:32:10.552891 phishgambling-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 20:17:27.000000 phishgambling-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 20:32:10.532241 phishgambling-0.2/phishgambling/
--rw-rw-rw-   0        0        0       24 2024-04-23 20:20:40.000000 phishgambling-0.2/phishgambling/__init__.py
--rw-rw-rw-   0        0        0     1696 2024-04-23 20:31:20.000000 phishgambling-0.2/phishgambling/main.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:32:10.550932 phishgambling-0.2/phishgambling.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 20:32:10.554886 phishgambling-0.2/setup.cfg
--rw-rw-rw-   0        0        0      439 2024-04-23 20:31:44.000000 phishgambling-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:11:19.611663 phishgambling-0.3/
+-rw-rw-rw-   0        0        0      128 2024-04-25 15:11:19.609663 phishgambling-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 20:17:27.000000 phishgambling-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 15:11:19.588547 phishgambling-0.3/phishgambling/
+-rw-rw-rw-   0        0        0       24 2024-04-23 20:20:40.000000 phishgambling-0.3/phishgambling/__init__.py
+-rw-rw-rw-   0        0        0     2672 2024-04-25 14:03:46.000000 phishgambling-0.3/phishgambling/main.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:11:19.607670 phishgambling-0.3/phishgambling.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-04-25 15:11:19.000000 phishgambling-0.3/phishgambling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-25 15:11:19.000000 phishgambling-0.3/phishgambling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:11:19.000000 phishgambling-0.3/phishgambling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-25 15:11:19.000000 phishgambling-0.3/phishgambling.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 15:11:19.000000 phishgambling-0.3/phishgambling.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:11:19.611663 phishgambling-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      439 2024-04-25 15:11:14.000000 phishgambling-0.3/setup.py
```


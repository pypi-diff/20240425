# Comparing `tmp/kmscalculator-0.0.1.tar.gz` & `tmp/kmscalculator-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmscalculator-0.0.1.tar", last modified: Thu Apr 25 06:58:53 2024, max compression
+gzip compressed data, was "kmscalculator-0.1.tar", last modified: Thu Apr 25 06:32:03 2024, max compression
```

## Comparing `kmscalculator-0.0.1.tar` & `kmscalculator-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 06:58:53.575770 kmscalculator-0.0.1/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      327 2024-04-25 06:58:53.575610 kmscalculator-0.0.1/PKG-INFO
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 06:58:53.574646 kmscalculator-0.0.1/calculator/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 05:29:41.000000 kmscalculator-0.0.1/calculator/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      100 2024-04-25 06:24:24.000000 kmscalculator-0.0.1/calculator/calculate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 06:58:53.575443 kmscalculator-0.0.1/kmscalculator.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      327 2024-04-25 06:58:53.000000 kmscalculator-0.0.1/kmscalculator.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      203 2024-04-25 06:58:53.000000 kmscalculator-0.0.1/kmscalculator.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-04-25 06:58:53.000000 kmscalculator-0.0.1/kmscalculator.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       11 2024-04-25 06:58:53.000000 kmscalculator-0.0.1/kmscalculator.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-04-25 06:58:53.575810 kmscalculator-0.0.1/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      486 2024-04-25 06:58:45.000000 kmscalculator-0.0.1/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 06:32:03.567875 kmscalculator-0.1/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      138 2024-04-25 06:32:03.567721 kmscalculator-0.1/PKG-INFO
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 06:32:03.566837 kmscalculator-0.1/calculator/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 05:29:41.000000 kmscalculator-0.1/calculator/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      100 2024-04-25 06:24:24.000000 kmscalculator-0.1/calculator/calculate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 06:32:03.567566 kmscalculator-0.1/kmscalculator.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      138 2024-04-25 06:32:03.000000 kmscalculator-0.1/kmscalculator.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      203 2024-04-25 06:32:03.000000 kmscalculator-0.1/kmscalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-04-25 06:32:03.000000 kmscalculator-0.1/kmscalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       11 2024-04-25 06:32:03.000000 kmscalculator-0.1/kmscalculator.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-04-25 06:32:03.567912 kmscalculator-0.1/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      234 2024-04-25 06:25:59.000000 kmscalculator-0.1/setup.py
```


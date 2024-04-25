# Comparing `tmp/poke_alan-1.0.0.tar.gz` & `tmp/poke_alan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poke_alan-1.0.0.tar", last modified: Tue Apr 23 18:48:30 2024, max compression
+gzip compressed data, was "poke_alan-1.0.1.tar", last modified: Thu Apr 25 19:11:17 2024, max compression
```

## Comparing `poke_alan-1.0.0.tar` & `poke_alan-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:48:30.724140 poke_alan-1.0.0/
--rw-rw-rw-   0        0        0      200 2024-04-23 18:48:30.722139 poke_alan-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 18:48:30.720142 poke_alan-1.0.0/Poke_Alan.egg-info/
--rw-rw-rw-   0        0        0      200 2024-04-23 18:48:30.000000 poke_alan-1.0.0/Poke_Alan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-23 18:48:30.000000 poke_alan-1.0.0/Poke_Alan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:48:30.000000 poke_alan-1.0.0/Poke_Alan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 18:48:30.000000 poke_alan-1.0.0/Poke_Alan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-23 18:48:30.000000 poke_alan-1.0.0/Poke_Alan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      146 2024-04-19 15:57:10.000000 poke_alan-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:48:30.717141 poke_alan-1.0.0/poke-base/
--rw-rw-rw-   0        0        0       39 2024-04-19 15:35:18.000000 poke_alan-1.0.0/poke-base/__init__.py
--rw-rw-rw-   0        0        0     2275 2024-04-19 15:35:18.000000 poke_alan-1.0.0/poke-base/random_pokemon.py
--rw-rw-rw-   0        0        0       42 2024-04-23 18:48:30.725138 poke_alan-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      372 2024-04-23 18:48:25.000000 poke_alan-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:17.038962 poke_alan-1.0.1/
+-rw-rw-rw-   0        0        0      200 2024-04-25 19:11:17.037962 poke_alan-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:17.035861 poke_alan-1.0.1/Poke_Alan.egg-info/
+-rw-rw-rw-   0        0        0      200 2024-04-25 19:11:16.000000 poke_alan-1.0.1/Poke_Alan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-25 19:11:16.000000 poke_alan-1.0.1/Poke_Alan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:11:16.000000 poke_alan-1.0.1/Poke_Alan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 19:11:16.000000 poke_alan-1.0.1/Poke_Alan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 19:11:16.000000 poke_alan-1.0.1/Poke_Alan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      146 2024-04-19 15:57:10.000000 poke_alan-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 19:11:17.033863 poke_alan-1.0.1/poke-base/
+-rw-rw-rw-   0        0        0       39 2024-04-19 15:35:18.000000 poke_alan-1.0.1/poke-base/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-17 00:15:39.000000 poke_alan-1.0.1/poke-base/pokemon.csv
+-rw-rw-rw-   0        0        0     2275 2024-04-19 15:35:18.000000 poke_alan-1.0.1/poke-base/random_pokemon.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 19:11:17.038962 poke_alan-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      370 2024-04-25 19:11:14.000000 poke_alan-1.0.1/setup.py
```

### Comparing `poke_alan-1.0.0/poke-base/random_pokemon.py` & `poke_alan-1.0.1/poke-base/random_pokemon.py`

 * *Files identical despite different names*


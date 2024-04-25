# Comparing `tmp/pokemon_library_lmba-1.0.1.tar.gz` & `tmp/pokemon_library_lmba-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokemon_library_lmba-1.0.1.tar", last modified: Wed Apr 24 18:32:52 2024, max compression
+gzip compressed data, was "pokemon_library_lmba-1.0.2.tar", last modified: Thu Apr 25 02:33:47 2024, max compression
```

## Comparing `pokemon_library_lmba-1.0.1.tar` & `pokemon_library_lmba-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:32:52.532371 pokemon_library_lmba-1.0.1/
--rw-rw-rw-   0        0        0      213 2024-04-24 18:32:52.526659 pokemon_library_lmba-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 18:32:52.495502 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/
--rw-rw-rw-   0        0        0       40 2024-04-19 15:54:14.000000 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:17:45.000000 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/pokemon.csv
--rw-rw-rw-   0        0        0     2399 2024-04-24 18:28:00.000000 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:32:52.523154 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/
--rw-rw-rw-   0        0        0      213 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2024-04-23 17:42:25.000000 pokemon_library_lmba-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 18:32:52.533391 pokemon_library_lmba-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      406 2024-04-24 18:29:54.000000 pokemon_library_lmba-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:33:47.243019 pokemon_library_lmba-1.0.2/
+-rw-rw-rw-   0        0        0      213 2024-04-25 02:33:47.237950 pokemon_library_lmba-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 02:33:47.197131 pokemon_library_lmba-1.0.2/Pokemon_Library-Lmba/
+-rw-rw-rw-   0        0        0       41 2024-04-25 02:32:16.000000 pokemon_library_lmba-1.0.2/Pokemon_Library-Lmba/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:17:45.000000 pokemon_library_lmba-1.0.2/Pokemon_Library-Lmba/pokemon.csv
+-rw-rw-rw-   0        0        0     2399 2024-04-24 18:28:00.000000 pokemon_library_lmba-1.0.2/Pokemon_Library-Lmba/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:33:47.231825 pokemon_library_lmba-1.0.2/Pokemon_Library_Lmba.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-25 02:33:46.000000 pokemon_library_lmba-1.0.2/Pokemon_Library_Lmba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-25 02:33:47.000000 pokemon_library_lmba-1.0.2/Pokemon_Library_Lmba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:33:46.000000 pokemon_library_lmba-1.0.2/Pokemon_Library_Lmba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 02:33:46.000000 pokemon_library_lmba-1.0.2/Pokemon_Library_Lmba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-25 02:33:46.000000 pokemon_library_lmba-1.0.2/Pokemon_Library_Lmba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2024-04-23 17:42:25.000000 pokemon_library_lmba-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:33:47.243099 pokemon_library_lmba-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-04-25 02:33:26.000000 pokemon_library_lmba-1.0.2/setup.py
```

### Comparing `pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/pokemon.csv` & `pokemon_library_lmba-1.0.2/Pokemon_Library-Lmba/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/random_pokemon.py` & `pokemon_library_lmba-1.0.2/Pokemon_Library-Lmba/random_pokemon.py`

 * *Files identical despite different names*


# Comparing `tmp/pokebola-1.0.1.tar.gz` & `tmp/pokebola-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokebola-1.0.1.tar", last modified: Thu Apr 25 02:13:38 2024, max compression
+gzip compressed data, was "pokebola-1.0.2.tar", last modified: Thu Apr 25 02:31:48 2024, max compression
```

## Comparing `pokebola-1.0.1.tar` & `pokebola-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 02:13:38.738495 pokebola-1.0.1/
--rw-rw-rw-   0        0        0      196 2024-04-25 02:13:38.738495 pokebola-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 02:13:38.738495 pokebola-1.0.1/Pokebola/
--rw-rw-rw-   0        0        0       41 2024-04-25 02:10:14.000000 pokebola-1.0.1/Pokebola/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 18:31:30.000000 pokebola-1.0.1/Pokebola/pokemon.csv
--rw-rw-rw-   0        0        0     2250 2024-04-25 02:10:14.000000 pokebola-1.0.1/Pokebola/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:13:38.738495 pokebola-1.0.1/Pokebola.egg-info/
--rw-rw-rw-   0        0        0      196 2024-04-25 02:13:38.000000 pokebola-1.0.1/Pokebola.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-25 02:13:38.000000 pokebola-1.0.1/Pokebola.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:13:38.000000 pokebola-1.0.1/Pokebola.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 02:13:38.000000 pokebola-1.0.1/Pokebola.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 02:13:38.000000 pokebola-1.0.1/Pokebola.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      150 2024-04-25 02:12:21.000000 pokebola-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 02:13:38.738495 pokebola-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      368 2024-04-25 02:10:14.000000 pokebola-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:31:48.829921 pokebola-1.0.2/
+-rw-rw-rw-   0        0        0      196 2024-04-25 02:31:48.828919 pokebola-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 02:31:48.811392 pokebola-1.0.2/Pokebola/
+-rw-rw-rw-   0        0        0       41 2024-04-25 02:10:14.000000 pokebola-1.0.2/Pokebola/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 18:31:30.000000 pokebola-1.0.2/Pokebola/pokemon.csv
+-rw-rw-rw-   0        0        0     2259 2024-04-25 02:22:32.000000 pokebola-1.0.2/Pokebola/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:31:48.827553 pokebola-1.0.2/Pokebola.egg-info/
+-rw-rw-rw-   0        0        0      196 2024-04-25 02:31:48.000000 pokebola-1.0.2/Pokebola.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-25 02:31:48.000000 pokebola-1.0.2/Pokebola.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:31:48.000000 pokebola-1.0.2/Pokebola.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 02:31:48.000000 pokebola-1.0.2/Pokebola.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 02:31:48.000000 pokebola-1.0.2/Pokebola.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      150 2024-04-25 02:12:21.000000 pokebola-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:31:48.829921 pokebola-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-25 02:31:44.000000 pokebola-1.0.2/setup.py
```

### Comparing `pokebola-1.0.1/Pokebola/pokemon.csv` & `pokebola-1.0.2/Pokebola/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokebola-1.0.1/Pokebola/random_pokemon.py` & `pokebola-1.0.2/Pokebola/random_pokemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pkg_resources
 import pandas as pd
 
 class RandomPokemon:
     FILE_PATH = pkg_resources.resource_filename(__name__, 'pokemon.csv')
 
     def __init__(self):
-        self._file = pd.read_csv(self.FILE_PATH)
+        self._file = pd.read_csv(RandomPokemon.FILE_PATH)
         self._pokemon = None
         self._number = None
         self._name = None
         self._type1 = None
         self._type2 = None
         self._total = None
         self._HP = None
```


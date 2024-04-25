# Comparing `tmp/pokemon_haru-1.0.0.tar.gz` & `tmp/pokemon_haru-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokemon_haru-1.0.0.tar", last modified: Tue Apr 23 19:36:01 2024, max compression
+gzip compressed data, was "pokemon_haru-1.0.1.tar", last modified: Thu Apr 25 19:18:03 2024, max compression
```

## Comparing `pokemon_haru-1.0.0.tar` & `pokemon_haru-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 19:36:01.458560 pokemon_haru-1.0.0/
--rw-rw-rw-   0        0        0      170 2024-04-23 19:36:01.435267 pokemon_haru-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-04-19 15:57:53.000000 pokemon_haru-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 19:36:01.217529 pokemon_haru-1.0.0/pokemon_haru/
--rw-rw-rw-   0        0        0       43 2024-04-19 15:57:53.000000 pokemon_haru-1.0.0/pokemon_haru/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:35:48.000000 pokemon_haru-1.0.0/pokemon_haru/pokemon.csv
--rw-rw-rw-   0        0        0     2346 2024-04-23 18:00:26.000000 pokemon_haru-1.0.0/pokemon_haru/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:36:01.418218 pokemon_haru-1.0.0/pokemon_haru.egg-info/
--rw-rw-rw-   0        0        0      170 2024-04-23 19:36:00.000000 pokemon_haru-1.0.0/pokemon_haru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-23 19:36:00.000000 pokemon_haru-1.0.0/pokemon_haru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 19:36:00.000000 pokemon_haru-1.0.0/pokemon_haru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 19:36:00.000000 pokemon_haru-1.0.0/pokemon_haru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 19:36:00.000000 pokemon_haru-1.0.0/pokemon_haru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 19:36:01.485134 pokemon_haru-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      341 2024-04-19 15:57:53.000000 pokemon_haru-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:18:03.810880 pokemon_haru-1.0.1/
+-rw-rw-rw-   0        0        0      195 2024-04-25 19:18:03.789906 pokemon_haru-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-04-19 15:57:53.000000 pokemon_haru-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 19:18:03.659855 pokemon_haru-1.0.1/pokemon_haru/
+-rw-rw-rw-   0        0        0       43 2024-04-19 15:57:53.000000 pokemon_haru-1.0.1/pokemon_haru/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:35:48.000000 pokemon_haru-1.0.1/pokemon_haru/pokemon.csv
+-rw-rw-rw-   0        0        0     2336 2024-04-24 18:39:53.000000 pokemon_haru-1.0.1/pokemon_haru/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:18:03.778718 pokemon_haru-1.0.1/pokemon_haru.egg-info/
+-rw-rw-rw-   0        0        0      195 2024-04-25 19:18:02.000000 pokemon_haru-1.0.1/pokemon_haru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-25 19:18:03.000000 pokemon_haru-1.0.1/pokemon_haru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:18:02.000000 pokemon_haru-1.0.1/pokemon_haru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 19:18:03.000000 pokemon_haru-1.0.1/pokemon_haru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-25 19:18:03.000000 pokemon_haru-1.0.1/pokemon_haru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 19:18:03.811981 pokemon_haru-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      373 2024-04-25 19:16:13.000000 pokemon_haru-1.0.1/setup.py
```

### Comparing `pokemon_haru-1.0.0/pokemon_haru/pokemon.csv` & `pokemon_haru-1.0.1/pokemon_haru/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokemon_haru-1.0.0/pokemon_haru/random_pokemon.py` & `pokemon_haru-1.0.1/pokemon_haru/random_pokemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import pkg_resources
 
 
 class RandomPokemon:
     FILE_PATH = pkg_resources.resource_filename(__name__, "pokemon.csv")
 
-    def __init_3222222222_(self):
+    def __init__(self):
         # _ variable privada
         self._file = pd.read_csv(self.FILE_PATH)
         self._pokemon = None
         # none=vacio
         self._number = None
         self._name = None
         self._type1 = None
```


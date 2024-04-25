# Comparing `tmp/dxrt-1.0.0.tar.gz` & `tmp/dxrt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxrt-1.0.0.tar", last modified: Tue Apr 23 18:10:34 2024, max compression
+gzip compressed data, was "dxrt-1.0.1.tar", last modified: Thu Apr 25 16:24:22 2024, max compression
```

## Comparing `dxrt-1.0.0.tar` & `dxrt-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrws---   0 u0_a226  (10226) media_rw  (1023)        0 2024-04-23 18:10:34.473102 dxrt-1.0.0/
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)      175 2024-04-23 18:10:34.457102 dxrt-1.0.0/PKG-INFO
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)      121 2024-04-19 15:57:17.000000 dxrt-1.0.0/README.md
-drwxrws---   0 u0_a226  (10226) media_rw  (1023)        0 2024-04-23 18:10:34.353102 dxrt-1.0.0/dxrt/
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)       42 2024-04-19 15:57:12.000000 dxrt-1.0.0/dxrt/__init__.py
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)    44028 2024-04-16 17:45:56.000000 dxrt-1.0.0/dxrt/pokemon.csv
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)     2127 2024-04-19 15:57:10.000000 dxrt-1.0.0/dxrt/random_pokemon.py
-drwxrws---   0 u0_a226  (10226) media_rw  (1023)        0 2024-04-23 18:10:34.441102 dxrt-1.0.0/dxrt.egg-info/
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)      175 2024-04-23 18:10:34.000000 dxrt-1.0.0/dxrt.egg-info/PKG-INFO
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)      214 2024-04-23 18:10:34.000000 dxrt-1.0.0/dxrt.egg-info/SOURCES.txt
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)        1 2024-04-23 18:10:34.000000 dxrt-1.0.0/dxrt.egg-info/dependency_links.txt
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)        7 2024-04-23 18:10:34.000000 dxrt-1.0.0/dxrt.egg-info/requires.txt
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)        5 2024-04-23 18:10:34.000000 dxrt-1.0.0/dxrt.egg-info/top_level.txt
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)       38 2024-04-23 18:10:34.473102 dxrt-1.0.0/setup.cfg
--rw-rw----   0 u0_a226  (10226) media_rw  (1023)      339 2024-04-19 15:57:14.000000 dxrt-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:24:22.532333 dxrt-1.0.1/
+-rw-rw-rw-   0        0        0      182 2024-04-25 16:24:22.530918 dxrt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2024-04-19 15:57:17.000000 dxrt-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:24:22.516220 dxrt-1.0.1/dxrt/
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:57:12.000000 dxrt-1.0.1/dxrt/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:45:56.000000 dxrt-1.0.1/dxrt/pokemon.csv
+-rw-rw-rw-   0        0        0     2127 2024-04-19 15:57:10.000000 dxrt-1.0.1/dxrt/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:24:22.528901 dxrt-1.0.1/dxrt.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-25 16:24:22.000000 dxrt-1.0.1/dxrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:24:22.533347 dxrt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      332 2024-04-25 16:24:16.000000 dxrt-1.0.1/setup.py
```

### Comparing `dxrt-1.0.0/dxrt/pokemon.csv` & `dxrt-1.0.1/dxrt/pokemon.csv`

 * *Files identical despite different names*

### Comparing `dxrt-1.0.0/dxrt/random_pokemon.py` & `dxrt-1.0.1/dxrt/random_pokemon.py`

 * *Files identical despite different names*


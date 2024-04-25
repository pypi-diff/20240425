# Comparing `tmp/crawlnet-0.0.6.tar.gz` & `tmp/crawlnet-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlnet-0.0.6.tar", last modified: Tue Apr 23 18:18:38 2024, max compression
+gzip compressed data, was "crawlnet-0.0.7.tar", last modified: Thu Apr 25 16:24:40 2024, max compression
```

## Comparing `crawlnet-0.0.6.tar` & `crawlnet-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:18:38.823805 crawlnet-0.0.6/
--rw-rw-rw-   0        0        0      794 2024-04-23 18:18:38.823805 crawlnet-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:18:38.782030 crawlnet-0.0.6/crawlnet/
--rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.6/crawlnet/__init__.py
--rw-rw-rw-   0        0        0    24417 2024-04-23 18:18:01.000000 crawlnet-0.0.6/crawlnet/cl3.py
--rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.6/crawlnet/cl4.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:18:38.811401 crawlnet-0.0.6/crawlnet.egg-info/
--rw-rw-rw-   0        0        0      794 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 18:18:38.823805 crawlnet-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-04-23 18:18:36.000000 crawlnet-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:24:40.329419 crawlnet-0.0.7/
+-rw-rw-rw-   0        0        0      794 2024-04-25 16:24:40.324069 crawlnet-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:24:40.235174 crawlnet-0.0.7/crawlnet/
+-rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.7/crawlnet/__init__.py
+-rw-rw-rw-   0        0        0    24418 2024-04-25 15:37:33.000000 crawlnet-0.0.7/crawlnet/cl3.py
+-rw-rw-rw-   0        0        0    31655 2024-04-25 16:23:45.000000 crawlnet-0.0.7/crawlnet/cl4.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:24:40.313983 crawlnet-0.0.7/crawlnet.egg-info/
+-rw-rw-rw-   0        0        0      794 2024-04-25 16:24:40.000000 crawlnet-0.0.7/crawlnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-25 16:24:40.000000 crawlnet-0.0.7/crawlnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:24:40.000000 crawlnet-0.0.7/crawlnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-25 16:24:40.000000 crawlnet-0.0.7/crawlnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 16:24:40.000000 crawlnet-0.0.7/crawlnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:24:40.330422 crawlnet-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-04-25 16:20:37.000000 crawlnet-0.0.7/setup.py
```

### Comparing `crawlnet-0.0.6/PKG-INFO` & `crawlnet-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.6
+Version: 0.0.7
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.6/crawlnet/cl3.py` & `crawlnet-0.0.7/crawlnet/cl3.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
     "fuzzy_sets_u_n": fuzzy_sets_u_n,
     "optimize_gen_algo_spray_dry": optimize_gen_algo_spray_dry,
     "clonal_select_algo": clonal_select_algo,
     "Deap": Deap,
     "ant_colony": ant_colony,
     "arti_immune_pr_damage_class": arti_immune_pr_damage_class,
     "art_neural_style_transfer_1": art_neural_style_transfer_1,
-    "art_neural_style_transfer_2": art_neural_style_transfer_2
+    "art_neural_style_transfer_2": art_neural_style_transfer_2,
 }
 
 
 class Writer:
     def __init__(self, filename):
         self.filename = os.path.join(os.getcwd(), filename)
         self.masterDict = masterDict
```

### Comparing `crawlnet-0.0.6/crawlnet.egg-info/PKG-INFO` & `crawlnet-0.0.7/crawlnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.6
+Version: 0.0.7
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.6/setup.py` & `crawlnet-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "CrawlNet"
 
 # Setting up
 setup(
     name="crawlnet",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```


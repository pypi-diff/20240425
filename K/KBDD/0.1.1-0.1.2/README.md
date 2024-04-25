# Comparing `tmp/KBDD-0.1.1.tar.gz` & `tmp/KBDD-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KBDD-0.1.1.tar", last modified: Thu Apr 25 10:16:14 2024, max compression
+gzip compressed data, was "KBDD-0.1.2.tar", last modified: Thu Apr 25 10:59:47 2024, max compression
```

## Comparing `KBDD-0.1.1.tar` & `KBDD-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:16:14.342362 KBDD-0.1.1/
-drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:16:14.341900 KBDD-0.1.1/KBDD.egg-info/
--rw-r--r--   0 liaochenpo   (501) staff       (20)      966 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      142 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/SOURCES.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/dependency_links.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 10:16:14.000000 KBDD-0.1.1/KBDD.egg-info/top_level.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.1/LICENSE.txt
--rw-r--r--   0 liaochenpo   (501) staff       (20)      966 2024-04-25 10:16:14.342118 KBDD-0.1.1/PKG-INFO
--rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.1/README.md
--rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 10:16:14.342414 KBDD-0.1.1/setup.cfg
--rw-r--r--   0 liaochenpo   (501) staff       (20)      775 2024-04-25 10:16:09.000000 KBDD-0.1.1/setup.py
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:59:47.022984 KBDD-0.1.2/
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:59:47.022397 KBDD-0.1.2/KBDD.egg-info/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      366 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/SOURCES.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        1 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/dependency_links.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        5 2024-04-25 10:59:46.000000 KBDD-0.1.2/KBDD.egg-info/top_level.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1068 2024-04-25 09:12:48.000000 KBDD-0.1.2/LICENSE.txt
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      751 2024-04-25 10:59:47.022697 KBDD-0.1.2/PKG-INFO
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      342 2024-04-25 09:04:43.000000 KBDD-0.1.2/README.md
+drwxr-xr-x   0 liaochenpo   (501) staff       (20)        0 2024-04-25 10:59:47.021952 KBDD-0.1.2/kbdd/
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      921 2024-04-25 08:44:54.000000 KBDD-0.1.2/kbdd/EGtest.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     8144 2024-04-25 09:20:03.000000 KBDD-0.1.2/kbdd/KGML_to_Matrix.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     5474 2024-04-25 08:57:54.000000 KBDD-0.1.2/kbdd/Network_score_with_cor.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)        0 2024-04-25 08:38:06.000000 KBDD-0.1.2/kbdd/__init__.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      823 2024-04-25 08:49:49.000000 KBDD-0.1.2/kbdd/connect_adj_set.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     4672 2024-04-25 08:48:06.000000 KBDD-0.1.2/kbdd/left_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1712 2024-04-25 08:57:38.000000 KBDD-0.1.2/kbdd/net_gen.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)     1296 2024-04-25 08:46:18.000000 KBDD-0.1.2/kbdd/rightmost_adj.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      859 2024-04-25 08:52:05.000000 KBDD-0.1.2/kbdd/show_graph_with_labels.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      522 2024-04-25 08:59:54.000000 KBDD-0.1.2/kbdd/truncated_power_law.py
+-rw-r--r--   0 liaochenpo   (501) staff       (20)       38 2024-04-25 10:59:47.023051 KBDD-0.1.2/setup.cfg
+-rw-r--r--   0 liaochenpo   (501) staff       (20)      567 2024-04-25 10:53:37.000000 KBDD-0.1.2/setup.py
```

### Comparing `KBDD-0.1.1/LICENSE.txt` & `KBDD-0.1.2/LICENSE.txt`

 * *Files identical despite different names*


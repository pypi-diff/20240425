# Comparing `tmp/feasytools-0.0.5.tar.gz` & `tmp/feasytools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\feasytools-0.0.5.tar", last modified: Tue Apr  2 11:54:26 2024, max compression
+gzip compressed data, was "dist\feasytools-0.0.6.tar", last modified: Thu Apr 25 02:25:11 2024, max compression
```

## Comparing `feasytools-0.0.5.tar` & `feasytools-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:54:26.000000 feasytools-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools/
--rw-rw-rw-   0        0        0     3797 2024-04-02 10:19:05.000000 feasytools-0.0.5/feasytools/argchk.py
--rw-rw-rw-   0        0        0     5348 2024-03-28 11:46:52.000000 feasytools-0.0.5/feasytools/pq.py
--rw-rw-rw-   0        0        0     1897 2024-03-23 07:36:53.000000 feasytools-0.0.5/feasytools/rangelist.py
--rw-rw-rw-   0        0        0    17755 2024-03-23 07:46:48.000000 feasytools-0.0.5/feasytools/table.py
--rw-rw-rw-   0        0        0     8469 2024-03-28 11:21:46.000000 feasytools-0.0.5/feasytools/tfunc.py
--rw-rw-rw-   0        0        0      255 2024-03-23 06:37:28.000000 feasytools-0.0.5/feasytools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      835 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      312 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 11:54:26.000000 feasytools-0.0.5/feasytools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      835 2024-04-02 11:54:26.000000 feasytools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-03-23 07:58:23.000000 feasytools-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 11:54:26.000000 feasytools-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-04-02 11:54:22.000000 feasytools-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:25:11.000000 feasytools-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools/
+-rw-rw-rw-   0        0        0     4903 2024-04-25 02:23:30.000000 feasytools-0.0.6/feasytools/argchk.py
+-rw-rw-rw-   0        0        0     5348 2024-03-28 11:46:52.000000 feasytools-0.0.6/feasytools/pq.py
+-rw-rw-rw-   0        0        0     1897 2024-03-23 07:36:53.000000 feasytools-0.0.6/feasytools/rangelist.py
+-rw-rw-rw-   0        0        0    17755 2024-03-23 07:46:48.000000 feasytools-0.0.6/feasytools/table.py
+-rw-rw-rw-   0        0        0     8469 2024-03-28 11:21:46.000000 feasytools-0.0.6/feasytools/tfunc.py
+-rw-rw-rw-   0        0        0      255 2024-03-23 06:37:28.000000 feasytools-0.0.6/feasytools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      835 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      312 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 02:25:11.000000 feasytools-0.0.6/feasytools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      835 2024-04-25 02:25:11.000000 feasytools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-03-23 07:58:23.000000 feasytools-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:25:11.000000 feasytools-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-04-25 02:17:10.000000 feasytools-0.0.6/setup.py
```

### Comparing `feasytools-0.0.5/feasytools/pq.py` & `feasytools-0.0.6/feasytools/pq.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.5/feasytools/rangelist.py` & `feasytools-0.0.6/feasytools/rangelist.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.5/feasytools/table.py` & `feasytools-0.0.6/feasytools/table.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.5/feasytools/tfunc.py` & `feasytools-0.0.6/feasytools/tfunc.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.5/feasytools.egg-info/PKG-INFO` & `feasytools-0.0.6/feasytools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feasytools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.
 Home-page: UNKNOWN
 Author: fmy_xfk
 License: UNKNOWN
 Description: # FEasyTools: Some useful components
         - dprov: Data provider as time functions
         - argchk: Argument parser with type checking
```

### Comparing `feasytools-0.0.5/PKG-INFO` & `feasytools-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feasytools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.
 Home-page: UNKNOWN
 Author: fmy_xfk
 License: UNKNOWN
 Description: # FEasyTools: Some useful components
         - dprov: Data provider as time functions
         - argchk: Argument parser with type checking
```


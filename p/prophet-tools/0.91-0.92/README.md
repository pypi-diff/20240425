# Comparing `tmp/prophet_tools-0.91.tar.gz` & `tmp/prophet_tools-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet_tools-0.91.tar", last modified: Wed Apr 24 22:00:18 2024, max compression
+gzip compressed data, was "prophet_tools-0.92.tar", last modified: Wed Apr 24 22:03:21 2024, max compression
```

## Comparing `prophet_tools-0.91.tar` & `prophet_tools-0.92.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 22:00:18.192846 prophet_tools-0.91/
--rw-rw-rw-   0        0        0      138 2024-04-24 22:00:18.192846 prophet_tools-0.91/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-09-29 07:18:11.000000 prophet_tools-0.91/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 22:00:18.187846 prophet_tools-0.91/prophet_tools/
--rw-rw-rw-   0        0        0        0 2024-04-23 19:32:58.000000 prophet_tools-0.91/prophet_tools/__init__.py
--rw-rw-rw-   0        0        0      149 2024-04-23 19:32:58.000000 prophet_tools-0.91/prophet_tools/auto_import.py
--rw-rw-rw-   0        0        0     1811 2024-04-23 19:32:58.000000 prophet_tools-0.91/prophet_tools/file_convertors.py
--rw-rw-rw-   0        0        0      268 2024-04-23 19:32:58.000000 prophet_tools-0.91/prophet_tools/how_to_import.py
--rw-rw-rw-   0        0        0     6970 2024-04-24 21:49:50.000000 prophet_tools-0.91/prophet_tools/my_functions.py
--rw-rw-rw-   0        0        0      463 2024-04-23 19:32:58.000000 prophet_tools-0.91/prophet_tools/parsing.py
--rw-rw-rw-   0        0        0     1287 2024-04-23 19:45:43.000000 prophet_tools-0.91/prophet_tools/terminal.py
--rw-rw-rw-   0        0        0     4164 2024-04-23 19:32:58.000000 prophet_tools-0.91/prophet_tools/всё_подряд.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:00:18.191846 prophet_tools-0.91/prophet_tools.egg-info/
--rw-rw-rw-   0        0        0      138 2024-04-24 22:00:18.000000 prophet_tools-0.91/prophet_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-04-24 22:00:18.000000 prophet_tools-0.91/prophet_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 22:00:18.000000 prophet_tools-0.91/prophet_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 19:48:57.000000 prophet_tools-0.91/prophet_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-04-24 22:00:18.000000 prophet_tools-0.91/prophet_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 22:00:18.193848 prophet_tools-0.91/setup.cfg
--rw-rw-rw-   0        0        0      241 2024-04-24 22:00:08.000000 prophet_tools-0.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:03:21.217879 prophet_tools-0.92/
+-rw-rw-rw-   0        0        0      138 2024-04-24 22:03:21.217879 prophet_tools-0.92/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-09-29 07:18:11.000000 prophet_tools-0.92/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 22:03:21.203878 prophet_tools-0.92/prophet_tools/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:32:58.000000 prophet_tools-0.92/prophet_tools/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-04-23 19:32:58.000000 prophet_tools-0.92/prophet_tools/auto_import.py
+-rw-rw-rw-   0        0        0     1811 2024-04-23 19:32:58.000000 prophet_tools-0.92/prophet_tools/file_convertors.py
+-rw-rw-rw-   0        0        0      268 2024-04-23 19:32:58.000000 prophet_tools-0.92/prophet_tools/how_to_import.py
+-rw-rw-rw-   0        0        0     7317 2024-04-24 22:02:53.000000 prophet_tools-0.92/prophet_tools/my_functions.py
+-rw-rw-rw-   0        0        0      463 2024-04-23 19:32:58.000000 prophet_tools-0.92/prophet_tools/parsing.py
+-rw-rw-rw-   0        0        0     1287 2024-04-23 19:45:43.000000 prophet_tools-0.92/prophet_tools/terminal.py
+-rw-rw-rw-   0        0        0     4164 2024-04-23 19:32:58.000000 prophet_tools-0.92/prophet_tools/всё_подряд.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:03:21.216880 prophet_tools-0.92/prophet_tools.egg-info/
+-rw-rw-rw-   0        0        0      138 2024-04-24 22:03:21.000000 prophet_tools-0.92/prophet_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-04-24 22:03:21.000000 prophet_tools-0.92/prophet_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:03:21.000000 prophet_tools-0.92/prophet_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 19:48:57.000000 prophet_tools-0.92/prophet_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-04-24 22:03:21.000000 prophet_tools-0.92/prophet_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:03:21.217879 prophet_tools-0.92/setup.cfg
+-rw-rw-rw-   0        0        0      241 2024-04-24 22:03:04.000000 prophet_tools-0.92/setup.py
```

### Comparing `prophet_tools-0.91/prophet_tools/file_convertors.py` & `prophet_tools-0.92/prophet_tools/file_convertors.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.91/prophet_tools/my_functions.py` & `prophet_tools-0.92/prophet_tools/my_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -193,15 +193,26 @@
         os.makedirs(path)
 
 def open_folder_in_explorer(folder):
     import os
     folder = folder.replace('/', '\\')
     os.popen(f'explorer {folder}')
 
-def check_in(what, where):
+def check_in(what, where, ignore_case=False):
+    def clear_case(what):
+        if type(what) is str:
+            what = what.lower()
+        if type(what) is list:
+            for i in range(len(what)):
+                what.insert(i, what.pop(i).lower())
+        return what
+
+    if ignore_case:
+        what = clear_case(what)
+        where = clear_case(where)
     if type(what) is type(where) is str:
         return what in where or where in what
     elif type(what) is str:
         for place in where:
             if what in place:
                 return True
     elif type(where) is str:
```

### Comparing `prophet_tools-0.91/prophet_tools/terminal.py` & `prophet_tools-0.92/prophet_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.91/prophet_tools/всё_подряд.py` & `prophet_tools-0.92/prophet_tools/всё_подряд.py`

 * *Files identical despite different names*


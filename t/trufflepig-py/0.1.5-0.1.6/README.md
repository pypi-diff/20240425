# Comparing `tmp/trufflepig-py-0.1.5.tar.gz` & `tmp/trufflepig-py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trufflepig-py-0.1.5.tar", last modified: Thu Apr  4 01:28:16 2024, max compression
+gzip compressed data, was "trufflepig-py-0.1.6.tar", last modified: Thu Apr 25 17:42:57 2024, max compression
```

## Comparing `trufflepig-py-0.1.5.tar` & `trufflepig-py-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 01:28:16.050904 trufflepig-py-0.1.5/
--rw-r--r--   0 adamtazi   (501) staff       (20)     1079 2024-02-29 01:34:02.000000 trufflepig-py-0.1.5/LICENSE
--rw-r--r--   0 adamtazi   (501) staff       (20)       93 2024-02-29 00:40:22.000000 trufflepig-py-0.1.5/MANIFEST.in
--rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-04-04 01:28:16.050728 trufflepig-py-0.1.5/PKG-INFO
--rw-r--r--   0 adamtazi   (501) staff       (20)      762 2024-02-27 19:30:04.000000 trufflepig-py-0.1.5/README.md
--rw-r--r--   0 adamtazi   (501) staff       (20)       38 2024-04-04 01:28:16.050944 trufflepig-py-0.1.5/setup.cfg
--rw-r--r--   0 adamtazi   (501) staff       (20)      215 2024-04-04 01:28:13.000000 trufflepig-py-0.1.5/setup.py
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 01:28:16.048581 trufflepig-py-0.1.5/src/
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 01:28:16.049650 trufflepig-py-0.1.5/src/trufflepig/
--rw-r--r--   0 adamtazi   (501) staff       (20)       56 2024-02-29 01:23:39.000000 trufflepig-py-0.1.5/src/trufflepig/__init__.py
--rw-r--r--   0 adamtazi   (501) staff       (20)       37 2024-04-03 21:03:55.000000 trufflepig-py-0.1.5/src/trufflepig/_constants.py
--rw-r--r--   0 adamtazi   (501) staff       (20)     3451 2024-02-29 01:30:26.000000 trufflepig-py-0.1.5/src/trufflepig/client.py
--rw-r--r--   0 adamtazi   (501) staff       (20)    23343 2024-04-04 01:21:51.000000 trufflepig-py-0.1.5/src/trufflepig/index.py
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 01:28:16.050572 trufflepig-py-0.1.5/src/trufflepig_py.egg-info/
--rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-04-04 01:28:16.000000 trufflepig-py-0.1.5/src/trufflepig_py.egg-info/PKG-INFO
--rw-r--r--   0 adamtazi   (501) staff       (20)      347 2024-04-04 01:28:16.000000 trufflepig-py-0.1.5/src/trufflepig_py.egg-info/SOURCES.txt
--rw-r--r--   0 adamtazi   (501) staff       (20)        1 2024-04-04 01:28:16.000000 trufflepig-py-0.1.5/src/trufflepig_py.egg-info/dependency_links.txt
--rw-r--r--   0 adamtazi   (501) staff       (20)       17 2024-04-04 01:28:16.000000 trufflepig-py-0.1.5/src/trufflepig_py.egg-info/requires.txt
--rw-r--r--   0 adamtazi   (501) staff       (20)       11 2024-04-04 01:28:16.000000 trufflepig-py-0.1.5/src/trufflepig_py.egg-info/top_level.txt
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-25 17:42:57.330653 trufflepig-py-0.1.6/
+-rw-r--r--   0 adamtazi   (501) staff       (20)     1079 2024-02-29 01:34:02.000000 trufflepig-py-0.1.6/LICENSE
+-rw-r--r--   0 adamtazi   (501) staff       (20)       93 2024-02-29 00:40:22.000000 trufflepig-py-0.1.6/MANIFEST.in
+-rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-04-25 17:42:57.330428 trufflepig-py-0.1.6/PKG-INFO
+-rw-r--r--   0 adamtazi   (501) staff       (20)      762 2024-02-27 19:30:04.000000 trufflepig-py-0.1.6/README.md
+-rw-r--r--   0 adamtazi   (501) staff       (20)       38 2024-04-25 17:42:57.330693 trufflepig-py-0.1.6/setup.cfg
+-rw-r--r--   0 adamtazi   (501) staff       (20)      215 2024-04-25 17:42:27.000000 trufflepig-py-0.1.6/setup.py
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-25 17:42:57.328435 trufflepig-py-0.1.6/src/
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-25 17:42:57.329415 trufflepig-py-0.1.6/src/trufflepig/
+-rw-r--r--   0 adamtazi   (501) staff       (20)       56 2024-02-29 01:23:39.000000 trufflepig-py-0.1.6/src/trufflepig/__init__.py
+-rw-r--r--   0 adamtazi   (501) staff       (20)       37 2024-04-03 21:03:55.000000 trufflepig-py-0.1.6/src/trufflepig/_constants.py
+-rw-r--r--   0 adamtazi   (501) staff       (20)     3627 2024-04-25 17:39:27.000000 trufflepig-py-0.1.6/src/trufflepig/client.py
+-rw-r--r--   0 adamtazi   (501) staff       (20)    23343 2024-04-04 01:21:51.000000 trufflepig-py-0.1.6/src/trufflepig/index.py
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-25 17:42:57.330245 trufflepig-py-0.1.6/src/trufflepig_py.egg-info/
+-rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-04-25 17:42:57.000000 trufflepig-py-0.1.6/src/trufflepig_py.egg-info/PKG-INFO
+-rw-r--r--   0 adamtazi   (501) staff       (20)      347 2024-04-25 17:42:57.000000 trufflepig-py-0.1.6/src/trufflepig_py.egg-info/SOURCES.txt
+-rw-r--r--   0 adamtazi   (501) staff       (20)        1 2024-04-25 17:42:57.000000 trufflepig-py-0.1.6/src/trufflepig_py.egg-info/dependency_links.txt
+-rw-r--r--   0 adamtazi   (501) staff       (20)       17 2024-04-25 17:42:57.000000 trufflepig-py-0.1.6/src/trufflepig_py.egg-info/requires.txt
+-rw-r--r--   0 adamtazi   (501) staff       (20)       11 2024-04-25 17:42:57.000000 trufflepig-py-0.1.6/src/trufflepig_py.egg-info/top_level.txt
```

### Comparing `trufflepig-py-0.1.5/LICENSE` & `trufflepig-py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trufflepig-py-0.1.5/README.md` & `trufflepig-py-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `trufflepig-py-0.1.5/src/trufflepig/client.py` & `trufflepig-py-0.1.6/src/trufflepig/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,18 @@
         -----------
         Index: A search index.
 
         Example:
         -----------
         index = trufflepig.get_index("myIndex")
         """
+        # check if the index exists
+        index_names = [index.index_name for index in self.list_indexes()]
+        if index_name not in index_names:
+            return None
         return Index(self.api_key, index_name)
 
     def list_indexes(self) -> List[Index]:
         """
         List indexes available to this user.
 
         Returns:
```

### Comparing `trufflepig-py-0.1.5/src/trufflepig/index.py` & `trufflepig-py-0.1.6/src/trufflepig/index.py`

 * *Files identical despite different names*


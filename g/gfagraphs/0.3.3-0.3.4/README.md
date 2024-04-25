# Comparing `tmp/gfagraphs-0.3.3.tar.gz` & `tmp/gfagraphs-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.3.3.tar", last modified: Wed Apr 24 13:48:03 2024, max compression
+gzip compressed data, was "gfagraphs-0.3.4.tar", last modified: Wed Apr 24 15:37:36 2024, max compression
```

## Comparing `gfagraphs-0.3.3.tar` & `gfagraphs-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.187340 gfagraphs-0.3.3/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.3/LICENSE
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.3/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.3/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.3/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      351 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.3/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.3/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.3/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.3/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    31188 2024-04-24 13:23:42.000000 gfagraphs-0.3.3/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.3/pgGraphs/nx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-24 13:48:03.187340 gfagraphs-0.3.3/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-04-24 13:47:52.000000 gfagraphs-0.3.3/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.336677 gfagraphs-0.3.4/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.4/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.4/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.4/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.4/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      351 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.4/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.4/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.4/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.4/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    32339 2024-04-24 15:24:54.000000 gfagraphs-0.3.4/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.4/pgGraphs/nx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-24 15:37:36.336677 gfagraphs-0.3.4/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-04-24 15:35:23.000000 gfagraphs-0.3.4/setup.py
```

### Comparing `gfagraphs-0.3.3/LICENSE` & `gfagraphs-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.3/PKG-INFO` & `gfagraphs-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.3/README.md` & `gfagraphs-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.3/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.4/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.3/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.4/gfagraphs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.3/pgGraphs/abstractions.py` & `gfagraphs-0.3.4/pgGraphs/abstractions.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.3/pgGraphs/gfaparser.py` & `gfagraphs-0.3.4/pgGraphs/gfaparser.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.3/pgGraphs/graph.py` & `gfagraphs-0.3.4/pgGraphs/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,14 +578,37 @@
                 len(path['path'])-len(segs)+1) if (segs == path_nodes[i:i+len(segs)])][::-1]
             # We go backwards to dodge index collisions
             for pos in positions:
                 path['path'][pos:pos-len(segs)+1] = [merge_name]
 
 ############### POsitionnal tag ###############
 
+    def compute_orientations(self) -> None:
+        """
+        Computes both predecessors and successors, by their orientations
+        This function is O(n) with n being the number of edges.
+        """
+        for node in self.segments.keys():
+            self.segments[node]['out_forward'] = set()
+            self.segments[node]['out_reverse'] = set()
+            self.segments[node]['in_forward'] = set()
+            self.segments[node]['in_reverse'] = set()
+        for (from_node, to_node), datas in self.lines.items():
+            for from_orientation, to_orientation in datas['orientation']:
+                if from_orientation == Orientation.FORWARD:
+                    self.segments[from_node]['out_forward'].add(
+                        (to_node, to_orientation))
+                    self.segments[to_node]['in_forward'].add(
+                        (from_node, from_orientation))
+                else:
+                    self.segments[from_node]['out_reverse'].add(
+                        (to_node, to_orientation))
+                    self.segments[to_node]['in_reverse'].add(
+                        (from_node, from_orientation))
+
     def compute_neighbors(self) -> None:
         """
         Computes both predecessors and successors
         This function is O(n) with n being the number of edges.
         """
         for node in self.segments.keys():
             self.segments[node]['successors'] = set()
```

### Comparing `gfagraphs-0.3.3/pgGraphs/nx.py` & `gfagraphs-0.3.4/pgGraphs/nx.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.3/pyproject.toml` & `gfagraphs-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.3.3"
+    version = "0.3.4"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.3.3/setup.py` & `gfagraphs-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.3.3"
+VN: str = "0.3.4"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = [
     'networkx',
     'tharos-pytools',
     'matplotlib',
     'mycolorpy',
 ]
```


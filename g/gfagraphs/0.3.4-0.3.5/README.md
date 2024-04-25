# Comparing `tmp/gfagraphs-0.3.4.tar.gz` & `tmp/gfagraphs-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.3.4.tar", last modified: Wed Apr 24 15:37:36 2024, max compression
+gzip compressed data, was "gfagraphs-0.3.5.tar", last modified: Thu Apr 25 13:03:58 2024, max compression
```

## Comparing `gfagraphs-0.3.4.tar` & `gfagraphs-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.336677 gfagraphs-0.3.4/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.4/LICENSE
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.4/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.4/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.4/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      351 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.4/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 15:37:36.335677 gfagraphs-0.3.4/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.4/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.4/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.4/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    32339 2024-04-24 15:24:54.000000 gfagraphs-0.3.4/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.4/pgGraphs/nx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-24 15:37:36.000000 gfagraphs-0.3.4/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-24 15:37:36.336677 gfagraphs-0.3.4/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-04-24 15:35:23.000000 gfagraphs-0.3.4/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 13:03:58.846691 gfagraphs-0.3.5/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.5/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-25 13:03:58.846691 gfagraphs-0.3.5/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.5/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 13:03:58.845692 gfagraphs-0.3.5/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.5/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.5/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 13:03:58.846691 gfagraphs-0.3.5/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-25 13:03:58.000000 gfagraphs-0.3.5/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      365 2024-04-25 13:03:58.000000 gfagraphs-0.3.5/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-25 13:03:58.000000 gfagraphs-0.3.5/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.5/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-25 13:03:58.000000 gfagraphs-0.3.5/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 13:03:58.845692 gfagraphs-0.3.5/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.5/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.5/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.5/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    32376 2024-04-25 13:03:22.000000 gfagraphs-0.3.5/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.5/pgGraphs/nx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-25 13:03:58.000000 gfagraphs-0.3.5/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-25 13:03:58.846691 gfagraphs-0.3.5/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-04-25 13:03:31.000000 gfagraphs-0.3.5/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 13:03:58.845692 gfagraphs-0.3.5/tests/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      536 2024-04-25 12:43:00.000000 gfagraphs-0.3.5/tests/test.py
```

### Comparing `gfagraphs-0.3.4/LICENSE` & `gfagraphs-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.4/PKG-INFO` & `gfagraphs-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.4/README.md` & `gfagraphs-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.4/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.5/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.4/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.5/gfagraphs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.4/pgGraphs/abstractions.py` & `gfagraphs-0.3.5/pgGraphs/abstractions.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.4/pgGraphs/gfaparser.py` & `gfagraphs-0.3.5/pgGraphs/gfaparser.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.4/pgGraphs/graph.py` & `gfagraphs-0.3.5/pgGraphs/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,25 +83,24 @@
                                         'orientation',
                                         {}
                                     ) | datas['orientation']
                                 except TypeError:
                                     print(name, self.lines[name].get(
                                         'orientation', {}), datas['orientation'])
                             if with_reverse_edges:
-                                (_ttad,) = datas['orientation']
                                 if name[::-1] not in self.lines:
                                     self.lines[name[::-1]] = {
                                         'orientation': set(
-                                            [(reverse(_ttad[0]), reverse(_ttad[1]))]
+                                            [datas['orientation'][::-1]]
                                         )
                                     }
                                     self.lines[name[::-1]]
                                 else:
                                     self.lines[name[::-1]]['orientation'] = self.lines[name[::-1]].get(
-                                        'orientation', set()) | set([(reverse(_ttad[0]), reverse(_ttad[1]))])
+                                        'orientation', set()) | set([datas['orientation'][::-1]])
 
                         case GFALine.HEADER:
                             self.headers.append(datas)
                         case _:
                             pass
 
     def __str__(self) -> str:
@@ -584,29 +583,33 @@
 
     def compute_orientations(self) -> None:
         """
         Computes both predecessors and successors, by their orientations
         This function is O(n) with n being the number of edges.
         """
         for node in self.segments.keys():
-            self.segments[node]['out_forward'] = set()
-            self.segments[node]['out_reverse'] = set()
-            self.segments[node]['in_forward'] = set()
-            self.segments[node]['in_reverse'] = set()
+            self.segments[node]['out'] = {
+                Orientation.FORWARD: set(),
+                Orientation.REVERSE: set(),
+            }
+            self.segments[node]['in'] = {
+                Orientation.FORWARD: set(),
+                Orientation.REVERSE: set(),
+            }
         for (from_node, to_node), datas in self.lines.items():
             for from_orientation, to_orientation in datas['orientation']:
                 if from_orientation == Orientation.FORWARD:
-                    self.segments[from_node]['out_forward'].add(
+                    self.segments[from_node]['out'][Orientation.FORWARD].add(
                         (to_node, to_orientation))
-                    self.segments[to_node]['in_forward'].add(
+                    self.segments[to_node]['in'][Orientation.FORWARD].add(
                         (from_node, from_orientation))
                 else:
-                    self.segments[from_node]['out_reverse'].add(
+                    self.segments[from_node]['out'][Orientation.REVERSE].add(
                         (to_node, to_orientation))
-                    self.segments[to_node]['in_reverse'].add(
+                    self.segments[to_node]['in'][[Orientation.REVERSE]].add(
                         (from_node, from_orientation))
 
     def compute_neighbors(self) -> None:
         """
         Computes both predecessors and successors
         This function is O(n) with n being the number of edges.
         """
```

### Comparing `gfagraphs-0.3.4/pgGraphs/nx.py` & `gfagraphs-0.3.5/pgGraphs/nx.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.4/pyproject.toml` & `gfagraphs-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.3.4"
+    version = "0.3.5"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.3.4/setup.py` & `gfagraphs-0.3.5/setup.py`

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
-VN: str = "0.3.4"
+VN: str = "0.3.5"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = [
     'networkx',
     'tharos-pytools',
     'matplotlib',
     'mycolorpy',
 ]
```


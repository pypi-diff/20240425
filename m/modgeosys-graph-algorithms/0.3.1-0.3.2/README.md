# Comparing `tmp/modgeosys_graph_algorithms-0.3.1.tar.gz` & `tmp/modgeosys_graph_algorithms-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.3.1.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.3.2.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.3.1.tar` & `modgeosys_graph_algorithms-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3364 2024-04-24 20:00:01.568472 modgeosys_graph_algorithms-0.3.1/README.md
--rw-r--r--   0        0        0      489 2024-04-24 20:52:25.797353 modgeosys_graph_algorithms-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.1/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-24 19:56:19.647912 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     7716 2024-04-24 20:40:43.795506 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     3311 2024-04-24 20:47:47.452657 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     8139 2024-04-24 20:46:32.640456 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0    23944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     3198 2024-04-06 22:43:36.508467 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3430 2024-04-24 21:52:17.921541 modgeosys_graph_algorithms-0.3.2/README.md
+-rw-r--r--   0        0        0      489 2024-04-24 22:02:24.066918 modgeosys_graph_algorithms-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.2/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-24 20:58:48.758144 modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     7716 2024-04-24 20:58:48.758144 modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     3366 2024-04-24 21:49:37.193157 modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     8139 2024-04-24 20:58:48.758144 modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    23944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3198 2024-04-06 22:43:36.508467 modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.2/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.3.1/README.md` & `modgeosys_graph_algorithms-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                                                           (3, ((0.0, 2.0), (2.0, 3.0))),
                                                           (1, ((2.0, 1.0), (2.0, 3.0)))),
                                         heuristic_distance_function=manhattan_distance)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
     larger_graph = pickle.load(pickled_sample_larger_graph_file)
+    larger_graph.heuristic_distance_function = manhattan_distance
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
 print(f'Toy A* Path:')
 pprint(toy_a_star_path)
 print()
 larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4,
```

### Comparing `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.3.2/src/modgeosys/graph/types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,14 +61,18 @@
                                                          (1, ((2.0, 1.0), (2.0, 3.0)))),
                                        heuristic_distance_function=manhattan_distance)
 
 
 @pytest.fixture
 def valid_graph_larger():
     with open('data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
-        return pickle.load(pickled_sample_larger_graph_file)
+        graph = pickle.load(pickled_sample_larger_graph_file)
+        graph.heuristic_distance_function = manhattan_distance
+        return graph
 
 
 @pytest.fixture
-def valid_graph_larger_with_string_edge_weights():
-    with open('data/graph_with_string_edge_weights.pickle', 'rb') as pickled_sample_larger_graph_file:
-        return pickle.load(pickled_sample_larger_graph_file)
+def valid_graph_larger_with_string_edge_weights(valid_graph_larger):
+    graph = valid_graph_larger
+    for edge in graph.edges:
+        edge.weight = str(edge.weight)
+    return graph
```

### Comparing `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.3.2/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.1/PKG-INFO` & `modgeosys_graph_algorithms-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
@@ -47,14 +47,15 @@
                                                           (3, ((0.0, 2.0), (2.0, 3.0))),
                                                           (1, ((2.0, 1.0), (2.0, 3.0)))),
                                         heuristic_distance_function=manhattan_distance)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
     larger_graph = pickle.load(pickled_sample_larger_graph_file)
+    larger_graph.heuristic_distance_function = manhattan_distance
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
 print(f'Toy A* Path:')
 pprint(toy_a_star_path)
 print()
 larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4,
```


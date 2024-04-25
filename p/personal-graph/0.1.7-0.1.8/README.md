# Comparing `tmp/personal_graph-0.1.7.tar.gz` & `tmp/personal_graph-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_graph-0.1.7.tar", max compression
+gzip compressed data, was "personal_graph-0.1.8.tar", max compression
```

## Comparing `personal_graph-0.1.7.tar` & `personal_graph-0.1.8.tar`

### file list

```diff
@@ -1,40 +1,33 @@
--rw-r--r--   0        0        0     1080 2024-03-13 05:55:36.893450 personal_graph-0.1.7/LICENSE
--rw-r--r--   0        0        0     5927 2024-04-20 12:33:56.682697 personal_graph-0.1.7/README.md
--rw-r--r--   0        0        0       54 2024-04-08 09:45:51.825318 personal_graph-0.1.7/personal_graph/__init__.py
--rw-r--r--   0        0        0    25676 2024-04-19 11:23:54.423395 personal_graph-0.1.7/personal_graph/database.py
--rw-r--r--   0        0        0      903 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/embeddings.py
--rw-r--r--   0        0        0     6031 2024-04-17 11:56:47.270908 personal_graph-0.1.7/personal_graph/graph.py
--rw-r--r--   0        0        0      142 2024-04-20 09:29:58.161412 personal_graph-0.1.7/personal_graph/ml.py
--rw-r--r--   0        0        0     1797 2024-04-19 18:12:33.056612 personal_graph-0.1.7/personal_graph/models.py
--rw-r--r--   0        0        0     4899 2024-04-20 12:33:56.682697 personal_graph-0.1.7/personal_graph/natural.py
--rw-r--r--   0        0        0     1161 2024-04-17 11:56:47.274908 personal_graph-0.1.7/personal_graph/retriever.py
--rw-r--r--   0        0        0       52 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-edge-embedding.sql
--rw-r--r--   0        0        0       48 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-edge.sql
--rw-r--r--   0        0        0       45 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-node-embedding.sql
--rw-r--r--   0        0        0       30 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/delete-node.sql
--rw-r--r--   0        0        0       97 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/existing-edge.sql
--rw-r--r--   0        0        0       39 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/existing-node.sql
--rw-r--r--   0        0        0       72 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/insert-edge-embedding.sql
--rw-r--r--   0        0        0       91 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/insert-edge.sql
--rw-r--r--   0        0        0       62 2024-04-08 05:20:20.734143 personal_graph-0.1.7/personal_graph/sql/insert-node-embedding.sql
--rw-r--r--   0        0        0       70 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/insert-node.sql
--rw-r--r--   0        0        0     1116 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/schema.sql
--rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.7/personal_graph/sql/search-edges-inbound.sql
--rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.7/personal_graph/sql/search-edges-outbound.sql
--rw-r--r--   0        0        0       80 2024-04-08 05:20:20.738142 personal_graph-0.1.7/personal_graph/sql/search-edges.sql
--rw-r--r--   0        0        0      252 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/search-node.template
--rw-r--r--   0        0        0      297 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/search-where.template
--rw-r--r--   0        0        0      609 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/traverse.template
--rw-r--r--   0        0        0       75 2024-04-12 11:09:18.207085 personal_graph-0.1.7/personal_graph/sql/update-node.sql
--rw-r--r--   0        0        0      283 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/sql/vector-search-edge.sql
--rw-r--r--   0        0        0      254 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/sql/vector-search-node.sql
--rw-r--r--   0        0        0        0 2024-04-08 05:20:20.742142 personal_graph-0.1.7/personal_graph/tests/__init__.py
--rw-r--r--   0        0        0     2455 2024-04-18 09:40:51.239348 personal_graph-0.1.7/personal_graph/tests/conftest.py
--rw-r--r--   0        0        0     3723 2024-04-08 05:20:20.742142 personal_graph-0.1.7/personal_graph/tests/test_database.py
--rw-r--r--   0        0        0     4551 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/tests/test_graph.py
--rw-r--r--   0        0        0        0 2024-04-08 05:20:20.746141 personal_graph-0.1.7/personal_graph/tests/test_ml.py
--rw-r--r--   0        0        0     1405 2024-04-12 11:09:18.211085 personal_graph-0.1.7/personal_graph/tests/test_natural.py
--rw-r--r--   0        0        0     1399 2024-04-08 05:20:20.746141 personal_graph-0.1.7/personal_graph/tests/test_visualizers.py
--rw-r--r--   0        0        0     4011 2024-04-17 11:56:47.274908 personal_graph-0.1.7/personal_graph/visualizers.py
--rw-r--r--   0        0        0      996 2024-04-20 12:33:56.682697 personal_graph-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7130 1970-01-01 00:00:00.000000 personal_graph-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-13 05:55:36.893450 personal_graph-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5927 2024-04-22 08:53:09.627733 personal_graph-0.1.8/README.md
+-rw-r--r--   0        0        0      299 2024-04-25 11:24:47.884191 personal_graph-0.1.8/personal_graph/__init__.py
+-rw-r--r--   0        0        0    26772 2024-04-25 11:24:47.884191 personal_graph-0.1.8/personal_graph/database.py
+-rw-r--r--   0        0        0      903 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/embeddings.py
+-rw-r--r--   0        0        0     6701 2024-04-25 11:24:47.888191 personal_graph-0.1.8/personal_graph/graph.py
+-rw-r--r--   0        0        0     6824 2024-04-25 11:24:47.888191 personal_graph-0.1.8/personal_graph/ml.py
+-rw-r--r--   0        0        0     1797 2024-04-25 11:24:47.888191 personal_graph-0.1.8/personal_graph/models.py
+-rw-r--r--   0        0        0     4899 2024-04-22 08:53:09.627733 personal_graph-0.1.8/personal_graph/natural.py
+-rw-r--r--   0        0        0     1161 2024-04-17 11:56:47.274908 personal_graph-0.1.8/personal_graph/retriever.py
+-rw-r--r--   0        0        0       52 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/delete-edge-embedding.sql
+-rw-r--r--   0        0        0       48 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/delete-edge.sql
+-rw-r--r--   0        0        0       45 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/delete-node-embedding.sql
+-rw-r--r--   0        0        0       30 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/delete-node.sql
+-rw-r--r--   0        0        0       97 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/existing-edge.sql
+-rw-r--r--   0        0        0       39 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/existing-node.sql
+-rw-r--r--   0        0        0       72 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/insert-edge-embedding.sql
+-rw-r--r--   0        0        0       91 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/insert-edge.sql
+-rw-r--r--   0        0        0       62 2024-04-08 05:20:20.734143 personal_graph-0.1.8/personal_graph/sql/insert-node-embedding.sql
+-rw-r--r--   0        0        0       70 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/insert-node.sql
+-rw-r--r--   0        0        0     1116 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/schema.sql
+-rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.8/personal_graph/sql/search-edges-inbound.sql
+-rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.8/personal_graph/sql/search-edges-outbound.sql
+-rw-r--r--   0        0        0       80 2024-04-08 05:20:20.738142 personal_graph-0.1.8/personal_graph/sql/search-edges.sql
+-rw-r--r--   0        0        0      252 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/search-node.template
+-rw-r--r--   0        0        0      297 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/search-where.template
+-rw-r--r--   0        0        0      609 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/traverse.template
+-rw-r--r--   0        0        0       75 2024-04-12 11:09:18.207085 personal_graph-0.1.8/personal_graph/sql/update-node.sql
+-rw-r--r--   0        0        0      283 2024-04-12 11:09:18.211085 personal_graph-0.1.8/personal_graph/sql/vector-search-edge.sql
+-rw-r--r--   0        0        0      254 2024-04-12 11:09:18.211085 personal_graph-0.1.8/personal_graph/sql/vector-search-node.sql
+-rw-r--r--   0        0        0     4011 2024-04-22 10:26:16.265399 personal_graph-0.1.8/personal_graph/visualizers.py
+-rw-r--r--   0        0        0     1048 2024-04-25 11:24:47.892191 personal_graph-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 personal_graph-0.1.8/PKG-INFO
```

### Comparing `personal_graph-0.1.7/LICENSE` & `personal_graph-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/README.md` & `personal_graph-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/personal_graph/database.py` & `personal_graph-0.1.8/personal_graph/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -458,14 +458,15 @@
 
             for id in edge_ids:
                 cursor.execute(read_sql("delete-edge-embedding.sql"), (id,))
 
             cursor.execute(read_sql("delete-node.sql"), (identifier,))
 
             cursor.execute(read_sql("delete-node-embedding.sql"), (node[0],))
+            connection.commit()
 
     return _remove_node
 
 
 def _generate_clause(
     key: str,
     predicate: str | None = None,
@@ -535,14 +536,24 @@
                 return result[0]
         else:
             return {}
 
     return _find_node
 
 
+def find_label(identifier: Any) -> CursorExecFunction:
+    def _find_label(cursor, connection):
+        node_label = cursor.execute(
+            "SELECT label from nodes where id=?", (identifier,)
+        ).fetchone()
+        return node_label
+
+    return _find_label
+
+
 def _parse_search_results(results: List[Tuple], idx: int = 0) -> List[Dict]:
     return [json.loads(item[idx]) for item in results]
 
 
 def find_nodes(
     where_clauses: List[str],
     bindings: Tuple,
@@ -646,14 +657,17 @@
                 "SELECT label, attributes from nodes where id=?", (node_id[0],)
             ).fetchone()
 
             similar_nodes = vector_search_node(node_data, threshold, 3)(
                 cursor, connection
             )
 
+            if similar_nodes is None:
+                continue
+
             if len(similar_nodes) < 1:
                 continue
 
             for rowid, _, _, _, _ in similar_nodes:
                 similar_node_id = cursor.execute(
                     "SELECT id from nodes where embed_id=?", (rowid,)
                 ).fetchone()
@@ -796,14 +810,42 @@
         ids = [id[0] for id in nodes]
 
         return ids
 
     return _fetch_nodes_from_db
 
 
+def find_indegree_edges(target_id: Any) -> CursorExecFunction:
+    def _indegree_edges(cursor, connection):
+        indegree = cursor.execute(
+            "SELECT source, label, attributes from edges where target=? ", (target_id,)
+        )
+
+        if indegree:
+            indegree = indegree.fetchall()
+
+        return indegree
+
+    return _indegree_edges
+
+
+def find_outdegree_edges(source_id: Any) -> CursorExecFunction:
+    def _outdegree_edges(cursor, connection):
+        outdegree = cursor.execute(
+            "SELECT target, label, attributes from edges where source=? ", (source_id,)
+        )
+
+        if outdegree:
+            outdegree = outdegree.fetchall()
+
+        return outdegree
+
+    return _outdegree_edges
+
+
 def all_connected_nodes(node_or_edge: Union[Node | Edge]) -> CursorExecFunction:
     def _connected_nodes(cursor, connection):
         nodes = None
         if isinstance(node_or_edge, Node):
             index = node_or_edge.id
             nodes = cursor.execute(
                 "SELECT source, target FROM edges WHERE source=? OR target=?",
```

### Comparing `personal_graph-0.1.7/personal_graph/embeddings.py` & `personal_graph-0.1.8/personal_graph/embeddings.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/personal_graph/graph.py` & `personal_graph-0.1.8/personal_graph/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,32 @@
     find_neighbors,
     find_outbound_neighbors,
     traverse,
     pruning,
     find_similar_nodes,
     nodes_list,
     vector_search_node,
+    find_label,
+    find_outdegree_edges,
+    find_indegree_edges,
 )
 from .natural import insert_into_graph, search_from_graph, visualize_knowledge_graph
 from .visualizers import graphviz_visualize
 
 
 class Graph(AbstractContextManager):
     def __init__(self, db_url: Optional[str] = None, auth_token: Optional[str] = None):
         self.db_url = db_url
         self.auth_token = auth_token
 
+    def __eq__(self, other):
+        if not isinstance(other, Graph):
+            return "Not of Graph Type"
+        return self.db_url == other.db_url and self.auth_token == other.auth_token
+
     def __enter__(self, schema_file: str = "schema.sql") -> Graph:
         if not self.db_url:
             # Support for local SQLite database
             self.connection = libsql.connect(":memory:")
         else:
             self.connection = libsql.connect(
                 database=self.db_url, auth_token=self.auth_token
@@ -127,14 +135,17 @@
 
     def remove_nodes(self, ids: List[Any]) -> None:
         atomic(remove_nodes(ids), self.db_url, self.auth_token)
 
     def search_node(self, node_id: Any) -> Any:
         return atomic(find_node(node_id), self.db_url, self.auth_token)
 
+    def search_node_label(self, node_id: Any) -> Any:
+        return atomic(find_label(node_id), self.db_url, self.auth_token)
+
     def traverse(
         self, source: Any, target: Optional[Any] = None, with_bodies: bool = False
     ) -> List:
         neighbors_fn = find_neighbors if with_bodies else find_outbound_neighbors
         path = traverse(
             db_url=self.db_url,
             auth_token=self.auth_token,
@@ -166,14 +177,20 @@
 
     def visualize(self, file: str, path: List[str]) -> Digraph:
         return graphviz_visualize(self.db_url, self.auth_token, file, path)
 
     def fetch_ids_from_db(self) -> List[str]:
         return atomic(nodes_list(), self.db_url, self.auth_token)
 
+    def search_indegree_edges(self, target) -> List[Any]:
+        return atomic(find_indegree_edges(target), self.db_url, self.auth_token)
+
+    def search_outdegree_edges(self, source) -> List[Any]:
+        return atomic(find_outdegree_edges(source), self.db_url, self.auth_token)
+
     def is_unique_prompt(self, text: str, threshold: float) -> bool:
         similar_nodes = atomic(
             vector_search_node({"body": text}, threshold, 1),
             self.db_url,
             self.auth_token,
         )
```

### Comparing `personal_graph-0.1.7/personal_graph/models.py` & `personal_graph-0.1.8/personal_graph/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,44 +9,44 @@
 class Node(BaseModel):
     id: Union[int, str] = Field(..., description="Unique Identifier for the node.")
     attributes: Union[str, Dict[str, str]] = Field(
         ..., min_length=1, description="Detailed information associated with the node."
     )
     label: str = Field(
         ...,
-        min_length=2,
+        min_length=1,
         description="Most related and unique name associated with the node.",
     )
 
 
 class Edge(BaseModel):
     source: Union[int, str] = Field(
         ..., description="identifier of the source node from which the edge originates."
     )
     target: Union[int, str] = Field(
         ..., description="identifier of the target node to which the edge points."
     )
     label: str = Field(
         ...,
-        min_length=2,
+        min_length=1,
         description="Most related and unique name associated with the edge.",
     )
     attributes: Union[str, Dict[str, str]] = Field(
         ...,
         min_length=1,
         description="Detailed information associated with the relationships.",
     )
 
 
 class EdgeInput(BaseModel):
     source: Node = Field(..., description="Source node from which the edge originates.")
     target: Node = Field(..., description="Target node to which the edge points.")
     label: str = Field(
         ...,
-        min_length=2,
+        min_length=1,
         description="Most related and unique name associated with the edge.",
     )
     attributes: Union[str, Dict[str, str]] = Field(
         ...,
         min_length=1,
         description="Detailed information associated within the relationships.",
     )
```

### Comparing `personal_graph-0.1.7/personal_graph/natural.py` & `personal_graph-0.1.8/personal_graph/natural.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/personal_graph/retriever.py` & `personal_graph-0.1.8/personal_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/personal_graph/sql/schema.sql` & `personal_graph-0.1.8/personal_graph/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/personal_graph/sql/traverse.template` & `personal_graph-0.1.8/personal_graph/sql/traverse.template`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/personal_graph/visualizers.py` & `personal_graph-0.1.8/personal_graph/visualizers.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.7/pyproject.toml` & `personal_graph-0.1.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "personal-graph"
-version = "0.1.7"
+version = "0.1.8"
 description = "Graph database in LibSQL"
 authors = ["Anubhuti Bhardwaj <anubhutibhardwaj11@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = [
     { path = "examples/personal-graph.ipynb" }
 ]
@@ -23,14 +23,15 @@
 fastapi = "^0.110.0"
 uvicorn = "^0.29.0"
 sqlean-py = "^3.45.1"
 streamlit = "^1.33.0"
 types-pygments = "^2.17.0.20240310"
 types-decorator = "^5.1.8.20240310"
 dspy-ai = "^2.4.5"
+networkx = {extras = ["default"], version = "^3.3"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 ruff = "^0.3.2"
 mypy = "^1.9.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `personal_graph-0.1.7/PKG-INFO` & `personal_graph-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-graph
-Version: 0.1.7
+Version: 0.1.8
 Summary: Graph database in LibSQL
 License: MIT
 Author: Anubhuti Bhardwaj
 Author-email: anubhutibhardwaj11@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Provides-Extra: scrollable-textbox
 Requires-Dist: dspy-ai (>=2.4.5,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: instructor (>=0.6.7,<0.7.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: libsql-experimental (>=0.0.28,<0.0.29)
+Requires-Dist: networkx[default] (>=3.3,<4.0)
 Requires-Dist: openai (>=1.14.2,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: pytest-mock (>=3.14.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: sqlean-py (>=3.45.1,<4.0.0)
 Requires-Dist: sqlite-vss (>=0.1.2,<0.2.0)
 Requires-Dist: streamlit (>=1.33.0,<2.0.0)
```


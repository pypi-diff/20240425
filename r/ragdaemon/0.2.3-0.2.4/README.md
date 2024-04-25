# Comparing `tmp/ragdaemon-0.2.3.tar.gz` & `tmp/ragdaemon-0.2.4.tar.gz`

## Comparing `ragdaemon-0.2.3.tar` & `ragdaemon-0.2.4.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/app.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/context.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/llm.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_comments.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_sample.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/app.py
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/context.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_comments.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_sample.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/PKG-INFO
```

### Comparing `ragdaemon-0.2.3/.github/workflows/run-tests.yml` & `ragdaemon-0.2.4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/app.py` & `ragdaemon-0.2.4/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/context.py` & `ragdaemon-0.2.4/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/daemon.py` & `ragdaemon-0.2.4/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/get_paths.py` & `ragdaemon-0.2.4/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/graph.py` & `ragdaemon-0.2.4/ragdaemon/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         str
     ]  # Used to fetch document: path/to/file:start-end, diff_ref:start-end
     checksum: Optional[str]  # Unique identifier for chroma; sha256 of the document
     active: bool  # Used to filter nodes for search
     chunks: Optional[
         list[dict[str, str]]
     ]  # For files, func/class/method. For diff, by file/hunk
+    summary: Optional[str]  # Generated summary of the node
 
 
 class EdgeMetadata(TypedDict):
     type: Literal["hierarchy", "diff"]
 
 
 def validate_attrs(attrs: dict[str, Any], type: Literal["node", "edge"]):
```

### Comparing `ragdaemon-0.2.3/ragdaemon/utils.py` & `ragdaemon-0.2.4/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/__init__.py` & `ragdaemon-0.2.4/ragdaemon/annotators/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from ragdaemon.annotators.base_annotator import Annotator  # noqa: F401
 from ragdaemon.annotators.chunker import Chunker
 from ragdaemon.annotators.chunker_line import ChunkerLine
 from ragdaemon.annotators.chunker_llm import ChunkerLLM
 from ragdaemon.annotators.diff import Diff
 from ragdaemon.annotators.hierarchy import Hierarchy
 from ragdaemon.annotators.layout_hierarchy import LayoutHierarchy
+from ragdaemon.annotators.summarizer import Summarizer
 
 annotators_map = {
     "hierarchy": Hierarchy,
     "chunker": Chunker,
     "chunker_llm": ChunkerLLM,
     "chunker_line": ChunkerLine,
     "diff": Diff,
     "layout_hierarchy": LayoutHierarchy,
+    "summarizer": Summarizer,
 }
```

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.2.4/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/chunker.py` & `ragdaemon-0.2.4/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.2.4/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.2.4/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/diff.py` & `ragdaemon-0.2.4/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.2.4/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.2.4/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/database/__init__.py` & `ragdaemon-0.2.4/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/database/chroma_database.py` & `ragdaemon-0.2.4/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/database/database.py` & `ragdaemon-0.2.4/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/database/lite_database.py` & `ragdaemon-0.2.4/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/static/favicon.ico` & `ragdaemon-0.2.4/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.2.4/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/static/js/main.js` & `ragdaemon-0.2.4/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.2.4/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/static/js/three/node.js` & `ragdaemon-0.2.4/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.2.4/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/ragdaemon/templates/index.html` & `ragdaemon-0.2.4/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/conftest.py` & `ragdaemon-0.2.4/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import subprocess
 import tempfile
 from pathlib import Path
-from unittest.mock import AsyncMock, patch
+from unittest.mock import AsyncMock
 
 import pytest
 
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, get_db
 
 
 @pytest.fixture
@@ -18,23 +18,14 @@
 @pytest.fixture
 def mock_db(cwd):
     return get_db(
         cwd, spice_client=AsyncMock(), embedding_model=DEFAULT_EMBEDDING_MODEL
     )
 
 
-@pytest.fixture
-def mock_get_llm_response():
-    with patch(
-        "ragdaemon.annotators.chunker_llm.ChunkerLLM.get_llm_response",
-        return_value={"chunks": []},
-    ) as mock:
-        yield mock
-
-
 @pytest.fixture(scope="function")
 def git_history(cwd):
     with tempfile.TemporaryDirectory() as tmpdir:
         tmpdir_path = Path(tmpdir)
         sample_dir = cwd
         shutil.copytree(sample_dir, tmpdir_path, dirs_exist_ok=True)
         # TODO: Use/save .ragdaemon records
```

### Comparing `ragdaemon-0.2.3/tests/test_comments.py` & `ragdaemon-0.2.4/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/test_context.py` & `ragdaemon-0.2.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/test_daemon.py` & `ragdaemon-0.2.4/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/test_get_paths.py` & `ragdaemon-0.2.4/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/test_sample.py` & `ragdaemon-0.2.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/annotators/test_chunker.py` & `ragdaemon-0.2.4/tests/annotators/test_chunker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from pathlib import Path
-from unittest.mock import AsyncMock
+from unittest.mock import AsyncMock, patch
 
 import pytest
 
 from ragdaemon.annotators import Chunker, ChunkerLLM
 from ragdaemon.daemon import Daemon
 from ragdaemon.graph import KnowledgeGraph
 
 
+@pytest.fixture
+def mock_get_llm_response():
+    with patch(
+        "ragdaemon.annotators.chunker_llm.ChunkerLLM.get_llm_response",
+        return_value={"chunks": []},
+    ) as mock:
+        yield mock
+
+
 def test_chunker_is_complete(cwd, mock_db):
     chunker = Chunker()
 
     empty_graph = KnowledgeGraph()
     assert chunker.is_complete(empty_graph, mock_db), "Empty graph is complete."
 
     hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
@@ -41,15 +50,14 @@
 
 
 @pytest.mark.asyncio
 async def test_chunker_llm_annotate(cwd, mock_get_llm_response, mock_db):
     daemon = Daemon(
         cwd=cwd,
         annotators={"hierarchy": {}},
-        graph_path=(Path.cwd() / "tests/data/hierarchy_graph.json"),
     )
     chunker = ChunkerLLM(spice_client=AsyncMock())
     actual = await chunker.annotate(daemon.graph, mock_db)
 
     for node, data in actual.nodes(data=True):
         assert data, f"Node {node} is missing data"
         if data["type"] == "file" and Path(node).suffix in chunker.chunk_extensions:
```

### Comparing `ragdaemon-0.2.3/tests/annotators/test_diff.py` & `ragdaemon-0.2.4/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/annotators/test_hierarchy.py` & `ragdaemon-0.2.4/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.2.4/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/data/chunker_graph.json` & `ragdaemon-0.2.4/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/data/context_message.txt` & `ragdaemon-0.2.4/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/data/diff_graph.json` & `ragdaemon-0.2.4/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/data/hierarchy_graph.json` & `ragdaemon-0.2.4/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.2.4/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/tests/sample/src/interface.py` & `ragdaemon-0.2.4/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/LICENSE` & `ragdaemon-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/README.md` & `ragdaemon-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.3/pyproject.toml` & `ragdaemon-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.2.3"
+version = "0.2.4"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.2.3/PKG-INFO` & `ragdaemon-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


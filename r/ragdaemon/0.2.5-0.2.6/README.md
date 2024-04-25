# Comparing `tmp/ragdaemon-0.2.5.tar.gz` & `tmp/ragdaemon-0.2.6.tar.gz`

## Comparing `ragdaemon-0.2.5.tar` & `ragdaemon-0.2.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/app.py
--rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/context.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/llm.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_sample.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/app.py
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/context.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/test_sample.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.6/PKG-INFO
```

### Comparing `ragdaemon-0.2.5/scratch.ipynb` & `ragdaemon-0.2.6/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tutorial.ipynb` & `ragdaemon-0.2.6/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/.github/workflows/run-tests.yml` & `ragdaemon-0.2.6/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/app.py` & `ragdaemon-0.2.6/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/context.py` & `ragdaemon-0.2.6/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/daemon.py` & `ragdaemon-0.2.6/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/get_paths.py` & `ragdaemon-0.2.6/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/graph.py` & `ragdaemon-0.2.6/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/utils.py` & `ragdaemon-0.2.6/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/__init__.py` & `ragdaemon-0.2.6/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.2.6/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/chunker.py` & `ragdaemon-0.2.6/ragdaemon/annotators/chunker.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import Database
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
-from ragdaemon.utils import get_document, hash_str
+from ragdaemon.utils import get_document, hash_str, truncate
 
 
 def is_chunk_valid(chunk: dict) -> bool:
     # Includes the correct fields
     if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
         return False
     # ID is in the correct format
@@ -134,14 +134,17 @@
                 record = {
                     "id": id,
                     "type": "chunk",
                     "ref": chunk["ref"],
                     "checksum": checksum,
                     "active": False,
                 }
+                document, truncate_ratio = truncate(document, db.embedding_model)
+                if truncate_ratio > 0 and verbose:
+                    print(f"Truncated {id} by {truncate_ratio:.2%}")
                 add_to_db["ids"].append(checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(record)
         except Exception as e:
             if verbose:
                 print(f"Error processing chunk {chunk}: {e}")
             continue
```

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.2.6/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.2.6/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/diff.py` & `ragdaemon-0.2.6/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.2.6/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.2.6/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.2.6/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/database/__init__.py` & `ragdaemon-0.2.6/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/database/chroma_database.py` & `ragdaemon-0.2.6/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/database/database.py` & `ragdaemon-0.2.6/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/database/lite_database.py` & `ragdaemon-0.2.6/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/static/favicon.ico` & `ragdaemon-0.2.6/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.2.6/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/static/js/main.js` & `ragdaemon-0.2.6/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.2.6/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/static/js/three/node.js` & `ragdaemon-0.2.6/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.2.6/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/ragdaemon/templates/index.html` & `ragdaemon-0.2.6/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/conftest.py` & `ragdaemon-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/test_comments.py` & `ragdaemon-0.2.6/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/test_context.py` & `ragdaemon-0.2.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/test_daemon.py` & `ragdaemon-0.2.6/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/test_get_paths.py` & `ragdaemon-0.2.6/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/test_sample.py` & `ragdaemon-0.2.6/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/annotators/test_chunker.py` & `ragdaemon-0.2.6/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/annotators/test_diff.py` & `ragdaemon-0.2.6/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/annotators/test_hierarchy.py` & `ragdaemon-0.2.6/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.2.6/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/annotators/test_summarizer.py` & `ragdaemon-0.2.6/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/data/chunker_graph.json` & `ragdaemon-0.2.6/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/data/context_message.txt` & `ragdaemon-0.2.6/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/data/diff_graph.json` & `ragdaemon-0.2.6/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/data/hierarchy_graph.json` & `ragdaemon-0.2.6/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.2.6/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/tests/sample/src/interface.py` & `ragdaemon-0.2.6/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/LICENSE` & `ragdaemon-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/README.md` & `ragdaemon-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.5/pyproject.toml` & `ragdaemon-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.2.5"
+version = "0.2.6"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.2.5/PKG-INFO` & `ragdaemon-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


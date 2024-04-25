# Comparing `tmp/ragdaemon-0.2.4.tar.gz` & `tmp/ragdaemon-0.2.5.tar.gz`

## Comparing `ragdaemon-0.2.4.tar` & `ragdaemon-0.2.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/app.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/context.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/llm.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_comments.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/test_sample.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/app.py
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/context.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/test_sample.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.5/PKG-INFO
```

### Comparing `ragdaemon-0.2.4/scratch.ipynb` & `ragdaemon-0.2.5/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tutorial.ipynb` & `ragdaemon-0.2.5/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/.github/workflows/run-tests.yml` & `ragdaemon-0.2.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/app.py` & `ragdaemon-0.2.5/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/context.py` & `ragdaemon-0.2.5/ragdaemon/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 from dict2xml import dict2xml
 from ragdaemon.annotators.diff import parse_diff_id
 from ragdaemon.database import Database
 from ragdaemon.graph import KnowledgeGraph
@@ -34,14 +37,34 @@
         self.graph = graph
         self.db = db
         self.verbose = verbose
         self.context = dict[
             str, dict[str, Any]
         ]()  # {path: {lines, tags, document, diff}}
 
+    def copy(self):
+        duplicate = ContextBuilder(self.graph, self.db, self.verbose)
+        duplicate.context = deepcopy(self.context)
+        return duplicate
+
+    def __add__(self, other: ContextBuilder) -> ContextBuilder:
+        duplicate = self.copy()
+        for path_str, data in other.context.items():
+            if path_str not in duplicate.context:
+                duplicate.context[path_str] = data
+            else:
+                duplicate.context[path_str]["lines"].update(data["lines"])
+                duplicate.context[path_str]["tags"].update(data["tags"])
+                duplicate.context[path_str]["diffs"].update(data["diffs"])
+                for line, comments in data["comments"].items():
+                    duplicate.context[path_str]["comments"].setdefault(line, []).extend(
+                        comments
+                    )
+        return duplicate
+
     def _add_path(self, path_str: str):
         """Create a new record in the context for the given path."""
         document = None
         if path_str in self.graph:
             checksum = self.graph.nodes[path_str]["checksum"]
             document = self.db.get(checksum)["documents"][0]
             if document.endswith("[TRUNCATED]"):
```

### Comparing `ragdaemon-0.2.4/ragdaemon/daemon.py` & `ragdaemon-0.2.5/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/get_paths.py` & `ragdaemon-0.2.5/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/graph.py` & `ragdaemon-0.2.5/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/utils.py` & `ragdaemon-0.2.5/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/__init__.py` & `ragdaemon-0.2.5/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.2.5/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/chunker.py` & `ragdaemon-0.2.5/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.2.5/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.2.5/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/diff.py` & `ragdaemon-0.2.5/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.2.5/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.2.5/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.2.5/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/database/__init__.py` & `ragdaemon-0.2.5/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/database/chroma_database.py` & `ragdaemon-0.2.5/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/database/database.py` & `ragdaemon-0.2.5/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/database/lite_database.py` & `ragdaemon-0.2.5/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/static/favicon.ico` & `ragdaemon-0.2.5/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.2.5/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/static/js/main.js` & `ragdaemon-0.2.5/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.2.5/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/static/js/three/node.js` & `ragdaemon-0.2.5/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.2.5/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/ragdaemon/templates/index.html` & `ragdaemon-0.2.5/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/conftest.py` & `ragdaemon-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/test_comments.py` & `ragdaemon-0.2.5/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/test_context.py` & `ragdaemon-0.2.5/tests/test_context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from pathlib import Path
 
+import pytest
+
 from ragdaemon.context import ContextBuilder
+from ragdaemon.daemon import Daemon
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import get_document
 
 
 def test_daemon_render_context(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
@@ -62,14 +65,39 @@
 13:        raise ValueError("Invalid operation")
 14:    return int(match.group(1)), match.group(2), int(match.group(3))
 ...
 """
     )
 
 
+@pytest.mark.asyncio
+async def test_context_builder_methods(cwd, mock_db):
+    daemon = Daemon(cwd)
+    await daemon.update()
+
+    context = daemon.get_context("")
+    context.add_ref("src/interface.py:3-5")
+
+    copied_context = context.copy()
+    copied_context.add_ref("src/interface.py:7-9")
+
+    assert context.context["src/interface.py"]["lines"] == set([3, 4, 5])
+    assert copied_context.context["src/interface.py"]["lines"] == set(
+        [3, 4, 5, 7, 8, 9]
+    )
+
+    different_context = daemon.get_context("")
+    different_context.add_ref("src/interface.py:17")
+    different_context.add_ref("src/operations.py")
+    combined_context = context + different_context
+
+    assert combined_context.context["src/interface.py"]["lines"] == set([3, 4, 5, 17])
+    assert combined_context.context["src/operations.py"]["lines"] == set(range(1, 22))
+
+
 def test_to_refs(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Setup Context
     context = ContextBuilder(KnowledgeGraph(), mock_db)
     context.context = {
```

### Comparing `ragdaemon-0.2.4/tests/test_daemon.py` & `ragdaemon-0.2.5/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/test_get_paths.py` & `ragdaemon-0.2.5/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/test_sample.py` & `ragdaemon-0.2.5/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/annotators/test_chunker.py` & `ragdaemon-0.2.5/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/annotators/test_diff.py` & `ragdaemon-0.2.5/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/annotators/test_hierarchy.py` & `ragdaemon-0.2.5/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.2.5/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/annotators/test_summarizer.py` & `ragdaemon-0.2.5/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/data/chunker_graph.json` & `ragdaemon-0.2.5/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/data/context_message.txt` & `ragdaemon-0.2.5/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/data/diff_graph.json` & `ragdaemon-0.2.5/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/data/hierarchy_graph.json` & `ragdaemon-0.2.5/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.2.5/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/tests/sample/src/interface.py` & `ragdaemon-0.2.5/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/LICENSE` & `ragdaemon-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/README.md` & `ragdaemon-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.4/pyproject.toml` & `ragdaemon-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.2.4"
+version = "0.2.5"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.2.4/PKG-INFO` & `ragdaemon-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


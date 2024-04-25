# Comparing `tmp/splitml-0.5.1.tar.gz` & `tmp/splitml-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitml-0.5.1.tar", last modified: Thu Apr 25 18:31:28 2024, max compression
+gzip compressed data, was "splitml-0.5.2.tar", last modified: Thu Apr 25 19:25:40 2024, max compression
```

## Comparing `splitml-0.5.1.tar` & `splitml-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.838999 splitml-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 18:31:19.000000 splitml-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 18:31:28.838999 splitml-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 18:31:19.000000 splitml-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 18:31:19.000000 splitml-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:31:28.838999 splitml-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.834999 splitml-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.834999 splitml-0.5.1/src/splitml/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/groupers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/html_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/pdf_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/splitml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.838999 splitml-0.5.1/src/splitml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:25:40.004111 splitml-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 19:25:30.000000 splitml-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 19:25:40.004111 splitml-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 19:25:30.000000 splitml-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 19:25:30.000000 splitml-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:25:40.004111 splitml-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:25:40.000111 splitml-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:25:40.000111 splitml-0.5.2/src/splitml/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/groupers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/html_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/pdf_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/splitml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-25 19:25:30.000000 splitml-0.5.2/src/splitml/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:25:40.004111 splitml-0.5.2/src/splitml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 19:25:39.000000 splitml-0.5.2/src/splitml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 19:25:39.000000 splitml-0.5.2/src/splitml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:25:39.000000 splitml-0.5.2/src/splitml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 19:25:39.000000 splitml-0.5.2/src/splitml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 19:25:39.000000 splitml-0.5.2/src/splitml.egg-info/top_level.txt
```

### Comparing `splitml-0.5.1/LICENSE` & `splitml-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splitml-0.5.1/PKG-INFO` & `splitml-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `splitml-0.5.1/README.md` & `splitml-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `splitml-0.5.1/pyproject.toml` & `splitml-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "splitml"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     { name="Hansimov" },
 ]
 description = "Split Markup Language (HTML and Markdown) to Groups and Nodes"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `splitml-0.5.1/src/splitml/constants.py` & `splitml-0.5.2/src/splitml/constants.py`

 * *Files identical despite different names*

### Comparing `splitml-0.5.1/src/splitml/groupers.py` & `splitml-0.5.2/src/splitml/groupers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from .stats import count_tokens
 
 
 class NodesGrouper:
     DEFAULT_MAX_TOKENS = [128, 512, 1024]
     DEFAULT_OVERLAP_NODE_COUNT = 1
 
+    def __init__(self, input_format: Literal["html", "markdown", "text"] = "html"):
+        self.input_format = input_format
+
     def group_nodes_by_order(
         self,
         nodes,
         max_tokens: list[int] = DEFAULT_MAX_TOKENS,
         overlap_node_count: int = DEFAULT_OVERLAP_NODE_COUNT,
     ):
         groups = []
@@ -31,23 +34,32 @@
         return groups
 
     def combine_groups(self, groups):
         grouped_nodes = []
         node_idxs_list = []
         for group in groups:
             text = "\n\n".join([node["text"] for node in group])
-            html = "\n\n".join([node["html"] for node in group])
-            group_tokens = count_tokens(text)
+
+            if self.input_format == "text":
+                html = ""
+                page_idxs = []
+                node_tags = []
+            else:
+                html = "\n\n".join([node["html"] for node in group])
+                page_idxs = [node["page_idx"] for node in group]
+                node_tags = [node["tag"] for node in group]
+
             node_idxs = [node["node_idx"] for node in group]
-            page_idxs = [node["page_idx"] for node in group]
-            node_tags = [node["tag"] for node in group]
+            group_tokens = count_tokens(text)
+
             if node_idxs in node_idxs_list:
                 continue
             else:
                 node_idxs_list.append(node_idxs)
+
             grouped_nodes.append(
                 {
                     "html": html,
                     "text": text,
                     "html_len": len(html),
                     "text_len": len(text),
                     "text_tokens": group_tokens,
```

### Comparing `splitml-0.5.1/src/splitml/html_splitter.py` & `splitml-0.5.2/src/splitml/html_splitter.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 
 from pathlib import Path
 
 from bs4 import BeautifulSoup
 from purehtml import purify_html_str
 from tclogger import logger
+from typing import Literal
 
 from .constants import SPLIT_TAGS, TAG_TYPE_MAP
 from .stats import count_tokens
 
 
 class HTMLSplitter:
     def get_tag_type(self, element):
@@ -56,25 +57,32 @@
             if child.name in SPLIT_TAGS:
                 return False
         return True
 
     def md2html(self, md_str):
         return markdown2.markdown(md_str)
 
-    def check_format(func):
-        def wrapper(self, html_str, format=None, **kwargs):
-            if format == "markdown":
+    def check_input_format(func):
+        def wrapper(
+            self, html_str, input_format: Literal["html", "markdown"] = "html", **kwargs
+        ):
+            if input_format == "markdown":
                 html_str = self.md2html(html_str)
-            format = "html"
-            return func(self, html_str, format, **kwargs)
+            return func(self, html_str, input_format, **kwargs)
 
         return wrapper
 
-    @check_format
-    def split_html_str(self, html_str, format=None, page_idx=-1, remove_seps=False):
+    @check_input_format
+    def split_html_str(
+        self,
+        html_str,
+        input_format: Literal["html", "markdown"] = "html",
+        page_idx=-1,
+        remove_seps=False,
+    ):
         results = []
         soup = BeautifulSoup(html_str, "html.parser")
         for idx, element in enumerate(soup.find_all(SPLIT_TAGS)):
             if not self.is_atomized(element):
                 continue
             element_str = str(element)
             markdown_str = purify_html_str(
@@ -99,19 +107,21 @@
                 "node_idx": idx,
                 "page_idx": page_idx,
             }
             results.append(item)
 
         return results
 
-    def split_html_file(self, html_path, format=None):
+    def split_html_file(
+        self, html_path, input_format: Literal["html", "markdown"] = "html"
+    ):
         ext = Path(html_path).suffix
-        if not format:
+        if not input_format:
             if ext == ".md":
-                format = "markdown"
+                input_format = "markdown"
             else:
-                format = "html"
+                input_format = "html"
         else:
-            format = format
+            input_format = input_format
 
         html_str = self.read_html_file(html_path)
-        return self.split_html_str(html_str, format=format)
+        return self.split_html_str(html_str, input_format=input_format)
```

### Comparing `splitml-0.5.1/src/splitml/pdf_splitter.py` & `splitml-0.5.2/src/splitml/pdf_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         html_splitter = HTMLSplitter()
         for page_idx, page in enumerate(tqdm(pdf_doc)):
             # logger.note(f"> Page {page_idx+1}")
             html_str = page.get_text("html")
             html_str = purify_html_str(html_str)
             # logger.mesg(html_str)
             nodes = html_splitter.split_html_str(
-                html_str, format="html", page_idx=page_idx
+                html_str, input_format="html", page_idx=page_idx
             )
             results.extend(nodes)
 
         return results
 
     def read_pdf_bytes(self, pdf_bytes):
         # https://github.com/pymupdf/PyMuPDF/issues/612
```

### Comparing `splitml-0.5.1/src/splitml/splitml.py` & `splitml-0.5.2/src/splitml/splitml.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 
 from tclogger import logger
 
 from .stats import stat_tokens
 from .groupers import NodesGrouper
 from .html_splitter import HTMLSplitter
 from .pdf_splitter import PDFSplitter
+from .text_splitter import TextSplitter
 
 
-def split_html_str(html_str: str, format=None):
-    return HTMLSplitter().split_html_str(html_str, format=format)
+def split_html_str(html_str: str, input_format=None):
+    return HTMLSplitter().split_html_str(html_str, input_format=input_format)
 
 
-def split_html_file(html_path: Union[Path, str], format=None):
-    return HTMLSplitter().split_html_file(html_path, format=format)
+def split_html_file(html_path: Union[Path, str], input_format=None):
+    return HTMLSplitter().split_html_file(html_path, input_format=input_format)
 
 
-def chunk_html_str(html_str: str, format=None):
-    nodes = HTMLSplitter().split_html_str(html_str, format=format)
+def chunk_html_str(html_str: str, input_format=None):
+    nodes = HTMLSplitter().split_html_str(html_str, input_format=input_format)
     grouped_nodes = NodesGrouper().group_nodes(nodes)
     return grouped_nodes
 
 
-def chunk_html_file(html_path: Union[Path, str], format=None):
-    nodes = HTMLSplitter().split_html_file(html_path, format=format)
+def chunk_html_file(html_path: Union[Path, str], input_format=None):
+    nodes = HTMLSplitter().split_html_file(html_path, input_format=input_format)
     grouped_nodes = NodesGrouper().group_nodes(nodes)
     return grouped_nodes
 
 
 def split_pdf_bytes(pdf_bytes: bytes):
     return PDFSplitter().split_pdf_bytes(pdf_bytes)
 
@@ -46,14 +47,34 @@
 
 def chunk_pdf_file(pdf_path: Union[Path, str]):
     nodes = PDFSplitter().split_pdf_file(pdf_path)
     grouped_nodes = NodesGrouper().group_nodes(nodes)
     return grouped_nodes
 
 
+def split_text_str(text_str: str):
+    return TextSplitter().split_text_str(text_str)
+
+
+def split_text_file(text_path: Union[Path, str]):
+    return TextSplitter().split_text_file(text_path)
+
+
+def chunk_text_str(text_str: str):
+    nodes = TextSplitter().split_text_str(text_str)
+    grouped_nodes = NodesGrouper("text").group_nodes(nodes)
+    return grouped_nodes
+
+
+def chunk_text_file(text_path: Union[Path, str]):
+    nodes = TextSplitter().split_text_file(text_path)
+    grouped_nodes = NodesGrouper("text").group_nodes(nodes)
+    return grouped_nodes
+
+
 if __name__ == "__main__":
     sample_root = Path(__file__).parent / "samples"
 
     # file_pattern = "*.html.md"
     # html_paths = sorted(
     #     list(sample_root.glob(file_pattern)),
     #     key=lambda x: str(x).lower(),
@@ -65,25 +86,42 @@
     #     nodes = splitter.split_html_file(html_path)
     #     logger.success(f"  - {len(nodes)} nodes.")
     #     stat_tokens(nodes)
     #     grouped_nodes = grouper.group_nodes(nodes)
     #     logger.success(f"  - {len(grouped_nodes)} grouped nodes.")
     #     stat_tokens(grouped_nodes)
 
-    file_pattern = "*.pdf"
-    pdf_paths = sorted(
+    # file_pattern = "*.pdf"
+    # pdf_paths = sorted(
+    #     list(sample_root.glob(file_pattern)),
+    #     key=lambda x: str(x).lower(),
+    # )[:1]
+    # splitter = PDFSplitter()
+    # for pdf_path in pdf_paths:
+    #     logger.note(f"> Processing: {pdf_path.name}")
+    #     nodes = splitter.split_pdf_file(pdf_path)
+    #     logger.success(f"  - {len(nodes)} nodes.")
+    #     stat_tokens(nodes)
+    #     grouped_nodes = NodesGrouper().group_nodes(nodes)
+    #     logger.success(f"  - {len(grouped_nodes)} grouped nodes.")
+    #     stat_tokens(grouped_nodes)
+
+    file_pattern = "*.html.md"
+    file_paths = sorted(
         list(sample_root.glob(file_pattern)),
         key=lambda x: str(x).lower(),
     )[:1]
-    splitter = PDFSplitter()
-    for pdf_path in pdf_paths:
-        logger.note(f"> Processing: {pdf_path.name}")
-        nodes = splitter.split_pdf_file(pdf_path)
+    splitter = TextSplitter()
+    grouper = NodesGrouper("text")
+    for file_path in file_paths:
+        logger.note(f"> Processing: {file_path.name}")
+        nodes = splitter.split_text_file(file_path)
         logger.success(f"  - {len(nodes)} nodes.")
         stat_tokens(nodes)
-        grouped_nodes = NodesGrouper().group_nodes(nodes)
+        grouped_nodes = grouper.group_nodes(nodes)
         logger.success(f"  - {len(grouped_nodes)} grouped nodes.")
         stat_tokens(grouped_nodes)
+
     logger.success(pformat(grouped_nodes[0], indent=4, sort_dicts=False))
 
     # [**/src]
     # python -m splitml.splitml
```

### Comparing `splitml-0.5.1/src/splitml/stats.py` & `splitml-0.5.2/src/splitml/stats.py`

 * *Files identical despite different names*

### Comparing `splitml-0.5.1/src/splitml.egg-info/PKG-INFO` & `splitml-0.5.2/src/splitml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


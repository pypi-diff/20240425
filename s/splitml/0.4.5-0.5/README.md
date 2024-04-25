# Comparing `tmp/splitml-0.4.5.tar.gz` & `tmp/splitml-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitml-0.4.5.tar", last modified: Thu Apr 25 15:01:40 2024, max compression
+gzip compressed data, was "splitml-0.5.tar", last modified: Thu Apr 25 16:38:46 2024, max compression
```

## Comparing `splitml-0.4.5.tar` & `splitml-0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.044650 splitml-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 15:01:31.000000 splitml-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-25 15:01:40.044650 splitml-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 15:01:31.000000 splitml-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 15:01:31.000000 splitml-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:01:40.044650 splitml-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.040650 splitml-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.040650 splitml-0.4.5/src/splitml/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/groupers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/html_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/splitml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.044650 splitml-0.4.5/src/splitml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.671649 splitml-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 16:38:36.000000 splitml-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 16:38:46.671649 splitml-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 16:38:36.000000 splitml-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-25 16:38:36.000000 splitml-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:38:46.671649 splitml-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.667649 splitml-0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.667649 splitml-0.5/src/splitml/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/groupers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/html_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/pdf_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/splitml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.667649 splitml-0.5/src/splitml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/top_level.txt
```

### Comparing `splitml-0.4.5/LICENSE` & `splitml-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `splitml-0.4.5/PKG-INFO` & `splitml-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.4.5
+Version: 0.5
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: purehtml
 Requires-Dist: markdown2
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken
+Requires-Dist: PyMuPDF
 
 # SplitML
 
 Split Markup Language (HTML and Markdown) to Groups and Nodes
 
 ![](https://img.shields.io/pypi/v/splitml?label=splitml&color=blue)
```

### Comparing `splitml-0.4.5/README.md` & `splitml-0.5/README.md`

 * *Files identical despite different names*

### Comparing `splitml-0.4.5/pyproject.toml` & `splitml-0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "splitml"
-version = "0.4.5"
+version = "0.5"
 authors = [
     { name="Hansimov" },
 ]
 description = "Split Markup Language (HTML and Markdown) to Groups and Nodes"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [ "purehtml", "markdown2", "beautifulsoup4", "tiktoken" ]
+dependencies = [ "purehtml", "markdown2", "beautifulsoup4", "tiktoken", "PyMuPDF" ]
 
 [project.urls]
 Homepage = "https://github.com/Hansimov/splitml"
 Issues = "https://github.com/Hansimov/splitml/issues"
```

### Comparing `splitml-0.4.5/src/splitml/constants.py` & `splitml-0.5/src/splitml/constants.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.5/src/splitml/groupers.py` & `splitml-0.5/src/splitml/groupers.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.5/src/splitml/html_splitter.py` & `splitml-0.5/src/splitml/html_splitter.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.5/src/splitml/splitml.py` & `splitml-0.5/src/splitml/splitml.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union
 
 from tclogger import logger
 
 from .stats import stat_tokens
 from .groupers import NodesGrouper
 from .html_splitter import HTMLSplitter
+from .pdf_splitter import PDFSplitter
 
 
 def split_html_str(html_str: str, format=None):
     return HTMLSplitter().split_html_str(html_str, format=format)
 
 
 def split_html_file(html_path: Union[Path, str], format=None):
@@ -24,28 +25,63 @@
 
 def chunk_html_file(html_path: Union[Path, str], format=None):
     nodes = HTMLSplitter().split_html_file(html_path, format=format)
     grouped_nodes = NodesGrouper().group_nodes(nodes)
     return grouped_nodes
 
 
+def split_pdf_bytes(pdf_bytes: bytes):
+    return PDFSplitter().split_pdf_bytes(pdf_bytes)
+
+
+def split_pdf_file(pdf_path: Union[Path, str]):
+    return PDFSplitter().split_pdf_file(pdf_path)
+
+
+def chunk_pdf_bytes(pdf_bytes: bytes):
+    nodes = PDFSplitter().split_pdf_bytes(pdf_bytes)
+    grouped_nodes = NodesGrouper().group_nodes(nodes)
+    return grouped_nodes
+
+
+def chunk_pdf_file(pdf_path: Union[Path, str]):
+    nodes = PDFSplitter().split_pdf_file(pdf_path)
+    grouped_nodes = NodesGrouper().group_nodes(nodes)
+    return grouped_nodes
+
+
 if __name__ == "__main__":
-    html_root = Path(__file__).parent / "samples"
+    sample_root = Path(__file__).parent / "samples"
 
-    file_pattern = "*.html.md"
-    html_paths = sorted(
-        list(html_root.glob(file_pattern)),
+    # file_pattern = "*.html.md"
+    # html_paths = sorted(
+    #     list(sample_root.glob(file_pattern)),
+    #     key=lambda x: str(x).lower(),
+    # )[:2]
+    # splitter = HTMLSplitter()
+    # grouper = NodesGrouper()
+    # for html_path in html_paths:
+    #     logger.note(f"> Processing: {html_path.name}")
+    #     nodes = splitter.split_html_file(html_path)
+    #     logger.success(f"  - {len(nodes)} nodes.")
+    #     stat_tokens(nodes)
+    #     grouped_nodes = grouper.group_nodes(nodes)
+    #     logger.success(f"  - {len(grouped_nodes)} grouped nodes.")
+    #     stat_tokens(grouped_nodes)
+
+    file_pattern = "*.pdf"
+    pdf_paths = sorted(
+        list(sample_root.glob(file_pattern)),
         key=lambda x: str(x).lower(),
-    )[:2]
-    splitter = HTMLSplitter()
-    grouper = NodesGrouper()
-    for html_path in html_paths:
-        logger.note(f"> Processing: {html_path.name}")
-        nodes = splitter.split_html_file(html_path)
+    )[:1]
+    splitter = PDFSplitter()
+    for pdf_path in pdf_paths:
+        logger.note(f"> Processing: {pdf_path.name}")
+        nodes = splitter.split_pdf_file(pdf_path)
         logger.success(f"  - {len(nodes)} nodes.")
         stat_tokens(nodes)
-        grouped_nodes = grouper.group_nodes(nodes)
+        grouped_nodes = NodesGrouper().group_nodes(nodes)
         logger.success(f"  - {len(grouped_nodes)} grouped nodes.")
         stat_tokens(grouped_nodes)
 
     # [**/src]
     # python -m splitml.splitml
```

### Comparing `splitml-0.4.5/src/splitml/stats.py` & `splitml-0.5/src/splitml/stats.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.5/src/splitml.egg-info/PKG-INFO` & `splitml-0.5/src/splitml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.4.5
+Version: 0.5
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: purehtml
 Requires-Dist: markdown2
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken
+Requires-Dist: PyMuPDF
 
 # SplitML
 
 Split Markup Language (HTML and Markdown) to Groups and Nodes
 
 ![](https://img.shields.io/pypi/v/splitml?label=splitml&color=blue)
```


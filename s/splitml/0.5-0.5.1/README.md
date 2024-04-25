# Comparing `tmp/splitml-0.5.tar.gz` & `tmp/splitml-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitml-0.5.tar", last modified: Thu Apr 25 16:38:46 2024, max compression
+gzip compressed data, was "splitml-0.5.1.tar", last modified: Thu Apr 25 18:31:28 2024, max compression
```

## Comparing `splitml-0.5.tar` & `splitml-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.671649 splitml-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 16:38:36.000000 splitml-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 16:38:46.671649 splitml-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 16:38:36.000000 splitml-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-25 16:38:36.000000 splitml-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:38:46.671649 splitml-0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.667649 splitml-0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.667649 splitml-0.5/src/splitml/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/groupers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/html_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/pdf_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/splitml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 16:38:36.000000 splitml-0.5/src/splitml/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:38:46.667649 splitml-0.5/src/splitml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 16:38:46.000000 splitml-0.5/src/splitml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.838999 splitml-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 18:31:19.000000 splitml-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 18:31:28.838999 splitml-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 18:31:19.000000 splitml-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 18:31:19.000000 splitml-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:31:28.838999 splitml-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.834999 splitml-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.834999 splitml-0.5.1/src/splitml/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/groupers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/html_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/pdf_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/splitml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 18:31:19.000000 splitml-0.5.1/src/splitml/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:28.838999 splitml-0.5.1/src/splitml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 18:31:28.000000 splitml-0.5.1/src/splitml.egg-info/top_level.txt
```

### Comparing `splitml-0.5/LICENSE` & `splitml-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splitml-0.5/PKG-INFO` & `splitml-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.5
+Version: 0.5.1
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `splitml-0.5/README.md` & `splitml-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `splitml-0.5/pyproject.toml` & `splitml-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "splitml"
-version = "0.5"
+version = "0.5.1"
 authors = [
     { name="Hansimov" },
 ]
 description = "Split Markup Language (HTML and Markdown) to Groups and Nodes"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `splitml-0.5/src/splitml/constants.py` & `splitml-0.5.1/src/splitml/constants.py`

 * *Files identical despite different names*

### Comparing `splitml-0.5/src/splitml/groupers.py` & `splitml-0.5.1/src/splitml/groupers.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,30 @@
         grouped_nodes = []
         node_idxs_list = []
         for group in groups:
             text = "\n\n".join([node["text"] for node in group])
             html = "\n\n".join([node["html"] for node in group])
             group_tokens = count_tokens(text)
             node_idxs = [node["node_idx"] for node in group]
+            page_idxs = [node["page_idx"] for node in group]
             node_tags = [node["tag"] for node in group]
             if node_idxs in node_idxs_list:
                 continue
             else:
                 node_idxs_list.append(node_idxs)
             grouped_nodes.append(
                 {
                     "html": html,
                     "text": text,
                     "html_len": len(html),
                     "text_len": len(text),
                     "text_tokens": group_tokens,
                     "node_idxs": node_idxs,
                     "node_tags": node_tags,
+                    "page_idxs": page_idxs,
                 }
             )
 
         return grouped_nodes
 
     def group_nodes(
         self,
```

### Comparing `splitml-0.5/src/splitml/html_splitter.py` & `splitml-0.5.1/src/splitml/html_splitter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import markdown2
+import re
 
 from pathlib import Path
 
 from bs4 import BeautifulSoup
 from purehtml import purify_html_str
 from tclogger import logger
 
@@ -15,14 +16,25 @@
         tag_type = ""
         for key, tags in TAG_TYPE_MAP.items():
             if element.name in tags:
                 tag_type = key
                 break
         return tag_type
 
+    def remove_separators(self, text: str) -> str:
+        new_text = text
+        chars_map = {
+            "\n+": " ",
+            "-\n": "",
+            "\f": "",
+        }
+        for k, v in chars_map.items():
+            new_text = re.sub(k, v, new_text)
+        return new_text
+
     def read_html_file(self, html_path):
         if not Path(html_path).exists():
             warn_msg = f"File not found: {html_path}"
             logger.warn(warn_msg)
             raise FileNotFoundError(warn_msg)
 
         encodings = ["utf-8", "latin-1"]
@@ -45,46 +57,51 @@
                 return False
         return True
 
     def md2html(self, md_str):
         return markdown2.markdown(md_str)
 
     def check_format(func):
-        def wrapper(self, html_str, format=None):
+        def wrapper(self, html_str, format=None, **kwargs):
             if format == "markdown":
                 html_str = self.md2html(html_str)
             format = "html"
-            return func(self, html_str, format)
+            return func(self, html_str, format, **kwargs)
 
         return wrapper
 
     @check_format
-    def split_html_str(self, html_str, format=None):
+    def split_html_str(self, html_str, format=None, page_idx=-1, remove_seps=False):
         results = []
         soup = BeautifulSoup(html_str, "html.parser")
         for idx, element in enumerate(soup.find_all(SPLIT_TAGS)):
             if not self.is_atomized(element):
                 continue
             element_str = str(element)
             markdown_str = purify_html_str(
                 element_str,
                 output_format="markdown",
                 keep_format_tags=False,
                 keep_group_tags=False,
                 math_style="latex",
             )
+
+            if remove_seps:
+                markdown_str = self.remove_separators(markdown_str)
+
             item = {
                 "html": element_str,
                 "text": markdown_str,
                 "tag": element.name,
                 "tag_type": self.get_tag_type(element),
                 "html_len": len(element_str),
                 "text_len": len(markdown_str),
                 "text_tokens": count_tokens(markdown_str),
                 "node_idx": idx,
+                "page_idx": page_idx,
             }
             results.append(item)
 
         return results
 
     def split_html_file(self, html_path, format=None):
         ext = Path(html_path).suffix
```

### Comparing `splitml-0.5/src/splitml/pdf_splitter.py` & `splitml-0.5.1/src/splitml/pdf_splitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from pathlib import Path
 
 from tclogger import logger
 from purehtml import purify_html_str
 
 from .html_splitter import HTMLSplitter
+from tqdm import tqdm
 
 
 class PDFSplitter:
-
     def split_pdf_doc(self, pdf_doc):
         results = []
         html_splitter = HTMLSplitter()
-        for page_idx, page in enumerate(pdf_doc):
-            logger.note(f"> Page {page_idx+1}")
+        for page_idx, page in enumerate(tqdm(pdf_doc)):
+            # logger.note(f"> Page {page_idx+1}")
             html_str = page.get_text("html")
             html_str = purify_html_str(html_str)
             # logger.mesg(html_str)
-            nodes = html_splitter.split_html_str(html_str, format=format)
+            nodes = html_splitter.split_html_str(
+                html_str, format="html", page_idx=page_idx
+            )
             results.extend(nodes)
 
         return results
 
     def read_pdf_bytes(self, pdf_bytes):
         # https://github.com/pymupdf/PyMuPDF/issues/612
         doc = fitz.open("pdf", pdf_bytes)
```

### Comparing `splitml-0.5/src/splitml/splitml.py` & `splitml-0.5.1/src/splitml/splitml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from pprint import pformat
 from typing import Union
 
 from tclogger import logger
 
 from .stats import stat_tokens
 from .groupers import NodesGrouper
 from .html_splitter import HTMLSplitter
@@ -78,10 +79,11 @@
         logger.note(f"> Processing: {pdf_path.name}")
         nodes = splitter.split_pdf_file(pdf_path)
         logger.success(f"  - {len(nodes)} nodes.")
         stat_tokens(nodes)
         grouped_nodes = NodesGrouper().group_nodes(nodes)
         logger.success(f"  - {len(grouped_nodes)} grouped nodes.")
         stat_tokens(grouped_nodes)
+    logger.success(pformat(grouped_nodes[0], indent=4, sort_dicts=False))
 
     # [**/src]
     # python -m splitml.splitml
```

### Comparing `splitml-0.5/src/splitml/stats.py` & `splitml-0.5.1/src/splitml/stats.py`

 * *Files identical despite different names*

### Comparing `splitml-0.5/src/splitml.egg-info/PKG-INFO` & `splitml-0.5.1/src/splitml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.5
+Version: 0.5.1
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


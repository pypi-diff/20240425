# Comparing `tmp/md2weasypdf-0.0.5.tar.gz` & `tmp/md2weasypdf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2weasypdf-0.0.5.tar", last modified: Tue Apr 23 06:20:04 2024, max compression
+gzip compressed data, was "md2weasypdf-0.0.6.tar", last modified: Thu Apr 25 07:01:38 2024, max compression
```

## Comparing `md2weasypdf-0.0.5.tar` & `md2weasypdf-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.291192 md2weasypdf-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-23 06:20:04.291192 md2weasypdf-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.287192 md2weasypdf-0.0.5/md2weasypdf/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.287192 md2weasypdf-0.0.5/md2weasypdf/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/textbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/toa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/md2weasypdf/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:20:04.287192 md2weasypdf-0.0.5/md2weasypdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 06:20:04.000000 md2weasypdf-0.0.5/md2weasypdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-23 06:20:04.291192 md2weasypdf-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:19:58.000000 md2weasypdf-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.180350 md2weasypdf-0.0.6/md2weasypdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/md2weasypdf/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/toa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/md2weasypdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/setup.py
```

### Comparing `md2weasypdf-0.0.5/LICENSE` & `md2weasypdf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/PKG-INFO` & `md2weasypdf-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.5/README.md` & `md2weasypdf-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/md2weasypdf/__main__.py` & `md2weasypdf-0.0.6/md2weasypdf/__main__.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/md2weasypdf/extensions/checkbox.py` & `md2weasypdf-0.0.6/md2weasypdf/extensions/checkbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/md2weasypdf/extensions/footnotes.py` & `md2weasypdf-0.0.6/md2weasypdf/extensions/footnotes.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,31 @@
 class FootnoteInlineProcessor(InlineProcessor):
     def __init__(self, pattern, footnotes):
         super().__init__(pattern)
         self.footnotes: FootnoteExtension = footnotes
 
     def handleMatch(self, m, data):
         note_id = m.group(1)
-        footnote = self.footnotes.footnotes[note_id]
-        if not footnote.inserted:
-            el = etree.Element("span", attrib={"class": "footnote", "data-footnote-id": note_id})
-            el.text = footnote.text
-            footnote.inserted = True
+        try:
+            footnote = self.footnotes.footnotes[note_id]
+
+        except KeyError:
+            return None, None, None
 
         else:
-            el = etree.Element("sup", attrib={"class": "footnote-ref", "data-footnote-id": note_id})
-            el.text = str(footnote.index)
+            if not footnote.inserted:
+                el = etree.Element("span", attrib={"class": "footnote", "data-footnote-id": note_id})
+                el.text = footnote.text
+                footnote.inserted = True
+
+            else:
+                el = etree.Element("sup", attrib={"class": "footnote-ref", "data-footnote-id": note_id})
+                el.text = str(footnote.index)
 
-        return el, m.start(0), m.end(0)
+            return el, m.start(0), m.end(0)
 
 
 def FootnoteTreeprocessor(Treeprocessor):
     pass
 
 
 class FootnoteExtension(Extension):
```

### Comparing `md2weasypdf-0.0.5/md2weasypdf/extensions/textbox.py` & `md2weasypdf-0.0.6/md2weasypdf/extensions/textbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/md2weasypdf/extensions/toa.py` & `md2weasypdf-0.0.6/md2weasypdf/extensions/toa.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/md2weasypdf/extensions/toc.py` & `md2weasypdf-0.0.6/md2weasypdf/extensions/toc.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/md2weasypdf/printer.py` & `md2weasypdf-0.0.6/md2weasypdf/printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,42 @@
 
 class Article(NamedTuple):
     source: Path
     title: str
     content: str
     meta: dict[str, object]
     has_custom_headline: bool
-    hash: str
+
+    @property
+    def hash(self):
+        return str(check_output(["git", "hash-object", self.source]), "utf-8")
+
+    @property
+    def modified_date(self):
+        return str(check_output(["git", "log", "-1", "--pretty=%cs", self.source]), "utf-8").strip()
 
 
 @dataclass
 class Document:
     title: str
     template: Template
     layout_dir: Path
     articles: List[Article]
 
+    @staticmethod
+    def get_commit():
+        if commit_sha_env := os.getenv("CI_COMMIT_SHORT_SHA", None):
+            return commit_sha_env
+
+        return str(check_output(["git", "rev-parse", "HEAD"]), "utf-8")[:8] + ("-dirty" if check_output(["git", "status", "-s"]) else "")
+
     def write_pdf(self, output_dir: Path, output_html: bool = False):
         html = self.template.render(
             date=date.today().isoformat(),
-            commit=os.getenv("CI_COMMIT_SHORT_SHA", "00000000"),
+            commit=self.get_commit(),
             articles=self.articles,
             title=self.title,
         )
 
         output_filename = self.title.replace(" ", "_")
         if output_html:
             with open(output_dir / f"{output_filename}.html", "w", encoding="utf-8") as html_file:
@@ -137,15 +151,14 @@
 
         return Article(
             source=source,
             title=source.name.removesuffix(".md").replace("_", " "),
             content=md.convert(content),
             meta=article.metadata,
             has_custom_headline=content.startswith("# "),
-            hash=str(check_output(["git", "hash-object", source]), "utf-8"),
         )
 
     def execute(self):
         self._load_template.cache_clear()
         articles: List[Article] = []
         if self.input.is_dir():
             for article_path in sorted(iglob(os.path.join(self.input, "**/*.md"), recursive=True)):
```

### Comparing `md2weasypdf-0.0.5/md2weasypdf.egg-info/PKG-INFO` & `md2weasypdf-0.0.6/md2weasypdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.5/md2weasypdf.egg-info/SOURCES.txt` & `md2weasypdf-0.0.6/md2weasypdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.5/setup.cfg` & `md2weasypdf-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md2weasypdf
-version = 0.0.5
+version = 0.0.6
 author = Manuel Stingl
 author_email = contact@stingl.st
 description = Print PDFs from Markdown Files using Weasyprint
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```


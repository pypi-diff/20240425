# Comparing `tmp/md2weasypdf-0.0.6.tar.gz` & `tmp/md2weasypdf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2weasypdf-0.0.6.tar", last modified: Thu Apr 25 07:01:38 2024, max compression
+gzip compressed data, was "md2weasypdf-0.0.7.tar", last modified: Thu Apr 25 09:41:19 2024, max compression
```

## Comparing `md2weasypdf-0.0.6.tar` & `md2weasypdf-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.180350 md2weasypdf-0.0.6/md2weasypdf/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/md2weasypdf/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/textbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/toa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/md2weasypdf/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/md2weasypdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 07:01:38.000000 md2weasypdf-0.0.6/md2weasypdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 07:01:38.184350 md2weasypdf-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:01:34.000000 md2weasypdf-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.685788 md2weasypdf-0.0.7/md2weasypdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/md2weasypdf/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/toa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/md2weasypdf/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/md2weasypdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 09:41:19.000000 md2weasypdf-0.0.7/md2weasypdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 09:41:19.689788 md2weasypdf-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:41:14.000000 md2weasypdf-0.0.7/setup.py
```

### Comparing `md2weasypdf-0.0.6/LICENSE` & `md2weasypdf-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/PKG-INFO` & `md2weasypdf-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.6/README.md` & `md2weasypdf-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/md2weasypdf/__main__.py` & `md2weasypdf-0.0.7/md2weasypdf/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import time
 import warnings
 from functools import partial
 from pathlib import Path
 from threading import Timer
 from typing import Callable, Optional
 
@@ -61,33 +62,38 @@
 
 def main(
     input: Annotated[Path, typer.Argument(help="Folder or file used as input")],
     output_dir: Annotated[Path, typer.Argument(help="Folder where resulting files are written to")] = Path("."),
     *,
     bundle: Annotated[bool, typer.Option(help="Bundle all input documents into a single output file")] = False,
     title: Annotated[Optional[str], typer.Option(help="Title of the resulting document. Can only be used in conjunction with bundle.")] = None,
-    layouts_dir: Annotated[Path, typer.Option(help="Base folder containing the available layouts")] = "layouts",
+    layouts_dir: Annotated[Path, typer.Option(help="Base folder containing the available layouts")] = Path("./layouts"),
     layout: Annotated[Optional[str], typer.Option(help="Default layout to use")] = None,
     output_html: Annotated[bool, typer.Option(help="Additionally output the raw HTML file which is used to create the pdf")] = False,
     filename_filter: Annotated[
         Optional[str],
         typer.Option(help="Regular expression to filter files in input directory by subpath and/or filename"),
     ] = None,
+    meta: Annotated[
+        Optional[str],
+        typer.Option(help="Metadata for document generation passed to the layout, pass values using a JSON object"),
+    ] = None,
     watch: Annotated[bool, typer.Option(help="Watch input directory for changes and re-run the conversion")] = False,
 ):
     try:
         printer = Printer(
             input=input,
             output_dir=output_dir,
             layouts_dir=layouts_dir,
             bundle=bundle,
             title=title,
             layout=layout,
             output_html=output_html,
             filename_filter=filename_filter,
+            meta=json.loads(meta) if meta else None,
         )
 
     except ValueError as error:
         console.print("Error:", error, style="bold red")
         raise typer.Exit(1)
 
     def execute():
```

### Comparing `md2weasypdf-0.0.6/md2weasypdf/extensions/checkbox.py` & `md2weasypdf-0.0.7/md2weasypdf/extensions/checkbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/md2weasypdf/extensions/footnotes.py` & `md2weasypdf-0.0.7/md2weasypdf/extensions/footnotes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xml.etree.ElementTree as etree
 from dataclasses import dataclass
 from typing import Dict
 
 from markdown import Markdown
-from markdown.extensions import Extension, footnotes
+from markdown.extensions import footnotes
 from markdown.inlinepatterns import InlineProcessor
 
 
 @dataclass
 class Footnote:
     text: str
     index: int
@@ -36,27 +36,22 @@
             else:
                 el = etree.Element("sup", attrib={"class": "footnote-ref", "data-footnote-id": note_id})
                 el.text = str(footnote.index)
 
             return el, m.start(0), m.end(0)
 
 
-def FootnoteTreeprocessor(Treeprocessor):
-    pass
-
-
-class FootnoteExtension(Extension):
+class FootnoteExtension(footnotes.FootnoteExtension):
     def __init__(self):
         self.footnotes: Dict[str, Footnote] = {}
 
     def setFootnote(self, id, text):
         self.footnotes[id] = Footnote(text, len(self.footnotes) + 1)
 
     def extendMarkdown(self, md: Markdown):
         md.registerExtension(self)
         self.parser = md.parser
         self.md = md
 
         md.parser.blockprocessors.register(footnotes.FootnoteBlockProcessor(self), 'footnote', 17)
         FOOTNOTE_RE = r'\[\^([^\]]*)\]'  # blah blah [^1] blah
         md.inlinePatterns.register(FootnoteInlineProcessor(FOOTNOTE_RE, self), 'footnote', 170)
-        # md.treeprocessors.register(FootnoteTreeprocessor(self), 'footnote', 45)
```

### Comparing `md2weasypdf-0.0.6/md2weasypdf/extensions/textbox.py` & `md2weasypdf-0.0.7/md2weasypdf/extensions/textbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/md2weasypdf/extensions/toa.py` & `md2weasypdf-0.0.7/md2weasypdf/extensions/toa.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/md2weasypdf/extensions/toc.py` & `md2weasypdf-0.0.7/md2weasypdf/extensions/toc.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/md2weasypdf/printer.py` & `md2weasypdf-0.0.7/md2weasypdf/printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,30 @@
 
 @dataclass
 class Document:
     title: str
     template: Template
     layout_dir: Path
     articles: List[Article]
+    meta: dict[str, object]
 
     @staticmethod
     def get_commit():
         if commit_sha_env := os.getenv("CI_COMMIT_SHORT_SHA", None):
             return commit_sha_env
 
         return str(check_output(["git", "rev-parse", "HEAD"]), "utf-8")[:8] + ("-dirty" if check_output(["git", "status", "-s"]) else "")
 
     def write_pdf(self, output_dir: Path, output_html: bool = False):
         html = self.template.render(
             date=date.today().isoformat(),
             commit=self.get_commit(),
             articles=self.articles,
             title=self.title,
+            meta=self.meta,
         )
 
         output_filename = self.title.replace(" ", "_")
         if output_html:
             with open(output_dir / f"{output_filename}.html", "w", encoding="utf-8") as html_file:
                 html_file.write(html)
 
@@ -90,23 +92,25 @@
         output_dir: Path,
         layouts_dir: Path = Path("layouts"),
         bundle: bool = False,
         title: Optional[str] = None,
         layout: Optional[str] = None,
         output_html: bool = False,
         filename_filter: Optional[str] = None,
+        meta: Optional[dict[str, object]] = None,
     ):
         self.input = self._ensure_path(input)
         self.output_dir = self._ensure_path(output_dir, dir=True, create=True)
         self.layouts_dir = self._ensure_path(layouts_dir, dir=True)
         self.bundle = bundle
         self.title = title
         self.layout = layout
         self.output_html = output_html
         self.filename_filter = re.compile(filename_filter) if filename_filter else None
+        self.meta = meta or {}
         self.jinja_env = Environment(
             autoescape=select_autoescape(),
             loader=FileSystemLoader(searchpath=[self.layouts_dir]),
         )
 
         if self.bundle:
             if not self.layout or not self.title:
@@ -173,27 +177,29 @@
         else:
             articles.append(self._load_article(self.input))
 
         write_options = {"output_dir": self.output_dir, "output_html": self.output_html}
 
         if self.bundle:
             doc = Document(
-                self.title,
+                self.title,  # type: ignore  # title cannot be empty when bundle is set
                 *self._load_template(self.layout),
-                articles,
+                articles=articles,
+                meta=self.meta,
             )
             yield doc, doc.write_pdf(**write_options)
 
         else:
             for article in articles:
                 try:
                     doc = Document(
                         article.title,
                         *self._load_template(article.meta.get('layout', self.layout)),
-                        [article],
+                        articles=[article],
+                        meta=self.meta | article.meta,
                     )
 
                 except ValueError as error:
                     raise ValueError(f"Could not create document for {article.source}: {error}") from error
 
                 yield doc, doc.write_pdf(**write_options)
```

### Comparing `md2weasypdf-0.0.6/md2weasypdf.egg-info/PKG-INFO` & `md2weasypdf-0.0.7/md2weasypdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `md2weasypdf-0.0.6/md2weasypdf.egg-info/SOURCES.txt` & `md2weasypdf-0.0.7/md2weasypdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.6/setup.cfg` & `md2weasypdf-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md2weasypdf
-version = 0.0.6
+version = 0.0.7
 author = Manuel Stingl
 author_email = contact@stingl.st
 description = Print PDFs from Markdown Files using Weasyprint
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```


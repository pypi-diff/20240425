# Comparing `tmp/rich-rst-1.2.0.tar.gz` & `tmp/rich_rst-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-rst-1.2.0.tar", last modified: Fri Jan 26 19:08:31 2024, max compression
+gzip compressed data, was "rich_rst-1.3.0.tar", last modified: Thu Apr 25 18:51:41 2024, max compression
```

## Comparing `rich-rst-1.2.0.tar` & `rich_rst-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 19:08:31.576624 rich-rst-1.2.0/
--rw-rw-rw-   0        0        0     1056 2022-02-06 12:37:40.000000 rich-rst-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     5962 2024-01-26 19:08:31.575647 rich-rst-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2022-02-10 16:31:46.000000 rich-rst-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-26 19:08:31.563931 rich-rst-1.2.0/rich_rst/
--rw-rw-rw-   0        0        0    29246 2024-01-26 19:04:34.000000 rich-rst-1.2.0/rich_rst/__init__.py
--rw-rw-rw-   0        0        0     4681 2024-01-26 19:01:42.000000 rich-rst-1.2.0/rich_rst/__main__.py
-drwxrwxrwx   0        0        0        0 2024-01-26 19:08:31.573697 rich-rst-1.2.0/rich_rst.egg-info/
--rw-rw-rw-   0        0        0     5962 2024-01-26 19:08:31.000000 rich-rst-1.2.0/rich_rst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-01-26 19:08:31.000000 rich-rst-1.2.0/rich_rst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 19:08:31.000000 rich-rst-1.2.0/rich_rst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-01-26 19:08:31.000000 rich-rst-1.2.0/rich_rst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-26 19:08:31.000000 rich-rst-1.2.0/rich_rst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1412 2024-01-26 19:08:31.577601 rich-rst-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-02-06 05:09:36.000000 rich-rst-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.292364 rich_rst-1.3.0/
+-rw-rw-rw-   0        0        0     1056 2022-02-06 12:37:40.000000 rich_rst-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5962 2024-04-25 18:51:41.292364 rich_rst-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4520 2022-02-10 16:31:46.000000 rich_rst-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.263064 rich_rst-1.3.0/rich_rst/
+-rw-rw-rw-   0        0        0    29705 2024-04-25 18:49:52.000000 rich_rst-1.3.0/rich_rst/__init__.py
+-rw-rw-rw-   0        0        0     4681 2024-01-26 19:01:42.000000 rich_rst-1.3.0/rich_rst/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.291387 rich_rst-1.3.0/rich_rst.egg-info/
+-rw-rw-rw-   0        0        0     5962 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1412 2024-04-25 18:51:41.300175 rich_rst-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-02-06 05:09:36.000000 rich_rst-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.289433 rich_rst-1.3.0/tests/
+-rw-rw-rw-   0        0        0     1593 2024-04-25 18:47:41.000000 rich_rst-1.3.0/tests/test_main.py
```

### Comparing `rich-rst-1.2.0/LICENSE` & `rich_rst-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-rst-1.2.0/PKG-INFO` & `rich_rst-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-rst
-Version: 1.2.0
+Version: 1.3.0
 Summary: A beautiful reStructuredText renderer for rich
 Home-page: https://wasi-master.github.io/rich-rst
 Author: Wasi Master
 Author-email: arianmollik323@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/wasi-master/rich-rst/issues
 Project-URL: Source, https://github.com/wasi-master/rich-rst
```

### Comparing `rich-rst-1.2.0/README.md` & `rich_rst-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rich-rst-1.2.0/rich_rst/__init__.py` & `rich_rst-1.3.0/rich_rst/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from rich.rule import Rule
 
 from pygments.lexers import guess_lexer
 from pygments.util import ClassNotFound
 
 __all__ = ("RST", "ReStructuredText", "reStructuredText", "RestructuredText")
 __author__ = "Arian Mollik Wasi (aka. Wasi Master)"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 install()
 
 
 class MLStripper(HTMLParser):
     """Utility class to strip out html for raw html source"""
     def __init__(self):
@@ -579,16 +579,22 @@
         self.log_errors = show_errors
         self.guess_lexer = guess_lexer
         self.default_lexer = default_lexer
         self.filename = filename
 
     def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult:
         # Parse the `markup` into a RST `document`.
-        option_parser = docutils.frontend.OptionParser(components=(docutils.parsers.rst.Parser,))
-        settings = option_parser.get_default_values()
+
+        # Docutils version compatability; from https://stackoverflow.com/a/75996218
+        if hasattr(docutils.frontend, 'get_default_settings'):
+            # docutils >= 0.18
+            settings = docutils.frontend.get_default_settings(docutils.parsers.rst.Parser)
+        else:
+            # docutils < 0.18
+            settings = docutils.frontend.OptionParser(components=(docutils.parsers.rst.Parser,)).get_default_values()
         settings.report_level = 69
         source = docutils.io.StringInput(self.markup)
         document = docutils.utils.new_document(self.filename, settings)
         rst_parser = docutils.parsers.rst.Parser()
         rst_parser.parse(source.read(), document)
 
         # Render the RST `document` using Rich.
@@ -597,14 +603,17 @@
             console=console,
             code_theme=self.code_theme,
             guess_lexer=self.guess_lexer,
             default_lexer=self.default_lexer,
         )
         document.walkabout(visitor)
 
+        if visitor.renderables and isinstance(visitor.renderables[-1], Text):
+            visitor.renderables[-1].rstrip()
+            visitor.renderables[-1].end = "\n"
         for renderable in visitor.renderables:
             yield from console.render(renderable, options)
         if self.log_errors and visitor.errors:
             for error in visitor.errors:
                 yield from console.render(error, options)
         style = console.get_style("restructuredtext.footer", default="none")
         border_style = console.get_style("restructuredtext.footer_border", default="grey74")
```

### Comparing `rich-rst-1.2.0/rich_rst/__main__.py` & `rich_rst-1.3.0/rich_rst/__main__.py`

 * *Files identical despite different names*

### Comparing `rich-rst-1.2.0/rich_rst.egg-info/PKG-INFO` & `rich_rst-1.3.0/rich_rst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-rst
-Version: 1.2.0
+Version: 1.3.0
 Summary: A beautiful reStructuredText renderer for rich
 Home-page: https://wasi-master.github.io/rich-rst
 Author: Wasi Master
 Author-email: arianmollik323@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/wasi-master/rich-rst/issues
 Project-URL: Source, https://github.com/wasi-master/rich-rst
```

### Comparing `rich-rst-1.2.0/setup.cfg` & `rich_rst-1.3.0/setup.cfg`

 * *Files identical despite different names*


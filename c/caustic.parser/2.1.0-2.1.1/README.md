# Comparing `tmp/caustic.parser-2.1.0.tar.gz` & `tmp/caustic.parser-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.parser-2.1.0.tar", last modified: Wed Apr 24 22:01:26 2024, max compression
+gzip compressed data, was "caustic.parser-2.1.1.tar", last modified: Thu Apr 25 04:28:25 2024, max compression
```

## Comparing `caustic.parser-2.1.0.tar` & `caustic.parser-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.417215 caustic.parser-2.1.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.1.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-24 22:01:26.413881 caustic.parser-2.1.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.1.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-24 22:00:47.000000 caustic.parser-2.1.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 22:01:26.417215 caustic.parser-2.1.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.407215 caustic.parser-2.1.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.407215 caustic.parser-2.1.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.413881 caustic.parser-2.1.0/src/caustic/parser/
--rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.1.0/src/caustic/parser/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     4274 2024-04-24 20:50:46.000000 caustic.parser-2.1.0/src/caustic/parser/cli.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3303 2024-04-24 21:45:30.000000 caustic.parser-2.1.0/src/caustic/parser/error.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.413881 caustic.parser-2.1.0/src/caustic.parser.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/entry_points.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 04:28:25.467044 caustic.parser-2.1.1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.1.1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 04:28:25.467044 caustic.parser-2.1.1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.1.1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-25 04:14:55.000000 caustic.parser-2.1.1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-25 04:28:25.467044 caustic.parser-2.1.1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 04:28:25.460378 caustic.parser-2.1.1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 04:28:25.460378 caustic.parser-2.1.1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 04:28:25.467044 caustic.parser-2.1.1/src/caustic/parser/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.1.1/src/caustic/parser/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     4274 2024-04-24 20:50:46.000000 caustic.parser-2.1.1/src/caustic/parser/cli.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3305 2024-04-25 04:27:15.000000 caustic.parser-2.1.1/src/caustic/parser/error.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 04:28:25.467044 caustic.parser-2.1.1/src/caustic.parser.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 04:28:25.000000 caustic.parser-2.1.1/src/caustic.parser.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-25 04:28:25.000000 caustic.parser-2.1.1/src/caustic.parser.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-25 04:28:25.000000 caustic.parser-2.1.1/src/caustic.parser.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-25 04:28:25.000000 caustic.parser-2.1.1/src/caustic.parser.egg-info/entry_points.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-25 04:28:25.000000 caustic.parser-2.1.1/src/caustic.parser.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-25 04:28:25.000000 caustic.parser-2.1.1/src/caustic.parser.egg-info/top_level.txt
```

### Comparing `caustic.parser-2.1.0/LICENSE` & `caustic.parser-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.1.0/PKG-INFO` & `caustic.parser-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.1.0
+Version: 2.1.1
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `caustic.parser-2.1.0/README.md` & `caustic.parser-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.1.0/pyproject.toml` & `caustic.parser-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.parser"
-version = "2.1.0"
+version = "2.1.1"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's parsing framework"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'syntax', 'grammar']
```

### Comparing `caustic.parser-2.1.0/src/caustic/parser/__init__.py` & `caustic.parser-2.1.1/src/caustic/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.1.0/src/caustic/parser/cli.py` & `caustic.parser-2.1.1/src/caustic/parser/cli.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.1.0/src/caustic/parser/error.py` & `caustic.parser-2.1.1/src/caustic/parser/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,37 +19,37 @@
             return f'/{r.regex.pattern}/'
         case parglare.grammar.StringRecognizer():
             return repr(r.value_cmp)
         case _:
             return repr(r)
 
 def format_pre_context(l: parglare.common.Location, lines: list[str], llen: int) -> cabc.Generator[str, None, None]:
-    yield f'{(l.line-2):0{llen}} {lines[l.line-2]}\n'
+    yield f'{(l.line-1):0{llen}} {lines[l.line-2]}\n'
 def format_post_context(l: parglare.common.Location, lines: list[str], llen: int) -> cabc.Generator[str, None, None]:
-    yield f'\n{(l.line_end-1):0{llen}} {lines[l.line_end-1]}'
+    yield f'\n{(l.line_end+1):0{llen}} {lines[l.line_end]}'
 def format_inner_context(l: parglare.common.Location, lines: list[str], llen: int) -> cabc.Generator[str, None, None]:
     if l.line == l.line_end:
         yield f'{l.line:0{llen}} {lines[l.line-1]}\n'
         yield f'{" "*llen} {" "*(l.column)}^'
         if l.column != l.column_end:
-            yield f'{"~"*(l.column_end-l.column)}^'
+            yield f'{"~"*(l.column_end-l.column-1)}^'
         return
     yield f'{" "*llen} {" "*(l.column-1)}v\n'
-    for ln in range(l.line, l.line_end):
+    for ln in range(l.line, l.line_end+1):
         yield f'{ln:0{llen}} {lines[ln-1]}\n'
-    yield f'{" "*llen} {" "*(l.column_end-1)}^'
+    yield f'{" "*llen} {" "*(l.column_end)}^'
 
 def format_context(l: parglare.common.Location,
                    precontext: bool = True, postcontext: bool = True) -> cabc.Generator[str, None, None]:
     lines = l.input_str.split('\n')
     llen = len(str(l.line_end))
     if precontext and (l.line > 1):
         yield from format_pre_context(l, lines, llen)
     yield from format_inner_context(l, lines, llen)
-    if postcontext and (l.line_end < len(lines)):
+    if postcontext and (l.line_end+1 < len(lines)):
         yield from format_post_context(l, lines, llen)
     
 
 def iformat_exc(e: parglare.ParseError, *, verbose_got: bool = False,
                 precontext: bool = True, postcontext: bool = True) -> cabc.Generator[str, None, None]:
     '''
         Formats a parsing error
```

### Comparing `caustic.parser-2.1.0/src/caustic.parser.egg-info/PKG-INFO` & `caustic.parser-2.1.1/src/caustic.parser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.1.0
+Version: 2.1.1
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


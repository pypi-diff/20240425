# Comparing `tmp/caustic.parser-2.2.1.tar.gz` & `tmp/caustic.parser-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.parser-2.2.1.tar", last modified: Thu Apr 25 05:56:03 2024, max compression
+gzip compressed data, was "caustic.parser-2.2.2.tar", last modified: Thu Apr 25 17:27:39 2024, max compression
```

## Comparing `caustic.parser-2.2.1.tar` & `caustic.parser-2.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 05:56:03.997094 caustic.parser-2.2.1/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.1/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 05:56:03.997094 caustic.parser-2.2.1/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.1/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-25 05:48:42.000000 caustic.parser-2.2.1/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-25 05:56:03.997094 caustic.parser-2.2.1/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 05:56:03.990428 caustic.parser-2.2.1/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 05:56:03.990428 caustic.parser-2.2.1/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 05:56:03.993761 caustic.parser-2.2.1/src/caustic/parser/
--rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.1/src/caustic/parser/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     5307 2024-04-25 05:54:48.000000 caustic.parser-2.2.1/src/caustic/parser/cli.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3305 2024-04-25 04:27:15.000000 caustic.parser-2.2.1/src/caustic/parser/error.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 05:56:03.993761 caustic.parser-2.2.1/src/caustic.parser.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 05:56:03.000000 caustic.parser-2.2.1/src/caustic.parser.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-25 05:56:03.000000 caustic.parser-2.2.1/src/caustic.parser.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-25 05:56:03.000000 caustic.parser-2.2.1/src/caustic.parser.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-25 05:56:03.000000 caustic.parser-2.2.1/src/caustic.parser.egg-info/entry_points.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-25 05:56:03.000000 caustic.parser-2.2.1/src/caustic.parser.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-25 05:56:03.000000 caustic.parser-2.2.1/src/caustic.parser.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.2/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.2/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-25 16:57:24.000000 caustic.parser-2.2.2/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.963727 caustic.parser-2.2.2/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.963727 caustic.parser-2.2.2/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/src/caustic/parser/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.2/src/caustic/parser/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     5307 2024-04-25 16:58:16.000000 caustic.parser-2.2.2/src/caustic/parser/cli.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3305 2024-04-25 04:27:15.000000 caustic.parser-2.2.2/src/caustic/parser/error.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-25 17:27:39.970394 caustic.parser-2.2.2/src/caustic.parser.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/entry_points.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-25 17:27:39.000000 caustic.parser-2.2.2/src/caustic.parser.egg-info/top_level.txt
```

### Comparing `caustic.parser-2.2.1/LICENSE` & `caustic.parser-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.1/PKG-INFO` & `caustic.parser-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.1
+Version: 2.2.2
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `caustic.parser-2.2.1/README.md` & `caustic.parser-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.1/pyproject.toml` & `caustic.parser-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.parser"
-version = "2.2.1"
+version = "2.2.2"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's parsing framework"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'syntax', 'grammar']
```

### Comparing `caustic.parser-2.2.1/src/caustic/parser/__init__.py` & `caustic.parser-2.2.2/src/caustic/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.1/src/caustic/parser/cli.py` & `caustic.parser-2.2.2/src/caustic/parser/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         SOURCE is the file to compile (defaults to STDIN)
 
         Note that the "pickle" format is the only format that can be used by the (default) compiler
             "pretty" is recommended for viewing (without post-processing)
         Note that the "tree" format will force the LR (the default parser if --glr is not set) parser to generate a tree
     '''
-    error = lambda *a,**kw: click.echo(click.style(*a), (255, 63, 63), color=True, file=sys.stderr, **kw)
+    error = lambda *a,**kw: click.echo(click.style(*a, (255, 63, 63)), color=True, file=sys.stderr, **kw)
     debug = (lambda *a,**kw: None) if quiet else (lambda *a,**kw: click.echo(*a, file=sys.stderr, **kw))
     real_source = str(source) != '-'
     tree_fmt = format == 'tree'
     # Load grammar
     if grammar is None:
         grammar = default_grammar()
         debug(f'Default grammar discovered at {grammar}')
```

### Comparing `caustic.parser-2.2.1/src/caustic/parser/error.py` & `caustic.parser-2.2.2/src/caustic/parser/error.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.1/src/caustic.parser.egg-info/PKG-INFO` & `caustic.parser-2.2.2/src/caustic.parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.1
+Version: 2.2.2
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


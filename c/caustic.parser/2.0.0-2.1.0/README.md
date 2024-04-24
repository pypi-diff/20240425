# Comparing `tmp/caustic.parser-2.0.0.tar.gz` & `tmp/caustic.parser-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.parser-2.0.0.tar", last modified: Wed Apr 24 21:01:26 2024, max compression
+gzip compressed data, was "caustic.parser-2.1.0.tar", last modified: Wed Apr 24 22:01:26 2024, max compression
```

## Comparing `caustic.parser-2.0.0.tar` & `caustic.parser-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 21:01:26.063847 caustic.parser-2.0.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.0.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     1919 2024-04-24 21:01:26.063847 caustic.parser-2.0.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.0.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1055 2024-04-24 20:51:10.000000 caustic.parser-2.0.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 21:01:26.063847 caustic.parser-2.0.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 21:01:26.057180 caustic.parser-2.0.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 21:01:26.057180 caustic.parser-2.0.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 21:01:26.060514 caustic.parser-2.0.0/src/caustic/parser/
--rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.0.0/src/caustic/parser/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     4274 2024-04-24 20:50:46.000000 caustic.parser-2.0.0/src/caustic/parser/cli.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1637 2024-04-24 15:53:12.000000 caustic.parser-2.0.0/src/caustic/parser/error.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 21:01:26.060514 caustic.parser-2.0.0/src/caustic.parser.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     1919 2024-04-24 21:01:25.000000 caustic.parser-2.0.0/src/caustic.parser.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-24 21:01:26.000000 caustic.parser-2.0.0/src/caustic.parser.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 21:01:25.000000 caustic.parser-2.0.0/src/caustic.parser.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-24 21:01:25.000000 caustic.parser-2.0.0/src/caustic.parser.egg-info/entry_points.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-24 21:01:25.000000 caustic.parser-2.0.0/src/caustic.parser.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 21:01:25.000000 caustic.parser-2.0.0/src/caustic.parser.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.417215 caustic.parser-2.1.0/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.1.0/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-24 22:01:26.413881 caustic.parser-2.1.0/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.1.0/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1001 2024-04-24 22:00:47.000000 caustic.parser-2.1.0/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 22:01:26.417215 caustic.parser-2.1.0/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.407215 caustic.parser-2.1.0/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.407215 caustic.parser-2.1.0/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.413881 caustic.parser-2.1.0/src/caustic/parser/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.1.0/src/caustic/parser/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     4274 2024-04-24 20:50:46.000000 caustic.parser-2.1.0/src/caustic/parser/cli.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3303 2024-04-24 21:45:30.000000 caustic.parser-2.1.0/src/caustic/parser/error.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 22:01:26.413881 caustic.parser-2.1.0/src/caustic.parser.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1860 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/entry_points.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       13 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 22:01:26.000000 caustic.parser-2.1.0/src/caustic.parser.egg-info/top_level.txt
```

### Comparing `caustic.parser-2.0.0/LICENSE` & `caustic.parser-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.0.0/PKG-INFO` & `caustic.parser-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.0.0
+Version: 2.1.0
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Other
 Classifier: Topic :: File Formats
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Compilers
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
```

### Comparing `caustic.parser-2.0.0/README.md` & `caustic.parser-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.0.0/pyproject.toml` & `caustic.parser-2.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.parser"
-version = "2.0.0"
+version = "2.1.0"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's parsing framework"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'syntax', 'grammar']
@@ -13,15 +13,14 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Other",
     "Topic :: File Formats",
     "Topic :: Software Development",
     "Topic :: Software Development :: Compilers",
-    "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Interpreters",
 ]
 
 [project.urls]
 Homepage = "https://codeberg.org/Caustic/CausticParser"
 Issues = "https://codeberg.org/Caustic/CausticParser/issues"
```

### Comparing `caustic.parser-2.0.0/src/caustic/parser/__init__.py` & `caustic.parser-2.1.0/src/caustic/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.0.0/src/caustic/parser/cli.py` & `caustic.parser-2.1.0/src/caustic/parser/cli.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.0.0/src/caustic.parser.egg-info/PKG-INFO` & `caustic.parser-2.1.0/src/caustic.parser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.0.0
+Version: 2.1.0
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Other
 Classifier: Topic :: File Formats
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Compilers
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
```


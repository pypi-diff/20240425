# Comparing `tmp/caustic.cst-1.0.0.tar.gz` & `tmp/caustic.cst-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.cst-1.0.0.tar", last modified: Wed Apr 24 16:01:16 2024, max compression
+gzip compressed data, was "caustic.cst-1.1.0.tar", last modified: Wed Apr 24 16:45:35 2024, max compression
```

## Comparing `caustic.cst-1.0.0.tar` & `caustic.cst-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:01:16.430384 caustic.cst-1.0.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-1.0.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)      982 2024-04-24 16:01:16.427051 caustic.cst-1.0.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      102 2024-04-23 20:25:04.000000 caustic.cst-1.0.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-04-23 20:26:37.000000 caustic.cst-1.0.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 16:01:16.430384 caustic.cst-1.0.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:01:16.417051 caustic.cst-1.0.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:01:16.417051 caustic.cst-1.0.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:01:16.427051 caustic.cst-1.0.0/src/caustic/cst/
--rw-r--r--   0 shae      (1000) shae      (1000)      314 2024-04-23 19:39:06.000000 caustic.cst-1.0.0/src/caustic/cst/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1248 2024-04-24 01:42:12.000000 caustic.cst-1.0.0/src/caustic/cst/atom.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1565 2024-04-24 01:14:03.000000 caustic.cst-1.0.0/src/caustic/cst/bases.py
--rw-r--r--   0 shae      (1000) shae      (1000)      485 2024-04-24 01:40:40.000000 caustic.cst-1.0.0/src/caustic/cst/block.py
--rw-r--r--   0 shae      (1000) shae      (1000)     4127 2024-04-24 02:01:35.000000 caustic.cst-1.0.0/src/caustic/cst/expression.py
--rw-r--r--   0 shae      (1000) shae      (1000)     2398 2024-04-23 22:09:49.000000 caustic.cst-1.0.0/src/caustic/cst/statement.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:01:16.427051 caustic.cst-1.0.0/src/caustic.cst.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)      982 2024-04-24 16:01:16.000000 caustic.cst-1.0.0/src/caustic.cst.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      349 2024-04-24 16:01:16.000000 caustic.cst-1.0.0/src/caustic.cst.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 16:01:16.000000 caustic.cst-1.0.0/src/caustic.cst.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 16:01:16.000000 caustic.cst-1.0.0/src/caustic.cst.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:45:35.267037 caustic.cst-1.1.0/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-1.1.0/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     3602 2024-04-24 16:45:35.263703 caustic.cst-1.1.0/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     2722 2024-04-24 16:42:56.000000 caustic.cst-1.1.0/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-04-24 16:36:29.000000 caustic.cst-1.1.0/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-24 16:45:35.267037 caustic.cst-1.1.0/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:45:35.257037 caustic.cst-1.1.0/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:45:35.257037 caustic.cst-1.1.0/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:45:35.263703 caustic.cst-1.1.0/src/caustic/cst/
+-rw-r--r--   0 shae      (1000) shae      (1000)      333 2024-04-24 16:34:28.000000 caustic.cst-1.1.0/src/caustic/cst/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1248 2024-04-24 01:42:12.000000 caustic.cst-1.1.0/src/caustic/cst/atom.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1565 2024-04-24 01:14:03.000000 caustic.cst-1.1.0/src/caustic/cst/bases.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      485 2024-04-24 01:40:40.000000 caustic.cst-1.1.0/src/caustic/cst/block.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     4127 2024-04-24 02:01:35.000000 caustic.cst-1.1.0/src/caustic/cst/expression.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:45:35.263703 caustic.cst-1.1.0/src/caustic/cst/mods/
+-rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-04-24 16:44:17.000000 caustic.cst-1.1.0/src/caustic/cst/mods/m_exception.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1673 2024-04-24 16:43:54.000000 caustic.cst-1.1.0/src/caustic/cst/statement.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-24 16:45:35.263703 caustic.cst-1.1.0/src/caustic.cst.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     3602 2024-04-24 16:45:35.000000 caustic.cst-1.1.0/src/caustic.cst.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      385 2024-04-24 16:45:35.000000 caustic.cst-1.1.0/src/caustic.cst.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-24 16:45:35.000000 caustic.cst-1.1.0/src/caustic.cst.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-24 16:45:35.000000 caustic.cst-1.1.0/src/caustic.cst.egg-info/top_level.txt
```

### Comparing `caustic.cst-1.0.0/LICENSE` & `caustic.cst-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.0.0/pyproject.toml` & `caustic.cst-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.cst"
-version = "1.0.0"
+version = "1.1.0"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's Abstract Syntax Tree, or CST"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'ast', 'syntax', 'tree']
```

### Comparing `caustic.cst-1.0.0/src/caustic/cst/atom.py` & `caustic.cst-1.1.0/src/caustic/cst/atom.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.0.0/src/caustic/cst/bases.py` & `caustic.cst-1.1.0/src/caustic/cst/bases.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.0.0/src/caustic/cst/expression.py` & `caustic.cst-1.1.0/src/caustic/cst/expression.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.0.0/src/caustic/cst/statement.py` & `caustic.cst-1.1.0/src/caustic/cst/statement.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 #!/bin/python3
 
 '''CST nodes for statements'''
 
 #> Imports
 import typing
 from dataclasses import dataclass, field
-from collections import abc as cabc
 
 from .bases import CausticASTNode, BaseStatement
 from .block import Block, Line
 #</Imports
 
 #> Header >/
 __all__ = ('ImportStatement', 'ExportStatement',
            'IfStatement', 'ElifStatement', 'ElseStatement',
-           'ForStatement', 'WhileStatement',
-           'RaiseStatement', 'TryStatement', 'CatchStatement', 'LowerStatement')
+           'ForStatement', 'WhileStatement')
 
 _dc = dataclass(slots=True)
 
 # External-related
 @_dc
 class ImportStatement(BaseStatement):
     '''Represents an import'''
@@ -57,24 +55,7 @@
     for_in: bool = field(default=False, kw_only=True)
 @_dc
 class WhileStatement(BaseStatement):
     '''Represents a while loop'''
     clause: CausticASTNode
     block: Block
     do_while: bool = field(default=False, kw_only=True)
-
-# Exception-related
-class RaiseStatement(BaseStatement):
-    '''Represents an exception-raising statement'''
-    target: CausticASTNode
-class TryStatement(BaseStatement):
-    '''Represents an exception-handling statement/block'''
-    block: Block
-    catch: 'CatchStatement' = field(kw_only=True)
-class CatchStatement(BaseStatement):
-    '''Represents the "catch" part of a `TryStatement`'''
-    catches: cabc.Sequence[CausticASTNode]
-    block: Block
-class LowerStatement(BaseStatement):
-    '''Represents an exception-ignoring statement/block'''
-    lowers: cabc.Sequence[CausticASTNode]
-    block: Block
```


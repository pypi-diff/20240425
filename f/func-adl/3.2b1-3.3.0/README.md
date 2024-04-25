# Comparing `tmp/func_adl-3.2b1.tar.gz` & `tmp/func_adl-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/func_adl-3.2b1.tar", last modified: Sun Feb 12 10:04:09 2023, max compression
+gzip compressed data, was "dist/func_adl-3.3.0.tar", last modified: Thu Apr 25 00:51:17 2024, max compression
```

## Comparing `func_adl-3.2b1.tar` & `func_adl-3.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-02-12 10:04:09.000000 func_adl-3.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-02-12 10:04:06.000000 func_adl-3.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl/ast/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/aggregate_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/ast_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/call_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/func_adl_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/function_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/syntatic_sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/object_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23874 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/util_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/util_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-12 10:04:06.000000 func_adl-3.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 10:04:09.000000 func_adl-3.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-02-12 10:04:06.000000 func_adl-3.2b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_object_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    28551 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_type_based_replacement_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_util_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-25 00:51:17.000000 func_adl-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-25 00:51:09.000000 func_adl-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/aggregate_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/ast_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/call_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/func_adl_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/function_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/ast/syntatic_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15904 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35421 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-25 00:51:09.000000 func_adl-3.3.0/func_adl/util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 00:51:17.000000 func_adl-3.3.0/func_adl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 00:51:09.000000 func_adl-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:51:17.000000 func_adl-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-25 00:51:09.000000 func_adl-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:51:17.000000 func_adl-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30055 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_type_based_replacement_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-25 00:51:09.000000 func_adl-3.3.0/tests/test_util_types.py
```

### Comparing `func_adl-3.2b1/PKG-INFO` & `func_adl-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: func_adl
-Version: 3.2b1
+Version: 3.3.0
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
-License: TBD
+License: MIT
 Platform: Any
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
 
 # func_adl
 
  Construct hierarchical data queries using SQL-like concepts in python.
```

### Comparing `func_adl-3.2b1/README.md` & `func_adl-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/ast/aggregate_shortcuts.py` & `func_adl-3.3.0/func_adl/ast/aggregate_shortcuts.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/ast/call_stack.py` & `func_adl-3.3.0/func_adl/ast/call_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-# Implement a call stack which can be used in all our ast parsers
+import ast
+from typing import Dict, List, Optional
 
 
 class argument_stack:
     """
     Simple stack class to hold name definitions. Each level
     can hide variables in the previous level if their names are the same.
     Otherwise it is possible to see them. When you pop a frame off,
     then all defined variables go away.
     """
 
     def __init__(self):
-        self._arg_transformer = [{}]
+        self._arg_transformer: List[Dict[str, ast.AST]] = [{}]
 
     def push_stack_frame(self):
         "Create a new frame in which to define variables"
         self._arg_transformer.append({})
 
     def pop_stack_frame(self):
-        "Remove the top most stack frame and discard the varables defined there"
+        "Remove the top most stack frame and discard the variables defined there"
         del self._arg_transformer[-1]
 
-    def lookup_name(self, name, default=None):
+    def lookup_name(self, name: str, default: Optional[ast.AST] = None) -> Optional[ast.AST]:
         """
         Look up name starting from the deepest frame
         on up until it is found.
-        Return name if it is not found.
 
         name - the name we should look up. Any object that can be a key in a dict
-        default - If none, if the name can't be found, return the name. Otherwise return whatever
-        default is.
+        default - returned if `name` can't be found.
         """
         for frames in reversed(self._arg_transformer):
             if name in frames:
                 return frames[name]
-        return name if default is None else default
+        return default
 
-    def define_name(self, name, val):
+    def define_name(self, name: str, val: ast.AST):
         "Add a definition to the current deepest stack frame"
         self._arg_transformer[-1][name] = val
 
 
 class stack_frame:
     """
     Python resource management class to deal with
```

### Comparing `func_adl-3.2b1/func_adl/ast/func_adl_ast_utils.py` & `func_adl-3.3.0/func_adl/ast/func_adl_ast_utils.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/ast/function_simplifier.py` & `func_adl-3.3.0/func_adl/ast/function_simplifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
 
     def visit_Subscript_Tuple(self, v: ast.Tuple, s: Union[ast.Num, ast.Constant, ast.Index]):
         """
         (t1, t2, t3...)[1] => t2
 
         Only works if index is a number
         """
-        # Get the value out - this is due to supporting python 3.6-3.9
+        # Get the value out - this is due to supporting python 3.7-3.9
         n = _get_value_from_index(s)
         if n is None:
             return ast.Subscript(v, s, ast.Load())
         assert isinstance(n, int), "Programming error: index is not an integer in tuple subscript"
         if n >= len(v.elts):
             raise FuncADLIndexError(
                 f"Attempt to access the {n}th element of a tuple only"
@@ -560,15 +560,15 @@
         if isinstance(visited_value, ast.Dict):
             return self.visit_Subscript_Dict_with_value(visited_value, node.attr)
 
         return ast.Attribute(value=visited_value, attr=node.attr, ctx=ast.Load())
 
 
 def _get_value_from_index(arg: Union[ast.Num, ast.Constant, ast.Index, ast.Str]) -> Optional[int]:
-    """Deal with 3.6, 3.7, and 3.8 differences in how indexing for list and tuple
+    """Deal with 3.7, and 3.8 differences in how indexing for list and tuple
     subscripts is handled.
 
     Args:
         arg (Union[ast.Num, ast.Constant, ast.Index]): Input ast to extract an index from.
                                                        Hopefully.
     """
```

### Comparing `func_adl-3.2b1/func_adl/ast/meta_data.py` & `func_adl-3.3.0/func_adl/ast/meta_data.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/ast/syntatic_sugar.py` & `func_adl-3.3.0/func_adl/ast/syntatic_sugar.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/event_dataset.py` & `func_adl-3.3.0/func_adl/event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/functions.py` & `func_adl-3.3.0/func_adl/functions.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/func_adl/object_stream.py` & `func_adl-3.3.0/func_adl/object_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import ast
+import copy
 import logging
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generic,
@@ -17,15 +18,15 @@
     cast,
 )
 
 from make_it_sync import make_sync
 
 from func_adl.util_types import unwrap_iterable
 
-from .util_ast import as_ast, function_call, parse_as_ast
+from .util_ast import as_ast, check_ast, function_call, parse_as_ast
 
 # Attribute that will be used to store the executor reference
 executor_attr_name = "_func_adl_executor"
 
 T = TypeVar("T")
 S = TypeVar("S")
 
@@ -61,15 +62,15 @@
     stream of `Jets` using the `SelectMany` method below. In that case, you'll no longer be able
     to tell the boundary between events.
 
     `TypeVar` T is the item type (so this represents, if one were to think of this as loop-a-ble,
     `Iterable[T]`).
     """
 
-    def __init__(self, the_ast: ast.AST, item_type: Type = Any):
+    def __init__(self, the_ast: ast.AST, item_type: Type = Any):  # type: ignore
         r"""
         Initialize the stream with the ast that will produce this stream of objects.
         The user will almost never use this initializer.
         """
         self._q_ast = the_ast
         self._item_type = item_type
 
@@ -83,14 +84,20 @@
         """Return the query `ast` that this `ObjectStream` represents
 
         Returns:
             ast.AST: The python `ast` that is represented by this query
         """
         return self._q_ast
 
+    def clone_with_new_ast(self, new_ast: ast.AST, new_type: type[S]) -> ObjectStream[S]:
+        clone = copy.deepcopy(self)
+        clone._q_ast = new_ast
+        clone._item_type = new_type
+        return clone  # type: ignore
+
     def SelectMany(
         self, func: Union[str, ast.Lambda, Callable[[T], Iterable[S]]]
     ) -> ObjectStream[S]:
         r"""
         Given the current stream's object type is an array or other iterable, return
         the items in this objects type, one-by-one. This has the effect of flattening a
         nested array.
@@ -106,17 +113,19 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
         n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(func))
+            self, _local_simplification(parse_as_ast(func, "SelectMany"))
         )
-        return ObjectStream[S](
+        check_ast(n_ast)
+
+        return self.clone_with_new_ast(
             function_call("SelectMany", [n_stream.query_ast, cast(ast.AST, n_ast)]),
             unwrap_iterable(rtn_type),
         )
 
     def Select(self, f: Union[str, ast.Lambda, Callable[[T], S]]) -> ObjectStream[S]:
         r"""
         Apply a transformation function to each object in the stream, yielding a new type of
@@ -132,17 +141,21 @@
 
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
-        n_stream, n_ast, rtn_type = remap_from_lambda(self, _local_simplification(parse_as_ast(f)))
-        return ObjectStream[S](
-            function_call("Select", [n_stream.query_ast, cast(ast.AST, n_ast)]), rtn_type
+        n_stream, n_ast, rtn_type = remap_from_lambda(
+            self, _local_simplification(parse_as_ast(f, "Select"))
+        )
+        check_ast(n_ast)
+        return self.clone_with_new_ast(
+            function_call("Select", [n_stream.query_ast, cast(ast.AST, n_ast)]),
+            rtn_type,
         )
 
     def Where(self, filter: Union[str, ast.Lambda, Callable[[T], bool]]) -> ObjectStream[T]:
         r"""
         Filter the object stream, allowing only items for which `filter` evaluates as true through.
 
         Arguments:
@@ -156,30 +169,32 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
         n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(filter))
+            self, _local_simplification(parse_as_ast(filter, "Where"))
         )
+        check_ast(n_ast)
         if rtn_type != bool:
             raise ValueError(f"The Where filter must return a boolean (not {rtn_type})")
-        return ObjectStream[T](
-            function_call("Where", [n_stream.query_ast, cast(ast.AST, n_ast)]), self.item_type
+        return self.clone_with_new_ast(
+            function_call("Where", [n_stream.query_ast, cast(ast.AST, n_ast)]),
+            self.item_type,
         )
 
     def MetaData(self, metadata: Dict[str, Any]) -> ObjectStream[T]:
         """Add metadata to the current object stream. The metadata is an arbitrary set of string
         key-value pairs. The backend must be able to properly interpret the metadata.
 
         Returns:
             ObjectStream: A new stream, of the same type and contents, but with metadata added.
         """
-        return ObjectStream[T](
+        return self.clone_with_new_ast(
             function_call("MetaData", [self._q_ast, as_ast(metadata)]), self.item_type
         )
 
     def QMetaData(self, metadata: Dict[str, Any]) -> ObjectStream[T]:
         """Add query metadata to the current object stream.
 
         - Metadata is never transmitted to any back end
@@ -191,34 +206,35 @@
             metadata (Dict[str, Any]): Metadata to be used later
 
         Returns:
             ObjectStream[T]: The object stream, with metadata attached
         """
         from .ast.meta_data import lookup_query_metadata
 
-        first = True
-        base_ast = self.query_ast
+        q_metadata = {}
         for k, v in metadata.items():
             found_md = lookup_query_metadata(self, k)
             add_md = False
             if found_md is None:
                 add_md = True
             elif found_md != v:
                 logging.getLogger(__name__).info(
                     f'Overwriting metadata "{k}" from its old value of "{found_md}" to "{v}"'
                 )
                 add_md = True
             if add_md:
-                if first:
-                    first = False
-                    base_ast = self.MetaData({}).query_ast
-                    base_ast._q_metadata = {}  # type: ignore
-                base_ast._q_metadata[k] = v  # type: ignore
+                q_metadata[k] = v  # type: ignore
 
-        return ObjectStream[T](base_ast, self.item_type)
+        base_ast = self.query_ast
+        if len(q_metadata) > 0:
+            new_self = self.clone_with_new_ast(copy.copy(base_ast), self.item_type)
+            new_self.query_ast._q_metadata = q_metadata  # type: ignore
+            return new_self
+        else:
+            return self.clone_with_new_ast(base_ast, self.item_type)
 
     def AsPandasDF(
         self, columns: Union[str, List[str]] = []
     ) -> ObjectStream[ReturnedDataPlaceHolder]:
         r"""
         Return a pandas stream that contains one item, an pandas `DataFrame`.
         This `DataFrame` will contain all the data fed to it. Only non-array datatypes are
@@ -268,15 +284,16 @@
             dataset.
         """
         if isinstance(columns, str):
             columns = [columns]
 
         return ObjectStream[ReturnedDataPlaceHolder](
             function_call(
-                "ResultTTree", [self._q_ast, as_ast(columns), as_ast(treename), as_ast(filename)]
+                "ResultTTree",
+                [self._q_ast, as_ast(columns), as_ast(treename), as_ast(filename)],
             )
         )
 
     as_ROOT_tree = AsROOTTTree
 
     def AsParquetFiles(
         self, filename: str, columns: Union[str, List[str]] = []
@@ -299,15 +316,15 @@
                                 suggestion.
             columns             If the data does not arrive by dictionary, then these are the
                                 column names.
 
         Returns:
 
             A new `ObjectStream` with type `[filename]`. This is because multiple files may be
-            written by the backend - the data should be concatinated together to get a final
+            written by the backend - the data should be concatenated together to get a final
             result. The order of the files back is consistent for different queries on the same
             dataset.
         """
         if isinstance(columns, str):
             columns = [columns]
 
         return ObjectStream[ReturnedDataPlaceHolder](
@@ -338,19 +355,20 @@
         return ObjectStream[ReturnedDataPlaceHolder](
             function_call("ResultAwkwardArray", [self._q_ast, as_ast(columns)])
         )
 
     as_awkward = AsAwkwardArray
 
     def _get_executor(
-        self, executor: Optional[Callable[[ast.AST, Optional[str]], Awaitable[Any]]] = None
+        self,
+        executor: Optional[Callable[[ast.AST, Optional[str]], Awaitable[Any]]] = None,
     ) -> Callable[[ast.AST, Optional[str]], Awaitable[Any]]:
         r"""
         Returns an executor that can be used to run this.
-        Logic seperated out as it is used from several different places.
+        Logic separated out as it is used from several different places.
 
         Arguments:
             executor            Callback to run the AST. Can be synchronous or coroutine.
 
         Returns:
             An executor that is either synchronous or a coroutine.
         """
```

### Comparing `func_adl-3.2b1/func_adl/type_based_replacement.py` & `func_adl-3.3.0/func_adl/type_based_replacement.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,27 +41,30 @@
 _FuncAdlFunction = NamedTuple(
     "_FuncAdlFunction",
     [
         ("name", str),
         ("function", Callable),
         (
             "processor_function",
-            Optional[Callable[[ObjectStream[U], ast.Call], Tuple[ObjectStream[U], ast.AST]]],
+            Optional[
+                Callable[
+                    [ObjectStream[U], ast.Call], Tuple[ObjectStream[U], ast.AST]  # type: ignore
+                ]
+            ],
         ),
     ],
 )
 _global_functions: Dict[str, _FuncAdlFunction] = {}
 
 
 def _load_default_global_functions():
     "Define the python standard functions that map straight through"
     # TODO: Add in other functions
 
-    def my_abs(x: float) -> float:
-        ...
+    def my_abs(x: float) -> float: ...  # noqa
 
     _global_functions["abs"] = _FuncAdlFunction("abs", my_abs, None)
 
 
 _load_default_global_functions()
 
 
@@ -83,15 +86,15 @@
 
     Args:
         function (Callable): The type definition for the function (type st)
         processor_function (Callable[[ObjectStream[T], ast.Call],
             Tuple[ObjectStream[T], ast.AST]]):
             The processor function that can modify the stream, etc.
     """
-    info = _FuncAdlFunction(function.__name__, function, processor_function)
+    info = _FuncAdlFunction(function.__name__, function, processor_function)  # type: ignore
     _global_functions[info.name] = info
 
 
 W = TypeVar("W")
 
 
 def func_adl_callable(
@@ -128,14 +131,15 @@
         ...
     ```
 
     Args:
         processor (Optional[Callable[[ObjectStream[W], ast.Call],
                   Tuple[ObjectStream[W], ast.AST]]], optional): [description]. Defaults to None.
     """
+
     # TODO: Do we really need to register this inside the decorator? Can we just register
     #       and return the function?
     def decorate(function: Callable):
         register_func_adl_function(function, processor)
         return function
 
     return decorate
@@ -154,15 +158,15 @@
             new_kw = list(keywords)
             new_kw.remove(kw)
             return kw.value, new_kw
     return None, keywords
 
 
 # Some functions to enable backwards compatibility.
-# Capability may be degraded in older versions - particularly 3.6.
+# Capability may be degraded in older versions.
 if sys.version_info >= (3, 8):  # pragma: no cover
 
     def get_type_args(tp):
         import typing
 
         return typing.get_args(tp)
 
@@ -214,15 +218,15 @@
 
     Args:
         c (type): Class to register
 
     Returns:
         [type]: [description]
     """
-    _g_collection_classes[c] = CollectionClassInfo(c)
+    _g_collection_classes[c] = CollectionClassInfo(c)  # type: ignore
     return c
 
 
 @register_func_adl_os_collection
 class ObjectStreamInternalMethods(ObjectStream[StreamItem]):
     """There are a number of methods and manipulations that are not
     available at the event level, but are at the collection level. For default
@@ -232,26 +236,25 @@
     in inherit from this and add your own custom methods on top of this.
 
     Note that these methods are *never* called. The key part of this is following
     the `item_type` through!! This is because this package does not yet know how
     to follow generics in python at runtime (think of this as poor man's type resolution).
     """
 
-    def __init__(self, a: ast.AST, item_type: Type):
-        super().__init__(a, item_type)
+    def __init__(self, a: ast.AST, item_type: Union[Type, object]):
+        super().__init__(a, item_type)  # type: ignore
 
     @property
     def item_type(self) -> Type:
         return self._item_type
 
     def First(self) -> StreamItem:
-        return self.item_type
+        return self.item_type  # type: ignore
 
-    def Count(self) -> int:
-        ...
+    def Count(self) -> int: ...  # noqa
 
     # TODO: Add all other items that belong here
 
 
 def _load_g_collection_classes():
     "Use for testing to reset a global collection"
     register_func_adl_os_collection(ObjectStreamInternalMethods)
@@ -444,15 +447,15 @@
 class _MethodTypeReturnInfo:
     """For a particular method call, the return info"""
 
     # Update version of the ast
     node: ast.Call
 
     # Return type
-    return_type: Type
+    return_type: Union[Type, object]
 
     # If full type resolution was done (e.g. lambda following), or
     # if there were no lambda arguments to follow.
     full_type_resolution: bool
 
     # The object we actually did the call against
     obj_info: Optional[_MethodObjectCandidate]
@@ -481,23 +484,23 @@
         Type: The return type of the expression given. `Any` means it couldn't
     """
     S = TypeVar("S")
 
     class type_transformer(ast.NodeTransformer, Generic[S]):
         def __init__(self, o_stream: ObjectStream[S]):
             self._stream = o_stream
-            self._found_types: Dict[Union[str, object], type] = {var_name: var_type}
+            self._found_types: Dict[Union[str, object], Union[type, object]] = {var_name: var_type}
 
         @property
         def stream(self) -> ObjectStream[S]:
             return self._stream  # type: ignore
 
         def lookup_type(self, name: Union[str, object]) -> Type:
             "Return the type for a node, Any if we do not know about it"
-            return self._found_types.get(name, Any)
+            return self._found_types.get(name, Any)  # type: ignore
 
         def process_method_call_on_stream_obj(
             self,
             obj_info: CollectionClassInfo,
             call_method_name: str,
             call_node: ast.Call,
             item_type: type,
```

### Comparing `func_adl-3.2b1/func_adl/util_ast.py` & `func_adl-3.3.0/func_adl/util_ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 from __future__ import annotations
 
 import ast
 import inspect
 import sys
 import tokenize
 from collections import defaultdict
+from types import ModuleType
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union, cast
 
-# Some functions to enable backwards compatibility.
-# Capability may be degraded in older versions - particularly 3.6.
-if sys.version_info >= (3, 8):  # pragma: no cover
 
-    def as_literal(p: Union[str, int, float, bool, None]) -> ast.Constant:
-        return ast.Constant(value=p, kind=None)
+def as_literal(p: Union[str, int, float, bool, None]) -> ast.Constant:
+    """Convert a python constant into an AST constant node.
 
-else:  # pragma: no cover
+    Args:
+        p (Union[str, int, float, bool, None]): what should be wrapped
 
-    def as_literal(p: Union[str, int, float, bool, None]):
-        if isinstance(p, str):
-            return ast.Str(p)
-        elif isinstance(p, (int, float)):
-            return ast.Num(p)
-        elif isinstance(p, bool):
-            return ast.NameConstant(p)
-        elif p is None:
-            return ast.NameConstant(None)
-        else:
-            raise ValueError(f"Unknown type {type(p)} - do not know how to make a literal!")
+    Returns:
+        ast.Constant: The ast constant node that represents the value.
+    """
+    return ast.Constant(value=p, kind=None)
 
 
 def as_ast(p_var: Any) -> ast.AST:
     """Convert any python constant into an ast
 
     Args:
         p_var   Some python variable that can be rendered with str(p_var)
@@ -328,16 +320,18 @@
 
     def visit_Name(self, node: ast.Name) -> Any:
         if self.is_arg(node.id):
             return node
 
         if node.id in self._lookup_dict:
             v = self._lookup_dict[node.id]
-            if not callable(v):
-                return as_literal(self._lookup_dict[node.id])
+            if not callable(v) and not isinstance(v, ModuleType):
+                # If it is something we know how to make into a literal, we just send it down
+                # like that.
+                return as_literal(v)
         return node
 
     def visit_Lambda(self, node: ast.Lambda) -> Any:
         self._ignore_stack.append([a.arg for a in node.args.args])
         v = super().generic_visit(node)
         self._ignore_stack.pop()
         return v
@@ -643,18 +637,22 @@
         if len(good_lambdas) == 0:
             raise ValueError(
                 f"Internal Error - Found no lambda in source with the arguments {caller_arg_list}"
             )
 
         if len(good_lambdas) > 1:
             raise ValueError(
-                "Found multiple calls to on same line"
+                "Found multiple calls on same line"
                 + ("" if caller_name is None else f" for {caller_name}")
                 + " - split the calls across "
-                "lines or change lambda argument names so they are different."
+                """lines or change lambda argument names so they are different. For example change:
+                    df.Select(lambda x: x + 1).Select(lambda x: x + 2)
+                    to:
+                    df.Select(lambda x: x + 1).Select(lambda y: y + 2)
+                """
             )
 
         lda = good_lambdas[0]
 
     return lda
 
 
@@ -708,7 +706,32 @@
         def visit_Call(self, node: ast.Call):
             self.generic_visit(node)
 
             if isinstance(node.func, ast.Name) and node.func.id == "MetaData":
                 callback(node.args[1])  # type: ignore
 
     metadata_finder().visit(a)
+
+
+g_legal_capture_types = (str, int, float, bool, complex, str, bytes, ModuleType)
+
+
+def check_ast(a: ast.AST):
+    """Check to make sure the ast does not have anything we can't send over the wire
+    in `qastle` or similar.
+
+    Args:
+        a (ast.AST): The AST to check
+
+    Raises:
+        ValueError: If something unsupported is found.
+    """
+
+    class ConstantTypeChecker(ast.NodeVisitor):
+        def visit_Constant(self, node: ast.Constant):
+            if not isinstance(node.value, g_legal_capture_types):
+                raise ValueError(f"Invalid constant type: {type(node.value)} for {ast.dump(node)}")
+            self.generic_visit(node)
+
+    # Usage example:
+    checker = ConstantTypeChecker()
+    checker.visit(a)
```

### Comparing `func_adl-3.2b1/func_adl/util_types.py` & `func_adl-3.3.0/func_adl/util_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import sys
+import typing
 from typing import Any, Dict, Optional, Tuple, Type, TypeVar
 
 if sys.version_info >= (3, 8):
     from typing import get_args, get_origin
 else:  # pragma: no cover
     # TODO: Remove this when we drop support for 3.7
     def get_args(tp):
@@ -21,17 +22,15 @@
         t = get_inherited(t)
 
     return t is not Any
 
 
 def _is_iterable_direct(t: Type) -> bool:
     "Is this type iterable?"
-    if getattr(t, "_name", None) == "Iterable":
-        return True
-    return False
+    return getattr(t, "_name", None) == "Iterable" or getattr(t, "__name__", None) == "Iterable"
 
 
 def get_inherited(t: Type) -> Type:
     """Returns the inherited type of `t`
 
     Notes:
     * This works for 3.7 forward (but not back!)
@@ -50,15 +49,26 @@
         return Any
 
     r = base_classes[0]  # type: ignore
 
     g_args = get_args(t)
     if len(g_args) > 0:
         mapping = {a.__name__: v for a, v in zip(r.__parameters__, g_args)}
-        r.__args__ = tuple(_resolve_type(t_arg, mapping) for t_arg in get_args(r))
+
+        r_base = get_origin(r)
+        assert r_base is not None, "Internal error"
+
+        # Get us back to typing if this is a common interface.
+        # This is not needed in python 3.11 and forward, where
+        # collections.abc.X can are all be parameterized.
+        if r_base.__name__ in typing.__dict__:
+            r_base = typing.__dict__[r_base.__name__]
+
+        # Re-parameterize the type with the information e have from this parameterization.
+        r = r_base[tuple(_resolve_type(t_arg, mapping) for t_arg in get_args(r))]
 
     return r
 
 
 def unwrap_iterable(t: Type) -> Type:
     "Unwrap an iterable type"
     # Try to find an iterable in the history somehow
@@ -113,15 +123,15 @@
     Args:
         t (Type): The type to resolve
         parameters (Dict[str, Type]): The dict of types to resolve
 
     Returns:
         None if `t` is parameterized by unknown type var's
         The resolved type (a copy leaving `t` untouched) if TypeVar's are filled in
-        The type if no substition is required.
+        The type if no substitution is required.
     """
     if isinstance(t, TypeVar):
         if t.__name__ in parameters:
             return parameters[t.__name__]
         return None
 
     template_params = getattr(t, "__parameters__", None)
```

### Comparing `func_adl-3.2b1/func_adl.egg-info/PKG-INFO` & `func_adl-3.3.0/func_adl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: func-adl
-Version: 3.2b1
+Version: 3.3.0
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
-License: TBD
+License: MIT
 Platform: Any
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
 
 # func_adl
 
  Construct hierarchical data queries using SQL-like concepts in python.
```

### Comparing `func_adl-3.2b1/func_adl.egg-info/SOURCES.txt` & `func_adl-3.3.0/func_adl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/setup.py` & `func_adl-3.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,37 @@
-# Need setuptools even though it isn't used - loads some plugins.
 import os
-from distutils.core import setup
+import sys
 
-from setuptools import find_packages  # noqa: F401
+from setuptools import find_packages, setup  # noqa: F401
+
+
+# Taken from Numba
+def _guard_python_version(max_python):
+    version_module = None
+    try:
+        from packaging import version as version_module
+    except ImportError:
+        try:
+            from setuptools._vendor.packaging import version as version_module
+        except ImportError:
+            pass
+
+    if version_module is None:
+        return
+
+    current_python = version_module.parse(".".join(map(str, sys.version_info[:3])))
+    max_python = version_module.parse(max_python)
+
+    if not current_python < max_python:
+        raise RuntimeError(
+            f"Cannot install on Python version {current_python} as Python {max_python}+ is not yet supported."
+        )
+
+
+_guard_python_version(max_python="3.13")
 
 # Use the readme as the long description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 extras_require = {
@@ -17,14 +42,15 @@
         "flake8",
         "coverage",
         "twine",
         "wheel",
         "astunparse",
         "black",
         "isort",
+        "numpy",
     ]
 }
 extras_require["complete"] = sorted(set(sum(extras_require.values(), [])))
 extras_require["complete"] = sorted(set(sum(extras_require.values(), [])))
 
 version = os.getenv("func_adl_version")
 if version is None:
@@ -43,35 +69,34 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="G. Watts (IRIS-HEP/UW Seattle)",
     author_email="gwatts@uw.edu",
     maintainer="Gordon Watts (IRIS-HEP/UW Seattle)",
     maintainer_email="gwatts@uw.edu",
     url="https://github.com/iris-hep/func_adl",
-    license="TBD",
+    license="MIT",
     test_suite="tests",
     install_requires=["make-it-sync"],
     setup_requires=["pytest-runner"],
     tests_require=["pytest>=3.9"],
     extras_require=extras_require,
     classifiers=[
         # "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
-        # "Development Status :: 5 - Production/Stable",
+        "Development Status :: 5 - Production/Stable",
         # "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.6",
         "Topic :: Software Development",
         "Topic :: Utilities",
     ],
     data_files=[],
-    python_requires=">=3.6, <3.12",
+    python_requires=">=3.7",
     platforms="Any",
 )
```

### Comparing `func_adl-3.2b1/tests/test_event_dataset.py` & `func_adl-3.3.0/tests/test_event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/tests/test_object_stream.py` & `func_adl-3.3.0/tests/test_object_stream.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Test the object stream
 import ast
 import asyncio
 import logging
+from _ast import Call
+from enum import Enum
 from typing import Any, Iterable, Optional, Tuple, TypeVar
 
 import pytest
 
 from func_adl import EventDataset
 from func_adl.object_stream import ObjectStream
 from func_adl.type_based_replacement import func_adl_callback
@@ -20,32 +22,29 @@
 class my_event_with_title(EventDataset):
     async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
         await asyncio.sleep(0.01)
         return a, title
 
 
 class dd_jet:
-    def pt(self) -> float:
-        ...
+    def pt(self) -> float: ...  # noqa
 
-    def eta(self) -> float:
-        ...
+    def eta(self) -> float: ...  # noqa
 
 
 T = TypeVar("T")
 
 
 def add_md_for_type(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     return s.MetaData({"hi": "there"}), a
 
 
 @func_adl_callback(add_md_for_type)
 class dd_event:
-    def Jets(self, bank: str) -> Iterable[dd_jet]:
-        ...
+    def Jets(self, bank: str) -> Iterable[dd_jet]: ...  # noqa
 
 
 class my_event_with_type(EventDataset[dd_event]):
     def __init__(self):
         super().__init__(dd_event)
 
     async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
@@ -71,14 +70,20 @@
         .Select("lambda j: j.pT()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
     )
     assert isinstance(r, ast.AST)
 
 
+def test_simple_query_one_line():
+    """Make sure we parse 2 functions on one line correctly"""
+    r = my_event().Select(lambda e: e.met).Where(lambda e: e > 10).value()
+    assert isinstance(r, ast.AST)
+
+
 def test_two_simple_query():
     r1 = (
         my_event()
         .SelectMany("lambda e: e.jets()")
         .Select("lambda j: j.pT()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
@@ -90,14 +95,33 @@
         .AsROOTTTree("junk.root", "analysis", ["jetPT"])
         .value()
     )
 
     assert ast.dump(r1) == ast.dump(r2)
 
 
+def test_query_bad_variable():
+    class my_type:
+        def __init__(self, n):
+            self._n = 10
+
+    my_10 = my_type(10)
+
+    with pytest.raises(ValueError) as e:
+        (
+            my_event()
+            .SelectMany(lambda e: e.jets())
+            .Select(lambda j: j.pT() > my_10)
+            .AsROOTTTree("junk.root", "analysis", "jetPT")
+            .value()
+        )
+
+    assert "my_type" in str(e)
+
+
 def test_with_types():
     r1 = my_event_with_type().SelectMany(lambda e: e.Jets("jets"))
     r = r1.Select(lambda j: j.eta()).value()
     assert isinstance(r, ast.AST)
     assert "there" in ast.dump(r)
 
 
@@ -288,14 +312,33 @@
 
     assert lookup_query_metadata(r1, "two") == "2"
     assert lookup_query_metadata(r2, "two") == "2+"
 
     assert len(caplog.text) == 0
 
 
+def test_query_metadata_not_empty():
+    r_base = my_event().QMetaData({"one": "1"})
+    q_ast = r_base.query_ast
+
+    class MDScanner(ast.NodeVisitor):
+        def visit_Call(self, node: Call) -> Any:
+            if not isinstance(node.func, ast.Name):
+                return self.generic_visit(node)
+            if node.func.id != "MetaData":
+                return self.generic_visit(node)
+            assert len(node.args) == 2
+            md_dict = node.args[1]
+            assert isinstance(md_dict, ast.Dict)
+            assert len(md_dict.keys) > 0
+            return self.generic_visit(node)
+
+    MDScanner().visit(q_ast)
+
+
 def test_nested_query_rendered_correctly():
     r = (
         my_event()
         .Where("lambda e: e.jets.Select(lambda j: j.pT()).Where(lambda j: j > 10).Count() > 0")
         .SelectMany("lambda e: e.jets()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
@@ -312,14 +355,33 @@
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
     )
     assert isinstance(r, ast.AST)
     assert "ListComp" not in ast.dump(r)
 
 
+def test_non_imported_function_call():
+    r = (
+        my_event()
+        .Select(lambda event: np.cos(event.MET_phi))  # type: ignore # noqa
+        .Where(lambda p: p > 0.0)
+        .value()
+    )  # NOQA
+    assert isinstance(r, ast.AST)
+    assert "Attribute(value=Name(id='np', ctx=Load()), attr='cos', ctx=Load())" in ast.dump(r)
+
+
+def test_imported_function_call():
+    import numpy as np
+
+    r = my_event().Select(lambda event: np.cos(event.MET_phi)).Where(lambda p: p > 0.0).value()
+    assert isinstance(r, ast.AST)
+    assert "Attribute(value=Name(id='np', ctx=Load()), attr='cos', ctx=Load())" in ast.dump(r)
+
+
 def test_bad_where():
     with pytest.raises(ValueError):
         my_event().Where("lambda e: 10").SelectMany("lambda e: e.jets()").AsROOTTTree(
             "junk.root", "analysis", "jetPT"
         ).value()
 
 
@@ -405,60 +467,54 @@
 def test_untyped():
     r = my_event()
     assert r.item_type == Any
 
 
 def test_typed():
     class Jet:
-        def pt(self) -> float:
-            ...
+        def pt(self) -> float: ...  # noqa
 
     class Evt:
-        def Jets(self) -> Iterable[Jet]:
-            ...
+        def Jets(self) -> Iterable[Jet]: ...  # noqa
 
     class evt_typed(EventDataset[Evt]):
         def __init__(self):
             super().__init__(Evt)
 
         async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
             await asyncio.sleep(0.01)
             return a
 
     r = evt_typed()
     assert r.item_type is Evt
 
 
 def test_typed_with_select():
-    class Jet:
-        ...
+    class Jet: ...  # noqa
 
     class Evt:
-        def Jets(self) -> Iterable[Jet]:
-            ...
+        def Jets(self) -> Iterable[Jet]: ...  # noqa
 
     class evt_typed(EventDataset[Evt]):
         def __init__(self):
             super().__init__(Evt)
 
         async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
             await asyncio.sleep(0.01)
             return a
 
     r = evt_typed().Select(lambda e: e.Jets())
     assert r.item_type is Iterable[Jet]
 
 
 def test_typed_with_selectmany():
-    class Jet:
-        ...
+    class Jet: ...  # noqa
 
     class Evt:
-        def Jets(self) -> Iterable[Jet]:
-            ...
+        def Jets(self) -> Iterable[Jet]: ...  # noqa
 
     class evt_typed(EventDataset[Evt]):
         def __init__(self):
             super().__init__(Evt)
 
         async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
             await asyncio.sleep(0.01)
@@ -466,61 +522,77 @@
 
     r = evt_typed().SelectMany(lambda e: e.Jets())
     assert r.item_type is Jet
 
 
 def test_typed_with_select_and_selectmany():
     class Jet:
-        def pt(self) -> float:
-            ...
+        def pt(self) -> float: ...  # noqa
 
     class Evt:
-        def Jets(self) -> Iterable[Jet]:
-            ...
+        def Jets(self) -> Iterable[Jet]: ...  # noqa
 
     class evt_typed(EventDataset[Evt]):
         def __init__(self):
             super().__init__(Evt)
 
         async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
             await asyncio.sleep(0.01)
             return a
 
-        def Jets(self) -> Iterable[Jet]:
-            ...
+        def Jets(self) -> Iterable[Jet]: ...  # noqa
 
     r1 = evt_typed().SelectMany(lambda e: e.Jets())
     r = r1.Select(lambda j: j.pt())
     assert r.item_type is float
 
 
 def test_typed_with_where():
     class Evt:
-        def MET(self) -> float:
-            ...
+        def MET(self) -> float: ...  # noqa
 
     class evt_typed(EventDataset[Evt]):
         def __init__(self):
             super().__init__(Evt)
 
         async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
             await asyncio.sleep(0.01)
             return a
 
     r = evt_typed().Where(lambda e: e.MET() > 100)
     assert r.item_type is Evt
 
 
 def test_typed_with_metadata():
-    class Evt:
-        ...
+    class Evt: ...  # noqa
 
     class evt_typed(EventDataset[Evt]):
         def __init__(self):
             super().__init__(Evt)
 
         async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
             await asyncio.sleep(0.01)
             return a
 
     r = evt_typed().MetaData({})
     assert r.item_type is Evt
+
+
+def test_typed_with_enum():
+    class Evt:
+        class Color(Enum):
+            red = 1
+            green = 2
+            blue = 3
+
+        def color(self) -> Color: ...  # noqa
+
+    class evt_typed(EventDataset[Evt]):
+        def __init__(self):
+            super().__init__(Evt)
+
+        async def execute_result_async(self, a: ast.AST, title: Optional[str] = None):
+            await asyncio.sleep(0.01)
+            return a
+
+    r = evt_typed().Select(lambda e: e.color())
+    assert r.item_type is Evt.Color
```

### Comparing `func_adl-3.2b1/tests/test_type_based_replacement.py` & `func_adl-3.3.0/tests/test_type_based_replacement.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,89 +13,77 @@
     register_func_adl_os_collection,
     remap_by_types,
     remap_from_lambda,
 )
 
 
 class Track:
-    def pt(self) -> float:
-        ...
+    def pt(self) -> float: ...  # noqa
 
-    def eta(self) -> float:
-        ...
+    def eta(self) -> float: ...  # noqa
 
 
 T = TypeVar("T")
 
 
 def add_track_extra_info(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     s_update = s.MetaData({"t": "track stuff"})
     return s_update, a
 
 
 @func_adl_callback(add_track_extra_info)
 class TrackStuff:
-    def pt(self) -> float:
-        ...
+    def pt(self) -> float: ...  # noqa
 
-    def eta(self) -> float:
-        ...
+    def eta(self) -> float: ...  # noqa
 
 
 class Jet:
-    def pt(self) -> float:
-        ...
+    def pt(self) -> float: ...  # noqa
 
-    def eta(self) -> float:
-        ...
+    def eta(self) -> float: ...  # noqa
 
-    def tracks(self) -> Iterable[Track]:
-        ...
+    def tracks(self) -> Iterable[Track]: ...  # noqa
 
 
 def ast_lambda(lambda_func: str) -> ast.Lambda:
     "Return the ast starting from the Lambda node"
     return ast.parse(lambda_func).body[0].value  # type: ignore
 
 
 def add_met_extra_info(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     s_update = s.MetaData({"j": "pxyz stuff"})
     return s_update, a
 
 
 @func_adl_callback(add_met_extra_info)
 class met_extra:
-    def pxy(self) -> float:
-        ...
+    def pxy(self) -> float: ...  # noqa
 
 
 def add_met_info(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     s_update = s.MetaData({"j": "pxy stuff"})
     return s_update, a
 
 
 def add_met_method_info(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     s_update = s.MetaData({"j": "custom stuff"})
     return s_update, a
 
 
 @func_adl_callback(add_met_info)
 class met:
-    def pxy(self) -> float:
-        ...
+    def pxy(self) -> float: ...  # noqa
 
-    def isGood(self) -> bool:
-        ...
+    def isGood(self) -> bool: ...  # noqa
 
-    def metobj(self) -> met_extra:
-        ...
+    def metobj(self) -> met_extra: ...  # noqa
 
     @func_adl_callback(add_met_method_info)
-    def custom(self) -> float:
-        ...
+    def custom(self) -> float: ...  # noqa
 
 
 def add_collection(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     """Add a collection to the object stream"""
     assert isinstance(a.func, ast.Attribute)
     if a.func.attr == "Jets":
         s_update = s.MetaData({"j": "stuff"})
@@ -109,46 +97,36 @@
 
 
 class MyIterable(Iterable[T]):
     def Last(self) -> T:
         "Return the last element in the sequence"
         ...
 
-    def Where(self, test: Callable[[T], bool]) -> Iterable[T]:
-        ...
+    def Where(self, test: Callable[[T], bool]) -> Iterable[T]: ...  # noqa
 
 
 @func_adl_callback(add_collection)
 class Event:
-    def Jets(self, bank: str = "default") -> Iterable[Jet]:
-        ...
+    def Jets(self, bank: str = "default") -> Iterable[Jet]: ...  # noqa
 
-    def JetsIterSub(self, bank: str = "default") -> MyIterable[Jet]:
-        ...
+    def JetsIterSub(self, bank: str = "default") -> MyIterable[Jet]: ...  # noqa
 
-    def Jets_req(self, bank_required: str) -> Iterable[Jet]:
-        ...
+    def Jets_req(self, bank_required: str) -> Iterable[Jet]: ...  # noqa
 
-    def MET(self) -> met:
-        ...
+    def MET(self) -> met: ...  # noqa
 
-    def MET_noreturntype(self):
-        ...
+    def MET_noreturntype(self): ...  # noqa
 
-    def Tracks(self) -> Iterable[Track]:
-        ...
+    def Tracks(self) -> Iterable[Track]: ...  # noqa
 
-    def TrackStuffs(self) -> Iterable[TrackStuff]:
-        ...
+    def TrackStuffs(self) -> Iterable[TrackStuff]: ...  # noqa
 
-    def EventNumber(self) -> int:
-        ...
+    def EventNumber(self) -> int: ...  # noqa
 
-    def MyLambdaCallback(self, cb: Callable) -> int:
-        ...
+    def MyLambdaCallback(self, cb: Callable) -> int: ...  # noqa
 
 
 def return_type_test(expr: str, arg_type: type, expected_type: type):
     s = ast_lambda(expr)
     objs = ObjectStream(ast.Name(id="e", ctx=ast.Load()), arg_type)
 
     _, _, expr_type = remap_by_types(objs, "e", arg_type, s)
@@ -172,15 +150,15 @@
 
 
 def test_float():
     return_type_test("1.5", int, float)
 
 
 def test_any():
-    return_type_test("e", Any, Any)
+    return_type_test("e", Any, Any)  # type: ignore
 
 
 def test_neg_float():
     return_type_test("-1.5", int, float)
 
 
 def test_add_int():
@@ -263,15 +241,15 @@
 
 
 def test_subscript():
     return_type_test("e[0]", Iterable[int], int)
 
 
 def test_subscript_any():
-    return_type_test("e[0]", Any, Any)
+    return_type_test("e[0]", Any, Any)  # type: ignore
 
 
 def test_collection():
     "A simple collection"
     s = ast_lambda("e.Jets('default')")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
@@ -365,18 +343,17 @@
     caplog.set_level(logging.WARNING)
 
     M = TypeVar("M")
 
     @register_func_adl_os_collection
     class CustomCollection(ObjectStream[M]):
         def __init__(self, a: ast.AST, item_type: Optional[Type] = None):
-            super().__init__(a, item_type)
+            super().__init__(a, item_type)  # type: ignore
 
-        def MyFirst(self) -> int:
-            ...
+        def MyFirst(self) -> int: ...  # noqa
 
     s = ast_lambda("e.Jets().MyFirst()")
     objs = CustomCollection[Event](ast.Name(id="e", ctx=ast.Load()), Event)
 
     _, _, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert expr_type == int
@@ -389,18 +366,17 @@
     caplog.set_level(logging.WARNING)
 
     M = TypeVar("M")
 
     @register_func_adl_os_collection
     class CustomCollection(ObjectStream[M]):
         def __init__(self, a: ast.AST, item_type=Any):
-            super().__init__(a, item_type)
+            super().__init__(a, item_type)  # type: ignore
 
-        def MyFirst(self, arg1: int, arg2: int) -> int:
-            ...
+        def MyFirst(self, arg1: int, arg2: int) -> int: ...  # noqa
 
     s = ast_lambda("e.Jets().MyFirst(1,3)")
     objs = CustomCollection[Event](ast.Name(id="e", ctx=ast.Load()))
 
     _, _, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert expr_type == int
@@ -415,16 +391,15 @@
     M = TypeVar("M")
 
     @register_func_adl_os_collection
     class CustomCollection_default(ObjectStream[M]):
         def __init__(self, a: ast.AST, item_type):
             super().__init__(a, item_type)
 
-        def Take(self, n: int = 5) -> ObjectStream[M]:
-            ...
+        def Take(self, n: int = 5) -> ObjectStream[M]: ...  # noqa
 
     s = ast_lambda("e.Jets().Take()")
     objs = CustomCollection_default[Event](ast.Name(id="e", ctx=ast.Load()), Event)
 
     _, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert expr_type == ObjectStream[Jet]
@@ -439,16 +414,15 @@
 
     M = TypeVar("M")
 
     class CustomCollection_Jet(ObjectStream[M]):
         def __init__(self, a: ast.AST, item_type):
             super().__init__(a, item_type)
 
-        def MyFirst(self) -> M:
-            ...
+        def MyFirst(self) -> M: ...  # noqa
 
     register_func_adl_os_collection(CustomCollection_Jet)
 
     s = ast_lambda("e.Jets().MyFirst()")
     objs = CustomCollection_Jet[Event](ast.Name(id="e", ctx=ast.Load()), Event)
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
@@ -689,16 +663,15 @@
     "Define a function we can use"
 
     def MySqrtProcessor(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
         new_s = s.MetaData({"j": "func_stuff"})
         return new_s, a
 
     @func_adl_callable(MySqrtProcessor)
-    def MySqrt(x: float) -> float:
-        ...
+    def MySqrt(x: float) -> float: ...  # noqa
 
     s = ast_lambda("MySqrt(2)")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()), item_type=Event)
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("MySqrt(2)"))
@@ -707,16 +680,15 @@
     assert expr_type == float
 
 
 def test_function_with_simple():
     "Define a function we can use"
 
     @func_adl_callable()
-    def MySqrt(x: float) -> float:
-        ...
+    def MySqrt(x: float) -> float: ...  # noqa
 
     s = ast_lambda("MySqrt(2)")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("MySqrt(2)"))
@@ -724,32 +696,30 @@
     assert expr_type == float
 
 
 def test_function_with_missing_arg():
     "Define a function we can use"
 
     @func_adl_callable()
-    def MySqrt(my_x: float) -> float:
-        ...
+    def MySqrt(my_x: float) -> float: ...  # noqa
 
     s = ast_lambda("MySqrt()")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     with pytest.raises(ValueError) as e:
         remap_by_types(objs, "e", Event, s)
 
     assert "my_x" in str(e)
 
 
 def test_function_with_default():
     "Define a function we can use"
 
     @func_adl_callable()
-    def MySqrt(x: float = 20) -> float:
-        ...
+    def MySqrt(x: float = 20) -> float: ...  # noqa
 
     s = ast_lambda("MySqrt()")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("MySqrt(20)"))
@@ -757,16 +727,15 @@
     assert expr_type == float
 
 
 def test_function_with_default_inside():
     "A function with a default arg that is inside a select"
 
     @func_adl_callable()
-    def MySqrt(x: float = 20) -> float:
-        ...
+    def MySqrt(x: float = 20) -> float: ...  # noqa
 
     s = ast_lambda("e.Jets().Select(lambda j: MySqrt())")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert ast.dump(new_s) == ast.dump(
@@ -776,16 +745,15 @@
     assert expr_type == Iterable[float]
 
 
 def test_function_with_keyword():
     "Define a function we can use"
 
     @func_adl_callable()
-    def MySqrt(x: float = 20) -> float:
-        ...
+    def MySqrt(x: float = 20) -> float: ...  # noqa
 
     s = ast_lambda("MySqrt(x=15)")
     objs = ObjectStream[Event](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", Event, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("MySqrt(15)"))
@@ -834,28 +802,73 @@
         nonlocal param_1_capture
         param_1_capture = param_1
         return (s.MetaData({"k": "stuff"}), a, float)
 
     class TEvent:
         @func_adl_parameterized_call(my_callback)
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     s = ast_lambda("e.info['fork'](55)")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
 
     new_objs, new_s, expr_type = remap_by_types(objs, "e", TEvent, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("e.info(55)"))
     assert ast.dump(new_objs.query_ast) == ast.dump(ast_lambda("MetaData(e, {'k': 'stuff'})"))
     assert expr_type == float
     assert param_1_capture == "fork"
 
 
+class NameToConstantTransformer(ast.NodeTransformer):
+    def __init__(self, target_id, replacement_value):
+        self.target_id = target_id
+        self.replacement_value = replacement_value
+
+    def visit_Name(self, node):
+        if node.id == self.target_id:
+            return ast.Constant(value=self.replacement_value)
+        return node
+
+
+def replace_name_with_constant(tree, target_id, replacement_value):
+    transformer = NameToConstantTransformer(target_id, replacement_value)
+    return transformer.visit(tree)
+
+
+def test_index_callback_1arg_type():
+    "Indexed callback - make sure arg is passed correctly when there is a type"
+
+    param_1_capture = None
+
+    def my_callback(
+        s: ObjectStream[T], a: ast.Call, param_1: str
+    ) -> Tuple[ObjectStream[T], ast.Call, Type]:
+        nonlocal param_1_capture
+        param_1_capture = param_1
+        return (s.MetaData({"k": "stuff"}), a, float)
+
+    class TEvent:
+        @func_adl_parameterized_call(my_callback)
+        @property
+        def info(self): ...  # noqa
+
+    s = ast_lambda("e.info[int](55)")
+    s = replace_name_with_constant(s, "int", int)
+
+    objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
+
+    new_objs, new_s, expr_type = remap_by_types(objs, "e", TEvent, s)
+
+    assert ast.dump(new_s) == ast.dump(ast_lambda("e.info(55)"))
+    assert ast.dump(new_objs.query_ast) == ast.dump(ast_lambda("MetaData(e, {'k': 'stuff'})"))
+    assert expr_type == float
+    assert param_1_capture == int
+
+
 def test_index_callback_2arg():
     "Indexed callback - make sure 2 args are passed correctly"
 
     param_1_capture = None
 
     def my_callback(
         s: ObjectStream[T], a: ast.Call, param_1: str
@@ -863,16 +876,15 @@
         nonlocal param_1_capture
         param_1_capture = param_1
         return (s.MetaData({"k": "stuff"}), a, float)
 
     class TEvent:
         @func_adl_parameterized_call(my_callback)
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     s = ast_lambda("e.info['fork', 22](55)")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
 
     remap_by_types(objs, "e", TEvent, s)
 
     assert param_1_capture == ("fork", 22)
@@ -889,16 +901,15 @@
         new_a.func = ast.Attribute(value=a.func.value, attr="dude", ctx=a.func.ctx)
 
         return (s, new_a, float)
 
     class TEvent:
         @func_adl_parameterized_call(my_callback)
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     s = ast_lambda("e.info['fork'](55)")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
 
     _, new_s, _ = remap_by_types(objs, "e", TEvent, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("e.dude(55)"))
@@ -915,20 +926,18 @@
         new_a.func = ast.Attribute(value=a.func.value, attr="dude", ctx=a.func.ctx)
 
         return (s, new_a, float)
 
     class MyJet:
         @func_adl_parameterized_call(my_callback)
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     class TEvent:
-        def Jets(self) -> Iterable[MyJet]:
-            ...
+        def Jets(self) -> Iterable[MyJet]: ...  # noqa
 
     s = ast_lambda("e.Jets().Select(lambda j: j.info['fork'](55))")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
 
     _, new_s, _ = remap_by_types(objs, "e", TEvent, s)
 
     assert ast.dump(new_s) == ast.dump(ast_lambda("e.Jets().Select(lambda j: j.dude(55))"))
@@ -946,16 +955,15 @@
         ) -> Tuple[ObjectStream[T], ast.Call, Type]:
             nonlocal param_1_capture
             param_1_capture = param_1
             return (s.MetaData({"k": "stuff"}), a, float)
 
         class TEvent:
             @func_adl_parameterized_call(my_callback)
-            def info(self):
-                ...
+            def info(self): ...  # noqa
 
     assert "info" in str(e)
 
 
 def test_index_callback_bad_prop():
     "Indexed callback - make sure arg is passed correctly"
 
@@ -967,16 +975,15 @@
         nonlocal param_1_capture
         param_1_capture = param_1
         return (s.MetaData({"k": "stuff"}), a, float)
 
     class TEvent:
         @func_adl_parameterized_call(my_callback)
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     s = ast_lambda("e.infoo['fork'](55)")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
     with pytest.raises(AttributeError) as e:
         remap_by_types(objs, "e", TEvent, s)
 
     assert "infoo" in str(e)
@@ -984,16 +991,15 @@
 
 
 def test_index_callback_prop_not_dec():
     "Indexed callback - make sure arg is passed correctly"
 
     class TEvent:
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     s = ast_lambda("e.info['fork'](55)")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
     with pytest.raises(ValueError) as e:
         remap_by_types(objs, "e", TEvent, s)
 
     assert "info" in str(e)
@@ -1001,16 +1007,15 @@
 
 
 def test_index_callback_prop_index_bad():
     "Indexed callback - make sure arg is passed correctly"
 
     class TEvent:
         @property
-        def info(self):
-            ...
+        def info(self): ...  # noqa
 
     s = ast_lambda("e.info['fork':'dork'](55)")
     objs = ObjectStream[TEvent](ast.Name(id="e", ctx=ast.Load()))
     with pytest.raises(ValueError) as e:
         remap_by_types(objs, "e", TEvent, s)
 
     assert "info" in str(e)
```

### Comparing `func_adl-3.2b1/tests/test_type_based_replacement_py310.py` & `func_adl-3.3.0/tests/test_type_based_replacement_py310.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2b1/tests/test_util_ast.py` & `func_adl-3.3.0/tests/test_util_ast.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from typing import Callable, cast
 
 import pytest
 
 from func_adl.util_ast import (
     _realign_indent,
     as_ast,
+    check_ast,
     function_call,
     lambda_args,
     lambda_body_replace,
     lambda_build,
     lambda_call,
     lambda_is_identity,
     lambda_is_true,
     lambda_test,
     lambda_unwrap,
     parse_as_ast,
     rewrite_func_as_lambda,
     scan_for_metadata,
 )
+from tests.test_type_based_replacement import replace_name_with_constant
 
 
 # Ast parsing
 def test_as_ast_integer():
     if sys.version_info < (3, 8):
         assert "Num(n=1)" == ast.dump(as_ast(1))
     elif sys.version_info < (3, 9):
@@ -359,23 +361,21 @@
     f = parse_as_ast(lambda a: unknown(a))  # type: ignore # NOQA
     assert "Name(id='unknown'" in ast.dump(f)
 
 
 def test_known_local_function():
     "function that is declared locally"
 
-    def doit(x):
-        ...
+    def doit(x): ...
 
     f = parse_as_ast(lambda a: doit(a))  # type: ignore # NOQA
     assert "Name(id='doit'" in ast.dump(f)
 
 
-def global_doit_non_func(x):
-    ...
+def global_doit_non_func(x): ...
 
 
 def test_known_global_function():
     "function that is declared locally"
 
     f = parse_as_ast(lambda a: global_doit_non_func(a))  # type: ignore # NOQA
     assert "Name(id='global_doit_non_func'" in ast.dump(f)
@@ -496,16 +496,15 @@
                 return y
 
             seen_funcs.append(x)
             return make_it
 
     class yo_baby:
         @h.dec_func(lambda y: y + 2)
-        def doit(self, x: int):
-            ...
+        def doit(self, x: int): ...
 
     assert len(seen_funcs) == 1
     l1 = parse_as_ast(seen_funcs[0], "dec_func")
     assert isinstance(l1.body, ast.BinOp)
     assert isinstance(l1.body.op, ast.Add)
 
 
@@ -678,14 +677,46 @@
         .value()
     )
     # fmt: on
     assert jets_pflow is not None  # Just to keep flake8 happy without adding a noqa above.
     assert "uncalibrated_collection" in ast.dump(found[0])
 
 
+def test_parse_select_where():
+    "Common lambas with different parent functions on one line - found in wild"
+
+    found = []
+
+    class my_obj:
+        def Where(self, x: Callable):
+            found.append(parse_as_ast(x, "Where"))
+            return self
+
+        def Select(self, x: Callable):
+            found.append(parse_as_ast(x, "Select"))
+            return self
+
+        def AsAwkwardArray(self, stuff: str):
+            return self
+
+        def value(self):
+            return self
+
+    jets_pflow_name = "hi"
+    ds_dijet = my_obj()
+
+    # fmt: off
+    jets_pflow = (
+        ds_dijet.Select(lambda e: e.met).Where(lambda e: e > 100)
+    )
+    # fmt: on
+    assert jets_pflow is not None  # Just to keep flake8 happy without adding a noqa above.
+    assert "met" in ast.dump(found[0])
+
+
 def test_parse_multiline_lambda_ok_with_one_as_arg():
     "Make sure we can properly parse a multi-line lambda - but now with argument"
 
     found = []
 
     class my_obj:
         def do_it(self, x: Callable, counter: int):
@@ -778,14 +809,59 @@
     )
     # fmt: on
 
     assert len(found) == 1
     assert "AntiKt4EMTopoJets" in ast.dump(found[0])
 
 
+def test_parse_paramertized_function_simple():
+    a = parse_as_ast(lambda e: e.jetAttribute["hi"](10))
+    d_text = ast.dump(a)
+    assert "Constant(value=10" in d_text
+    assert "Constant(value='hi'" in d_text
+
+
+def test_parse_parameterized_function_type():
+    a = parse_as_ast(lambda e: e.jetAttribute[int](10))
+    d_text = ast.dump(a)
+    assert "Constant(value=10" in d_text
+
+    # Needs to be updated...
+    assert "Name(id='int'" in d_text
+
+
+def test_parse_parameterized_function_defined_type():
+    class my_type:
+        bogus: int = 10
+
+    a = parse_as_ast(lambda e: e.jetAttribute[my_type](10))
+    d_text = ast.dump(a)
+    assert "Constant(value=10" in d_text
+
+    # Needs to be updated...
+    assert "Name(id='my_type'" in d_text
+
+
+def test_parse_parameterized_function_instance():
+    class my_type:
+        def __init__(self, n):
+            self._n = n
+
+    my_10 = my_type(10)
+
+    a = parse_as_ast(lambda e: e.jetAttribute[my_10](10))
+    d_text = ast.dump(a)
+    assert "Constant(value=10" in d_text
+
+    # Needs to be updated...
+    assert (
+        "Constant(value=<tests.test_util_ast.test_parse_parameterized_function_instance" in d_text
+    )
+
+
 def test_parse_metadata_there():
     recoreded = None
 
     def callback(a: ast.arg):
         nonlocal recoreded
         recoreded = a
 
@@ -809,7 +885,25 @@
 
 def test_realign_indent_2lines():
     assert _realign_indent("    test()\n    dude()") == "test()\ndude()"
 
 
 def test_realign_indent_2lines_uneven():
     assert _realign_indent("    test()\n        dude()") == "test()\n    dude()"
+
+
+def test_check_ast_good():
+    check_ast(ast.parse("1 + 2 + 'abc'"))
+
+
+def test_check_ast_bad():
+    class my_type:
+        def __init__(self, n):
+            self._n = n
+
+    mt = my_type(10)
+    a = ast.parse("1 + 2 + abc")
+    a = replace_name_with_constant(a, "abc", mt)
+    with pytest.raises(ValueError) as e:
+        check_ast(a)
+
+    assert "my_type" in str(e)
```

### Comparing `func_adl-3.2b1/tests/test_util_types.py` & `func_adl-3.3.0/tests/test_util_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     T = TypeVar("T")
 
     class bogus(Iterable[T]):
         pass
 
     myc = bogus[int]
 
-    assert get_inherited(myc) == Iterable[int]
+    assert get_inherited(myc) == Iterable[int]  # type: ignore
 
 
 def test_get_inherited_two_levels():
     T = TypeVar("T")
     U = TypeVar("U")
 
     class bogus(Generic[T]):
@@ -102,14 +102,27 @@
     class bogus2(bogus[Iterable[U]]):
         pass
 
     myc = bogus2[int]
     assert get_inherited(myc) == bogus[Iterable[int]]
 
 
+def test_get_inherited_generic_twice():
+    T = TypeVar("T")
+
+    class bogus(Iterable[T]):
+        pass
+
+    myc = bogus[int]
+    assert get_inherited(myc) == Iterable[int]  # type: ignore
+
+    myd = bogus[float]
+    assert get_inherited(myd) == Iterable[float]  # type: ignore
+
+
 def test_build_type_int():
     assert build_type_dict_from_type(int) == {}
 
 
 def test_build_type_generic():
     T = TypeVar("T")
```


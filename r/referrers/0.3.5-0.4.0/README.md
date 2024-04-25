# Comparing `tmp/referrers-0.3.5.tar.gz` & `tmp/referrers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.3.5.tar", max compression
+gzip compressed data, was "referrers-0.4.0.tar", max compression
```

## Comparing `referrers-0.3.5.tar` & `referrers-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-19 22:42:51.326436 referrers-0.3.5/LICENSE
--rw-r--r--   0        0        0     8135 2024-04-19 22:42:51.326436 referrers-0.3.5/README.md
--rw-r--r--   0        0        0      372 2024-04-19 22:42:51.326436 referrers-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-19 22:42:51.326436 referrers-0.3.5/src/referrers/__init__.py
--rw-r--r--   0        0        0    37144 2024-04-19 22:42:51.330436 referrers-0.3.5/src/referrers/impl.py
--rw-r--r--   0        0        0     8668 1970-01-01 00:00:00.000000 referrers-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 15:50:01.890532 referrers-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8135 2024-04-25 15:50:01.890532 referrers-0.4.0/README.md
+-rw-r--r--   0        0        0      372 2024-04-25 15:50:01.890532 referrers-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-25 15:50:01.890532 referrers-0.4.0/src/referrers/__init__.py
+-rw-r--r--   0        0        0    38723 2024-04-25 15:50:01.894532 referrers-0.4.0/src/referrers/impl.py
+-rw-r--r--   0        0        0     8668 1970-01-01 00:00:00.000000 referrers-0.4.0/PKG-INFO
```

### Comparing `referrers-0.3.5/LICENSE` & `referrers-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.3.5/README.md` & `referrers-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `referrers-0.3.5/src/referrers/impl.py` & `referrers-0.4.0/src/referrers/impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import gc
 import inspect
+import logging
 import sys
 import traceback
 from abc import ABC, abstractmethod
 from copy import copy
 from dataclasses import dataclass
 from itertools import chain
 from types import FrameType
@@ -26,18 +27,24 @@
 )
 
 import networkx as nx
 
 _PACKAGE_PREFIX = "referrers."
 
 _TYPE_LOCAL = "local"
+_TYPE_CLOSURE = "closure"
 _TYPE_GLOBAL = "global"
 _TYPE_OBJECT = "object"
 _TYPE_MODULE_VARIABLE = "module variable"
 
+logging.basicConfig(
+    format="[%(levelname)s] %(asctime)s %(message)s", level=logging.INFO
+)
+logger = logging.getLogger(__name__)
+
 
 @dataclass(frozen=True)
 class ReferrerGraphNode:
     """
     Represents a node in a referrer graph.
     """
 
@@ -298,14 +305,33 @@
             selector_func=lambda x: f"{frame.f_code.co_name}.{x[0]} ({_TYPE_LOCAL})",
         )
 
     def get_type(self) -> str:
         return _TYPE_LOCAL
 
 
+class ClosureVariableNameFinder(NameFinder):
+    def __init__(self):
+        self._closure_function_names: Dict[int, List[str]] = collections.defaultdict(
+            list
+        )
+        for var_value in gc.get_objects():
+            if hasattr(var_value, "__closure__") and var_value.__closure__:
+                for cell in var_value.__closure__:
+                    self._closure_function_names[id(cell.cell_contents)].append(
+                        f"{str(var_value)} ({_TYPE_CLOSURE})"
+                    )
+
+    def get_names(self, target_object: Any) -> Set[str]:
+        return set(self._closure_function_names.get(id(target_object), []))
+
+    def get_type(self) -> str:
+        return _TYPE_CLOSURE
+
+
 class GlobalVariableNameFinder(NameFinder):
     """
     Gets the names of global variables that refer to the target object, across the
     stack frames of all threads.
 
     The `get_names` method returns the names of global variables for the
     top-most frame of each thread that contains references to the target object.
@@ -469,19 +495,23 @@
                     _filter_container(
                         parent_object,
                         extractor_func=lambda x: enumerate(x),
                         filter_func=lambda x: x[1] is target_object,
                         selector_func=lambda x: f"{type(parent_object).__name__}[{x[0]}]",
                     )
                 )
-        except Exception:
+        except Exception as e:
             # Certain containers don't support iteration. We can't do anything about that,
             # so we just fall back to the more general name for the parent object.
             # The catch-all exception isn't ideal, but we don't know what exceptions
             # the container types might raise.
+            logger.warning(
+                f"Error encountered while iterating over a container: {e}. "
+                f"Falling-back to the parent object's type name."
+            )
             pass
         # If we couldn't find any more specific names, fall back to the parent's type name.
         if not names:
             names.add(f"{type(parent_object).__name__} (object)")
         return names
 
     def get_type(self) -> str:
@@ -641,18 +671,24 @@
 
     def _is_excluded(self, obj: Any) -> bool:
         # We exclude these objects because anything referenced by them should be picked-up
         # elsewhere (locals global etc), and excluding them speeds things up a lot.
         return inspect.isframe(obj) or inspect.isroutine(obj) or inspect.ismodule(obj)
 
     def _get_referrers(self, target_object: Any) -> Iterable[Any]:
-        if gc.is_tracked(target_object):
-            return gc.get_referrers(target_object)
-        else:
-            return self._untracked_objects_referrers.get(id(target_object), [])
+        # This might be empty if the object is not tracked. However, in some cases untracked
+        # objects have referrers, so we need to eliminate duplicates.
+        refs = gc.get_referrers(target_object)
+        ref_ids = {id(ref) for ref in refs}
+        for untracked_referrer in self._untracked_objects_referrers.get(
+            id(target_object), []
+        ):
+            if id(untracked_referrer) not in ref_ids:
+                refs.append(untracked_referrer)
+        return refs
 
     def _get_initial_target_node(
         self, target_object: Any
     ) -> Tuple[ReferrerGraphNode, Any, int]:
         name = f"{type(target_object).__name__} instance"
         return (
             ReferrerGraphNode(name=name, id=id(target_object), type="object"),
@@ -837,14 +873,15 @@
 
 def _get_name_finders(
     module_prefixes: Collection[str],
 ) -> Sequence[NameFinder]:
     finders = [
         LocalVariableNameFinder(),
         GlobalVariableNameFinder(),
+        ClosureVariableNameFinder(),
     ]
     for module_prefix in module_prefixes:
         finders.append(ModuleLevelNameFinder(module_prefix))
     return finders
 
 
 def _get_referrer_name_finders(
@@ -911,15 +948,19 @@
     """
     try:
         return {
             selector_func(item)
             for item in extractor_func(container)
             if filter_func(item)
         }
-    except RuntimeError:
+    except RuntimeError as e:
         # If we get a RuntimeError, it's likely that the iterable is being modified while
         # we're iterating over it. In this case we make a copy of the container and try again.
+        logger.warning(
+            f"Runtime error encountered while iterating over a container: {e}"
+            f"Retrying with a copy."
+        )
         return {
             selector_func(item)
             for item in extractor_func(copy(container))
             if filter_func(item)
         }
```

### Comparing `referrers-0.3.5/PKG-INFO` & `referrers-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: referrers
-Version: 0.3.5
+Version: 0.4.0
 Summary: Finds the graph of referrers for a Python object
 Author: Neil Ferguson
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


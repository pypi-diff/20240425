# Comparing `tmp/django_hierarchical_models-1.0.2.tar.gz` & `tmp/django_hierarchical_models-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hierarchical_models-1.0.2.tar", max compression
+gzip compressed data, was "django_hierarchical_models-1.1.0.tar", max compression
```

## Comparing `django_hierarchical_models-1.0.2.tar` & `django_hierarchical_models-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/LICENSE
--rw-r--r--   0        0        0     1568 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/README.md
--rw-r--r--   0        0        0       22 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/__init__.py
--rw-r--r--   0        0        0      499 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/alm.py
--rw-r--r--   0        0        0      754 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/exceptions.py
--rw-r--r--   0        0        0    14345 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/interface.py
--rw-r--r--   0        0        0     1104 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/node.py
--rw-r--r--   0        0        0    12577 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/nsm.py
--rw-r--r--   0        0        0     2735 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/django_hierarchical_models/models/pem.py
--rw-r--r--   0        0        0      828 2024-04-22 16:00:51.225044 django_hierarchical_models-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 django_hierarchical_models-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-25 14:11:21.750670 django_hierarchical_models-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3627 2024-04-25 14:11:21.750670 django_hierarchical_models-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-25 14:11:21.750670 django_hierarchical_models-1.1.0/django_hierarchical_models/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/alm.py
+-rw-r--r--   0        0        0      754 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/exceptions.py
+-rw-r--r--   0        0        0    14214 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/interface.py
+-rw-r--r--   0        0        0     1104 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/node.py
+-rw-r--r--   0        0        0    12674 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/nsm.py
+-rw-r--r--   0        0        0     2808 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/django_hierarchical_models/models/pem.py
+-rw-r--r--   0        0        0     1141 2024-04-25 14:11:21.754670 django_hierarchical_models-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 django_hierarchical_models-1.1.0/PKG-INFO
```

### Comparing `django_hierarchical_models-1.0.2/LICENSE` & `django_hierarchical_models-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.0.2/django_hierarchical_models/models/alm.py` & `django_hierarchical_models-1.1.0/django_hierarchical_models/models/alm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from typing import TypeVar
+
 from django.db import models
 from django.db.models import QuerySet
 
-from django_hierarchical_models.models.interface import HierarchicalModelInterface, T
+from django_hierarchical_models.models.interface import HierarchicalModelInterface
+
+T = TypeVar("T", bound="AdjacencyListModel")
 
 
 class AdjacencyListModel(HierarchicalModelInterface):
     """Adjacency List Model implementation of HierarchicalModel.
 
     Class description here.
 
@@ -29,23 +33,24 @@
     class Meta:
         abstract = True
 
     # ------------------------ override HierarchicalModel ------------------- #
 
     def parent(self: T) -> T | None:
         self.refresh_from_db(fields=("_parent",))
-        return self._parent
+        return self._parent  # type: ignore
 
     def is_child_of(self: T, parent: T) -> bool:
         self.refresh_from_db(fields=("_parent",))
-        if self._parent is None:
-            return False
-        if self._parent == parent:
-            return True
-        return self._parent.is_child_of(parent)
+        self_parent = self._parent
+        while self_parent is not None:
+            if self_parent == parent:
+                return True
+            self_parent = self_parent._parent
+        return False
 
     def _set_parent(self: T, parent: T | None):
         self._parent = parent
         self.save(update_fields=["_parent"])
 
     def set_parent_unchecked(self: T, parent: T | None):
         """Sets the parent of this instance without checking for cycles."""
```

### Comparing `django_hierarchical_models-1.0.2/django_hierarchical_models/models/exceptions.py` & `django_hierarchical_models-1.1.0/django_hierarchical_models/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.0.2/django_hierarchical_models/models/interface.py` & `django_hierarchical_models-1.1.0/django_hierarchical_models/models/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,69 @@
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
+import copy
 from collections import deque
 from collections.abc import Callable
 from typing import TypeVar
 
 from django.db import models
-from django.db.models import Manager, QuerySet
+from django.db.models import QuerySet
+from django.db.models.manager import BaseManager
 
 from django_hierarchical_models.models.exceptions import (
     AlreadyHasParentException,
     CycleException,
     NotAChildException,
 )
 from django_hierarchical_models.models.node import Node
 
 T = TypeVar("T", bound="HierarchicalModelInterface")
 
 
-class HierarchicalModelABCMeta(ABCMeta, type(models.Model)):
-    pass
-
-
-class HierarchicalModelInterface(models.Model, metaclass=HierarchicalModelABCMeta):
+class HierarchicalModelInterface(models.Model):
     """Django Model with support for hierarchical data.
 
     This interface is implemented multiple times with different tradeoffs.
     Because of the advantages of some implementations, they might have methods
     available which are not available on the interface.
     """
 
     # ------------------------ override models.Model ------------------------ #
 
     class Meta:
         abstract = True
 
     # ------------------------ public abstract methods ---------------------- #
 
-    @abstractmethod
     def parent(self: T) -> T | None:
         """The parent of the HierarchicalModel instance.
 
         Can trigger a `refresh_from_db` for certain internal fields.
 
         Returns:
             Parent instance, or None if there is no parent.
         """
-        pass
+        raise NotImplementedError()
 
-    @abstractmethod
     def is_child_of(self: T, parent: T) -> bool:
         """Checks if the instance is at any level a child to the parent."""
-        pass
+        raise NotImplementedError()
 
-    @abstractmethod
     def direct_children(self: T) -> QuerySet[T]:
         """Gets all the direct descendants of a model.
 
         If there are no children the QuerySet will be emtpy.
 
         In the course of finding all direct children, some models may have to
         evaluate QuerySets, others might not.
 
         Returns:
             An unordered QuerySet of all direct children of this model.
         """
-        pass
+        raise NotImplementedError()
 
     # ------------------------ public class methods ------------------------- #
     # the following models are default implementations which might be
     # overridden by different HierarchicalModel implementations
 
     def set_parent(self: T, parent: T | None):
         """Assigns the given model as the parent.
@@ -147,29 +141,31 @@
              that many levels.
 
         Returns:
             An ordered list of the instance's ancestors, starting with the
             closest on the left side of the list, and the root at the right.
         """
 
-        if self.parent() is None or (max_level is not None and max_level <= 0):
+        parent = self.parent()
+        if parent is None or (max_level is not None and max_level <= 0):
             return []
         if max_level is not None:
             max_level -= 1
-        return [self.parent()] + self.parent().ancestors(max_level=max_level)
+        return [parent] + parent.ancestors(max_level=max_level)
 
     def root(self: T) -> T:
         """Gives the root of the node.
 
         Returns:
             Returns the first parent with no parent.
         """
-        if self.parent() is None:
+        parent = self.parent()
+        if parent is None:
             return self
-        return self.parent().root()
+        return parent.root()
 
     def children(
         self: T,
         max_generations: int | None = None,
         max_siblings: int | None = None,
         max_total: int | None = None,
         sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None = None,
@@ -195,133 +191,136 @@
         if (
             (max_generations is not None and max_generations < 1)
             or (max_siblings is not None and max_siblings < 1)
             or (max_total is not None and max_total < 2)
         ):
             return root
         self._child_finder(
-            root, max_generations, max_siblings, max_total, sibling_transform
+            root,
+            max_generations or -1,
+            max_siblings or -1,
+            max_total or -1,
+            sibling_transform,
         )
         return root
 
     # ------------------------ private class methods ------------------------ #
 
     def _child_finder(
         self: T,
         root: Node[T],
-        max_generations: int | None,
-        max_siblings: int | None,
-        max_total: int | None,
-        sibling_transform: Callable[[QuerySet[T]], QuerySet[T]],
+        max_generations: int,
+        max_siblings: int,
+        max_total: int,
+        sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
     ):
         """Evaluates the children of the given node.
 
         If a function were to be overridden for finding children, this would be
         the one.
 
         This version uses the optional parameters get a function from a
         dispatch table. The functions in this dispatch table use a queue to do
         a BFS on the given root node.
         """
         f = _dispatch_table[
             (
-                max_generations is not None,
-                max_siblings is not None,
-                max_total is not None,
+                max_generations > -1,
+                max_siblings > -1,
+                max_total > -1,
             )
         ]
         f(root, max_generations, max_siblings, max_total, sibling_transform)
 
     @property
-    def _manager(self: T) -> Manager[T]:
+    def _manager(self: T) -> BaseManager[T]:
         """Convenience method to get the object manager at runtime."""
         return self.__class__._default_manager
 
     # ------------------------ private abstract methods --------------------- #
 
-    @abstractmethod
     def _set_parent(self: T, parent: T | None):
         """The actual mechanism of setting the parent.
 
         No checks for cycles or anything happen in this function.
 
         Args:
             parent: The parent to be set to.
         """
-        pass
+        raise NotImplementedError()
 
     # ------------------------ dispatch functions --------------------------- #
 
 
 def _no_no_no(
     root: Node[T],
-    max_generations: int,
-    max_siblings: int,
-    max_total: int,
+    _: int,
+    __: int,
+    ___: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root)])
+    queue = deque([(copy.copy(root), root)])
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         children = node.instance.direct_children()
         if sibling_transform is not None:
             children = sibling_transform(children)
         for child in children:
             child_node = Node[T](child)
             queue.append((node, child_node))
 
 
 def _yes_no_no(
     root: Node[T],
     max_generations: int,
-    max_siblings: int,
-    max_total: int,
+    _: int,
+    __: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root, 0)])
+    queue = deque([(copy.copy(root), root, 0)])
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             children = node.instance.direct_children()
             if sibling_transform is not None:
                 children = sibling_transform(children)
             for child in children:
                 child_node = Node[T](child)
                 queue.append((node, child_node, generation + 1))
 
 
 def _no_yes_no(
     root: Node[T],
-    max_generations: int,
+    _: int,
     max_siblings: int,
-    max_total: int,
+    __: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root)])
+    queue = deque([(copy.copy(root), root)])
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         children = node.instance.direct_children()
         if sibling_transform is not None:
             children = sibling_transform(children)
         for child in children[:max_siblings]:
             child_node = Node[T](child)
             queue.append((node, child_node))
 
 
 def _no_no_yes(
     root: Node[T],
-    max_generations: int,
-    max_siblings: int,
+    _: int,
+    __: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root)])
+    queue = deque([(copy.copy(root), root)])
     max_total -= 1
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         children = node.instance.direct_children()
         if sibling_transform is not None:
             children = sibling_transform(children)
@@ -331,18 +330,18 @@
             max_total -= 1
 
 
 def _yes_yes_no(
     root: Node[T],
     max_generations: int,
     max_siblings: int,
-    max_total: int,
+    _: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root, 0)])
+    queue = deque([(copy.copy(root), root, 0)])
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             children = node.instance.direct_children()
             if sibling_transform is not None:
                 children = sibling_transform(children)
@@ -350,19 +349,19 @@
                 child_node = Node[T](child)
                 queue.append((node, child_node, generation + 1))
 
 
 def _yes_no_yes(
     root: Node[T],
     max_generations: int,
-    max_siblings: int,
+    _: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root, 0)])
+    queue = deque([(copy.copy(root), root, 0)])
     max_total -= 1
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             children = node.instance.direct_children()
             if sibling_transform is not None:
@@ -371,20 +370,20 @@
                 child_node = Node[T](child)
                 queue.append((node, child_node, generation + 1))
                 max_total -= 1
 
 
 def _no_yes_yes(
     root: Node[T],
-    max_generations: int,
+    _: int,
     max_siblings: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root)])
+    queue = deque([(copy.copy(root), root)])
     max_total -= 1
     while queue:
         parent_node, node = queue.popleft()
         parent_node.children.append(node)
         num_siblings = min(max_siblings, max_total)
         children = node.instance.direct_children()
         if sibling_transform is not None:
@@ -398,15 +397,15 @@
 def _yes_yes_yes(
     root: Node[T],
     max_generations: int,
     max_siblings: int,
     max_total: int,
     sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None,
 ):
-    queue = deque([(Node[T](None), root, 0)])
+    queue = deque([(copy.copy(root), root, 0)])
     max_total -= 1
     while queue:
         parent_node, node, generation = queue.popleft()
         parent_node.children.append(node)
         if generation < max_generations:
             num_siblings = min(max_siblings, max_total)
             children = node.instance.direct_children()
```

### Comparing `django_hierarchical_models-1.0.2/django_hierarchical_models/models/node.py` & `django_hierarchical_models-1.1.0/django_hierarchical_models/models/node.py`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-1.0.2/django_hierarchical_models/models/nsm.py` & `django_hierarchical_models-1.1.0/django_hierarchical_models/models/nsm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from typing import TypeVar
+
 from django.db import models
 from django.db.models import F, Max, QuerySet
 
-from django_hierarchical_models.models.interface import HierarchicalModelInterface, T
+from django_hierarchical_models.models.interface import HierarchicalModelInterface
+
+T = TypeVar("T", bound="NestedSetModel")
 
 
 class NestedSetModel(HierarchicalModelInterface):
     """Nested Set Model implementation of HierarchicalModel.
 
     Each model has two integer fields, a left and a right. In NSM, if a model's
     left value is lower than another, and it's right value is higher, the
@@ -286,28 +290,28 @@
             An unordered QuerySet of all direct children of this model.
         """
         self.refresh_from_db(fields=("_left", "_right"))
         children_chunk = self._manager.filter(
             _left__gt=self._left, _right__lt=self._right
         ).order_by("_left")
         direct_children = []
-        while children_chunk.exists():
-            next_child = children_chunk.first()
+        next_child = children_chunk.first()
+        while next_child is not None:
             direct_children.append(next_child.pk)
             children_chunk = children_chunk.filter(_left__gt=next_child._right)
+            next_child = children_chunk.first()
         return self._manager.filter(pk__in=direct_children)
 
     def root(self: T) -> T:
         self.refresh_from_db(fields=("_left", "_right"))
         parents_query = self._manager.filter(
             _left__lt=self._left, _right__gt=self._right
         )
-        if not parents_query.exists():
-            return self
-        return parents_query.order_by("_left").first()
+        root = parents_query.order_by("_left").first()
+        return root if root is not None else self
 
     # ------------------------ public class methods ------------------------- #
 
     def num_children(self) -> int:
         self.refresh_from_db(fields=("_left", "_right"))
         return (self._right - self._left) // 2
```

### Comparing `django_hierarchical_models-1.0.2/django_hierarchical_models/models/pem.py` & `django_hierarchical_models-1.1.0/django_hierarchical_models/models/pem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from typing import TypeVar
+
 from django.db import connection, models
 from django.db.models import QuerySet
 
-from django_hierarchical_models.models.interface import HierarchicalModelInterface, T
+from django_hierarchical_models.models.interface import HierarchicalModelInterface
+
+T = TypeVar("T", bound="PathEnumerationModel")
 
 
 class PathEnumerationModel(HierarchicalModelInterface):
     pass
 
     # ------------------------ class members -------------------------------- #
```


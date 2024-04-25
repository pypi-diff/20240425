# Comparing `tmp/ofnodes-1.7.0.tar.gz` & `tmp/ofnodes-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.7.0.tar", max compression
+gzip compressed data, was "ofnodes-1.7.1.tar", max compression
```

## Comparing `ofnodes-1.7.0.tar` & `ofnodes-1.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.7.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.7.0/README.md
--rw-r--r--   0        0        0      590 2024-04-23 19:27:37.585725 ofnodes-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-22 18:07:58.574458 ofnodes-1.7.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.7.0/src/ofnodes/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.0/src/ofnodes/components/nodes/__init__ copy.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.0/src/ofnodes/components/nodes/__init__.py
--rw-r--r--   0        0        0     2676 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/nodes/descriptors.py
--rw-r--r--   0        0        0      817 2024-04-23 19:26:45.294035 ofnodes-1.7.0/src/ofnodes/components/nodes/mixins.py
--rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/structures/__init__.py
--rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/structures/descriptors.py
--rw-r--r--   0        0        0    20313 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/structures/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1520 2024-04-23 18:51:28.074288 ofnodes-1.7.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.7.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0     2632 2024-04-23 19:26:45.294035 ofnodes-1.7.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.7.1/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.7.1/README.md
+-rw-r--r--   0        0        0      590 2024-04-25 04:49:09.706501 ofnodes-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-1.7.1/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.7.1/src/ofnodes/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.1/src/ofnodes/components/nodes/__init__ copy.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.1/src/ofnodes/components/nodes/__init__.py
+-rw-r--r--   0        0        0     2676 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/nodes/descriptors.py
+-rw-r--r--   0        0        0      817 2024-04-23 19:26:45.294035 ofnodes-1.7.1/src/ofnodes/components/nodes/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/structures/__init__.py
+-rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/structures/descriptors.py
+-rw-r--r--   0        0        0    20313 2024-04-23 17:49:14.794379 ofnodes-1.7.1/src/ofnodes/components/structures/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.1/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-23 18:51:28.074288 ofnodes-1.7.1/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.7.1/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.1/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0     2749 2024-04-25 04:48:44.850592 ofnodes-1.7.1/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.7.1/PKG-INFO
```

### Comparing `ofnodes-1.7.0/LICENSE` & `ofnodes-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/README.md` & `ofnodes-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/pyproject.toml` & `ofnodes-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.7.0"
+version = "1.7.1"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.7.0/src/ofnodes/components/nodes/descriptors.py` & `ofnodes-1.7.1/src/ofnodes/components/nodes/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/src/ofnodes/components/nodes/mixins.py` & `ofnodes-1.7.1/src/ofnodes/components/nodes/mixins.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/src/ofnodes/components/structures/descriptors.py` & `ofnodes-1.7.1/src/ofnodes/components/structures/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/src/ofnodes/components/structures/mixins.py` & `ofnodes-1.7.1/src/ofnodes/components/structures/mixins.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.7.1/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.7.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.7.1/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,20 @@
         self._head: Optional[SinglyNode] = None
         self._tail: Optional[SinglyNode] = None
         self._target: Optional[Any|SinglyNode] = None
         if values:
             for value in values:
                 self.tail = value
 
+    def cycle_detection(self):
+
+        if self.tail.next is not None:
+            return True
+        return False
+
     def __add__(self, other):
         self.tail = other  # tail attr will validate
 
 
     def __repr__(self) -> str:
         #return f"{type(self).__name__}(head={type(self.head).__name__}, tail={self.tail})"
         if not self._head:
```

### Comparing `ofnodes-1.7.0/PKG-INFO` & `ofnodes-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.7.0
+Version: 1.7.1
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


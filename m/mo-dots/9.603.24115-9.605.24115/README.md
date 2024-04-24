# Comparing `tmp/mo_dots-9.603.24115.tar.gz` & `tmp/mo_dots-9.605.24115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_dots-9.603.24115.tar", last modified: Wed Apr 24 11:15:32 2024, max compression
+gzip compressed data, was "mo_dots-9.605.24115.tar", last modified: Wed Apr 24 22:22:08 2024, max compression
```

## Comparing `mo_dots-9.603.24115.tar` & `mo_dots-9.605.24115.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:15:32.315593 mo_dots-9.603.24115/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.603.24115/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-24 11:15:32.314456 mo_dots-9.603.24115/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.603.24115/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:15:32.299488 mo_dots-9.603.24115/mo_dots/
--rw-rw-rw-   0        0        0    13479 2024-04-24 10:11:14.000000 mo_dots-9.603.24115/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16648 2024-04-24 11:15:23.000000 mo_dots-9.603.24115/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4324 2024-04-24 10:11:14.000000 mo_dots-9.603.24115/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10450 2024-04-24 10:11:14.000000 mo_dots-9.603.24115/mo_dots/lists.py
--rw-rw-rw-   0        0        0     7076 2024-04-24 08:54:27.000000 mo_dots-9.603.24115/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5476 2024-04-24 10:11:14.000000 mo_dots-9.603.24115/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1423 2024-04-24 10:04:39.000000 mo_dots-9.603.24115/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:15:32.312082 mo_dots-9.603.24115/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-24 11:15:32.000000 mo_dots-9.603.24115/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-24 11:15:32.000000 mo_dots-9.603.24115/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:15:32.000000 mo_dots-9.603.24115/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.603.24115/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-24 11:15:32.000000 mo_dots-9.603.24115/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 11:15:32.000000 mo_dots-9.603.24115/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 11:15:32.315593 mo_dots-9.603.24115/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-24 11:15:26.000000 mo_dots-9.603.24115/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:22:08.114419 mo_dots-9.605.24115/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.605.24115/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-24 22:22:08.114419 mo_dots-9.605.24115/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.605.24115/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 22:22:08.103472 mo_dots-9.605.24115/mo_dots/
+-rw-rw-rw-   0        0        0    13485 2024-04-24 22:21:59.000000 mo_dots-9.605.24115/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16710 2024-04-24 22:21:59.000000 mo_dots-9.605.24115/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4399 2024-04-24 22:21:59.000000 mo_dots-9.605.24115/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10467 2024-04-24 22:21:59.000000 mo_dots-9.605.24115/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     7124 2024-04-24 22:21:59.000000 mo_dots-9.605.24115/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5501 2024-04-24 22:21:59.000000 mo_dots-9.605.24115/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1423 2024-04-24 10:04:39.000000 mo_dots-9.605.24115/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:22:08.114419 mo_dots-9.605.24115/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-24 22:22:08.000000 mo_dots-9.605.24115/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-24 22:22:08.000000 mo_dots-9.605.24115/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:22:08.000000 mo_dots-9.605.24115/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.605.24115/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-24 22:22:08.000000 mo_dots-9.605.24115/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 22:22:08.000000 mo_dots-9.605.24115/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:22:08.114419 mo_dots-9.605.24115/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-24 22:22:03.000000 mo_dots-9.605.24115/setup.py
```

### Comparing `mo_dots-9.603.24115/LICENSE` & `mo_dots-9.605.24115/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_dots-9.603.24115/PKG-INFO` & `mo_dots-9.605.24115/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.603.24115
+Version: 9.605.24115
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.603.24115/README.md` & `mo_dots-9.605.24115/README.md`

 * *Files identical despite different names*

### Comparing `mo_dots-9.603.24115/mo_dots/__init__.py` & `mo_dots-9.605.24115/mo_dots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 
 def missing(value):
     raise NotImplementedError("use is_missing")
 
 
 def fromkeys(keys, value=None):
-    if value == None:
+    if is_null(value):
         return Data()
     return dict_to_data(dict.fromkeys(keys, value))
 
 
 def set_default(d, *dicts):
     """
     RECURSIVE MERGE OF MULTIPLE dicts MOST IMPORTANT FIRST
@@ -146,15 +146,15 @@
     for k, default_value in default.items():
         raw_value = from_data(default_value)  # TWO DIFFERENT Dicts CAN SHARE id() BECAUSE THEY ARE SHORT LIVED
         if is_data(d):
             existing_value = d.get(k)
         else:
             existing_value = _get_attr(d, [k])
 
-        if existing_value == None:
+        if is_null(existing_value):
             if default_value != None:
                 if _get(default_value, CLASS) in datas._data_types:
                     df = seen.get(id(raw_value))
                     if df is not None:
                         _set_attr(d, [k], df)
                     else:
                         copy_dict = {}
@@ -324,18 +324,18 @@
 
     attr_name = path[-1]
 
     # ACTUAL SETTING OF VALUE
     try:
         old_value = _get_attr(obj, [attr_name])
         old_type = _get(old_value, CLASS)
-        if old_value == None or is_primitive(old_value):
+        if is_null(old_value) or is_primitive(old_value):
             old_value = None
             new_value = value
-        elif value == None:
+        elif is_null(value):
             new_value = None
         else:
             new_value = _get(old_value, CLASS)(value)  # TRY TO MAKE INSTANCE OF SAME CLASS
     except Exception:
         old_value = None
         new_value = value
 
@@ -431,15 +431,15 @@
 
     # AFTER
     def do_it(a):
         for x in listwrap(a):
             # do something
 
     """
-    if value == None:
+    if is_null(value):
         return FlatList()
     elif is_list(value):
         if isinstance(value, list):
             return list_to_data(value)
         else:
             return value
     elif is_many(value):
@@ -463,15 +463,15 @@
         return from_data(v)
 
 
 def tuplewrap(value):
     """
     INTENDED TO TURN lists INTO tuples FOR USE AS KEYS
     """
-    if value == None:
+    if is_null(value):
         return tuple()
     elif is_many(value):
         return tuple(tuplewrap(v) if is_sequence(v) else v for v in value)
     else:
         return (from_data(value),)
```

### Comparing `mo_dots-9.603.24115/mo_dots/datas.py` & `mo_dots-9.605.24115/mo_dots/datas.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     iteritems,
     long,
     text,
     MutableMapping,
     OrderedDict,
     first,
 )
-from mo_imports import expect
+from mo_imports import expect, export
 
 from mo_dots.fields import split_field, literal_field, concat_field
 from mo_dots.nones import Null, NullType, null_types, is_null
 from mo_dots.utils import CLASS, SLOT
 from mo_dots.utils import get_logger
 
 (
@@ -102,15 +102,15 @@
         d = _get(self, SLOT)
         if _get(d, CLASS) is dict:
             yield from d.items()
         else:
             yield from d.__iter__()
 
     def __getitem__(self, key):
-        if key == None:
+        if is_null(key):
             return Null
         if key == ".":
             output = _get(self, SLOT)
             if _get(output, CLASS) in _data_types:
                 return self
             else:
                 return output
@@ -135,15 +135,15 @@
         if is_null(o):
             return NullType(d, key)
         return to_data(o)
 
     def __setitem__(self, key, value):
         if key == "":
             get_logger().error("key is empty string.  Probably a bad idea")
-        if key == None:
+        if is_null(key):
             return Null
         if key == ".":
             # SOMETHING TERRIBLE HAPPENS WHEN value IS NOT A Mapping;
             # HOPEFULLY THE ONLY OTHER METHOD RUN ON self IS from_data()
             v = from_data(value)
             if is_many(v):
                 _set(self, CLASS, FlatList)
@@ -158,20 +158,20 @@
                 else:
                     d[key] = value
                 return self
 
             seq = _split_field(key)
             for k in seq[:-1]:
                 d = _getdefault(d, k)
-            if value == None:
+            if is_null(value):
                 try:
                     d.pop(seq[-1], None)
                 except Exception as _:
                     pass
-            elif d == None:
+            elif is_null(d):
                 d[literal_field(seq[-1])] = value
             elif is_sequence(d):
                 for dd in d:
                     from_data(dd)[seq[-1]] = value
             else:
                 d[seq[-1]] = value
             return self
@@ -244,19 +244,19 @@
         d = _get(self, SLOT)
         if not _get(other, CLASS) in _data_types:
             if is_missing(d) or (isinstance(d, dict) and not d):
                 _set(self, SLOT, other)
             return self
 
         for ok, ov in other.items():
-            if ov == None:
+            if is_null(ov):
                 continue
 
             sv = to_data(d.get(ok))
-            if sv == None:
+            if is_null(sv):
                 d[ok] = ov
             elif is_data(sv):
                 d[ok] = sv | ov
         return self
 
     def __hash__(self):
         d = _get(self, SLOT)
@@ -266,15 +266,15 @@
         if self is other:
             return True
 
         d = _get(self, SLOT)
         if _get(d, CLASS) is not dict:
             return d == other
 
-        if not d and other == None:
+        if not d and is_null(other):
             return False
 
         if _get(other, CLASS) not in _data_types:
             return False
         e = other
         for k, v in d.items():
             if e.get(k) != v:
@@ -307,15 +307,15 @@
 
     def iteritems(self):
         # LOW LEVEL ITERATION, NO WRAPPING
         d = _get(self, SLOT)
         return ((k, to_data(v)) for k, v in iteritems(d))
 
     def pop(self, key, default=Null):
-        if key == None:
+        if is_null(key):
             return Null
         if key == ".":
             raise NotImplemented()
 
         key = str(key)
         d = _get(self, SLOT)
 
@@ -327,15 +327,15 @@
                 elif is_list(d):
                     d = [_getdefault(dd, n) for dd in d]
                 else:
                     d = _getdefault(d, n)  # EVERYTHING ELSE TREATS n AS LITERAL
             key = seq[-1]
 
         o = d.get(key)
-        if o == None:
+        if is_null(o):
             if default is Null:
                 return NullType(d, key)
             return default
 
         d[key] = None
         return to_data(o)
 
@@ -387,15 +387,15 @@
     def __delattr__(self, key):
         key = str(key)
         d = _get(self, SLOT)
         d.pop(key, None)
 
     def setdefault(self, k, d=None):
         v = self[k]
-        if v == None:
+        if is_null(v):
             self[k] = d
             return d
         return v
 
     def __str__(self):
         return str(_get(self, SLOT))
 
@@ -443,15 +443,15 @@
     for k in get_keys(obj):
         try:
             v = obj[literal_field(k)]
             if is_missing(v):
                 continue
             kk = concat_field(parent, literal_field(k))
             vv = object_to_data(v)
-            yield from _leaves(kk, vv, path+(_id,))
+            yield from _leaves(kk, vv, path + (_id,))
         except Exception as cause:
             get_logger().error("Do not know how to handle", cause=cause)
 
 
 def _split_field(field):
     """
     SIMPLE SPLIT, NO CHECKS
@@ -479,15 +479,15 @@
         d += dict_to_data({"$": other})
         d["."] = d["$"]
         return d
 
     d = from_data(self)
     for ok, ov in other.items():
         sv = d.get(ok)
-        if sv == None:
+        if is_null(sv):
             d[ok] = from_data(deepcopy(ov))
         elif isinstance(ov, (Decimal, float, long, int)):
             if _get(sv, CLASS) in _data_types:
                 get_logger().error(
                     "can not add {{stype}} with {{otype}",
                     stype=_get(sv, CLASS).__name__,
                     otype=_get(ov, CLASS).__name__,
@@ -591,15 +591,15 @@
 wrap_leaves = leaves_to_data
 
 
 def _leaves_to_data(value):
     """
     RETURN UNWRAPPED STRUCTURES
     """
-    if value == None:
+    if is_null(value):
         return None
 
     if is_primitive(value):
         return value
 
     class_ = _get(value, CLASS)
     if class_ in _data_types:
@@ -623,15 +623,15 @@
             d = output
             for k in seq[:-1]:
                 e = d.get(k, None)
                 if not is_data(e):
                     e = d[k] = {}
                 d = e
 
-            if value == None:
+            if is_null(value):
                 d.pop(seq[-1], None)
             else:
                 d[seq[-1]] = value
         return output
 
     if hasattr(value, "__iter__"):
         return [_leaves_to_data(v) for v in value]
@@ -645,7 +645,10 @@
 def is_primitive(value):
     return isinstance(value, _primitive_types)
 
 
 def register_primitive(_type):
     global _primitive_types
     _primitive_types = tuple(set(_primitive_types + (_type,)))
+
+
+export("mo_dots.fields", is_missing)
```

### Comparing `mo_dots-9.603.24115/mo_dots/fields.py` & `mo_dots-9.605.24115/mo_dots/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import re
 import sys
 
 from mo_future import generator_types, flatten
+from mo_imports import expect
 
 from mo_dots.utils import get_logger, CLASS
 
+is_missing, is_null = expect("is_missing", "is_null")
+
 _module_type = type(sys.modules[__name__])
 _builtin_zip = zip
 _get = object.__getattribute__
 
 
 ESCAPE_DOTS1 = re.compile(r"(^\.|\.$)")  # DOTS AT START/END
 ESCAPE_DOTS2 = re.compile(r"(?<!^)\.(?!$)")  # INTERNAL DOTS
@@ -41,15 +44,15 @@
 
 
 def tail_field(field):
     """
     RETURN THE FIRST STEP IN PATH, ALONG WITH THE REMAINING TAILf
     IN (first, rest) PAIR
     """
-    if field == "." or field == None or field == "":
+    if field == "." or is_missing(field):
         return ".", "."
     elif "." in field:
         path = split_field(field)
         if path[0].startswith("."):
             return path[0], join_field(path[1:])
         return literal_field(path[0]), join_field(path[1:])
     else:
@@ -119,15 +122,15 @@
     return False
 
 
 def endswith_field(field, suffix):
     """
     RETURN True IF field PATH STRING ENDS WITH suffix PATH STRING
     """
-    if suffix == None:
+    if is_null(suffix):
         return False
     if suffix == ".":
         return True
 
     if field.endswith(suffix):
         ls = len(suffix)
         if len(field) == ls or field[-ls - 1] in (".", "\b") and field[-ls - 2] not in (".", "\b"):
```

### Comparing `mo_dots-9.603.24115/mo_dots/lists.py` & `mo_dots-9.605.24115/mo_dots/lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import types
 from copy import deepcopy
 
 from mo_future import generator_types, first
 from mo_imports import expect, delay_import, export
 
 from mo_dots.datas import is_missing, hash_value
-from mo_dots.nones import Null
+from mo_dots.nones import Null, is_null
 from mo_dots.utils import CLASS, SLOT
 
 Log = delay_import("mo_logs.Log")
 object_to_data, coalesce, to_data, from_data, get_attr = expect(
     "object_to_data", "coalesce", "to_data", "from_data", "get_attr"
 )
 
@@ -37,15 +37,15 @@
     """
 
     __slots__ = [SLOT]
 
     def __init__(self, vals=None):
         """ USE THE vals, NOT A COPY """
         # list.__init__(self)
-        if vals == None:
+        if is_null(vals):
             _set(self, SLOT, [])
         elif _get(vals, CLASS) is FlatList:
             _set(self, SLOT, vals.list)
         else:
             _set(self, SLOT, vals)
 
     def __getitem__(self, index):
@@ -193,74 +193,74 @@
         lst = _get(self, SLOT)
         if not lst:
             return _null_hash
         return hash_value(lst[0])
 
     def __eq__(self, other):
         lst = _get(self, SLOT)
-        if other == None:
+        if is_null(other):
             return len(lst) == 0
 
         try:
             if len(lst) != len(other):
                 return False
             return all([s == o for s, o in zip(lst, other)])
         except Exception:
             return False
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __add__(self, other):
         output = list(_get(self, SLOT))
-        if other == None:
+        if is_null(other):
             return self
         elif is_many(other):
             output.extend(from_data(other))
         else:
             output.append(other)
         return FlatList(vals=output)
 
     __or__ = __add__
 
     def __radd__(self, other):
         output = list(_get(self, SLOT))
-        if other == None:
+        if is_null(other):
             return self
         elif is_many(other):
             output = list(from_data(other)) + output
         else:
             output = [other] + output
         return FlatList(vals=output)
 
     def __iadd__(self, other):
-        if other == None:
+        if is_null(other):
             return self
         elif is_many(other):
             self.extend(from_data(other))
         else:
             self.append(other)
         return self
 
     def right(self, num):
         """
         WITH SLICES BEING FLAT, WE NEED A SIMPLE WAY TO SLICE FROM THE RIGHT [-num:]
         """
-        if num == None:
+        if is_null(num):
             return self
         if num <= 0:
             return Null
 
         return FlatList(_get(self, SLOT)[-num:])
 
     def limit(self, num):
         """
         NOT REQUIRED, BUT EXISTS AS OPPOSITE OF right()
         """
-        if num == None:
+        if is_null(num):
             return self
         if num <= 0:
             return Null
 
         return FlatList(_get(self, SLOT)[:num])
 
     left = limit
@@ -384,8 +384,8 @@
 export("mo_dots.datas", is_list)
 export("mo_dots.datas", list_to_data)
 export("mo_dots.datas", FlatList)
 export("mo_dots.datas", is_sequence)
 export("mo_dots.datas", is_many)
 
 export("mo_dots.nones", is_sequence)
-export("mo_dots.nones", FlatList)
+export("mo_dots.nones", FlatList)
```

### Comparing `mo_dots-9.603.24115/mo_dots/nones.py` & `mo_dots-9.605.24115/mo_dots/nones.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 from mo_future import none_type
-from mo_imports import expect
+from mo_imports import expect, export
 
 from mo_dots.utils import CLASS, KEY, SLOT
 
 to_data, get_attr, is_sequence, FlatList = expect("to_data", "get_attr", "is_sequence", "FlatList")
 
 _get = object.__getattribute__
 _set = object.__setattr__
@@ -188,18 +188,18 @@
         return output
 
     def __getattr__(self, key):
         key = str(key)
 
         o = to_data(_get(self, SLOT))
         k = _get(self, KEY)
-        if o == None:
+        if is_null(o):
             return NullType(self, key)
         v = o.get(k)
-        if v == None:
+        if is_null(v):
             return NullType(self, key)
         try:
             return v.get(key)
         except Exception as e:
             from mo_logs import Log
 
             Log.error("not expected", cause=e)
@@ -270,16 +270,16 @@
             if force:
                 obj[path0] = value
             else:
                 _setdefault(obj, path0, value)
             return
 
         old_value = get_attr(obj, path0)
-        if old_value == None:
-            if value == None:
+        if is_null(old_value):
+            if is_null(value):
                 return
             else:
                 obj[path0] = old_value = {}
 
         _assign_to_null(old_value, path[1:], value)
     except Exception as e:
         raise e
@@ -315,14 +315,16 @@
 
 
 def _setdefault(obj, key, value):
     """
     DO NOT USE __dict__.setdefault(obj, key, value), IT DOES NOT CHECK FOR obj[key] == None
     """
     v = obj.get(key)
-    if v == None:
+    if is_null(v):
         obj[key] = value
         return value
     return v
 
 
 null_types = (none_type, NullType)
+
+export("mo_dots.fields", is_null)
```

### Comparing `mo_dots-9.603.24115/mo_dots/objects.py` & `mo_dots-9.605.24115/mo_dots/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,22 +133,25 @@
     try:
         keys = known_types[_type] = _type.__slots__
         return keys
     except Exception:
         pass
 
     keys = known_types[_type] = tuple(
-        k for k in dir(_type) if k not in ignored_attributes and getattr(_type, k).__class__.__name__ in ["member_descriptor", "getset_descriptor"]
+        k
+        for k in dir(_type)
+        if k not in ignored_attributes
+        and getattr(_type, k).__class__.__name__ in ["member_descriptor", "getset_descriptor"]
     )
     return keys
 
 
 def object_to_data(v):
     try:
-        if v == None:
+        if is_null(v):
             return Null
     except Exception:
         pass
 
     if is_primitive(v):
         return v
```

### Comparing `mo_dots-9.603.24115/mo_dots/utils.py` & `mo_dots-9.605.24115/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.603.24115/mo_dots.egg-info/PKG-INFO` & `mo_dots-9.605.24115/mo_dots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.603.24115
+Version: 9.605.24115
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.603.24115/setup.py` & `mo_dots-9.605.24115/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.603.24115',
+    version='9.605.24115',
     zip_safe=False
 )
```


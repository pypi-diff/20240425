# Comparing `tmp/njson-1.1.0.tar.gz` & `tmp/njson-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njson-1.1.0.tar", max compression
+gzip compressed data, was "njson-1.2.0.tar", max compression
```

## Comparing `njson-1.1.0.tar` & `njson-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-22 04:52:19.621926 njson-1.1.0/LICENSE
--rw-r--r--   0        0        0     3742 2024-04-22 04:52:19.622926 njson-1.1.0/README.md
--rw-r--r--   0        0        0      162 2024-04-22 04:52:19.622926 njson-1.1.0/njson/__init__.py
--rw-r--r--   0        0        0    29137 2024-04-22 04:52:19.622926 njson-1.1.0/njson/njson.py
--rw-r--r--   0        0        0      568 2024-04-22 04:52:19.622926 njson-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 njson-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-25 06:59:00.601168 njson-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7432 2024-04-25 06:59:00.601168 njson-1.2.0/README.md
+-rw-r--r--   0        0        0      162 2024-04-25 06:59:00.601168 njson-1.2.0/njson/__init__.py
+-rw-r--r--   0        0        0    40938 2024-04-25 06:59:00.601168 njson-1.2.0/njson/njson.py
+-rw-r--r--   0        0        0      568 2024-04-25 06:59:00.601168 njson-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8344 1970-01-01 00:00:00.000000 njson-1.2.0/PKG-INFO
```

### Comparing `njson-1.1.0/LICENSE` & `njson-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `njson-1.1.0/njson/njson.py` & `njson-1.2.0/njson/njson.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 from typing import Iterable, Union, Hashable, Any, Type, Callable, Mapping
+try:
+    from typing import Self
+except ImportError:
+    from typing import TypeVar
+    Self = TypeVar("Self", bound="NestedJson")
 from types import GeneratorType
 from itertools import zip_longest, dropwhile
 from collections import deque, abc
 from pathlib import Path
 import json, io
 
 # -----------------------------------------------------------------------------
@@ -125,17 +130,17 @@
         '''Return `NestedJson` with data parsed as nested data-series.'''
         return self.parent._as_parsed_nested_data_series
 
 # -----------------------------------------------------------------------------
 # NestedJson class
 
 class NestedJson(abc.Mapping):
-    '''Provide fast JSON-like data transformation to and from nested
-    parent-child and flat label-value data items, such as Pandas `Series` with
-    MultiIndex index.
+    '''Provide fast JSON-like data manipulation and transformation to and from
+    nested parent-child and flat label-value data items, such as Pandas `Series`
+    with `MultiIndex` index.
 
     Args:
         data (list,dict): json-like nested data
 
     Attributes:
         data (dict,list): Return input data.
         str (str): Return data as json str.
@@ -160,15 +165,15 @@
             parsed.ds (NestedJson): Return `NestedJson` with input data parsed
                 as data-series (skip parsing sub-elements).
 
     Example usage:
         ## Flatten and unflatten nested json-like or flat-dict-like data.
         ```python
         >>> import njson as nj
-        >>> d = {'a': 1, 'b': [{}}, {'d': 2}]}
+        >>> d = {'a': 1, 'b': [{}, {'d': 2}]}
         >>> njd = nj.NestedJson(d)
         >>> print(njd.data) # source data
         >>> print(njd.flat_dict) # data as flat-dict with parent key tuples
         >>> print(njd.data_series) # with event length parent key tuples
         >>> print(njd.data_series_bfill) # even length key tuples aligned rigth
         >>> print(njd.get('b')) # get data
         >>> print(njd.get('b', 0)) # get nested data
@@ -183,16 +188,16 @@
         {'d': 2}
         '{"a": 1, "b": [{}, {"d": 2}]}'
         ```
 
         **Note**
         * Flat-dict keys are parent key tuples of nested json-like data values.
         * List value parent key labels in flat-dict are integer values.
-        * Empty dict, list, tuple, set values are not "flattened", as they have
-          no nested values or parent keys for nested values.
+        * Empty dict and list values are not "flattened", as they have no
+          nested values or parent keys for nested values.
         * The `.data_series` - a flat-dict with even length key tuples - has 
           similar data structure to pandas `Series` with `MultiIndex`. As such, 
           key tuple length normalization prepares data for efficient creation
           of Pandas `Series` objects from deeply nested JSON object data.
 
         ## Transforming Pandas `Series`, `DataFrame` to and from JSON-like data
         ```python
@@ -227,54 +232,114 @@
         * Pass `NestedJson` to pandas `Series.to_dict(into = NestedJson)` to
           directly derive `NestedJson` from Pandas `Series` data.
         * Stacking and unstacking Pandas `Series` with `.unstack()` and
           `.stack()` allows to tranform the nested JSON-like data to and from
           convenient tabular-like Pandas `DataFrame` data structure. Note that
           (un)stacking by default sorts the level(s) in the resulting index or
           columns and therefore can alter the order of elements.
+
+        ## Manipulate nested json-like data.
+        ```python
+        >>> import njson as nj
+        >>> d = {'a': 1, 'b': [{}, {'d': 2}]}
+        >>> njd = nj.NestedJson(d)
+        >>> # source data
+        >>> print(njd.data)
+        >>> # add new nested data
+        >>> print(njd.setdefault([{'k1': 'v', 'k2': 'v', 'k3': 'v'}], 'c').data)
+        >>> # clear single key,value pair from nested dict
+        >>> print(njd.clear('c', 0, 'k1').data)
+        >>> # clear all values from nested dict
+        >>> print(njd.clear('c', 0).data)
+        >>> # remove existing sub-element
+        >>> print(njd.remove('b', 1).data)
+        >>> # add new or update existing sub-element or value
+        >>> print(njd.update({'d': 2}, 'b', 1).data)
+        >>> # replace existing sub-element or value
+        >>> print(njd.replace('replaced', 'b', 1).data)
+        >>> # if key does not exist, replace doesn't add new data
+        >>> print(njd.replace('notreplaced', 'b', 2).data)
+        >>> # add new list value value at start position index
+        >>> print(njd.setdefault('new list value at start', 'b', -3).data)
+        {'a': 1, 'b': [{}, {'d': 2}]}
+        {'a': 1, 'b': [{}, {'d': 2}], 'c': [{'k1': 'v', 'k2': 'v', 'k3': 'v'}]}
+        {'a': 1, 'b': [{}, {'d': 2}], 'c': [{'k2': 'v', 'k3': 'v'}]}
+        {'a': 1, 'b': [{}, {'d': 2}], 'c': [{}]}
+        {'a': 1, 'b': [{}], 'c': [{}]}
+        {'a': 1, 'b': [{}, {'d': 2}], 'c': [{}]}
+        {'a': 1, 'b': [{}, 'replaced'], 'c': [{}]}
+        {'a': 1, 'b': [{}, 'replaced'], 'c': [{}]}
+        {'a': 1, 'b': ['new list value at start', {}, 'replaced'], 'c': [{}]}
+        ```
+
+        **Note**
+        * Data manipulation methods `.clear()`, `.remove()`, `.update()`, 
+          `.replace()`, and `.setdefault()` return `NestedJson` object. Such
+          that it is possible to pipe mutiple data manpiluation operations.
     '''
 
     _FILLVALUE = ''
 
     def __init__(
         self,
-        data: Union[dict, list] = None,
+        data: Union[dict, list],
     ) -> None:
         if type(data) is GeneratorType:
             self.data = dict(data)
         elif type(data) is NestedJson:
             self.data = data.data
         else:
             self.data = data
 
     def __getitem__(self, key) -> dict:
         '''Implement evaluation of self[key].'''
-        if key == (slice(None, None, None),):
-            return self.data
-        elif type(key) is tuple:
-            return self._get(*key)
-        elif type(key) is slice:
-            if key == slice(None, None, None):
+        if type(key) is not tuple:
+            key = (key,)
+        if type(key[0]) is slice:
+            if key[0] == slice(None, None, None):
                 return self.data
-            return NestedJson._get_slice(self.data, key)
+            else:
+                return NestedJson._get_slice(self.data, key[0])
         else:
-            return self._get(key)
+            return self._get(*key)
 
     def __contains__(self, key) -> bool:
         '''Return boolean indicating if key is in `NestedJson`.'''
         try:
             if type(key) is tuple:
                 self._get(*key)
             else:
                 self._get(key)
         except:
             return False
         else:
             return True
 
+    def __delitem__(self, key) -> None:
+        '''Delete the nested `NestedJson` element for the specified key.
+
+        Args:
+            key (Hashable): Parent key tuple.
+
+        Raises:
+            KeyError
+                If the key is not in `NestedJson`.
+        '''
+        if type(key) is not tuple:
+            key = (key,)
+        if key[0] == slice(None, None, None):
+            self.data.clear()
+        elif key in self:
+            if len(key) == 1:
+                del self.data[key[0]]
+            else:
+                del self._get(*key[:-1])[key[-1]]
+        else:
+            raise KeyError
+
     def __eq__(self, other: object) -> bool:
         '''Return `NestedJson` equal to other.'''
         if isinstance(other, (dict, list)):
             return self.data == other
         elif not isinstance(other, self.__class__):
             raise TypeError
         return self.data == other.data
@@ -282,15 +347,14 @@
     def __ne__(self, other: object) -> bool:
         '''Return `NestedJson` not Equal to other.'''
         return not self.__eq__(other)
 
     def __setitem__(self, key, value) -> None:
         '''Update nested `NestedJson` value.'''
         if type(key) is tuple:
-            print(key)
             if key[1:]:
                 pks, ck = key[:-1], key[-1]
                 if pks not in self:
                     raise IndexError("Key out of bounds.")
                 else:
                     parent_data = self._get(*pks)
                     parent_data[ck] = value
@@ -331,65 +395,59 @@
     @staticmethod
     def _nlevels(data):
         if type(data) is dict and data:
             return 1 + max([
                 NestedJson._nlevels(item) for item in data.values()
                 if (
                     type(item) is dict or
-                    type(item) is list or
-                    type(item) is tuple or
-                    type(item) is set
+                    type(item) is list
                 ) and item
             ] or [0])
         if (
             type(data) is list or
-            type(data) is tuple or
-            type(data) is set
+            type(data) is tuple
         ) and data:
             return 1 + max([
                 NestedJson._nlevels(item) for item in data
                 if (
                     type(item) is dict or
-                    type(item) is list or
-                    type(item) is tuple or
-                    type(item) is set
+                    type(item) is list
                 ) and item
             ] or [0])
         return 0
 
     @staticmethod
     def _count_nested_values(data) -> list:
         if not (
             type(data) is dict or
-            type(data) is list or
-            type(data) is tuple or
-            type(data) is set
+            type(data) is list
         ):
             return 1
         elif len(data) == 0:
             return 0
         else:
             length = 0
             for value in (data.values() if type(data) is dict else data):
                 if (
                     type(value) is dict or
-                    type(value) is list or
-                    type(value) is tuple or
-                    type(value) is set
+                    type(value) is list
                 ) and data:
                     length += NestedJson._count_nested_values(value)
                 else:
                     length += 1
         return length
 
     @staticmethod
     def _nested_get(data: Union[list,dict], *keys: Hashable) -> Any:
         '''Get sub-element from nested json-like data.'''
         for k in keys:
-            data = data[k]
+            if type(data) is dict or type(data) is list:
+                data = data[k]
+            else:
+                raise KeyError
         return data
 
     def _get(self, *keys: Hashable) -> Any:
         '''Get sub-element from `NestedJson` data.'''
         return NestedJson._nested_get(self.data, *keys)
 
     @staticmethod
@@ -506,29 +564,25 @@
         else:
             return keys
 
     @staticmethod
     def _nested_get_values(data) -> list:
         if not (
             type(data) is dict or
-            type(data) is list or
-            type(data) is tuple or
-            type(data) is set
+            type(data) is list
         ):
             return data
         elif not data:
             return data
         else:
             result = []
             for value in (data.values() if type(data) is dict else data):
                 if (
                     type(value) is dict or
-                    type(value) is list or
-                    type(value) is tuple or
-                    type(value) is set
+                    type(value) is list
                 ):
                     if not value:
                         result.append(value)
                     else:
                         result += NestedJson._nested_get_values(value)
                 else:
                     result.append(value)
@@ -545,31 +599,27 @@
         elif type(data) is dict:
             return data.items()
 
     @staticmethod
     def _nested_get_keys_lists(data) -> list:
         if not (
             type(data) is dict or
-            type(data) is list or
-            type(data) is tuple or
-            type(data) is set
+            type(data) is list
         ):
             return []
         else:
             result = []
             for key, value in list(NestedJson._to_dictlike_mapping(data)):
                 if isinstance(key, tuple):
                     key = list(key)
                 else:
                     key = [key]
                 if (
                     type(value) is dict or
-                    type(value) is list or
-                    type(value) is tuple or
-                    type(value) is set
+                    type(value) is list
                 ):
                     if len(value) == 0:
                         result.append(key)
                     else:
                         for subkey in NestedJson._nested_get_keys_lists(value):
                             result.append(
                                 key + subkey
@@ -653,14 +703,34 @@
             else:
                 return NestedJson._nest_data_series(data)
         elif type(data) is list and data:
             return [NestedJson._nested_nest_data_series(val) for val in data]
         else:
             return data
 
+    @staticmethod
+    def _nested_get_existing_parent_key(
+        data: Union[list,dict],
+        *key: Hashable
+    ) -> Any:
+        '''Get parent keys that exist in nested json-like data from the
+        specified keys.'''
+        parent_key = []
+        for k in key:
+            if type(data) is dict or type(data) is list:
+                try:
+                    data[k]
+                    parent_key.append(k)
+                    data = data[k]
+                except (KeyError, IndexError, TypeError) as error:
+                    break
+            else:
+                break
+        return tuple(parent_key)
+
     @property
     def _keys(self):
         return NestedJson._nested_get_keys(self.data)
 
     @property
     def _values(self):
         return NestedJson._nested_get_values(self.data)
@@ -759,14 +829,213 @@
         parsed.fd (NestedJson): Return `NestedJson` with input data parsed
             as flat-dict.
         parsed.ds (NestedJson): Return `NestedJson` with input data parsed
             as data-series.
         '''
         return _ParsedNestedJson(self)
 
+    def remove(self, *key: Hashable) -> Self:
+        '''If the key is in the `NestedJson` remove the sub-element and return
+        `NestedJson`; otherwise, return `NestedJson`.
+        '''
+        if key and key in self:
+            del self[key]
+        return self
+
+    def replace(self, value: Any, *key: Hashable) -> Self:
+        '''If the key is in the `NestedJson` replace the sub-element with value
+        and return `NestedJson`; otherwise, return `NestedJson`.
+        '''
+        if key and key in self:
+            self[key] = value
+        return self
+
+    def clear(self, *key: Hashable) -> Self:
+        ''' If no key is provided, clear root data list or dict and return
+        `NestedJson`. If the key is not in the `NestedJson`, return
+        `NestedJson`; otherwise, clear nested dict or list sub-element or
+        delete the value from the most nested parent dict or list sub-element
+        and return `NestedJson`.
+        '''
+        if not key:
+            self.data.clear()
+            return self
+        elif key in self:
+            element = self.get(*key)
+            if (type(element) is dict or type(element) is list) and element:
+                element.clear()
+                return self
+            else:
+                if len(key) == 1:
+                    del self.data[key[0]]
+                    return self
+                elif len(key) >= 2:
+                    del self._get(*key[:-1])[key[-1]]
+                    return self
+        else:
+            return self
+
+    def update(self, value: Any, *key: Hashable) -> Self:
+        '''Update `NestedJson` data by replacing existing json-like data key
+        sub-element or by adding missing sub-elements via `.update()` for dict
+        sub-elements or `.insert()` or `.append()` for list sub-elements.
+        If no key is provided, return `NestedJson`.
+        If no part of the parent key is in the `NestedJson`, add the missing
+        flat-dict parent keys with the specified value as nested json-like data
+        to `NestedJson` and return updated `NestedJson`.
+        If part of the parent key is in the `NestedJson` and existing 
+        sub-element is a dictionary, update dictionary at the specified 
+        sub-element key with the missing flat-dict parent keys with the
+        specified value as nested json-like data and return updated
+        `NestedJson`.
+        Otherwise, if existing sub-element is a list and first missing key label
+        is integer in list index, replace list value at the specified 
+        sub-element index position with the missing flat-dict parent keys with
+        the specified value as nested json-like data and return `NestedJson`.
+        Otherwise, if existing sub-element is a list and first missing key label
+        is not integer, append missing flat-dict parent keys with the specified
+        value to the list and return updated `NestedJson`.
+        '''
+        if not key:
+            return self
+        else:
+            parent_key = self._nested_get_existing_parent_key(self.data, *key)
+            if not parent_key:
+                if type(self.data) is dict:
+                    if len(key) == 1:
+                        self.data[key[0]] = value
+                        return self
+                    elif len(key) > 1:
+                        self.data[key[0]] = NestedJson._nested_nest_flat_dict(
+                            {key[1:]: value}
+                        )
+                        return self
+                elif type(self.data) is list:
+                    if len(key) == 1:
+                        if type(key[0]) is int:
+                            self.data.insert(key[0], value)
+                            return self
+                        else:
+                            self.data.append(
+                                NestedJson._nested_nest_flat_dict(
+                                    {key: value}
+                                )
+                            )
+                            return self
+                    elif len(key) > 1:
+                        if type(key[0]) is int:
+                            self.data.insert(
+                                key[0],
+                                NestedJson._nested_nest_flat_dict(
+                                    {key[1:]: value}
+                                )
+                            )
+                            return self
+                        else:
+                            self.data.append(
+                                NestedJson._nested_nest_flat_dict(
+                                    {key: value}
+                                )
+                            )
+                            return self
+            elif len(key) > len(parent_key):
+                nest_key = key[len(parent_key):]
+                if parent_key:
+                    data = self._get(*parent_key)
+                else:
+                    data = self.data
+                if type(data) is dict:
+                    if len(nest_key) == 1:
+                        data[nest_key[0]] = value
+                        return self
+                    elif len(nest_key) > 1:
+                        data[nest_key[0]] = NestedJson._nested_nest_flat_dict(
+                            {nest_key[1:]: value}
+                        )
+                        return self
+                elif type(data) is list:
+                    if len(nest_key) == 1:
+                        if type(nest_key[0]) is int:
+                            data.insert(nest_key[0], value)
+                            return self
+                        else:
+                            data.append(
+                                NestedJson._nested_nest_flat_dict(
+                                    {nest_key: value}
+                                )
+                            )
+                            return self
+                    elif len(nest_key) > 1:
+                        if type(nest_key[0]) is int:
+                            data.insert(
+                                nest_key[0],
+                                NestedJson._nested_nest_flat_dict(
+                                    {nest_key[1:]: value}
+                                )
+                            )
+                            return self
+                        else:
+                            data.append(
+                                NestedJson._nested_nest_flat_dict(
+                                    {nest_key: value}
+                                )
+                            )
+                            return self
+                else:
+                    if len(parent_key) == 1:
+                        self.data[parent_key[0]] = (
+                            NestedJson._nested_nest_flat_dict(
+                                {nest_key: value}
+                            )
+                        )
+                        return self
+                    elif len(parent_key) >= 2:
+                        self._get(*parent_key[:-1])[parent_key[-1]] = (
+                            NestedJson._nested_nest_flat_dict(
+                                {nest_key: value}
+                            )
+                        )
+                        return self
+            else:
+                if len(parent_key) == 1:
+                    self.data[parent_key[0]] = value
+                    return self
+                elif len(parent_key) >= 2:
+                    self._get(*parent_key[:-1])[parent_key[-1]] = value
+                    return self
+            return self
+
+    def setdefault(self, value: Any, *key: Hashable) -> Self:
+        '''If the key is in the `NestedJson`, return `NestedJson` without adding
+        new sub-element data.
+        Otherwise, update `NestedJson` data by replacing existing json-like data
+        key sub-element or by adding missing sub-elements via `.update()` for
+        dict sub-elements or `.insert()` and `.append()` for list sub-elements.
+        If no key is provided, return `NestedJson`.
+        If no part of the parent key is in the `NestedJson`, add the missing
+        flat-dict parent keys with the specified value as nested json-like data
+        to `NestedJson` and return updated `NestedJson`.
+        If part of the parent key is in the `NestedJson` and existing 
+        sub-element is a dictionary, update dictionary at the specified 
+        sub-element key with the missing flat-dict parent keys with the
+        specified value as nested json-like data and return updated
+        `NestedJson`.
+        Otherwise, if existing sub-element is a list and first missing key label
+        is integer in list index, replace list value at the specified 
+        sub-element index position with the missing flat-dict parent keys with
+        the specified value as nested json-like data and return `NestedJson`.
+        Otherwise, if existing sub-element is a list and first missing key label
+        is not integer, append missing flat-dict parent keys with the specified
+        value to the list and return updated `NestedJson`.
+        '''
+        if key in self or not key:
+            return self
+        else:
+            return self.update(value, *key)
+
     def get(self, *key: Hashable, default=None) -> Any:
         '''Get any nested element or return value of keyword agrument `default`
         if key is not found.'''
         try:
             return self._get(*key)
         except KeyError:
             return default
@@ -839,8 +1108,8 @@
         bfill = False
     ) -> Iterable:
         '''Pass `NestedJson`'s `.data_series` as argument to `fn`.'''
         return fn(self.data_series)
 
     def pipe_mapping(self, fn: Callable[[Mapping], Any]) -> Any:
         '''Pass `NestedJson`'s iterable as argument to `fn`.'''
-        return fn(self._mapping)
+        return fn(self._mapping)
```

### Comparing `njson-1.1.0/pyproject.toml` & `njson-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "njson"
-version = "1.1.0"
+version = "1.2.0"
 description = "Provide fast JSON-like data transformation to and from nested parent-child and flat label-value data items, such as Pandas `Series` with MultiIndex index."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/njson"
 documentation = "https://gitlab.com/martins-bruvelis/njson/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `njson-1.1.0/PKG-INFO` & `njson-1.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,72 @@
-Metadata-Version: 2.1
-Name: njson
-Version: 1.1.0
-Summary: Provide fast JSON-like data transformation to and from nested parent-child and flat label-value data items, such as Pandas `Series` with MultiIndex index.
-Home-page: https://gitlab.com/martins-bruvelis/njson
-Author: Martins Bruvelis
-Author-email: martins.bruvelis@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Project-URL: Documentation, https://gitlab.com/martins-bruvelis/njson/-/blob/main/README.md
-Project-URL: Repository, https://gitlab.com/martins-bruvelis/njson
-Description-Content-Type: text/markdown
-
 # njson: efficient JSON-like data transformation tool
 
 ## What is it?
 Provide fast JSON-like data transformation to and from nested
-parent-child and flat label-value data items, such as Pandas `Series` with
-MultiIndex index.
+parent-child and flat label-value data items, such as Pandas `Series`
+with MultiIndex index.
 
 ## Features
 
-* Transformation are optimized for speed, to allow parsing deeply nested json-like data with millions of data points in seconds.
-* Transformation are lazily computed properties only calculated when accessed for the first time. Initializing NestedJson object does not require parsing the source data.
-* NestedJson is Pure-Python package that runs on JupyterLite, Pyodide, PyScript, Cloudflare Workers in Python, etc.
-* Itegrates with pandas for quick data transformation to and from pandas `Series` and `DataFrame`.
+* Transformation are optimized for speed, to allow parsing deeply 
+  nested json-like data with millions of data points in seconds.
+* Transformation are lazily computed properties only calculated when
+  accessed for the first time. Initializing NestedJson object does not
+  require parsing the source data.
+* NestedJson is Pure-Python package that runs on JupyterLite, Pyodide,
+  PyScript, Cloudflare Workers in Python, etc.
+* Itegrates with pandas for quick data transformation to and from
+  pandas `Series` and `DataFrame`.
 * Provides easy access to nested data at any level using parent keys.
+* Provides easy way to pipe data manipulation methods for editing nested
+  json-like data. 
 
 ## Example usage
 ### Flatten and unflatten nested json-like or flat-dict-like data.
 ```python
 >>> import njson as nj
->>> d = {'a': 1, 'b': [{}}, {'d': 2}]}
+>>> d = {'a': 1, 'b': [{}, {'d': 2}]}
 >>> njd = nj.NestedJson(d)
 >>> print(njd.data) # source data
 >>> print(njd.flat_dict) # data as flat-dict with parent key tuples
->>> print(njd.data_series) # data as flat-dict with parent key tuples
->>> print(njd.data_series_bfill) # ... even length key tuples aligned "rigth"
+>>> print(njd.data_series) # with event length parent key tuples
+>>> print(njd.data_series_bfill) # even length key tuples aligned rigth
 >>> print(njd.get('b')) # get data
 >>> print(njd.get('b', 0)) # get nested data
 >>> print(njd.get('b', 1)) # get data at any nesting level
->>> njd.parsed.nfd.str # json str of origianl data parsed as nested flat-dict
+>>> njd.parsed.nfd.str # json str of `.data` parsed as nested flat-dict
 {'a': 1, 'b': [{}, {'d': 2}]}
 {('a',): 1, ('b', 0): {}, ('b', 1, 'd'): 2}
 {('a', '', ''): 1, ('b', 0, ''): {}, ('b', 1, 'd'): 2}
 {('', '', 'a'): 1, ('', 'b', 0): {}, ('b', 1, 'd'): 2}
 [{}, {'d': 2}]
 {}
 {'d': 2}
 '{"a": 1, "b": [{}, {"d": 2}]}'
 ```
 
 **Note**
-* All flat-dict keys are tuples representing parent keys of json-like data.
-* The flat-dict labels keys for nested lists are integer values.
-* Empty dict,  list, tuple, set values are not flattened, as they have no values
-  or parent keys.
-* The `.data_series` flat-dict with even length key tuples has similar data
-  structure to pandas `MultiIndex` `Series`. Key tuple length normalization 
-  prepares data for efficient creation of Pandas `Series` objects from deeply
-  nested JSON object data.
+* Flat-dict keys are parent key tuples of nested json-like data values.
+* List value parent key labels in flat-dict are integer values.
+* Empty dict and list values are not "flattened", as they have no
+  nested values or parent keys for nested values.
+* The `.data_series` - a flat-dict with even length key tuples - has 
+  similar data structure to pandas `Series` with `MultiIndex`. As such, 
+  key tuple length normalization prepares data for efficient creation
+  of Pandas `Series` objects from deeply nested JSON object data.
 
 ### Transforming Pandas `Series`, `DataFrame` to and from JSON-like data
 ```python
 >>> import pandas as pd
 >>> import njson as nj
 >>> d = {'a': 1, 'b': [{}, {'d': 2}]}
 >>> njd = nj.NestedJson(d)
->>> ds = njd.to_data_series(pd.Series)
->>> print(ds)
->>> print(ds.unstack(level = [0]))
+>>> ds = njd.to_data_series(into = pd.Series)
+>>> print(ds) # pandas Series from NestedJson
+>>> print(ds.unstack(level = [0])) # to DataFrame from Series
 >>> print(ds.to_dict(into = NestedJson).parsed.nds.data)
 <class 'pandas.core.series.Series'>
 a           1
 b  0       {}
    1  d     2
 dtype: object
             d
@@ -89,28 +77,109 @@
 b  0       {}
    1  d     2
 dtype: object
 {'a': 1, 'b': [{}, {'d': 2}]}
 ```
 
 **Note**
-* Pass pandas Series `pd.Series` to NestedJson 
-  `NestedJson.to_data_series(into = NestedJson)` to directly 
-  derive Pandas `Series` data. Then access `.parsed.nds.data`
-  attribute to return nested JSON-like data.
-* Pass `NestedJson` to pandas `Series.to_dict(into = NestedJson)` to directly 
-  derive `NestedJson` from Pandas `Series` data.
-* Stacking and unstacking Pandas `Series` with `.unstack()` and `.stack()`
-  allows to tranform the nested JSON-like data to and from convenient 
-  tabular-like Pandas `DataFrame` data structure. Note that (un)stacking
-  by default sorts the level(s) in the resulting index/columns and therefore can
-  alter the order of elements.
+* Pass pandas `Series` to `NestedJson`'s `.to_data_series` method to
+  directly derive Pandas `Series` data. Then access `.parsed.nds.data`
+  attribute to derive nested JSON-like data.
+* Pass `NestedJson` to pandas `Series.to_dict(into = NestedJson)` to
+  directly derive `NestedJson` from Pandas `Series` data.
+* Stacking and unstacking Pandas `Series` with `.unstack()` and
+  `.stack()` allows to tranform the nested JSON-like data to and from
+  convenient tabular-like Pandas `DataFrame` data structure. Note that
+  (un)stacking by default sorts the level(s) in the resulting index or
+  columns and therefore can alter the order of elements.
+
+### Manipulate nested json-like data.
+```python
+>>> import njson as nj
+>>> d = {'a': 1, 'b': [{}, {'d': 2}]}
+>>> njd = nj.NestedJson(d)
+>>> # source data
+>>> print(njd.data)
+>>> # add new nested data
+>>> print(njd.setdefault([{'k1': 'v', 'k2': 'v', 'k3': 'v'}], 'c').data)
+>>> # clear single key,value pair from nested dict
+>>> print(njd.clear('c', 0, 'k1').data)
+>>> # clear all values from nested dict
+>>> print(njd.clear('c', 0).data)
+>>> # remove existing sub-element
+>>> print(njd.remove('b', 1).data)
+>>> # add new or update existing sub-element or value
+>>> print(njd.update({'d': 2}, 'b', 1).data)
+>>> # replace existing sub-element or value
+>>> print(njd.replace('replaced', 'b', 1).data)
+>>> # if key does not exist, replace doesn't add new data
+>>> print(njd.replace('notreplaced', 'b', 2).data)
+>>> # add new list value value at start position index
+>>> print(njd.setdefault('new list value at start', 'b', -3).data)
+{'a': 1, 'b': [{}, {'d': 2}]}
+{'a': 1, 'b': [{}, {'d': 2}], 'c': [{'k1': 'v', 'k2': 'v', 'k3': 'v'}]}
+{'a': 1, 'b': [{}, {'d': 2}], 'c': [{'k2': 'v', 'k3': 'v'}]}
+{'a': 1, 'b': [{}, {'d': 2}], 'c': [{}]}
+{'a': 1, 'b': [{}], 'c': [{}]}
+{'a': 1, 'b': [{}, {'d': 2}], 'c': [{}]}
+{'a': 1, 'b': [{}, 'replaced'], 'c': [{}]}
+{'a': 1, 'b': [{}, 'replaced'], 'c': [{}]}
+{'a': 1, 'b': ['new list value at start', {}, 'replaced'], 'c': [{}]}
+```
+
+**Note**
+* Data manipulation methods `.clear()`, `.remove()`, `.update()`, 
+  `.replace()`, and `.setdefault()` return `NestedJson` object. Such
+  that it is possible to pipe mutiple data manpiluation operations.
 
 ### Read JSON files
 
 ```python
 >>> import njson as nj
 >>> njd_from_file = nj.read_json('path-to.json')
 >>> njd_from_str = nj.read_json_str('{"a": 1, "b": [{}, {"d": 2}]}')
 >>> njd_from_str.flat_dict
 {('a',): 1, ('b', 0): {}, ('b', 1, 'd'): 2}
 ```
+
+## Changelog
+
+### v1.2
+#### Features
+* Add data manipulation methods `.clear()`, `.remove()`, `.update()`, 
+  `.replace()`, and `.setdefault()`.
+
+#### Bug Fixes
+* Do not flatten `tuple` and `set` objects, to avoid non-reversable data
+  transformations via implicit data converstions from tuples to lists.
+
+### v1.1
+#### Features
+* Add methods `.pipe_flat_dict()`, `.pipe_data_series()`, 
+  `.pipe_mapping()` to pipe flat-dict, data-series, mapping, in addition
+  to `.pipe_data()`.
+* Add optimzied `NestedJsonKeysView`, `NestedJsonValuesView`,
+  `NestedJsonItemsView` for `.keys()`, `.values()`, and `.items()`
+  methods.
+
+### v1.0
+#### Features
+* Initial implementation of fast JSON-like data transformation to and 
+  from nested parent-child and flat label-value data items.
+* Flat-dict keys are parent key tuples of nested json-like data values.
+* List value parent key labels in flat-dict are integer values.
+* Empty dict and list values are not "flattened", as they have
+  no nested values or parent keys for nested values.
+* The `.data_series()` - a flat-dict with even length key tuples - has 
+  similar data structure to pandas `Series` with `MultiIndex`. As such, 
+  key tuple length normalization prepares data for efficient creation
+  of Pandas `Series` objects from deeply nested JSON object data.
+* Pass pandas `Series` to `NestedJson`'s `.to_data_series` method to
+  directly derive Pandas `Series` data. Then access `.parsed.nds.data`
+  attribute to derive nested JSON-like data.
+* Pass `NestedJson` to pandas `Series.to_dict(into = NestedJson)` to
+  directly derive `NestedJson` from Pandas `Series` data.
+* Stacking and unstacking Pandas `Series` with `.unstack()` and
+  `.stack()` allows to tranform the nested JSON-like data to and from
+  convenient tabular-like Pandas `DataFrame` data structure. Note that
+  (un)stacking by default sorts the level(s) in the resulting index or
+  columns and therefore can alter the order of elements.
```


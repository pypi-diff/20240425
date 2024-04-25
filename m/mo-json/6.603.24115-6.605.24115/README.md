# Comparing `tmp/mo_json-6.603.24115.tar.gz` & `tmp/mo_json-6.605.24115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_json-6.603.24115.tar", last modified: Wed Apr 24 11:27:23 2024, max compression
+gzip compressed data, was "mo_json-6.605.24115.tar", last modified: Wed Apr 24 22:33:31 2024, max compression
```

## Comparing `mo_json-6.603.24115.tar` & `mo_json-6.605.24115.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:27:23.237545 mo_json-6.603.24115/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:20:36.000000 mo_json-6.603.24115/LICENSE
--rw-rw-rw-   0        0        0    11731 2024-04-24 11:27:23.236457 mo_json-6.603.24115/PKG-INFO
--rw-rw-rw-   0        0        0    10214 2024-03-15 11:50:58.000000 mo_json-6.603.24115/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:27:23.228335 mo_json-6.603.24115/mo_json/
--rw-rw-rw-   0        0        0    10557 2024-03-21 02:31:33.000000 mo_json-6.603.24115/mo_json/__init__.py
--rw-rw-rw-   0        0        0      592 2024-02-15 02:44:26.000000 mo_json-6.603.24115/mo_json/array.py
--rw-rw-rw-   0        0        0      313 2023-04-14 10:26:27.000000 mo_json-6.603.24115/mo_json/decoder.py
--rw-rw-rw-   0        0        0    15671 2024-04-23 00:37:33.000000 mo_json-6.603.24115/mo_json/encoder.py
--rw-rw-rw-   0        0        0     5733 2024-04-23 00:37:33.000000 mo_json-6.603.24115/mo_json/scrubber.py
--rw-rw-rw-   0        0        0    16226 2024-04-23 00:37:33.000000 mo_json-6.603.24115/mo_json/stream.py
--rw-rw-rw-   0        0        0    17556 2024-03-16 19:49:48.000000 mo_json-6.603.24115/mo_json/typed_encoder.py
--rw-rw-rw-   0        0        0     4057 2024-03-16 16:18:12.000000 mo_json-6.603.24115/mo_json/typed_object.py
--rw-rw-rw-   0        0        0    11797 2024-03-21 02:31:33.000000 mo_json-6.603.24115/mo_json/types.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:27:23.234292 mo_json-6.603.24115/mo_json.egg-info/
--rw-rw-rw-   0        0        0    11731 2024-04-24 11:27:23.000000 mo_json-6.603.24115/mo_json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-04-24 11:27:23.000000 mo_json-6.603.24115/mo_json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:27:23.000000 mo_json-6.603.24115/mo_json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2024-04-24 11:27:23.000000 mo_json-6.603.24115/mo_json.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 11:27:23.000000 mo_json-6.603.24115/mo_json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 11:27:23.237545 mo_json-6.603.24115/setup.cfg
--rw-rw-rw-   0        0        0    11626 2024-04-24 11:27:18.000000 mo_json-6.603.24115/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:33:31.257982 mo_json-6.605.24115/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:20:36.000000 mo_json-6.605.24115/LICENSE
+-rw-rw-rw-   0        0        0    11731 2024-04-24 22:33:31.257982 mo_json-6.605.24115/PKG-INFO
+-rw-rw-rw-   0        0        0    10214 2024-03-15 11:50:58.000000 mo_json-6.605.24115/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 22:33:31.249525 mo_json-6.605.24115/mo_json/
+-rw-rw-rw-   0        0        0    10557 2024-03-21 02:31:33.000000 mo_json-6.605.24115/mo_json/__init__.py
+-rw-rw-rw-   0        0        0      592 2024-02-15 02:44:26.000000 mo_json-6.605.24115/mo_json/array.py
+-rw-rw-rw-   0        0        0      313 2023-04-14 10:26:27.000000 mo_json-6.605.24115/mo_json/decoder.py
+-rw-rw-rw-   0        0        0    15671 2024-04-23 00:37:33.000000 mo_json-6.605.24115/mo_json/encoder.py
+-rw-rw-rw-   0        0        0     5733 2024-04-23 00:37:33.000000 mo_json-6.605.24115/mo_json/scrubber.py
+-rw-rw-rw-   0        0        0    16226 2024-04-23 00:37:33.000000 mo_json-6.605.24115/mo_json/stream.py
+-rw-rw-rw-   0        0        0    17556 2024-03-16 19:49:48.000000 mo_json-6.605.24115/mo_json/typed_encoder.py
+-rw-rw-rw-   0        0        0     4057 2024-03-16 16:18:12.000000 mo_json-6.605.24115/mo_json/typed_object.py
+-rw-rw-rw-   0        0        0    11797 2024-03-21 02:31:33.000000 mo_json-6.605.24115/mo_json/types.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:33:31.257982 mo_json-6.605.24115/mo_json.egg-info/
+-rw-rw-rw-   0        0        0    11731 2024-04-24 22:33:31.000000 mo_json-6.605.24115/mo_json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-04-24 22:33:31.000000 mo_json-6.605.24115/mo_json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:33:31.000000 mo_json-6.605.24115/mo_json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2024-04-24 22:33:31.000000 mo_json-6.605.24115/mo_json.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 22:33:31.000000 mo_json-6.605.24115/mo_json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:33:31.257982 mo_json-6.605.24115/setup.cfg
+-rw-rw-rw-   0        0        0    11626 2024-04-24 22:33:26.000000 mo_json-6.605.24115/setup.py
```

### Comparing `mo_json-6.603.24115/LICENSE` & `mo_json-6.605.24115/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/PKG-INFO` & `mo_json-6.605.24115/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.603.24115
+Version: 6.605.24115
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -14,18 +14,18 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: mo-dots==9.603.24115
+Requires-Dist: mo-dots==9.605.24115
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.603.24115
-Requires-Dist: mo-times==5.603.24115
+Requires-Dist: mo-logs==8.605.24115
+Requires-Dist: mo-times==5.605.24115
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
 Requires-Dist: pytz>=2024.1; extra == "tests"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "tests"
 
 # More JSON Tools
```

### Comparing `mo_json-6.603.24115/README.md` & `mo_json-6.605.24115/README.md`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/__init__.py` & `mo_json-6.605.24115/mo_json/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/array.py` & `mo_json-6.605.24115/mo_json/array.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/encoder.py` & `mo_json-6.605.24115/mo_json/encoder.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/scrubber.py` & `mo_json-6.605.24115/mo_json/scrubber.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/stream.py` & `mo_json-6.605.24115/mo_json/stream.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/typed_encoder.py` & `mo_json-6.605.24115/mo_json/typed_encoder.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/typed_object.py` & `mo_json-6.605.24115/mo_json/typed_object.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json/types.py` & `mo_json-6.605.24115/mo_json/types.py`

 * *Files identical despite different names*

### Comparing `mo_json-6.603.24115/mo_json.egg-info/PKG-INFO` & `mo_json-6.605.24115/mo_json.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.603.24115
+Version: 6.605.24115
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -14,18 +14,18 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: mo-dots==9.603.24115
+Requires-Dist: mo-dots==9.605.24115
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.603.24115
-Requires-Dist: mo-times==5.603.24115
+Requires-Dist: mo-logs==8.605.24115
+Requires-Dist: mo-times==5.605.24115
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
 Requires-Dist: pytz>=2024.1; extra == "tests"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "tests"
 
 # More JSON Tools
```

### Comparing `mo_json-6.603.24115/setup.py` & `mo_json-6.605.24115/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More JSON Tools! ',
     extras_require={"tests":["mo-testing>=8.591.24112","mo-threads>=6.589.24111","pytz>=2024.1","beautifulsoup4>=4.12.3"]},
-    install_requires=["hjson","mo-dots==9.603.24115","mo-future==7.584.24095","mo-logs==8.603.24115","mo-times==5.603.24115"],
+    install_requires=["hjson","mo-dots==9.605.24115","mo-future==7.584.24095","mo-logs==8.605.24115","mo-times==5.605.24115"],
     license='MPL 2.0',
     long_description='# More JSON Tools\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-json.svg)](https://pypi.org/project/mo-json/)\n [![Build Status](https://github.com/klahnakoski/mo-json/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-json/actions/workflows/build.yml)\n [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-json/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-json?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-json)](https://pepy.tech/project/mo-json)\n\n\nThis set of modules provides the following benefits:\n\n* Serialize more datastructures into JSON\n* More flexibility  in what\'s accepted as "JSON"\n* Iterate over massive JSON easily (`mo_json.stream`)\n* Provide a bijection between strictly typed JSON, and dynamic typed JSON.\n\n\n## Recent Changes\n\n* **Version 6.x.x** - Typed encoder no longer encodes to typed multivalues, rather, encodes to array of typed values.  For example, instead of \n\n      {"a": {"~n~": [1, 2]}}\n\n  we get \n      \n      {"a": {"~a~": [{"~n~": 1},{"~n~": 2}]}} \n\n## Usage\n\n### Encode using `__json__`\n\nAdd a `__json__` method to any class you wish to serialize to JSON. It is incumbent on you to ensure valid JSON is emitted:\n\n    class MyClass(object):\n        def __init__(self, a, b):\n            self.a = a\n            self.b = b\n\n        def __json__(self):\n            separator = "{"\n            for k, v in self.__dict__.items():\n                yield separator\n                separator = ","\n                yield value2json(k)+": "+value2json(v)\n            yield "}"\n\nWith the `__json__` function defined, you may use the `value2json` function:\n\n    from mo_json import value2json\n    \n    result = value2json(MyClass(a="name", b=42))    \n\n\n### Encode using `__data__`\n\nAdd a `__data__` method that will convert your class into some JSON-serializable data structures.  You may find this easier to implement than emitting pure JSON.  **If both `__data__` and `__json__` exist, then `__json__` is used.**   \n\n    from mo_json import value2json\n\n    class MyClass(object):\n        def __init__(self, a, b):\n            self.a = a\n            self.b = b\n\n        def __data__(self):\n            return self.__dict__\n   \n    result = value2json(MyClass(a="name", b=42))    \n\n\n### Decoding\n\nThe `json2value` function provides a couple of options\n\n* `flexible` - will be very forgiving of JSON accepted (see [hjson](https://pypi.org/project/hjson/))\n* `leaves` - will interpret keys with dots ("`.`") as dot-delimited paths\n\n\n```\nfrom mo_json import json2value\n\nresult = json2value(\n    "http.headers.referer: http://example.com", \n    flexible=True, \n    leaves=True\n)\nassert result=={\'http\': {\'headers\': {\'referer\': \'http://example.com\'}}}\n```\n \nNotice the lack of quotes in the JSON (hjson) and the deep structure created by the dot-delimited path name\n\n## Running tests\n\n    pip install -r tests/requirements.txt\n    set PYTHONPATH=.    \n    python.exe -m unittest discover tests\n\n\n## Module Details\n\n### Method `mo_json.scrub()`\n\nRemove, or convert, a number of objects from a structure that are not JSON-izable. It is faster to `scrub` and use the default (aka c-based) python encoder than it is to use `default` serializer that forces the use of an interpreted python encoder. \n\n----------------------\n\n### Module `mo_json.stream`\n\nA module that supports queries over very large JSON\nstrings. The overall objective is to make a large JSON document appear like\na hierarchical database, where arrays of any depth, can be queried like\ntables. \n\n\n#### Limitations\n\nThis is not a generic streaming JSON parser. It is only intended to breakdown the top-level array, or object for less memory usage.  \n\n*  **Array values must be the last object property** - If you query into a \n   nested array, all sibling properties found after that array must be ignored \n   (must not be in the `expected_vars`). The code will raise an exception if\n   you can not extract all expected variables.\n\n----------------------\n\n### Method `mo_json.stream.parse()`\n\nWill return an iterator over all objects found in the JSON stream.\n\n**Parameters:**\n\n* **json** - a parameter-less function, when called returns some number of\n  bytes from the JSON stream. It can also be a string.\n* **path** - a dot-delimited string specifying the path to the nested JSON. Use \n  `"."` if your JSON starts with `[`, and is a list.\n* **expected_vars** - a list of strings specifying the full property names \n  required (all other properties are ignored)\n\n#### Common Usage\n\nThe most common use of `parse()` is to iterate over all the objects in a large, top-level, array:\n\n    parse(json, path=".", required_vars=["."]}\n\nFor example, given the following JSON: \n\n    [\n        {"a": 1},\n        {"a": 2},\n        {"a": 3},\n        {"a": 4}\n    ]\n\nreturns a generator that provides\n\n    {"a": 1}\n    {"a": 2}\n    {"a": 3}\n    {"a": 4}\n\n\n#### Examples\n\n**Simple Iteration**\n\n    json = {"b": "done", "a": [1, 2, 3]}\n    parse(json, path="a", required_vars=["a", "b"]}\n\nWe will iterate through the array found on property `a`, and return both `a` and `b` variables. It will return the following values:\n\n    {"b": "done", "a": 1}\n    {"b": "done", "a": 2}\n    {"b": "done", "a": 3}\n\n\n**Bad - Property follows array**\n\nThe same query, but different JSON with `b` following `a`:\n\n    json = {"a": [1, 2, 3], "b": "done"}\n    parse(json, path="a", required_vars=["a", "b"]}\n\nSince property `b` follows the array we\'re iterating over, this will raise an error.\n\n**Good - No need for following properties**\n\nThe same JSON, but different query, which does not require `b`:\n\n    json = {"a": [1, 2, 3], "b": "done"}\n    parse(json, path="a", required_vars=["a"]}\n\nIf we do not require `b`, then streaming will proceed just fine:\n\n    {"a": 1}\n    {"a": 2}\n    {"a": 3}\n\n**Complex Objects**\n\nThis streamer was meant for very long lists of complex objects. Use dot-delimited naming to refer to full name of the property\n\n    json = [{"a": {"b": 1, "c": 2}}, {"a": {"b": 3, "c": 4}}, ...\n    parse(json, path=".", required_vars=["a.c"])\n\nThe dot (`.`) can be used to refer to the top-most array. Notice the structure is maintained, but only includes the required variables.\n\n    {"a": {"c": 2}}\n    {"a": {"c": 4}}\n    ...\n\n**Nested Arrays**\n\nNested array iteration is meant to mimic a left-join from parent to child table;\nas such, it includes every record in the parent. \n\n    json = [\n        {"o": 1: "a": [{"b": 1}: {"b": 2}: {"b": 3}: {"b": 4}]},\n        {"o": 2: "a": {"b": 5}},\n        {"o": 3}\n    ]\n    parse(json, path=[".", "a"], required_vars=["o", "a.b"])\n\nThe `path` parameter can be a list, which is used to indicate which properties\nare expected to have an array, and to iterate over them. Please notice if no\narray is found, it is treated like a singleton array, and missing arrays still\nproduce a result.\n\n    {"o": 1, "a": {"b": 1}}\n    {"o": 1, "a": {"b": 2}}\n    {"o": 1, "a": {"b": 3}}\n    {"o": 1, "a": {"b": 4}}\n    {"o": 2, "a": {"b": 5}}\n    {"o": 3}\n\n**Large top-level objects**\n\nSome JSON is a single large object, rather than an array of objects. In these cases, you can use the `items` operator to iterate through all name/value pairs of an object:\n\n    json = {\n        "a": "test",\n        "b": 2,\n        "c": [1, 2]\n    }\n    parse(json, {"items": "."}, {"name", "value"})   \n\nproduces an iterator of\n\n    {"name": "a", "value": "test"} \n    {"name": "b", "value": 2} \n    {"name": "c", "value": [1,2]} \n\n----------------------\n\n### Module `typed_encoder`\n\n\nOne reason that NoSQL documents stores are wonderful is their schema can automatically expand to accept new properties. Unfortunately, this flexibility is not limitless; A string assigned to property prevents an object being assigned to the same, or visa-versa. This flexibility is under attack by the strict-typing zealots; who, in their self-righteous delusion, believe explicit types are better. They make the lives of humans worse; as we are forced to toil over endless schema modifications.\n\nThis module translates JSON documents into "typed" form; which allows document containers to store both objects and primitives in the same property. This also enables the storage of values with no containing object! \n\nThe typed JSON has a different form than the original, and queries into the document store must take this into account. This conversion is intended to be hidden behind a query abstraction layer that can understand this format.\n\n#### How it works\n\nThere are three main conversions:\n\n1. Primitive values are replaced with single-property objects, where the property name indicates the data type of the value stored:\n   ```\n   {"a": true} -> {"a": {"~b~": true}} \n   {"a": 1   } -> {"a": {"~n~": 1   }} \n   {"a": "1" } -> {"a": {"~s~": "1" }}\n   ```\n2. JSON objects get an additional property, `~e~`, to mark existence. This allows us to query for object existence, and to count the number of objects.\n   ```    \n   {"a": {}} -> {"a": {"~e~": 1}, "~e~": 1}  \n   ```\n3. JSON arrays are contained in a new object, along with `~e~` to count the number of elements in the array:\n   ```    \n   {"a": [1, 2, 3]} -> {"a": {\n       "~e~": 3, \n       "~a~": [\n           {"~n~": 1},\n           {"~n~": 2},\n           {"~n~": 3}\n       ]\n   }}\n   ```\n   Note the sum of `a.~e~` works for both objects and arrays; letting us interpret sub-objects as single-value nested object arrays. \n\n### Function `typed_encode()`\n\nAccepts a `dict`, `list`, or primitive value, and generates the typed JSON that can be inserted into a document store.\n\n### Function `json2typed()`\n\nConverts an existing JSON unicode string and returns the typed JSON unicode string for the same.\n\n\n----------------------\n\n**Update Mar2016** - *PyPy version 5.x appears to have improved C integration to\nthe point that the C library callbacks are no longer a significant overhead:\nThis pure Python JSON encoder is no longer faster than a compound C/Python\nsolution.*\n\nFast JSON encoder used in `convert.value2json()` when running in Pypy. Run the\n[speed test](https://github.com/klahnakoski/mo-json/blob/dev/tests/speedtest_json.py)\nto compare with default implementation and ujson\n\n',
     long_description_content_type='text/markdown',
     name='mo-json',
     packages=["mo_json"],
     url='https://github.com/klahnakoski/mo-json',
-    version='6.603.24115'
+    version='6.605.24115'
 )
```

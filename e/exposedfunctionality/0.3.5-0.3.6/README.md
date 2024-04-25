# Comparing `tmp/exposedfunctionality-0.3.5.tar.gz` & `tmp/exposedfunctionality-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exposedfunctionality-0.3.5.tar", max compression
+gzip compressed data, was "exposedfunctionality-0.3.6.tar", max compression
```

## Comparing `exposedfunctionality-0.3.5.tar` & `exposedfunctionality-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      931 2024-03-22 12:46:05.832207 exposedfunctionality-0.3.5/exposedfunctionality/__init__.py
--rw-r--r--   0        0        0     5931 2024-03-19 11:47:57.200983 exposedfunctionality-0.3.5/exposedfunctionality/func.py
--rw-r--r--   0        0        0      629 2024-03-20 12:35:07.144630 exposedfunctionality-0.3.5/exposedfunctionality/function_parser/__init__.py
--rw-r--r--   0        0        0     5016 2024-03-22 05:24:47.079676 exposedfunctionality-0.3.5/exposedfunctionality/function_parser/custom_wrapper.py
--rw-r--r--   0        0        0    24418 2024-03-19 08:08:29.972664 exposedfunctionality-0.3.5/exposedfunctionality/function_parser/docstring_parser.py
--rw-r--r--   0        0        0    11090 2024-03-19 08:44:57.104823 exposedfunctionality-0.3.5/exposedfunctionality/function_parser/function_parser.py
--rw-r--r--   0        0        0    18389 2024-03-20 12:57:33.116878 exposedfunctionality-0.3.5/exposedfunctionality/function_parser/types.py
--rw-r--r--   0        0        0      260 2023-10-24 07:15:20.622816 exposedfunctionality-0.3.5/exposedfunctionality/variables/__init__.py
--rw-r--r--   0        0        0    10652 2024-03-19 11:01:14.319146 exposedfunctionality-0.3.5/exposedfunctionality/variables/core.py
--rw-r--r--   0        0        0     1215 2023-12-19 07:09:00.926530 exposedfunctionality-0.3.5/exposedfunctionality/variables/middleware.py
--rw-r--r--   0        0        0     1091 2023-10-11 14:22:00.855154 exposedfunctionality-0.3.5/LICENSE
--rw-r--r--   0        0        0      489 2024-03-22 12:45:54.975789 exposedfunctionality-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5676 2024-03-19 11:47:33.563917 exposedfunctionality-0.3.5/README.md
--rw-r--r--   0        0        0     6276 1970-01-01 00:00:00.000000 exposedfunctionality-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      931 2024-04-25 13:24:56.006291 exposedfunctionality-0.3.6/exposedfunctionality/__init__.py
+-rw-r--r--   0        0        0     5931 2024-03-19 11:47:57.200983 exposedfunctionality-0.3.6/exposedfunctionality/func.py
+-rw-r--r--   0        0        0      629 2024-03-20 12:35:07.144630 exposedfunctionality-0.3.6/exposedfunctionality/function_parser/__init__.py
+-rw-r--r--   0        0        0     5016 2024-03-22 05:24:47.079676 exposedfunctionality-0.3.6/exposedfunctionality/function_parser/custom_wrapper.py
+-rw-r--r--   0        0        0    24418 2024-03-19 08:08:29.972664 exposedfunctionality-0.3.6/exposedfunctionality/function_parser/docstring_parser.py
+-rw-r--r--   0        0        0    11090 2024-03-19 08:44:57.104823 exposedfunctionality-0.3.6/exposedfunctionality/function_parser/function_parser.py
+-rw-r--r--   0        0        0    18381 2024-04-25 13:24:34.472882 exposedfunctionality-0.3.6/exposedfunctionality/function_parser/types.py
+-rw-r--r--   0        0        0      260 2023-10-24 07:15:20.622816 exposedfunctionality-0.3.6/exposedfunctionality/variables/__init__.py
+-rw-r--r--   0        0        0    10652 2024-03-19 11:01:14.319146 exposedfunctionality-0.3.6/exposedfunctionality/variables/core.py
+-rw-r--r--   0        0        0     1215 2023-12-19 07:09:00.926530 exposedfunctionality-0.3.6/exposedfunctionality/variables/middleware.py
+-rw-r--r--   0        0        0     1091 2023-10-11 14:22:00.855154 exposedfunctionality-0.3.6/LICENSE
+-rw-r--r--   0        0        0      489 2024-04-25 13:24:50.497021 exposedfunctionality-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5676 2024-03-19 11:47:33.563917 exposedfunctionality-0.3.6/README.md
+-rw-r--r--   0        0        0     6327 1970-01-01 00:00:00.000000 exposedfunctionality-0.3.6/PKG-INFO
```

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/__init__.py` & `exposedfunctionality-0.3.6/exposedfunctionality/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from . import function_parser
 from .variables import ExposedValue, add_exposed_value, get_exposed_values
 from . import func
 
 from .function_parser.custom_wrapper import controlled_wrapper, update_wrapper
 from .function_parser import serialize_type
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 
 __all__ = [
     "function_parser",
     "ExposedValue",
     "variables",
     "add_exposed_value",
     "get_exposed_values",
```

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/func.py` & `exposedfunctionality-0.3.6/exposedfunctionality/func.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/function_parser/__init__.py` & `exposedfunctionality-0.3.6/exposedfunctionality/function_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/function_parser/custom_wrapper.py` & `exposedfunctionality-0.3.6/exposedfunctionality/function_parser/custom_wrapper.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/function_parser/docstring_parser.py` & `exposedfunctionality-0.3.6/exposedfunctionality/function_parser/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/function_parser/function_parser.py` & `exposedfunctionality-0.3.6/exposedfunctionality/function_parser/function_parser.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/function_parser/types.py` & `exposedfunctionality-0.3.6/exposedfunctionality/function_parser/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
             elif origin in [dict, Dict]:
                 key_type = type_to_string(t.__args__[0])
                 value_type = type_to_string(t.__args__[1])
                 return f"Dict[{key_type}, {value_type}]"
             elif origin in [tuple, Tuple]:
                 return f"Tuple[{', '.join([type_to_string(subtype) for subtype in t.__args__])}]"
             elif origin is Union:
-                return f"Union[{', '.join(sorted([type_to_string(subtype) for subtype in t.__args__]))}]"
+                return f"Union[{', '.join([type_to_string(subtype) for subtype in t.__args__])}]"
             elif origin in [Type, type]:
                 if hasattr(t, "__args__"):
                     return f"Type[{type_to_string(t.__args__[0])}]"
                 # else: already handeld by the simple "Type" entry
                 #    return "Type"
             elif origin in [set, Set]:
                 return f"Set[{type_to_string(t.__args__[0])}]"
```

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/variables/core.py` & `exposedfunctionality-0.3.6/exposedfunctionality/variables/core.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/exposedfunctionality/variables/middleware.py` & `exposedfunctionality-0.3.6/exposedfunctionality/variables/middleware.py`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/LICENSE` & `exposedfunctionality-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/README.md` & `exposedfunctionality-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `exposedfunctionality-0.3.5/PKG-INFO` & `exposedfunctionality-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: exposedfunctionality
-Version: 0.3.5
+Version: 0.3.6
 Summary: tool to expose functionalities to multiple tools
 License: MIT
 Author: Julian Kimmig
 Author-email: julian.kimmig@linkdlab.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # ExposedFunctionality
 
 ExposedFunctionality is a Python library designed to facilitate the interaction between backend code and frontend interfaces. It enables developers to expose backend methods and variables in a structured and secure way, making it easier to integrate with front-end systems or API endpoints. This library is particularly useful in scenarios where backend logic needs to be accessed or manipulated from a front-end application or through web API calls.
```


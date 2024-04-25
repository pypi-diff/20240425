# Comparing `tmp/graphene_django_extended-1.0.2.tar.gz` & `tmp/graphene_django_extended-1.1.0.tar.gz`

## Comparing `graphene_django_extended-1.0.2.tar` & `graphene_django_extended-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/__init__.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/connection.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/converter.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/interface.py
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/mutation.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/Pipfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/delete_mutation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/fields.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/global_id_serializer_mutation.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/inputs.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/model_mutation.py
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/_mutations/mutations.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/search/__init__.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/search/connection.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/search/field.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/search/node.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/search/types.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/graphene_django_extended/tests/test_interface.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/.gitignore
--rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/LICENSE
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 graphene_django_extended-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/__init__.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/connection.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/converter.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/interface.py
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/mutation.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/Pipfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/delete_mutation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/fields.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/global_id_serializer_mutation.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/inputs.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/model_mutation.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/_mutations/mutations.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/search/__init__.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/search/connection.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/search/field.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/search/node.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/search/types.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/graphene_django_extended/tests/test_interface.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/.gitignore
+-rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/LICENSE
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 graphene_django_extended-1.1.0/PKG-INFO
```

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/connection.py` & `graphene_django_extended-1.1.0/graphene_django_extended/connection.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/converter.py` & `graphene_django_extended-1.1.0/graphene_django_extended/converter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/interface.py` & `graphene_django_extended-1.1.0/graphene_django_extended/interface.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/mutation.py` & `graphene_django_extended-1.1.0/graphene_django_extended/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/_mutations/delete_mutation.py` & `graphene_django_extended-1.1.0/graphene_django_extended/_mutations/delete_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/_mutations/global_id_serializer_mutation.py` & `graphene_django_extended-1.1.0/graphene_django_extended/_mutations/global_id_serializer_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/_mutations/model_mutation.py` & `graphene_django_extended-1.1.0/graphene_django_extended/_mutations/model_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/_mutations/mutations.py` & `graphene_django_extended-1.1.0/graphene_django_extended/_mutations/mutations.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/search/connection.py` & `graphene_django_extended-1.1.0/graphene_django_extended/search/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import graphene
 from django.db.models import Q
-from graphene_django.fields import DjangoConnectionField
+
+# from graphene_django.fields import DjangoConnectionField
 from graphene_django.filter import DjangoFilterConnectionField
 
 from ..connection import DjangoInterfaceConnectionField
 
 
 class SearchDjangoConnectionFieldMixin:
     def __init__(self, type_, *args, **kwargs):
@@ -30,16 +31,16 @@
             query = queries.pop()
             for item in queries:
                 query |= item
             return queryset.filter(query)
         return queryset
 
     @classmethod
-    def resolve_queryset(cls, connection, iterable, info, args):
-        queryset = super().resolve_queryset(connection, iterable, info, args)
+    def resolve_queryset(cls, connection, iterable, info, args, **kwargs):
+        queryset = super().resolve_queryset(connection, iterable, info, args, **kwargs)
         print("CN", info, info.context, args, cls)
 
         node_type = connection._meta.node
         # Apply search filter if 'search' argument is provided and 'search_fields' are defined
         if (
             "search" in args
             and hasattr(node_type, "_meta")
@@ -49,15 +50,15 @@
             search_fields = node_type._meta.search_fields
             queryset = cls.merge_querystrings(queryset, search_value, search_fields)
 
         return queryset
 
 
 class SearchDjangoConnectionField(
-    SearchDjangoConnectionFieldMixin, DjangoConnectionField
+    SearchDjangoConnectionFieldMixin, DjangoFilterConnectionField
 ):
     """
     Extension of DjangoFilterConnectionField to include search functionality
     based on a predefined list of searchable fields.
     """
```

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/search/field.py` & `graphene_django_extended-1.1.0/graphene_django_extended/search/field.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/search/node.py` & `graphene_django_extended-1.1.0/graphene_django_extended/search/node.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/search/types.py` & `graphene_django_extended-1.1.0/graphene_django_extended/search/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/graphene_django_extended/tests/test_interface.py` & `graphene_django_extended-1.1.0/graphene_django_extended/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/LICENSE` & `graphene_django_extended-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.0.2/pyproject.toml` & `graphene_django_extended-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphene-django-extended"
-version = "1.0.2"
+version = "1.1.0"
 #authors = [
 #  { name="Example Author", email="author@example.com" },
 #]
 description = "A collection of utility classes to extend the base functionality of graphene_django"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `graphene_django_extended-1.0.2/PKG-INFO` & `graphene_django_extended-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.3
 Name: graphene-django-extended
-Version: 1.0.2
+Version: 1.1.0
 Summary: A collection of utility classes to extend the base functionality of graphene_django
 Project-URL: Homepage, https://github.com/AztlanEngineering/graphene-django-extended
 Project-URL: Issues, https://github.com/AztlanEngineering/graphene-django-extended/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-CAVEATS 
+
+## CAVEATS 
 - No tests for now 
 - Stubs are missing for graphene and graphene-django
 - Unstable API - needs more usage
+- Version 1.0.2 is the most stable
+- Version 1.1 includes filtering capabilities (from DjangoFilterConnectionField), which is NOT an opt-in. It requires all Nodes to have filter_fields defined. It might also break the DjangoInterface, untested yet.
 
-TODO
+## TODO
 - Make sure Sphinx generates docs from all files
 - generate html instead of md ???
 - add general introduction and usage guide on the docs
 
-Build
+## Build
 `hatch build` or `python -m hatch build`
 `hatch publish` or `python -m hatch publish` with username `__token__`. Make sure the [keyrings backend](https://github.com/jaraco/keyrings.alt) is installed. 
 On arch `pacman -S python-hatch python-keyrings-alt`, publish with `username:__token__`
 The default keyring is located at `~/.local/share/python_keyring/` and uses the name "main". Again this is not a recommended implementation, just a quick and dirty keyring usage
```


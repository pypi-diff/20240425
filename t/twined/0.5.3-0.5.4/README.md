# Comparing `tmp/twined-0.5.3.tar.gz` & `tmp/twined-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twined-0.5.3.tar", last modified: Thu Oct 19 16:17:47 2023, max compression
+gzip compressed data, was "twined-0.5.4.tar", last modified: Thu Apr 25 15:59:06 2024, max compression
```

## Comparing `twined-0.5.3.tar` & `twined-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.190711 twined-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-10-19 16:17:44.000000 twined-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-19 16:17:44.000000 twined-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2023-10-19 16:17:47.190711 twined-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-10-19 16:17:44.000000 twined-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-19 16:17:47.190711 twined-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-10-19 16:17:44.000000 twined-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.186711 twined-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12327 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_manifest_strands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_monitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_schema_strands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_twine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2023-10-19 16:17:44.000000 twined-0.5.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.186711 twined-0.5.3/twined/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-19 16:17:44.000000 twined-0.5.3/twined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-10-19 16:17:44.000000 twined-0.5.3/twined/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.186711 twined-0.5.3/twined/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-19 16:17:44.000000 twined-0.5.3/twined/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.190711 twined-0.5.3/twined/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-10-19 16:17:44.000000 twined-0.5.3/twined/schema/children_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-10-19 16:17:44.000000 twined-0.5.3/twined/schema/manifest_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)  2174030 2023-10-19 16:17:44.000000 twined-0.5.3/twined/schema/plotly_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2023-10-19 16:17:44.000000 twined-0.5.3/twined/schema/twine_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    18315 2023-10-19 16:17:44.000000 twined-0.5.3/twined/twine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.190711 twined-0.5.3/twined/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-10-19 16:17:44.000000 twined-0.5.3/twined/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-10-19 16:17:44.000000 twined-0.5.3/twined/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-10-19 16:17:44.000000 twined-0.5.3/twined/utils/load_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-19 16:17:44.000000 twined-0.5.3/twined/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:17:47.186711 twined-0.5.3/twined.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2023-10-19 16:17:47.000000 twined-0.5.3/twined.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-19 16:17:47.000000 twined-0.5.3/twined.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 16:17:47.000000 twined-0.5.3/twined.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-19 16:17:47.000000 twined-0.5.3/twined.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-19 16:17:47.000000 twined-0.5.3/twined.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 15:59:04.000000 twined-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-25 15:59:04.000000 twined-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-25 15:59:06.823912 twined-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-25 15:59:04.000000 twined-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 15:59:06.823912 twined-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 15:59:04.000000 twined-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.819912 twined-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_manifest_strands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_schema_strands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_twine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-25 15:59:04.000000 twined-0.5.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.819912 twined-0.5.4/twined/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 15:59:04.000000 twined-0.5.4/twined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-25 15:59:04.000000 twined-0.5.4/twined/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.819912 twined-0.5.4/twined/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-25 15:59:04.000000 twined-0.5.4/twined/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/twined/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:04.000000 twined-0.5.4/twined/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2174030 2024-04-25 15:59:04.000000 twined-0.5.4/twined/schema/plotly_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-25 15:59:04.000000 twined-0.5.4/twined/schema/twine_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-25 15:59:04.000000 twined-0.5.4/twined/twine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/twined/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 15:59:04.000000 twined-0.5.4/twined/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:59:06.823912 twined-0.5.4/twined.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:59:06.000000 twined-0.5.4/twined.egg-info/top_level.txt
```

### Comparing `twined-0.5.3/LICENSE` & `twined-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/PKG-INFO` & `twined-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: twined
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library to help digital twins and data services talk to one another
 Home-page: https://www.github.com/octue/twined
 Author: Octue (github: octue)
 License: MIT
 Keywords: digital,twins,data,services,python,schema
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonschema~=4.4.0
 Requires-Dist: python-dotenv
```

### Comparing `twined-0.5.3/README.md` & `twined-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/setup.cfg` & `twined-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/setup.py` & `twined-0.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     readme_text = f.read()
 
 with open("LICENSE") as f:
     license_text = f.read()
 
 setup(
     name="twined",
-    version="0.5.3",
+    version="0.5.4",
     py_modules=[],
     install_requires=["jsonschema ~= 4.4.0", "python-dotenv"],
     url="https://www.github.com/octue/twined",
     license="MIT",
     author="Octue (github: octue)",
     description="A library to help digital twins and data services talk to one another",
     long_description=readme_text,
@@ -29,12 +29,13 @@
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     keywords=["digital", "twins", "data", "services", "python", "schema"],
 )
```

### Comparing `twined-0.5.3/tests/test_children.py` & `twined-0.5.4/tests/test_children.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import unittest
 
 from twined import Twine, exceptions
 from .base import BaseTestCase
 
 
 class TestChildrenTwine(BaseTestCase):
-    """Tests related to the twine itself - ensuring that valid and invalid
-    `children` entries in a twine file work as expected
-    """
+    """Tests ensuring that valid and invalid `children` entries in a twine file work as expected."""
 
     def test_invalid_children_dict_not_array(self):
-        """Ensures InvalidTwine exceptions are raised when instantiating twines where `children` entry is incorrectly
-        specified as a dict, not an array
+        """Ensure that `InvalidTwine` exceptions are raised when instantiating twines where `children` entry is
+        incorrectly specified as a dict, not an array.
         """
         with self.assertRaises(exceptions.InvalidTwine):
             Twine(source="""{"children": {}}""")
 
     def test_invalid_children_no_key(self):
-        """Ensures InvalidTwine exceptions are raised when instantiating twines where a child
-        is specified without the required `key` field
+        """Ensure that `InvalidTwine` exceptions are raised when instantiating twines where a child is specified without
+        the required `key` field.
         """
         source = """
             {
-                "children": [{"purpose": "The purpose.", "notes": "Here are some notes.", "filters": "tags:gis"}]
+                "children": [{"purpose": "The purpose.", "notes": "Here are some notes."}]
             }
         """
 
         with self.assertRaises(exceptions.InvalidTwine):
             Twine(source=source)
 
     def test_valid_children(self):
         """Ensures that a twine with one child can be instantiated correctly."""
         source = """
             {
-                "children": [{"key": "gis", "purpose": "The purpose.", "notes": "Some notes.", "filters": "tags:gis"}]
+                "children": [{"key": "gis", "purpose": "The purpose.", "notes": "Some notes."}]
             }
         """
         self.assertEqual(len(Twine(source=source).children), 1)
 
     def test_empty_children(self):
         """Ensures that a twine file will validate with an empty list object as children"""
         twine = Twine(source="""{"children": []}""")
@@ -45,15 +43,15 @@
 
 
 class TestChildrenValidation(BaseTestCase):
     """Tests related to whether validation of children occurs successfully (given a valid twine)"""
 
     VALID_TWINE_WITH_CHILDREN = """
         {
-            "children": [{"key": "gis", "purpose": "The purpose", "notes": "Some notes.", "filters": "tags:gis"}]
+            "children": [{"key": "gis", "purpose": "The purpose", "notes": "Some notes."}]
         }
     """
 
     VALID_CHILD_VALUE = """
         [
             {
                 "key": "gis",
```

### Comparing `twined-0.5.3/tests/test_credentials.py` & `twined-0.5.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/tests/test_manifest_strands.py` & `twined-0.5.4/tests/test_manifest_strands.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/tests/test_monitors.py` & `twined-0.5.4/tests/test_monitors.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/tests/test_schema_strands.py` & `twined-0.5.4/tests/test_schema_strands.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/tests/test_twine.py` & `twined-0.5.4/tests/test_twine.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/tests/test_utils.py` & `twined-0.5.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/twined/exceptions.py` & `twined-0.5.4/twined/exceptions.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/twined/schema/plotly_schema.json` & `twined-0.5.4/twined/schema/plotly_schema.json`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/twined/schema/twine_schema.json` & `twined-0.5.4/twined/schema/twine_schema.json`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/twined/twine.py` & `twined-0.5.4/twined/twine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+import importlib.metadata
 import json as jsonlib
 import logging
 import os
-import pkg_resources
 from dotenv import load_dotenv
 from jsonschema import ValidationError, validate as jsonschema_validate
 
+
+try:
+    # python < 3.9
+    import importlib_resources
+except ModuleNotFoundError:
+    # python >= 3.9
+    import importlib.resources as importlib_resources
+
 from . import exceptions
 from .utils import load_json, trim_suffix
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -28,14 +36,18 @@
     *SCHEMA_STRANDS,
     *MANIFEST_STRANDS,
     *CREDENTIAL_STRANDS,
     *CHILDREN_STRANDS,
 )
 
 
+CHILDREN_SCHEMA = "https://jsonschema.registry.octue.com/octue/children/0.1.0.json"
+MANIFEST_SCHEMA = "https://jsonschema.registry.octue.com/octue/manifest/0.1.0.json"
+
+
 class Twine:
     """Twine class manages validation of inputs and outputs to/from a data service, based on spec in a 'twine' file.
 
     Instantiate a Twine by providing a file name or a utf-8 encoded string containing valid json.
     The twine is itself validated to be correct on instantiation of Twine().
 
     Note: Instantiating the twine does not validate that any inputs to an application are correct - it merely
@@ -88,41 +100,40 @@
 
         :param str strand:
         :return dict:
         """
         if strand == "twine":
             # The data is a twine. A twine *contains* schema, but we also need to verify that it matches a certain
             # schema itself. The twine schema is distributed with this packaged to ensure version consistency...
-            schema_path = "schema/twine_schema.json"
+            return jsonlib.loads(
+                importlib_resources.files("twined.schema").joinpath("twine_schema.json").read_text(encoding="utf-8")
+            )
 
-        elif strand in CHILDREN_STRANDS:
+        if strand in CHILDREN_STRANDS:
             # The data is a list of children. The "children" strand of the twine describes matching criteria for
             # the children, not the schema of the "children" data, which is distributed with this package to ensure
             # version consistency...
-            schema_path = "schema/children_schema.json"
+            return {"$ref": CHILDREN_SCHEMA}
 
-        elif strand in MANIFEST_STRANDS:
+        if strand in MANIFEST_STRANDS:
             # The data is a manifest of files. The "*_manifest" strands of the twine describe matching criteria used to
             # filter files appropriate for consumption by the digital twin, not the schema of the manifest data, which
             # is distributed with this package to ensure version consistency...
-            schema_path = "schema/manifest_schema.json"
-
-        else:
-            if strand not in SCHEMA_STRANDS:
-                raise exceptions.UnknownStrand(f"Unknown strand {strand}. Try one of {ALL_STRANDS}.")
+            return {"$ref": MANIFEST_SCHEMA}
 
-            # Get schema from twine.json file.
-            schema_key = strand + "_schema"
+        if strand not in SCHEMA_STRANDS:
+            raise exceptions.UnknownStrand(f"Unknown strand {strand}. Try one of {ALL_STRANDS}.")
 
-            try:
-                return getattr(self, schema_key)
-            except AttributeError:
-                raise exceptions.StrandNotFound(f"Cannot validate - no {schema_key} strand in the twine")
+        # Get schema from twine.json file.
+        schema_key = strand + "_schema"
 
-        return jsonlib.loads(pkg_resources.resource_string("twined", schema_path))
+        try:
+            return getattr(self, schema_key)
+        except AttributeError:
+            raise exceptions.StrandNotFound(f"Cannot validate - no {schema_key} strand in the twine")
 
     def _validate_against_schema(self, strand, data):
         """Validate data against a schema, raises exceptions of type Invalid<strand>Json if not compliant.
 
         Can be used to validate:
             - the twine file contents itself against the present version twine spec
             - children data against the required schema for the present version twine spec
@@ -139,15 +150,15 @@
             logger.debug("Validated %s against schema", strand)
 
         except ValidationError as e:
             raise exceptions.invalid_contents_map[strand](str(e))
 
     def _validate_twine_version(self, twine_file_twined_version):
         """Validate that the installed version is consistent with an optional version specification in the twine file."""
-        installed_twined_version = pkg_resources.get_distribution("twined").version
+        installed_twined_version = importlib.metadata.version("twined")
         logger.debug(
             "Twine versions... %s installed, %s specified in twine", installed_twined_version, twine_file_twined_version
         )
         if (twine_file_twined_version is not None) and (installed_twined_version != twine_file_twined_version):
             raise exceptions.TwineVersionConflict(
                 f"Twined library version conflict. Twine file requires {twine_file_twined_version} but you have {installed_twined_version} installed"
             )
```

### Comparing `twined-0.5.3/twined/utils/encoders.py` & `twined-0.5.4/twined/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/twined/utils/load_json.py` & `twined-0.5.4/twined/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `twined-0.5.3/twined.egg-info/PKG-INFO` & `twined-0.5.4/twined.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: twined
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library to help digital twins and data services talk to one another
 Home-page: https://www.github.com/octue/twined
 Author: Octue (github: octue)
 License: MIT
 Keywords: digital,twins,data,services,python,schema
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsonschema~=4.4.0
 Requires-Dist: python-dotenv
```

### Comparing `twined-0.5.3/twined.egg-info/SOURCES.txt` & `twined-0.5.4/twined.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 twined/twine.py
 twined.egg-info/PKG-INFO
 twined.egg-info/SOURCES.txt
 twined.egg-info/dependency_links.txt
 twined.egg-info/requires.txt
 twined.egg-info/top_level.txt
 twined/migrations/__init__.py
-twined/schema/children_schema.json
-twined/schema/manifest_schema.json
+twined/schema/__init__.py
 twined/schema/plotly_schema.json
 twined/schema/twine_schema.json
 twined/utils/__init__.py
 twined/utils/encoders.py
 twined/utils/load_json.py
 twined/utils/strings.py
```


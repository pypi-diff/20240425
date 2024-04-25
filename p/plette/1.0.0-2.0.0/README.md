# Comparing `tmp/plette-1.0.0.tar.gz` & `tmp/plette-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plette-1.0.0.tar", last modified: Sun Feb  4 16:17:13 2024, max compression
+gzip compressed data, was "plette-2.0.0.tar", last modified: Thu Apr 25 07:34:42 2024, max compression
```

## Comparing `plette-1.0.0.tar` & `plette-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 16:17:13.707377 plette-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-04 16:16:56.000000 plette-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-04 16:16:56.000000 plette-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-04 16:17:13.707377 plette-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-04 16:16:56.000000 plette-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-04 16:16:56.000000 plette-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-04 16:17:13.707377 plette-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-04 16:16:56.000000 plette-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 16:17:13.703377 plette-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 16:17:13.703377 plette-1.0.0/src/plette/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-04 16:16:56.000000 plette-1.0.0/src/plette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-04 16:16:56.000000 plette-1.0.0/src/plette/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-02-04 16:16:56.000000 plette-1.0.0/src/plette/lockfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-02-04 16:16:56.000000 plette-1.0.0/src/plette/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-02-04 16:16:56.000000 plette-1.0.0/src/plette/pipfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 16:17:13.707377 plette-1.0.0/src/plette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-04 16:17:13.000000 plette-1.0.0/src/plette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-04 16:17:13.000000 plette-1.0.0/src/plette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 16:17:13.000000 plette-1.0.0/src/plette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-04 16:17:13.000000 plette-1.0.0/src/plette.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-04 16:17:13.000000 plette-1.0.0/src/plette.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 16:17:01.000000 plette-1.0.0/src/plette.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 16:17:13.707377 plette-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_lockfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_models_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_models_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_models_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_models_requires.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_models_sourcecollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_models_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_pipfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-04 16:16:56.000000 plette-1.0.0/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.751733 plette-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 07:34:29.000000 plette-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 07:34:29.000000 plette-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 07:34:42.751733 plette-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 07:34:29.000000 plette-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 07:34:29.000000 plette-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 07:34:42.751733 plette-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 07:34:29.000000 plette-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.743733 plette-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.747733 plette-2.0.0/src/plette/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/lockfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.747733 plette-2.0.0/src/plette/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-25 07:34:29.000000 plette-2.0.0/src/plette/pipfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.751733 plette-2.0.0/src/plette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 07:34:42.000000 plette-2.0.0/src/plette.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:34:33.000000 plette-2.0.0/src/plette.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:34:42.747733 plette-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_lockfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_pipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-25 07:34:29.000000 plette-2.0.0/tests/test_scripts.py
```

### Comparing `plette-1.0.0/LICENSE` & `plette-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plette-1.0.0/PKG-INFO` & `plette-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plette
-Version: 1.0.0
+Version: 2.0.0
 Summary: Structured Pipfile and Pipfile.lock models.
 Author-email: Tzu-ping Chung <uranusjr@gmail.com>
 License: ISC License
 Project-URL: Homepage, https://github.com/sarugaku/plette
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `plette-1.0.0/README.rst` & `plette-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plette-1.0.0/pyproject.toml` & `plette-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plette-1.0.0/src/plette/__main__.py` & `plette-2.0.0/src/plette/__main__.py`

 * *Files identical despite different names*

### Comparing `plette-1.0.0/src/plette/lockfiles.py` & `plette-2.0.0/src/plette/lockfiles.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,45 @@
-# pylint: disable=missing-module-docstring,missing-class-docstring
-# pylint: disable=missing-function-docstring
-# pylint: disable=no-member
-
-import dataclasses
 import json
 import numbers
 
 import collections.abc as collections_abc
 
-from dataclasses import dataclass, field, asdict
-from typing import Optional
 
-from .models import BaseModel, Meta, PackageCollection, Package, remove_empty_values
+from .models import DataModel, Meta, PackageCollection
 
-PIPFILE_SPEC_CURRENT = 6
 
+class _LockFileEncoder(json.JSONEncoder):
+    """A specilized JSON encoder to convert loaded data into a lock file.
 
-def flatten_versions(d):
-    copy = {}
-    # Iterate over a copy of the dictionary
-    for key, value in d.items():
-        # If the key is "version", replace the key with the value
-        copy[key] = value["version"]
-    return copy
-
-
-class DCJSONEncoder(json.JSONEncoder):
-    def default(self, o):
-        if dataclasses.is_dataclass(o):
-            o = dataclasses.asdict(o)
-            if "_meta" in o:
-                o["_meta"]["pipfile-spec"] = o["_meta"].pop("pipfile_spec")
-                o["_meta"]["hash"] = {o["_meta"]["hash"]["name"]: o["_meta"]["hash"]["value"]}
-                o["_meta"]["sources"] = o["_meta"]["sources"].pop("sources")
-
-            remove_empty_values(o)
-
-            for section in ["default", "develop"]:
-                try:
-                    o[section] = flatten_versions(o[section])
-                except KeyError:
-                    continue
-            # add silly default values
-            if "develop" not in o:
-                o["develop"] = {}
-            if "requires" not in o["_meta"]:
-                o["_meta"]["requires"] = {}
-            return o
-        return super().default(o)
+    This adds a few characteristics to the encoder:
+
+    * The JSON is always prettified with indents and spaces.
+    * The output is always UTF-8-encoded text, never binary, even on Python 2.
+    """
+    def __init__(self):
+        super(_LockFileEncoder, self).__init__(
+            indent=4, separators=(",", ": "), sort_keys=True,
+        )
+
+    def encode(self, obj):
+        content = super(_LockFileEncoder, self).encode(obj)
+        if not isinstance(content, str):
+            content = content.decode("utf-8")
+        content += "\n"
+        return content
+
+    def iterencode(self, obj):
+        for chunk in super(_LockFileEncoder, self).iterencode(obj):
+            if not isinstance(chunk, str):
+                chunk = chunk.decode("utf-8")
+            yield chunk
+        yield "\n"
+
+
+PIPFILE_SPEC_CURRENT = 6
 
 
 def _copy_jsonsafe(value):
     """Deep-copy a value into JSON-safe types.
     """
     if isinstance(value, (str, numbers.Number)):
         return value
@@ -60,103 +48,130 @@
     if isinstance(value, collections_abc.Iterable):
         return [_copy_jsonsafe(v) for v in value]
     if value is None:   # This doesn't happen often for us.
         return None
     return str(value)
 
 
-@dataclass
-class Lockfile(BaseModel):
-    """Representation of a Pipfile.lock."""
-
-    _meta: Optional[Meta]
-    default: Optional[dict] =  field(default_factory=dict)
-    develop: Optional[dict] = field(default_factory=dict)
-
-    def __post_init__(self):
-        """Run validation methods if declared.
-        The validation method can be a simple check
-        that raises ValueError or a transformation to
-        the field value.
-        The validation is performed by calling a function named:
-            `validate_<field_name>(self, value) -> field.type`
-        """
-        super().__post_init__()
-        self.meta = self._meta
-
-    def validate__meta(self, value):
-        return self.validate_meta(value)
-
-    def validate_meta(self, value):
-        if "_meta" in value:
-            value = value["_meta"]
-        if 'pipfile-spec' in value:
-            value['pipfile_spec'] = value.pop('pipfile-spec')
-        return Meta(**value)
-
-    def validate_default(self, value):
-        packages = {}
-        for name, spec in value.items():
-            packages[name] = Package(spec)
-        return packages
+class Lockfile(DataModel):
+    """Representation of a Pipfile.lock.
+    """
+    __SCHEMA__ = {
+        "_meta": {"type": "dict", "required": True},
+        "default": {"type": "dict", "required": True},
+        "develop": {"type": "dict", "required": True},
+    }
+
+    @classmethod
+    def validate(cls, data):
+        for key, value in data.items():
+            if key == "_meta":
+                Meta.validate(value)
+            else:
+                PackageCollection.validate(value)
 
     @classmethod
-    def load(cls, fh, encoding=None):
+    def load(cls, f, encoding=None):
         if encoding is None:
-            data = json.load(fh)
+            data = json.load(f)
         else:
-            data = json.loads(fh.read().decode(encoding))
-        return cls(**data)
+            data = json.loads(f.read().decode(encoding))
+        return cls(data)
 
     @classmethod
     def with_meta_from(cls, pipfile, categories=None):
         data = {
             "_meta": {
-                "hash": pipfile.get_hash().__dict__,
+                "hash": _copy_jsonsafe(pipfile.get_hash()._data),
                 "pipfile-spec": PIPFILE_SPEC_CURRENT,
-                "requires": _copy_jsonsafe(getattr(pipfile, "requires", {})),
+                "requires": _copy_jsonsafe(pipfile._data.get("requires", {})),
+                "sources": _copy_jsonsafe(pipfile.sources._data),
             },
         }
-
-        data["_meta"].update(asdict(pipfile.sources))
-
         if categories is None:
-            data["default"] = _copy_jsonsafe(getattr(pipfile, "packages", {}))
-            data["develop"] = _copy_jsonsafe(getattr(pipfile, "dev-packages", {}))
+            data["default"] = _copy_jsonsafe(pipfile._data.get("packages", {}))
+            data["develop"] = _copy_jsonsafe(pipfile._data.get("dev-packages", {}))
         else:
             for category in categories:
-                if category in ["default", "packages"]:
-                    data["default"] = _copy_jsonsafe(getattr(pipfile,"packages", {}))
-                elif category in ["develop", "dev-packages"]:
-                    data["develop"] = _copy_jsonsafe(
-                            getattr(pipfile,"dev-packages", {}))
+                if category == "default" or category == "packages":
+                    data["default"] = _copy_jsonsafe(pipfile._data.get("packages", {}))
+                elif category == "develop" or category == "dev-packages":
+                    data["develop"] = _copy_jsonsafe(pipfile._data.get("dev-packages", {}))
                 else:
-                    data[category] = _copy_jsonsafe(getattr(pipfile, category, {}))
+                    data[category] = _copy_jsonsafe(pipfile._data.get(category, {}))
         if "default" not in data:
-            data["default"] = {}
+            data["default"]  = {}
         if "develop" not in data:
             data["develop"] = {}
         return cls(data)
 
     def __getitem__(self, key):
-        value = self[key]
+        value = self._data[key]
         try:
             if key == "_meta":
-                return Meta(**value)
-            return PackageCollection(value)
+                return Meta(value)
+            else:
+                return PackageCollection(value)
         except KeyError:
             return value
 
+    def __setitem__(self, key, value):
+        if isinstance(value, DataView):
+            self._data[key] = value._data
+        else:
+            self._data[key] = value
+
     def is_up_to_date(self, pipfile):
         return self.meta.hash == pipfile.get_hash()
 
-    def dump(self, fh):
-        json.dump(self, fh, cls=DCJSONEncoder)
-        self.meta = self._meta
+    def dump(self, f, encoding=None):
+        encoder = _LockFileEncoder()
+        if encoding is None:
+            for chunk in encoder.iterencode(self._data):
+                f.write(chunk)
+        else:
+            content = encoder.encode(self._data)
+            f.write(content.encode(encoding))
 
     @property
     def meta(self):
-        return self._meta
+        try:
+            return self["_meta"]
+        except KeyError:
+            raise AttributeError("meta")
 
     @meta.setter
     def meta(self, value):
-        self._meta = value
+        self["_meta"] = value
+
+    @property
+    def _meta(self):
+        try:
+            return self["_meta"]
+        except KeyError:
+            raise AttributeError("meta")
+
+    @_meta.setter
+    def _meta(self, value):
+        self["_meta"] = value
+
+    @property
+    def default(self):
+        try:
+            return self["default"]
+        except KeyError:
+            raise AttributeError("default")
+
+    @default.setter
+    def default(self, value):
+        self["default"] = value
+
+    @property
+    def develop(self):
+        try:
+            return self["develop"]
+        except KeyError:
+            raise AttributeError("develop")
+
+    @develop.setter
+    def develop(self, value):
+        self["develop"] = value
```

### Comparing `plette-1.0.0/src/plette.egg-info/PKG-INFO` & `plette-2.0.0/src/plette.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plette
-Version: 1.0.0
+Version: 2.0.0
 Summary: Structured Pipfile and Pipfile.lock models.
 Author-email: Tzu-ping Chung <uranusjr@gmail.com>
 License: ISC License
 Project-URL: Homepage, https://github.com/sarugaku/plette
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `plette-1.0.0/tests/test_lockfiles.py` & `plette-2.0.0/tests/test_lockfiles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# pylint: disable=missing-module-docstring,missing-class-docstring
-# pylint: disable=missing-function-docstring
-# pylint: disable=no-member
-import json
+from __future__ import unicode_literals
+
 import textwrap
 
+import pytest
+
 from plette import Lockfile, Pipfile
-from plette.models import Package, SourceCollection, Hash, Requires
+from plette.models import Package, SourceCollection
 
 
 HASH = "9aaf3dbaf8c4df3accd4606eb2275d3b91c9db41be4fd5a97ecc95d79a12cfe6"
 
 
-def test_lockfile_load_sources(tmpdir):
+def test_lockfile_load(tmpdir):
     fi = tmpdir.join("in.json")
     fi.write(textwrap.dedent(
         """\
         {
             "_meta": {
                 "hash": {"sha256": "____hash____"},
                 "pipfile-spec": 6,
@@ -40,42 +40,14 @@
     assert lock.meta.sources == SourceCollection([
         {
             'url': 'https://pypi.org/simple',
             'verify_ssl': True,
             'name': 'pypi',
         },
     ])
-
-
-def test_lockfile_load_sources_package_spec(tmpdir):
-    fi = tmpdir.join("in.json")
-    fi.write(textwrap.dedent(
-        """\
-        {
-            "_meta": {
-                "hash": {"sha256": "____hash____"},
-                "pipfile-spec": 6,
-                "requires": {},
-                "sources": [
-                    {
-                        "name": "pypi",
-                        "url": "https://pypi.org/simple",
-                        "verify_ssl": true
-                    }
-                ]
-            },
-            "default": {
-                "flask": {"version": "*"},
-                "jinja2": "*"
-            },
-            "develop": {}
-        }
-        """,
-    ).replace("____hash____", HASH))
-    lock = Lockfile.load(fi)
     assert lock.default["jinja2"] == Package("*")
 
 
 def test_lockfile_dump_format(tmpdir):
     content = textwrap.dedent(
         """\
         {
@@ -108,45 +80,43 @@
     fi.write(content)
     lock = Lockfile.load(fi)
 
     # Don't use `lock.dump(outpath)`. It has some flushing issues.
     outpath = tmpdir.join("out.json")
     with outpath.open("w") as f:
         lock.dump(f)
-    loaded = json.loads(outpath.read())
-    assert "_meta" in loaded
-    assert json.loads(outpath.read()) == json.loads(content)
+
+    assert outpath.read() == content
 
 
 def test_lockfile_from_pipfile_meta():
-    pipfile = Pipfile(**{
-        "sources": [
+    pipfile = Pipfile({
+        "source": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": True,
             },
         ],
         "requires": {
             "python_version": "3.7",
         }
     })
-
     pipfile_hash_value = pipfile.get_hash().value
     lockfile = Lockfile.with_meta_from(pipfile)
 
-    pipfile.requires["python_version"] = "3.8"
-    pipfile.sources.sources.append({
+    pipfile.requires._data["python_version"] = "3.8"
+    pipfile.sources.append({
         "name": "devpi",
         "url": "http://localhost/simple",
         "verify_ssl": True,
     })
 
-    assert lockfile.meta.hash == Hash.from_dict({"sha256": pipfile_hash_value})
-    assert lockfile.meta.requires == Requires(python_version={'python_version': '3.7'}, python_full_version=None)
-    assert lockfile.meta.sources == SourceCollection([
+    assert lockfile.meta.hash._data == {"sha256": pipfile_hash_value}
+    assert lockfile.meta.requires._data == {"python_version": "3.7"}
+    assert lockfile.meta.sources._data == [
         {
             "name": "pypi",
             "url": "https://pypi.org/simple",
             "verify_ssl": True,
         },
-    ])
+    ]
```

### Comparing `plette-1.0.0/tests/test_pipfiles.py` & `plette-2.0.0/tests/test_pipfiles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import textwrap
 
+import pytest
+
 from plette import Pipfile
 from plette.models import PackageCollection, SourceCollection
 
 
 def test_source_section():
     section = SourceCollection([
         {
@@ -21,72 +23,74 @@
         {
             "name": "devpi",
             "url": "https://$USER:$PASS@mydevpi.localhost",
             "verify_ssl": False,
         },
     ])
     section[0].verify_ssl = True
-    assert section == SourceCollection([
+    assert section._data == [
         {
             "name": "devpi",
             "url": "https://$USER:$PASS@mydevpi.localhost",
             "verify_ssl": True,
         },
-    ])
+    ]
 
 
 def test_package_section():
     section = PackageCollection({
         "flask": {"version": "*"},
         "jinja2": "*",
     })
-    assert section.packages["jinja2"].version == "*"
+    assert section["jinja2"].version == "*"
+    with pytest.raises(KeyError) as ctx:
+        section["mosql"]
+    assert str(ctx.value) == repr("mosql")
 
 
 def test_pipfile_load(tmpdir):
     fi = tmpdir.join("Pipfile.in")
     fi.write(textwrap.dedent("""
         [packages]
         flask = { version = "*" }
         jinja2 = '*'   # A comment.
     """))
     p = Pipfile.load(fi)
-
-    assert p.source == SourceCollection([
+    assert p["source"] == SourceCollection([
         {
             'url': 'https://pypi.org/simple',
             'verify_ssl': True,
             'name': 'pypi',
         },
     ])
-    assert p.packages == {
+    assert p["packages"] == PackageCollection({
         "flask": {"version": "*"},
         "jinja2": "*",
-    }
+    })
 
 
 def test_pipfile_preserve_format(tmpdir):
     fi = tmpdir.join("Pipfile.in")
     fi.write(textwrap.dedent(
         """\
         [packages]
         flask = { version = "*" }
         jinja2 = '*'
         """,
     ))
-    pf= Pipfile.load(fi)
-    pf.source[0].verify_ssl = False
+    p = Pipfile.load(fi)
+    p["source"][0].verify_ssl = False
 
     fo = tmpdir.join("Pipfile.out")
-    pf.dump(fo)
+    p.dump(fo)
     assert fo.read() == textwrap.dedent(
         """\
         [[source]]
         name = "pypi"
-        verify_ssl = false
         url = "https://pypi.org/simple"
+        verify_ssl = false
 
         [packages]
         flask = { version = "*" }
         jinja2 = '*'
         """,
     )
```

### Comparing `plette-1.0.0/tests/test_scripts.py` & `plette-2.0.0/tests/test_scripts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import pytest
 
+from plette.models.base import DataValidationError
 from plette.models import Script
 
 
 def test_parse():
     script = Script(['python', '-c', "print('hello')"])
     assert script.command == 'python'
     assert script.args == ['-c', "print('hello')"], script
 
 
 def test_parse_error():
-    with pytest.raises(IndexError):
+    with pytest.raises(DataValidationError) as ctx:
         Script('')
 
+    assert str(ctx.value) == "Script cannot be empty", ctx
+
+
 def test_cmdify():
     script = Script(['python', '-c', "print('hello world')"])
     cmd = script.cmdify()
     assert cmd == 'python -c "print(\'hello world\')"', script
 
 
 def test_cmdify_extend():
```


# Comparing `tmp/pytm-1.3.0.tar.gz` & `tmp/pytm-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytm-1.3.0.tar", last modified: Mon Feb 26 22:53:46 2024, max compression
+gzip compressed data, was "pytm-1.3.1.tar", max compression
```

## Comparing `pytm-1.3.0.tar` & `pytm-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,16 @@
-drwxrwxr-x   0 izar      (1000) izar      (1000)        0 2024-02-26 22:53:46.816372 pytm-1.3.0/
--rw-rw-r--   0 izar      (1000) izar      (1000)     2161 2023-11-10 16:24:08.000000 pytm-1.3.0/LICENSE
--rw-rw-r--   0 izar      (1000) izar      (1000)       57 2023-11-10 16:24:08.000000 pytm-1.3.0/MANIFEST.in
--rw-rw-r--   0 izar      (1000) izar      (1000)    17956 2024-02-26 22:53:46.816372 pytm-1.3.0/PKG-INFO
--rw-rw-r--   0 izar      (1000) izar      (1000)    17288 2024-02-26 22:18:45.000000 pytm-1.3.0/README.md
--rw-rw-r--   0 izar      (1000) izar      (1000)      354 2023-11-10 16:24:08.000000 pytm-1.3.0/pyproject.toml
-drwxrwxr-x   0 izar      (1000) izar      (1000)        0 2024-02-26 22:53:46.812372 pytm-1.3.0/pytm/
--rw-rw-r--   0 izar      (1000) izar      (1000)     1234 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/__init__.py
-drwxrwxr-x   0 izar      (1000) izar      (1000)        0 2024-02-26 22:53:46.812372 pytm-1.3.0/pytm/images/
--rw-rw-r--   0 izar      (1000) izar      (1000)    13242 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/images/datastore.png
--rw-rw-r--   0 izar      (1000) izar      (1000)    13242 2024-02-26 22:18:45.000000 pytm-1.3.0/pytm/images/datastore_black.png
--rw-rw-r--   0 izar      (1000) izar      (1000)     3805 2024-02-26 22:18:45.000000 pytm-1.3.0/pytm/images/datastore_darkgreen.png
--rw-rw-r--   0 izar      (1000) izar      (1000)     3806 2024-02-26 22:18:45.000000 pytm-1.3.0/pytm/images/datastore_firebrick3.png
--rw-rw-r--   0 izar      (1000) izar      (1000)     3797 2024-02-26 22:18:45.000000 pytm-1.3.0/pytm/images/datastore_gold.png
--rw-rw-r--   0 izar      (1000) izar      (1000)    31437 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/images/lambda.png
--rw-rw-r--   0 izar      (1000) izar      (1000)     3232 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/json.py
--rw-rw-r--   0 izar      (1000) izar      (1000)    65373 2024-02-26 22:18:45.000000 pytm-1.3.0/pytm/pytm.py
--rw-rw-r--   0 izar      (1000) izar      (1000)     1337 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/report_util.py
--rw-rw-r--   0 izar      (1000) izar      (1000)     3586 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/template_engine.py
-drwxrwxr-x   0 izar      (1000) izar      (1000)        0 2024-02-26 22:53:46.812372 pytm-1.3.0/pytm/threatlib/
--rw-rw-r--   0 izar      (1000) izar      (1000)   252042 2023-11-10 16:24:08.000000 pytm-1.3.0/pytm/threatlib/threats.json
-drwxrwxr-x   0 izar      (1000) izar      (1000)        0 2024-02-26 22:53:46.812372 pytm-1.3.0/pytm.egg-info/
--rw-rw-r--   0 izar      (1000) izar      (1000)    17956 2024-02-26 22:53:46.000000 pytm-1.3.0/pytm.egg-info/PKG-INFO
--rw-rw-r--   0 izar      (1000) izar      (1000)      542 2024-02-26 22:53:46.000000 pytm-1.3.0/pytm.egg-info/SOURCES.txt
--rw-rw-r--   0 izar      (1000) izar      (1000)        1 2024-02-26 22:53:46.000000 pytm-1.3.0/pytm.egg-info/dependency_links.txt
--rw-rw-r--   0 izar      (1000) izar      (1000)       18 2024-02-26 22:53:46.000000 pytm-1.3.0/pytm.egg-info/requires.txt
--rw-rw-r--   0 izar      (1000) izar      (1000)        5 2024-02-26 22:53:46.000000 pytm-1.3.0/pytm.egg-info/top_level.txt
--rw-rw-r--   0 izar      (1000) izar      (1000)       38 2024-02-26 22:53:46.816372 pytm-1.3.0/setup.cfg
--rw-rw-r--   0 izar      (1000) izar      (1000)     1344 2024-02-26 22:51:19.000000 pytm-1.3.0/setup.py
-drwxrwxr-x   0 izar      (1000) izar      (1000)        0 2024-02-26 22:53:46.812372 pytm-1.3.0/tests/
--rw-rw-r--   0 izar      (1000) izar      (1000)     9468 2023-12-05 16:55:53.000000 pytm-1.3.0/tests/test_private_func.py
--rw-rw-r--   0 izar      (1000) izar      (1000)    53628 2024-02-26 22:18:45.000000 pytm-1.3.0/tests/test_pytmfunc.py
+-rw-r--r--   0        0        0     2161 2024-01-17 17:59:24.637293 pytm-1.3.1/LICENSE
+-rw-r--r--   0        0        0      356 2024-04-25 15:54:42.877383 pytm-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      299 2024-01-17 17:59:24.640391 pytm-1.3.1/pytm/TODO.txt
+-rw-r--r--   0        0        0     1234 2024-01-17 17:59:24.640475 pytm-1.3.1/pytm/__init__.py
+-rw-r--r--   0        0        0    13242 2024-01-17 17:59:24.640681 pytm-1.3.1/pytm/images/datastore.png
+-rw-r--r--   0        0        0    13242 2024-03-21 12:04:29.379505 pytm-1.3.1/pytm/images/datastore_black.png
+-rw-r--r--   0        0        0     3805 2024-03-21 12:04:29.379637 pytm-1.3.1/pytm/images/datastore_darkgreen.png
+-rw-r--r--   0        0        0     3806 2024-03-21 12:04:29.379756 pytm-1.3.1/pytm/images/datastore_firebrick3.png
+-rw-r--r--   0        0        0     3797 2024-03-21 12:04:29.379863 pytm-1.3.1/pytm/images/datastore_gold.png
+-rw-r--r--   0        0        0    31437 2024-01-17 17:59:24.640843 pytm-1.3.1/pytm/images/lambda.png
+-rw-r--r--   0        0        0     3232 2024-01-17 17:59:24.640976 pytm-1.3.1/pytm/json.py
+-rw-r--r--   0        0        0    65849 2024-04-23 12:29:59.947841 pytm-1.3.1/pytm/pytm.py
+-rw-r--r--   0        0        0     1337 2024-01-17 17:59:24.641381 pytm-1.3.1/pytm/report_util.py
+-rw-r--r--   0        0        0     3586 2024-01-17 17:59:24.641483 pytm-1.3.1/pytm/template_engine.py
+-rw-r--r--   0        0        0   252042 2024-01-17 17:59:24.641942 pytm-1.3.1/pytm/threatlib/threats.json
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 pytm-1.3.1/PKG-INFO
```

### Comparing `pytm-1.3.0/LICENSE` & `pytm-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/__init__.py` & `pytm-1.3.1/pytm/__init__.py`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/images/datastore.png` & `pytm-1.3.1/pytm/images/datastore.png`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/images/datastore_black.png` & `pytm-1.3.1/pytm/images/datastore_black.png`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/images/datastore_darkgreen.png` & `pytm-1.3.1/pytm/images/datastore_darkgreen.png`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/images/datastore_firebrick3.png` & `pytm-1.3.1/pytm/images/datastore_firebrick3.png`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/images/datastore_gold.png` & `pytm-1.3.1/pytm/images/datastore_gold.png`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/images/lambda.png` & `pytm-1.3.1/pytm/images/lambda.png`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/json.py` & `pytm-1.3.1/pytm/json.py`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/pytm.py` & `pytm-1.3.1/pytm/pytm.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from hashlib import sha224
 from itertools import combinations
 from shutil import rmtree
 from textwrap import indent, wrap
 from weakref import WeakKeyDictionary
 from datetime import datetime
 
-from pydal import DAL, Field
-
 from .template_engine import SuperFormatter
 
 """ Helper functions """
 
 """ The base for this (descriptors instead of properties) has been
     shamelessly lifted from
     https://nbviewer.jupyter.org/urls/gist.github.com/ChrisBeaumont/5758381/raw/descriptor_writeup.ipynb
@@ -603,33 +601,37 @@
     description = varString("")
     condition = varString(
         "",
         doc="""a Python expression that should evaluate
 to a boolean True or False""",
     )
     details = varString("")
+    likelihood = varString("")
     severity = varString("")
     mitigations = varString("")
+    prerequisites = varString("")
     example = varString("")
     references = varString("")
     target = ()
 
     def __init__(self, **kwargs):
         self.id = kwargs["SID"]
         self.description = kwargs.get("description", "")
+        self.likelihood = kwargs.get("Likelihood Of Attack", "")
         self.condition = kwargs.get("condition", "True")
         target = kwargs.get("target", "Element")
         if not isinstance(target, str) and isinstance(target, Iterable):
             target = tuple(target)
         else:
             target = (target,)
         self.target = tuple(getattr(sys.modules[__name__], x) for x in target)
         self.details = kwargs.get("details", "")
         self.severity = kwargs.get("severity", "")
         self.mitigations = kwargs.get("mitigations", "")
+        self.prerequisites = kwargs.get("prerequisites", "")
         self.example = kwargs.get("example", "")
         self.references = kwargs.get("references", "")
 
     def _safeset(self, attr, value):
         try:
             setattr(self, attr, value)
         except ValueError:
@@ -1170,14 +1172,33 @@
                         + f"{base_path}/{src}"
                     )
 
         return ""
 
     def sqlDump(self, filename):
         try:
+            from pydal import DAL, Field
+        except ImportError as e:
+            raise UIError(
+                e, """This feature requires the pyDAL package,
+    Please install the package via pip or your packagemanger of choice.
+                """
+            )
+
+        @lru_cache(maxsize=None)
+        def get_table(db, klass):
+            name = klass.__name__
+            fields = [
+                Field("SID" if i == "id" else i)
+                for i in dir(klass)
+                if not i.startswith("_") and not callable(getattr(klass, i))
+            ]
+            return db.define_table(name, fields)
+
+        try:
             rmtree("./sqldump")
             os.mkdir("./sqldump")
         except OSError as e:
             if e.errno != errno.ENOENT:
                 raise
             else:
                 os.mkdir("./sqldump")
@@ -1195,36 +1216,27 @@
             Boundary,
             TM,
             Threat,
             Lambda,
             Data,
             Finding,
         ):
-            self.get_table(db, klass)
+            get_table(db, klass)
 
         for e in TM._threats + TM._data + TM._elements + self.findings + [self]:
-            table = self.get_table(db, e.__class__)
+            table = get_table(db, e.__class__)
             row = {}
             for k, v in serialize(e).items():
                 if k == "id":
                     k = "SID"
                 row[k] = ", ".join(str(i) for i in v) if isinstance(v, list) else v
             db[table].bulk_insert([row])
 
         db.close()
 
-    @lru_cache(maxsize=None)
-    def get_table(self, db, klass):
-        name = klass.__name__
-        fields = [
-            Field("SID" if i == "id" else i)
-            for i in dir(klass)
-            if not i.startswith("_") and not callable(getattr(klass, i))
-        ]
-        return db.define_table(name, fields)
 
 
 class Controls:
     """Controls implemented by/on and Element"""
 
     authenticatesDestination = varBool(
         False,
@@ -1960,15 +1972,15 @@
         if isinstance(obj, TM) and i == "_elements":
             value = [e for e in value if isinstance(e, (Actor, Asset))]
         if value is not None:
             if isinstance(value, (Element, Data)):
                 value = value.name
             elif isinstance(obj, Threat) and i == "target":
                 value = [v.__name__ for v in value]
-            elif i == "levels" or i == "sourceFiles":
+            elif i in ("levels", "sourceFiles", "assumptions"):
                 value = list(value)
             elif (
                 not nested
                 and not isinstance(value, str)
                 and isinstance(value, Iterable)
             ):
                 value = [v.id if isinstance(v, Finding) else v.name for v in value]
```

### Comparing `pytm-1.3.0/pytm/report_util.py` & `pytm-1.3.1/pytm/report_util.py`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/template_engine.py` & `pytm-1.3.1/pytm/template_engine.py`

 * *Files identical despite different names*

### Comparing `pytm-1.3.0/pytm/threatlib/threats.json` & `pytm-1.3.1/pytm/threatlib/threats.json`

 * *Files identical despite different names*


# Comparing `tmp/asp_selftest-0.0.1.tar.gz` & `tmp/asp_selftest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_selftest-0.0.1.tar", last modified: Thu Apr 25 14:05:37 2024, max compression
+gzip compressed data, was "asp_selftest-0.0.2.tar", last modified: Thu Apr 25 14:37:16 2024, max compression
```

## Comparing `asp_selftest-0.0.1.tar` & `asp_selftest-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:05:37.332007 asp_selftest-0.0.1/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.1/LICENSE
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.1/MANIFEST.in
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3396 2024-04-25 14:05:37.331833 asp_selftest-0.0.1/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2783 2024-04-25 12:49:31.000000 asp_selftest-0.0.1/README.md
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      778 2024-04-25 13:26:47.000000 asp_selftest-0.0.1/pyproject.toml
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-04-25 14:05:37.332053 asp_selftest-0.0.1/setup.cfg
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:05:37.330123 asp_selftest-0.0.1/src/
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:05:37.331049 asp_selftest-0.0.1/src/asp_selftest/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 13:23:42.000000 asp_selftest-0.0.1/src/asp_selftest/__init__.py
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      526 2024-03-01 15:10:30.000000 asp_selftest-0.0.1/src/asp_selftest/example.lp
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-02-19 15:49:37.000000 asp_selftest-0.0.1/src/asp_selftest/queens.lp
--rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)     3074 2024-03-11 14:48:52.000000 asp_selftest-0.0.1/src/asp_selftest/runasptests.py
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:05:37.331664 asp_selftest-0.0.1/src/asp_selftest.egg-info/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3396 2024-04-25 14:05:37.000000 asp_selftest-0.0.1/src/asp_selftest.egg-info/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      320 2024-04-25 14:05:37.000000 asp_selftest-0.0.1/src/asp_selftest.egg-info/SOURCES.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-04-25 14:05:37.000000 asp_selftest-0.0.1/src/asp_selftest.egg-info/dependency_links.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-04-25 14:05:37.000000 asp_selftest-0.0.1/src/asp_selftest.egg-info/top_level.txt
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:37:16.650075 asp_selftest-0.0.2/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.2/LICENSE
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.2/MANIFEST.in
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3396 2024-04-25 14:37:16.649891 asp_selftest-0.0.2/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2783 2024-04-25 12:49:31.000000 asp_selftest-0.0.2/README.md
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      790 2024-04-25 14:36:45.000000 asp_selftest-0.0.2/pyproject.toml
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-04-25 14:37:16.650113 asp_selftest-0.0.2/setup.cfg
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:37:16.648183 asp_selftest-0.0.2/src/
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:37:16.648999 asp_selftest-0.0.2/src/asp_selftest/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      526 2024-03-01 15:10:30.000000 asp_selftest-0.0.2/src/asp_selftest/example.lp
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-02-19 15:49:37.000000 asp_selftest-0.0.2/src/asp_selftest/queens.lp
+-rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)     3302 2024-04-25 14:23:40.000000 asp_selftest-0.0.2/src/asp_selftest/runasptests.py
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-04-25 14:37:16.649720 asp_selftest-0.0.2/src/asp_selftest.egg-info/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3396 2024-04-25 14:37:16.000000 asp_selftest-0.0.2/src/asp_selftest.egg-info/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      334 2024-04-25 14:37:16.000000 asp_selftest-0.0.2/src/asp_selftest.egg-info/SOURCES.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-04-25 14:37:16.000000 asp_selftest-0.0.2/src/asp_selftest.egg-info/dependency_links.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-04-25 14:37:16.000000 asp_selftest-0.0.2/src/asp_selftest.egg-info/entry_points.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-04-25 14:37:16.000000 asp_selftest-0.0.2/src/asp_selftest.egg-info/top_level.txt
```

### Comparing `asp_selftest-0.0.1/LICENSE` & `asp_selftest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.1/PKG-INFO` & `asp_selftest-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `asp_selftest-0.0.1/README.md` & `asp_selftest-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.1/pyproject.toml` & `asp_selftest-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "asp_selftest"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Erik Groeneveld", email="ejgroene@ieee.org" },
 ]
 description = "A tool for running in-source unittests for Anwer Set Programming (ASP)"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: ASP",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
 ]
 
 
+[project.scripts]
+asp-tests = "asp_selftest:runasptests"
+
+
 [project.urls]
 Homepage = "https://github.com/ejgroene/asp-selftest"
 Issues = "https://github.com/ejgroene/asp-selftest/issues"
 
 
-[tool.setuptools]
-include-package-data = true
-
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `asp_selftest-0.0.1/src/asp_selftest/example.lp` & `asp_selftest-0.0.2/src/asp_selftest/example.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.1/src/asp_selftest/queens.lp` & `asp_selftest-0.0.2/src/asp_selftest/queens.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.1/src/asp_selftest/runasptests.py` & `asp_selftest-0.0.2/src/asp_selftest/runasptests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3.11
+#!/usr/bin/env python3
 import clingo
 import sys
 import ast
 
 from clingo.script import enable_python
 enable_python()
 
@@ -16,73 +16,74 @@
 p = parse_signature("one(two, three)")
 assert p == ('one', [('two', []), ('three', [])]), p
 p = parse_signature("one(2, 3)")
 assert p == ('one', [2, 3]), p
 p = parse_signature("one(two(2, aap), three(42))")
 assert p == ('one', [('two', [2, ('aap', [])]), ('three', [42])]), p
 
-program_file = sys.argv[1]
+if __name__ == '__main__':
+    program_file = sys.argv[1]
 
-# read all the #program parts and register their dependencies
-lines = open(program_file).readlines()
-print(f"Read {len(lines)} lines.")
-programs = {}
-
-for i, line in enumerate(lines):
-    if line.startswith('#program'):
-        name, deps = parse_signature(line.split('#program')[1].strip()[:-1])
-        if name in programs:
-            raise Exception("Duplicate test name: " + name)
-        programs[name] = deps
-        # rewrite into valid ASP (turn functions into plain terms)
-        lines[i] = f"#program {name}({','.join(dep[0] for dep in deps)})."
-
-
-class Tester:
-
-    def __init__(self):
-        self._asserts = set()
-        self._models_ist = 0
-        self._models_soll = -1
-
-    def all(self, term):
-        """ ASP API: add a named assert to be checked for each model """
-        self._asserts.add(clingo.Function("assert", [term]))
-        #print("ALL:", term)
-        return term
-
-    def models(self, n):
-        """ ASP API: add assert for the total number of models """
-        self._models_soll = n.number
-        return self.all(clingo.Function("models", [n]))
-
-    def on_model(self, model):
-        """ Callback when model is found; count model and check all asserts. """
-        self._models_ist += 1
-        failures = [a for a in self._asserts if not model.contains(a)]
-        assert not failures, f"FAILED: {', '.join(map(str, failures))}\nMODEL: {model}"
-        return model
-
-    def report(self):
-        """ When done, check assert(@models(n)) explicitly, then report. """
-        assert self._models_ist == self._models_soll, f"Expected {self._models_soll} models, found {self._models_ist}."
-        print(f" {len(self._asserts)} asserts,  {self._models_ist} models.  OK")
-
-
-    def concat(self, *args):
-        return clingo.String(''.join(a.string for a in args))
-
-
-sys.tracebacklimit = 0
-
-control = clingo.Control(['0'])
-control.add('\n'.join(lines))
-
-for name, deps in programs.items():
-    if name.startswith('test'):
-        print(name, end=', ', flush=True)
-        tester = Tester()
-        programs = [(name, [clingo.Number(1) for _ in deps])] + \
-                   [(depname, [clingo.parse_term(str(a)) for a in depargs]) for depname, depargs in deps]
-        control.ground(programs, context = tester)
-        control.solve(on_model = tester.on_model)
-        tester.report()
+    # read all the #program parts and register their dependencies
+    lines = open(program_file).readlines()
+    print(f"Read {len(lines)} lines.")
+    programs = {}
+
+    for i, line in enumerate(lines):
+        if line.startswith('#program'):
+            name, deps = parse_signature(line.split('#program')[1].strip()[:-1])
+            if name in programs:
+                raise Exception("Duplicate test name: " + name)
+            programs[name] = deps
+            # rewrite into valid ASP (turn functions into plain terms)
+            lines[i] = f"#program {name}({','.join(dep[0] for dep in deps)})."
+
+
+    class Tester:
+
+        def __init__(self):
+            self._asserts = set()
+            self._models_ist = 0
+            self._models_soll = -1
+
+        def all(self, term):
+            """ ASP API: add a named assert to be checked for each model """
+            self._asserts.add(clingo.Function("assert", [term]))
+            #print("ALL:", term)
+            return term
+
+        def models(self, n):
+            """ ASP API: add assert for the total number of models """
+            self._models_soll = n.number
+            return self.all(clingo.Function("models", [n]))
+
+        def on_model(self, model):
+            """ Callback when model is found; count model and check all asserts. """
+            self._models_ist += 1
+            failures = [a for a in self._asserts if not model.contains(a)]
+            assert not failures, f"FAILED: {', '.join(map(str, failures))}\nMODEL: {model}"
+            return model
+
+        def report(self):
+            """ When done, check assert(@models(n)) explicitly, then report. """
+            assert self._models_ist == self._models_soll, f"Expected {self._models_soll} models, found {self._models_ist}."
+            print(f" {len(self._asserts)} asserts,  {self._models_ist} models.  OK")
+
+
+        def concat(self, *args):
+            return clingo.String(''.join(a.string for a in args))
+
+
+    sys.tracebacklimit = 0
+
+    control = clingo.Control(['0'])
+    control.add('\n'.join(lines))
+
+    for name, deps in programs.items():
+        if name.startswith('test'):
+            print(name, end=', ', flush=True)
+            tester = Tester()
+            programs = [(name, [clingo.Number(1) for _ in deps])] + \
+                       [(depname, [clingo.parse_term(str(a)) for a in depargs]) for depname, depargs in deps]
+            control.ground(programs, context = tester)
+            control.solve(on_model = tester.on_model)
+            tester.report()
```

### Comparing `asp_selftest-0.0.1/src/asp_selftest.egg-info/PKG-INFO` & `asp_selftest-0.0.2/src/asp_selftest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```


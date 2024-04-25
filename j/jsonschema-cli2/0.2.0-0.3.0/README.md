# Comparing `tmp/jsonschema_cli2-0.2.0.tar.gz` & `tmp/jsonschema_cli2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_cli2-0.2.0.tar", max compression
+gzip compressed data, was "jsonschema_cli2-0.3.0.tar", max compression
```

## Comparing `jsonschema_cli2-0.2.0.tar` & `jsonschema_cli2-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/LICENSE
--rw-r--r--   0        0        0     2952 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/__init__.py
--rw-r--r--   0        0        0      110 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/__main__.py
--rw-r--r--   0        0        0     2221 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/args.py
--rw-r--r--   0        0        0      377 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/cli.py
--rw-r--r--   0        0        0       99 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/exceptions.py
--rw-r--r--   0        0        0      550 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/handlers.py
--rw-r--r--   0        0        0      910 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/load.py
--rw-r--r--   0        0        0      269 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/resolvers.py
--rw-r--r--   0        0        0     3831 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/jsonschema_cli2/tests/test_cli.py
--rw-r--r--   0        0        0      879 2024-04-25 20:19:54.424954 jsonschema_cli2-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 jsonschema_cli2-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2953 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/__main__.py
+-rw-r--r--   0        0        0     2221 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/args.py
+-rw-r--r--   0        0        0      377 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/cli.py
+-rw-r--r--   0        0        0       99 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/exceptions.py
+-rw-r--r--   0        0        0      550 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/handlers.py
+-rw-r--r--   0        0        0      910 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/load.py
+-rw-r--r--   0        0        0      269 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/resolvers.py
+-rw-r--r--   0        0        0     3831 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/jsonschema_cli2/tests/test_cli.py
+-rw-r--r--   0        0        0     1739 2024-04-25 20:50:04.701678 jsonschema_cli2-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4087 1970-01-01 00:00:00.000000 jsonschema_cli2-0.3.0/PKG-INFO
```

### Comparing `jsonschema_cli2-0.2.0/LICENSE` & `jsonschema_cli2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-0.2.0/README.md` & `jsonschema_cli2-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # JsonSchema CLI
 
 A thin wrapper over [Python Jsonschema](https://github.com/Julian/jsonschema) to allow validating shcemas easily using simple CLI commands.
 
 ## Installing
 
-`pip install jsonschema-cli`
+`pip install jsonschema-cli2`
 
 ## Security
 
 The `$ref` resolving will automatically resolve to any path using basic `$ref` notation:
 
 ```json
 {"$ref": "my-custom.json#...."}
```

### Comparing `jsonschema_cli2-0.2.0/jsonschema_cli2/args.py` & `jsonschema_cli2-0.3.0/jsonschema_cli2/args.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-0.2.0/jsonschema_cli2/handlers.py` & `jsonschema_cli2-0.3.0/jsonschema_cli2/handlers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-0.2.0/jsonschema_cli2/load.py` & `jsonschema_cli2-0.3.0/jsonschema_cli2/load.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-0.2.0/jsonschema_cli2/tests/test_cli.py` & `jsonschema_cli2-0.3.0/jsonschema_cli2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema_cli2-0.2.0/PKG-INFO` & `jsonschema_cli2-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: jsonschema-cli2
-Version: 0.2.0
-Summary: A thin wrapper over to allow validating shcemas easily using simple CLI commands.
-Author: Solairen
+Version: 0.3.0
+Summary: A thin wrapper over to allow validating schemas easily using simple CLI commands.
+Author: solairen
 Author-email: solairen@solairen.tech
 Requires-Python: >=3.8
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: jsonschema (>=3.2.0)
 Requires-Dist: pyyaml (>=5.3.1)
 Description-Content-Type: text/markdown
 
 This is based on the frok from [jsonschema-cli](https://github.com/eyal-mor/jsonschema-cli.git).
 
 # JsonSchema CLI
 
 A thin wrapper over [Python Jsonschema](https://github.com/Julian/jsonschema) to allow validating shcemas easily using simple CLI commands.
 
 ## Installing
 
-`pip install jsonschema-cli`
+`pip install jsonschema-cli2`
 
 ## Security
 
 The `$ref` resolving will automatically resolve to any path using basic `$ref` notation:
 
 ```json
 {"$ref": "my-custom.json#...."}
```


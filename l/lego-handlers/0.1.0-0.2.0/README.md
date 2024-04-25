# Comparing `tmp/lego_handlers-0.1.0.tar.gz` & `tmp/lego_handlers-0.2.0.tar.gz`

## Comparing `lego_handlers-0.1.0.tar` & `lego_handlers-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/.github/workflows/CD.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/scripts/new-release.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/src/lego_handlers/__init__.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/src/lego_handlers/components.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/src/lego_handlers/py.typed
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/tests/test_something.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/.gitignore
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/.github/workflows/CD.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/scripts/new-release.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/src/lego_handlers/__init__.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/src/lego_handlers/components.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/src/lego_handlers/py.typed
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/tests/test_something.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/.gitignore
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-0.2.0/PKG-INFO
```

### Comparing `lego_handlers-0.1.0/requirements-dev.lock` & `lego_handlers-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.1.0/.github/workflows/CD.yml` & `lego_handlers-0.2.0/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.1.0/.github/workflows/CI.yml` & `lego_handlers-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.1.0/scripts/new-release.py` & `lego_handlers-0.2.0/scripts/new-release.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.1.0/src/lego_handlers/components.py` & `lego_handlers-0.2.0/src/lego_handlers/components.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.1.0/tests/test_something.py` & `lego_handlers-0.2.0/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.1.0/pyproject.toml` & `lego_handlers-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lego-handlers"
-version = "0.1.0"
+version = "0.2.0"
 description = "Add your description here"
 authors = [{ name = "Tomperez98", email = "tomasperezalvarez@gmail.com" }]
 dependencies = [
     "result>=0.16.1",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```


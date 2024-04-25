# Comparing `tmp/gouge-2.2.1.tar.gz` & `tmp/gouge-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gouge-2.2.1.tar", last modified: Sun Apr  7 14:05:55 2024, max compression
+gzip compressed data, was "gouge-2.2.2.tar", last modified: Thu Apr 25 11:21:07 2024, max compression
```

## Comparing `gouge-2.2.1.tar` & `gouge-2.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.564555 gouge-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-07 14:05:45.000000 gouge-2.2.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-07 14:05:45.000000 gouge-2.2.1/.devcontainer/init.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-07 14:05:45.000000 gouge-2.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-07 14:05:45.000000 gouge-2.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-07 14:05:45.000000 gouge-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-07 14:05:45.000000 gouge-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 14:05:45.000000 gouge-2.2.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 14:05:45.000000 gouge-2.2.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-07 14:05:45.000000 gouge-2.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-07 14:05:55.564555 gouge-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-07 14:05:45.000000 gouge-2.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/_static/pre-formatter-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/_static/pre-formatter-not-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/_static/snapshot1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.560555 gouge-2.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-07 14:05:45.000000 gouge-2.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 14:05:45.000000 gouge-2.2.1/fabfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-07 14:05:45.000000 gouge-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:05:55.564555 gouge-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.556555 gouge-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.564555 gouge-2.2.1/src/gouge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:45.000000 gouge-2.2.1/src/gouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-07 14:05:45.000000 gouge-2.2.1/src/gouge/colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-07 14:05:45.000000 gouge-2.2.1/src/gouge/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-07 14:05:45.000000 gouge-2.2.1/src/gouge/parseable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-07 14:05:45.000000 gouge-2.2.1/src/gouge/preformatters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:45.000000 gouge-2.2.1/src/gouge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.564555 gouge-2.2.1/src/gouge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-07 14:05:55.000000 gouge-2.2.1/src/gouge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-07 14:05:55.000000 gouge-2.2.1/src/gouge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:05:55.000000 gouge-2.2.1/src/gouge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 14:05:55.000000 gouge-2.2.1/src/gouge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 14:05:55.000000 gouge-2.2.1/src/gouge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:55.564555 gouge-2.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-07 14:05:45.000000 gouge-2.2.1/test/test_caplog.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 14:05:45.000000 gouge-2.2.1/test/test_coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-07 14:05:45.000000 gouge-2.2.1/test/test_colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 14:05:45.000000 gouge-2.2.1/test/test_preformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-07 14:05:45.000000 gouge-2.2.1/test/test_shifting_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-25 11:21:00.000000 gouge-2.2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 11:21:00.000000 gouge-2.2.2/.devcontainer/init.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 11:21:00.000000 gouge-2.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-25 11:21:00.000000 gouge-2.2.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 11:21:00.000000 gouge-2.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 11:21:00.000000 gouge-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-25 11:21:00.000000 gouge-2.2.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 11:21:00.000000 gouge-2.2.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 11:21:00.000000 gouge-2.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 11:21:07.064050 gouge-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-25 11:21:00.000000 gouge-2.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/pre-formatter-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/pre-formatter-not-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/snapshot1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 11:21:00.000000 gouge-2.2.2/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 11:21:00.000000 gouge-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:21:07.064050 gouge-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/src/gouge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/parseable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/preformatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/src/gouge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_caplog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_preformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_shifting_filter.py
```

### Comparing `gouge-2.2.1/.devcontainer/devcontainer.json` & `gouge-2.2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/.github/workflows/main.yml` & `gouge-2.2.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/.gitignore` & `gouge-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/.pre-commit-config.yaml` & `gouge-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/PKG-INFO` & `gouge-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.2.1
+Version: 2.2.2
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.2.1/README.rst` & `gouge-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/docs/Makefile` & `gouge-2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/docs/_static/pre-formatter-applied.png` & `gouge-2.2.2/docs/_static/pre-formatter-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/docs/_static/pre-formatter-not-applied.png` & `gouge-2.2.2/docs/_static/pre-formatter-not-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/docs/_static/snapshot1.png` & `gouge-2.2.2/docs/_static/snapshot1.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/docs/changelog.rst` & `gouge-2.2.2/docs/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
   This helps reading tracebacks when using complex frameworks (like SQLAlchemy,
   Flask, Starlette, ...).
 
 * [2.2.1] - fix: If the message or traceback contained Python string-template
   variables the output could either break or cause incorrect output. This is
   now fixed.
 
+* [2.2.2] - fix: Correctly initialise the "highlighted_path" value
+
 Version 2.1
 -----------
 
 * Added support for pre-formatters.
 * Provide bundled pre-formatter for ``uvicorn.access`` via
   ``gouge.preformatters``
```

### Comparing `gouge-2.2.1/docs/conf.py` & `gouge-2.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/docs/index.rst` & `gouge-2.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/fabfile.py` & `gouge-2.2.2/fabfile.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/pyproject.toml` & `gouge-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gouge"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
     {name = "Michel Albert", email = "michel@albert.lu"},
 ]
 description = "Collection of logging formatters."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {text = "BSD-3-Clause"}
```

### Comparing `gouge-2.2.1/src/gouge/colourcli.py` & `gouge-2.2.2/src/gouge/colourcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,19 +103,18 @@
             python_310_args.pop("validate")
         super().__init__(fmt, datefmt, style, **python_310_args)
         self.show_threads = show_threads
         self.show_exc = show_exc
         self.force_styling = force_styling
         self.show_pid = show_pid
         self.pre_formatters = pre_formatters or {}
-        self.highlighted_path = highlighted_path
         if (Path.cwd() / "src").exists():
             self.highlighted_path = Path.cwd() / "src"
         else:
-            self.highlighted_path = None
+            self.highlighted_path = highlighted_path
 
     def format(self, record: LogRecord) -> str:
         if record.levelno <= logging.DEBUG:
             colorize = clr.Style.BRIGHT + clr.Fore.BLACK
         elif record.levelno <= logging.INFO:
             colorize = clr.Fore.CYAN
         elif record.levelno <= logging.WARNING:
```

### Comparing `gouge-2.2.1/src/gouge/filters.py` & `gouge-2.2.2/src/gouge/filters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/src/gouge/parseable.py` & `gouge-2.2.2/src/gouge/parseable.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/src/gouge/preformatters.py` & `gouge-2.2.2/src/gouge/preformatters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/src/gouge.egg-info/PKG-INFO` & `gouge-2.2.2/src/gouge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.2.1
+Version: 2.2.2
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.2.1/src/gouge.egg-info/SOURCES.txt` & `gouge-2.2.2/src/gouge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/test/test_coloring.py` & `gouge-2.2.2/test/test_coloring.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/test/test_colourcli.py` & `gouge-2.2.2/test/test_colourcli.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/test/test_preformatter.py` & `gouge-2.2.2/test/test_preformatter.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.1/test/test_shifting_filter.py` & `gouge-2.2.2/test/test_shifting_filter.py`

 * *Files identical despite different names*


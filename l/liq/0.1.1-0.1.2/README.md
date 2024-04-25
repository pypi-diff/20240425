# Comparing `tmp/liq-0.1.1.tar.gz` & `tmp/liq-0.1.2.tar.gz`

## Comparing `liq-0.1.1.tar` & `liq-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 liq-0.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 liq-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 liq-0.1.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 liq-0.1.1/Dockerfile
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 liq-0.1.1/src/liq/__init__.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 liq-0.1.1/src/liq/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 liq-0.1.1/src/liq/_version.py
--rw-r--r--   0        0        0   161571 2020-02-02 00:00:00.000000 liq-0.1.1/test/hq.jpg
--rw-r--r--   0        0        0    83142 2020-02-02 00:00:00.000000 liq-0.1.1/test/lq.jpg
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 liq-0.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 liq-0.1.1/LICENSE
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 liq-0.1.1/README.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 liq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 liq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 liq-0.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 liq-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 liq-0.1.2/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 liq-0.1.2/Dockerfile
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 liq-0.1.2/src/liq/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 liq-0.1.2/src/liq/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 liq-0.1.2/src/liq/_version.py
+-rw-r--r--   0        0        0   161571 2020-02-02 00:00:00.000000 liq-0.1.2/test/hq.jpg
+-rw-r--r--   0        0        0    83142 2020-02-02 00:00:00.000000 liq-0.1.2/test/lq.jpg
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 liq-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 liq-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 liq-0.1.2/README.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 liq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 liq-0.1.2/PKG-INFO
```

### Comparing `liq-0.1.1/.gitlab-ci.yml` & `liq-0.1.2/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,17 @@
   image: python:${PY_VERSION}
   parallel:
     matrix:
       - PY_VERSION:
         # Maintain parity with pyproject.toml
         - "3.12"
         - "3.11"
+        - "3.10"
+        - "3.9"
+        - "3.8"
   stage: test
   dependencies:
     - build package
   before_script:
     - apt-get update && apt-get install -y libmagickwand-dev
   script:
     # These commands all serve as tests, at least as long as there is no decent real test framework implemented.
```

### Comparing `liq-0.1.1/.pre-commit-config.yaml` & `liq-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/Dockerfile` & `liq-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/src/liq/__init__.py` & `liq-0.1.2/src/liq/__init__.py`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/src/liq/__main__.py` & `liq-0.1.2/src/liq/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from typing import Tuple
 
 import click
 
 from . import run_liq
 from ._version import __version__
 
 QTEAL = click.style("Q", fg="cyan") + click.style("teal", fg="bright_black")
@@ -28,15 +29,15 @@
     help="\b\n" + LOGO + "\n" + HELP,
 )
 @click.version_option(__version__)
 @click.option("-q", "--quality", type=click.IntRange(min=0, max=100), default=75, show_default=True)
 @click.option("--fix/--no-fix", is_flag=True, default=False, show_default=True)
 @click.option("-v", "--verbose", is_flag=True, default=False, help="log the detected quality of every image")
 @click.argument("paths", type=click.Path(path_type=Path, exists=True, file_okay=True, dir_okay=False), nargs=-1, required=True)
-def main(quality: int, fix: bool, verbose: bool, paths: tuple[Path]):
+def main(quality: int, fix: bool, verbose: bool, paths: Tuple[Path]):
     changes = False
     # can't use any or all builtins because they short circuit
     for path in paths:
         changes = run_liq(quality, fix, verbose, path) or changes
     if changes:
         exit(1)
```

### Comparing `liq-0.1.1/test/hq.jpg` & `liq-0.1.2/test/hq.jpg`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/test/lq.jpg` & `liq-0.1.2/test/lq.jpg`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/LICENSE` & `liq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/README.md` & `liq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `liq-0.1.1/pyproject.toml` & `liq-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "liq"
 description = "Limit Image Quality, pre-commit hook"
 readme = "README.md"
 license = { file="LICENSE" }
 authors = [
     {name = "Dries Kennes", email = "dries.kennes@qteal.com"}
 ]
-requires-python = ">=3.11"   # Maintain parity with tested versions in the CI
+requires-python = ">=3.8"   # Maintain parity with tested versions in the CI
 dynamic = ["version"]
 
 dependencies = [
     "click~=8.1",
     "wand~=0.6",
 ]
 
@@ -23,14 +23,21 @@
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/liq/_version.py"
 
+# Test on old Python versions
+[tool.hatch.envs.test]
+[[tool.hatch.envs.test.matrix]]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+[tool.hatch.envs.test.scripts]
+liq_test = 'liq -v test/*'
+
 #  ___       __  __
 # | _ \_  _ / _|/ _|
 # |   / || |  _|  _|
 # |_|_\\_,_|_| |_|
 [tool.ruff]
 line-length = 140
 fix = true
```

### Comparing `liq-0.1.1/PKG-INFO` & `liq-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: liq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Limit Image Quality, pre-commit hook
 Author-email: Dries Kennes <dries.kennes@qteal.com>
 License: MIT License
         
         Copyright (c) 2024 Dries Kennes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Requires-Dist: click~=8.1
 Requires-Dist: wand~=0.6
 Description-Content-Type: text/markdown
 
 # Limit Image Quality
 
 ```
```


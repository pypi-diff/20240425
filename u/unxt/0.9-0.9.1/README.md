# Comparing `tmp/unxt-0.9.tar.gz` & `tmp/unxt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  2 18:21:24 2024, max compression
+gzip compressed data, last modified: Tue Apr 23 18:21:37 2024, max compression
```

## Comparing `unxt-0.9.tar` & `unxt-0.9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      366 2024-04-02 18:21:24.000000 unxt-0.9/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-04-02 18:21:24.000000 unxt-0.9/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-02 18:21:24.000000 unxt-0.9/.gitattributes
--rw-r--r--   0        0        0     2558 2024-04-02 18:21:24.000000 unxt-0.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-02 18:21:24.000000 unxt-0.9/.readthedocs.yml
--rw-r--r--   0        0        0      439 2024-04-02 18:21:24.000000 unxt-0.9/conftest.py
--rw-r--r--   0        0        0     2809 2024-04-02 18:21:24.000000 unxt-0.9/noxfile.py
--rw-r--r--   0        0        0     2389 2024-04-02 18:21:24.000000 unxt-0.9/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-02 18:21:24.000000 unxt-0.9/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-02 18:21:24.000000 unxt-0.9/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1540 2024-04-02 18:21:24.000000 unxt-0.9/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1630 2024-04-02 18:21:24.000000 unxt-0.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0      862 2024-04-02 18:21:24.000000 unxt-0.9/docs/conf.py
--rw-r--r--   0        0        0      191 2024-04-02 18:21:24.000000 unxt-0.9/docs/index.md
--rw-r--r--   0        0        0      554 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/__init__.py
--rw-r--r--   0        0        0      263 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_typing.py
--rw-r--r--   0        0        0      406 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_version.py
--rw-r--r--   0        0        0       82 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_version.pyi
--rw-r--r--   0        0        0     4692 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/experimental.py
--rw-r--r--   0        0        0        0 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/py.typed
--rw-r--r--   0        0        0      710 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/__init__.py
--rw-r--r--   0        0        0    15618 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/base.py
--rw-r--r--   0        0        0     3615 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/base_parametric.py
--rw-r--r--   0        0        0     1121 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/compat.py
--rw-r--r--   0        0        0     2938 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/core.py
--rw-r--r--   0        0        0     2570 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/distance.py
--rw-r--r--   0        0        0      569 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/fast.py
--rw-r--r--   0        0        0     3780 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/functional.py
--rw-r--r--   0        0        0     3375 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/register_dispatches.py
--rw-r--r--   0        0        0    90018 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/register_primitives.py
--rw-r--r--   0        0        0     1222 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/_quantity/utils.py
--rw-r--r--   0        0        0      404 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/__init__.py
--rw-r--r--   0        0        0     4407 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_base.py
--rw-r--r--   0        0        0     2849 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_core.py
--rw-r--r--   0        0        0      785 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_realizations.py
--rw-r--r--   0        0        0     2714 2024-04-02 18:21:24.000000 unxt-0.9/src/unxt/unitsystems/_utils.py
--rw-r--r--   0        0        0       13 2024-04-02 18:21:24.000000 unxt-0.9/tests/__init__.py
--rw-r--r--   0        0        0      185 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_package.py
--rw-r--r--   0        0        0      817 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_plum.py
--rw-r--r--   0        0        0    12184 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_quantity.py
--rw-r--r--   0        0        0     3716 2024-04-02 18:21:24.000000 unxt-0.9/tests/test_unitsystems.py
--rw-r--r--   0        0        0       13 2024-04-02 18:21:24.000000 unxt-0.9/tests/quaxed/__init__.py
--rw-r--r--   0        0        0    46419 2024-04-02 18:21:24.000000 unxt-0.9/tests/quaxed/test_array_api.py
--rw-r--r--   0        0        0      626 2024-04-02 18:21:24.000000 unxt-0.9/tests/quaxed/test_numpy.py
--rw-r--r--   0        0        0     2218 2024-04-02 18:21:24.000000 unxt-0.9/.gitignore
--rw-r--r--   0        0        0     1528 2024-04-02 18:21:24.000000 unxt-0.9/LICENSE
--rw-r--r--   0        0        0     1387 2024-04-02 18:21:24.000000 unxt-0.9/README.md
--rw-r--r--   0        0        0     5690 2024-04-02 18:21:24.000000 unxt-0.9/pyproject.toml
--rw-r--r--   0        0        0     5172 2024-04-02 18:21:24.000000 unxt-0.9/PKG-INFO
+-rw-r--r--   0        0        0      366 2024-04-23 18:21:37.000000 unxt-0.9.1/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-23 18:21:37.000000 unxt-0.9.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-23 18:21:37.000000 unxt-0.9.1/.gitattributes
+-rw-r--r--   0        0        0     2558 2024-04-23 18:21:37.000000 unxt-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-23 18:21:37.000000 unxt-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0      439 2024-04-23 18:21:37.000000 unxt-0.9.1/conftest.py
+-rw-r--r--   0        0        0     2809 2024-04-23 18:21:37.000000 unxt-0.9.1/noxfile.py
+-rw-r--r--   0        0        0     2389 2024-04-23 18:21:37.000000 unxt-0.9.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-23 18:21:37.000000 unxt-0.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-23 18:21:37.000000 unxt-0.9.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1540 2024-04-23 18:21:37.000000 unxt-0.9.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1630 2024-04-23 18:21:37.000000 unxt-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      862 2024-04-23 18:21:37.000000 unxt-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0      191 2024-04-23 18:21:37.000000 unxt-0.9.1/docs/index.md
+-rw-r--r--   0        0        0      554 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_typing.py
+-rw-r--r--   0        0        0      411 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_version.py
+-rw-r--r--   0        0        0       82 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_version.pyi
+-rw-r--r--   0        0        0     4692 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/experimental.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/py.typed
+-rw-r--r--   0        0        0      710 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/__init__.py
+-rw-r--r--   0        0        0    15652 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/base.py
+-rw-r--r--   0        0        0     3615 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/base_parametric.py
+-rw-r--r--   0        0        0     1121 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/compat.py
+-rw-r--r--   0        0        0     2938 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/core.py
+-rw-r--r--   0        0        0     2570 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/distance.py
+-rw-r--r--   0        0        0      569 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/fast.py
+-rw-r--r--   0        0        0     3780 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/functional.py
+-rw-r--r--   0        0        0     3375 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/register_dispatches.py
+-rw-r--r--   0        0        0    90018 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/register_primitives.py
+-rw-r--r--   0        0        0     1222 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/_quantity/utils.py
+-rw-r--r--   0        0        0      404 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/unitsystems/__init__.py
+-rw-r--r--   0        0        0     4407 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/unitsystems/_base.py
+-rw-r--r--   0        0        0     2849 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/unitsystems/_core.py
+-rw-r--r--   0        0        0      785 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/unitsystems/_realizations.py
+-rw-r--r--   0        0        0     2714 2024-04-23 18:21:37.000000 unxt-0.9.1/src/unxt/unitsystems/_utils.py
+-rw-r--r--   0        0        0       13 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/test_package.py
+-rw-r--r--   0        0        0      817 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/test_plum.py
+-rw-r--r--   0        0        0    12184 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/test_quantity.py
+-rw-r--r--   0        0        0     3716 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/test_unitsystems.py
+-rw-r--r--   0        0        0       13 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/quaxed/__init__.py
+-rw-r--r--   0        0        0    46419 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/quaxed/test_array_api.py
+-rw-r--r--   0        0        0      626 2024-04-23 18:21:37.000000 unxt-0.9.1/tests/quaxed/test_numpy.py
+-rw-r--r--   0        0        0     2218 2024-04-23 18:21:37.000000 unxt-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1528 2024-04-23 18:21:37.000000 unxt-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1387 2024-04-23 18:21:37.000000 unxt-0.9.1/README.md
+-rw-r--r--   0        0        0     5771 2024-04-23 18:21:37.000000 unxt-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5712 2024-04-23 18:21:37.000000 unxt-0.9.1/PKG-INFO
```

### Comparing `unxt-0.9/.pre-commit-config.yaml` & `unxt-0.9.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.21.3
+    rev: v3.24.0
     hooks:
       - id: commitizen
       # - id: commitizen-branch
       #   stages: [push]
 
   - repo: meta
     hooks:
@@ -18,15 +18,15 @@
 
   - repo: https://github.com/scientific-python/cookie
     rev: 2024.03.10
     hooks:
       - id: sp-repo-review
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
@@ -39,22 +39,22 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.1
+    rev: 0.28.2
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.5"
+    rev: "v0.4.1"
     hooks:
       # Run the linter
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: ["--fix", "--show-fixes"]
       # Run the formatter
       - id: ruff-format
```

### Comparing `unxt-0.9/noxfile.py` & `unxt-0.9.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/.github/CONTRIBUTING.md` & `unxt-0.9.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `unxt-0.9/.github/matchers/pylint.json` & `unxt-0.9.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `unxt-0.9/.github/workflows/cd.yml` & `unxt-0.9.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `unxt-0.9/.github/workflows/ci.yml` & `unxt-0.9.1/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
       - name: Test package
         run: >-
           python -m pytest src docs tests -ra --cov --cov-report=xml
           --cov-report=term --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.1
+        uses: codecov/codecov-action@v4.3.0
```

### Comparing `unxt-0.9/docs/conf.py` & `unxt-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/__init__.py` & `unxt-0.9.1/src/unxt/__init__.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/experimental.py` & `unxt-0.9.1/src/unxt/experimental.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/__init__.py` & `unxt-0.9.1/src/unxt/_quantity/__init__.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/base.py` & `unxt-0.9.1/src/unxt/_quantity/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,15 @@
         return self.to_units(units)
 
     def to_value(self, units: Unit) -> ArrayLike:
         """Return the value in the given units.
 
         See :meth:`AbstractQuantity.to_units_value`.
         """
+        return self.to_units_value(units)
 
     # ===============================================================
     # Array API
 
     def __array_namespace__(self, *, api_version: Any = None) -> "ArrayAPINamespace":
         return xp
 
@@ -416,15 +417,15 @@
 
         Examples
         --------
         >>> from unxt import Quantity
         >>> q1 = Quantity(1, "m")
         >>> try: hash(q1)
         ... except TypeError as e: print(e)
-        unhashable type: 'ArrayImpl'
+        unhashable type: ...
 
         """
         return hash(tuple(getattr(self, f.name) for f in fields(self)))
 
     # ===============================================================
     # I/O
```

### Comparing `unxt-0.9/src/unxt/_quantity/base_parametric.py` & `unxt-0.9.1/src/unxt/_quantity/base_parametric.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/compat.py` & `unxt-0.9.1/src/unxt/_quantity/compat.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/core.py` & `unxt-0.9.1/src/unxt/_quantity/core.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/distance.py` & `unxt-0.9.1/src/unxt/_quantity/distance.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/fast.py` & `unxt-0.9.1/src/unxt/_quantity/fast.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/functional.py` & `unxt-0.9.1/src/unxt/_quantity/functional.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/register_dispatches.py` & `unxt-0.9.1/src/unxt/_quantity/register_dispatches.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/register_primitives.py` & `unxt-0.9.1/src/unxt/_quantity/register_primitives.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/_quantity/utils.py` & `unxt-0.9.1/src/unxt/_quantity/utils.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/unitsystems/_base.py` & `unxt-0.9.1/src/unxt/unitsystems/_base.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/unitsystems/_core.py` & `unxt-0.9.1/src/unxt/unitsystems/_core.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/unitsystems/_realizations.py` & `unxt-0.9.1/src/unxt/unitsystems/_realizations.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/src/unxt/unitsystems/_utils.py` & `unxt-0.9.1/src/unxt/unitsystems/_utils.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/tests/test_plum.py` & `unxt-0.9.1/tests/test_plum.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/tests/test_quantity.py` & `unxt-0.9.1/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/tests/test_unitsystems.py` & `unxt-0.9.1/tests/test_unitsystems.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/tests/quaxed/test_array_api.py` & `unxt-0.9.1/tests/quaxed/test_array_api.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/tests/quaxed/test_numpy.py` & `unxt-0.9.1/tests/quaxed/test_numpy.py`

 * *Files identical despite different names*

### Comparing `unxt-0.9/.gitignore` & `unxt-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `unxt-0.9/LICENSE` & `unxt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unxt-0.9/README.md` & `unxt-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `unxt-0.9/pyproject.toml` & `unxt-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
   ]
   dependencies = [
     "quaxed >= 0.3",
-    "astropy",
-    "equinox",
-    "jax",
+    "astropy>=6.0",
+    "equinox>0.11",
+    "jax>0.4",
     "jaxlib",
     "jaxtyping",
     "quax>=0.0.3",
   ]
   description = "Quantities in JAX"
   dynamic = ["version"]
   license.file = "LICENSE"
@@ -144,14 +144,15 @@
       "COM812",  # <- for ruff.format
       "D103",    # Missing docstring in public function  # TODO: resolve
       "D105",    # Missing docstring in magic method
       "D107",    # Missing docstring in __init__
       "D203",    # 1 blank line required before class docstring
       "D213",    # Multi-line docstring summary should start at the second line
       "ERA001",  # Commented out code
+      "F722",    # Syntax error in forward annotation <- jaxtyping
       "F811",    # redefinition of unused '...'  <- plum-dispatch
       "F821",    # undefined name '...'  <- jaxtyping
       "FIX002",  # Line contains TODO
       "ISC001",  # Conflicts with formatter
       "PD",      # Pandas
       "PLR09",   # Too many <...>
       "PLR2004", # Magic value used in comparison
```

### Comparing `unxt-0.9/PKG-INFO` & `unxt-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: unxt
-Version: 0.9
+Version: 0.9.1
 Summary: Quantities in JAX
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/unxt/issues
 Project-URL: Changelog, https://github.com/GalacticDynamics/unxt/releases
 Project-URL: Discussions, https://github.com/GalacticDynamics/unxt/discussions
 Project-URL: Homepage, https://github.com/GalacticDynamics/unxt
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License: BSD 3-Clause License
@@ -47,27 +47,38 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Requires-Dist: astropy
-Requires-Dist: equinox
-Requires-Dist: jax
+Requires-Dist: astropy>=6.0
+Requires-Dist: equinox>0.11
+Requires-Dist: jax>0.4
 Requires-Dist: jaxlib
 Requires-Dist: jaxtyping
 Requires-Dist: quax>=0.0.3
 Requires-Dist: quaxed>=0.3
 Provides-Extra: all
-Requires-Dist: unxt[dev]; extra == 'all'
-Requires-Dist: unxt[docs]; extra == 'all'
-Requires-Dist: unxt[test]; extra == 'all'
+Requires-Dist: furo>=2023.08.17; extra == 'all'
+Requires-Dist: hypothesis[numpy]; extra == 'all'
+Requires-Dist: myst-parser>=0.13; extra == 'all'
+Requires-Dist: pytest-arraydiff; extra == 'all'
+Requires-Dist: pytest-cov>=3; extra == 'all'
+Requires-Dist: pytest<8,>=6; extra == 'all'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'all'
+Requires-Dist: sphinx-copybutton; extra == 'all'
+Requires-Dist: sphinx>=7.0; extra == 'all'
+Requires-Dist: sybil; extra == 'all'
 Provides-Extra: dev
-Requires-Dist: unxt[test]; extra == 'dev'
+Requires-Dist: hypothesis[numpy]; extra == 'dev'
+Requires-Dist: pytest-arraydiff; extra == 'dev'
+Requires-Dist: pytest-cov>=3; extra == 'dev'
+Requires-Dist: pytest<8,>=6; extra == 'dev'
+Requires-Dist: sybil; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: test
```


# Comparing `tmp/quaxed-0.3.8.tar.gz` & `tmp/quaxed-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Apr 24 03:58:22 2024, max compression
+gzip compressed data, last modified: Thu Apr 25 15:09:51 2024, max compression
```

## Comparing `quaxed-0.3.8.tar` & `quaxed-0.4.tar`

### file list

```diff
@@ -1,57 +1,62 @@
--rw-r--r--   0        0        0      380 2024-04-24 03:58:22.000000 quaxed-0.3.8/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-04-24 03:58:22.000000 quaxed-0.3.8/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-24 03:58:22.000000 quaxed-0.3.8/.gitattributes
--rw-r--r--   0        0        0     2899 2024-04-24 03:58:22.000000 quaxed-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-24 03:58:22.000000 quaxed-0.3.8/.readthedocs.yml
--rw-r--r--   0        0        0     2778 2024-04-24 03:58:22.000000 quaxed-0.3.8/noxfile.py
--rw-r--r--   0        0        0     2387 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1539 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1641 2024-04-24 03:58:22.000000 quaxed-0.3.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      834 2024-04-24 03:58:22.000000 quaxed-0.3.8/docs/conf.py
--rw-r--r--   0        0        0      193 2024-04-24 03:58:22.000000 quaxed-0.3.8/docs/index.md
--rw-r--r--   0        0        0      945 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/__init__.py
--rw-r--r--   0        0        0     1728 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/_jax.py
--rw-r--r--   0        0        0      411 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/_version.py
--rw-r--r--   0        0        0       82 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/_version.pyi
--rw-r--r--   0        0        0      620 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/lax.py
--rw-r--r--   0        0        0      407 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/operator.py
--rw-r--r--   0        0        0     2044 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/operator.pyi
--rw-r--r--   0        0        0        0 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/py.typed
--rw-r--r--   0        0        0     1687 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/__init__.py
--rw-r--r--   0        0        0      145 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_constants.py
--rw-r--r--   0        0        0     7836 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_creation_functions.py
--rw-r--r--   0        0        0      882 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_data_type_functions.py
--rw-r--r--   0        0        0       89 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_dispatch.py
--rw-r--r--   0        0        0     6639 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_elementwise_functions.py
--rw-r--r--   0        0        0      287 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_indexing_functions.py
--rw-r--r--   0        0        0      756 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_linear_algebra_functions.py
--rw-r--r--   0        0        0     1716 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_manipulation_functions.py
--rw-r--r--   0        0        0      772 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_searching_functions.py
--rw-r--r--   0        0        0      630 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_set_functions.py
--rw-r--r--   0        0        0      623 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_sorting_functions.py
--rw-r--r--   0        0        0     1913 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_statistical_functions.py
--rw-r--r--   0        0        0      707 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_types.py
--rw-r--r--   0        0        0      569 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_utility_functions.py
--rw-r--r--   0        0        0      158 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/_utils.py
--rw-r--r--   0        0        0     3447 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/fft.py
--rw-r--r--   0        0        0     3714 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/array_api/linalg.py
--rw-r--r--   0        0        0      253 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/numpy/__init__.py
--rw-r--r--   0        0        0     8948 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/numpy/_core.py
--rw-r--r--   0        0        0       84 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/scipy/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/scipy/special.py
--rw-r--r--   0        0        0     1925 2024-04-24 03:58:22.000000 quaxed-0.3.8/src/quaxed/scipy/special.pyi
--rw-r--r--   0        0        0       21 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0    38885 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/myarray.py
--rw-r--r--   0        0        0      177 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/test_package.py
--rw-r--r--   0        0        0       31 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/array_api/__init__.py
--rw-r--r--   0        0        0     1710 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/array_api/test_jax.py
--rw-r--r--   0        0        0    35919 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/array_api/test_myarray.py
--rw-r--r--   0        0        0       27 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/numpy/__init__.py
--rw-r--r--   0        0        0     1784 2024-04-24 03:58:22.000000 quaxed-0.3.8/tests/numpy/test_jax.py
--rw-r--r--   0        0        0     2218 2024-04-24 03:58:22.000000 quaxed-0.3.8/.gitignore
--rw-r--r--   0        0        0     1528 2024-04-24 03:58:22.000000 quaxed-0.3.8/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-24 03:58:22.000000 quaxed-0.3.8/README.md
--rw-r--r--   0        0        0     4254 2024-04-24 03:58:22.000000 quaxed-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3289 2024-04-24 03:58:22.000000 quaxed-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-04-25 15:09:51.000000 quaxed-0.4/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-25 15:09:51.000000 quaxed-0.4/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-25 15:09:51.000000 quaxed-0.4/.gitattributes
+-rw-r--r--   0        0        0     2900 2024-04-25 15:09:51.000000 quaxed-0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-25 15:09:51.000000 quaxed-0.4/.readthedocs.yml
+-rw-r--r--   0        0        0     2778 2024-04-25 15:09:51.000000 quaxed-0.4/noxfile.py
+-rw-r--r--   0        0        0     2387 2024-04-25 15:09:51.000000 quaxed-0.4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-25 15:09:51.000000 quaxed-0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-25 15:09:51.000000 quaxed-0.4/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1539 2024-04-25 15:09:51.000000 quaxed-0.4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1641 2024-04-25 15:09:51.000000 quaxed-0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      834 2024-04-25 15:09:51.000000 quaxed-0.4/docs/conf.py
+-rw-r--r--   0        0        0      193 2024-04-25 15:09:51.000000 quaxed-0.4/docs/index.md
+-rw-r--r--   0        0        0      945 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/__init__.py
+-rw-r--r--   0        0        0     1728 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_jax.py
+-rw-r--r--   0        0        0      707 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_types.py
+-rw-r--r--   0        0        0      231 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_utils.py
+-rw-r--r--   0        0        0      406 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_version.py
+-rw-r--r--   0        0        0       82 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/_version.pyi
+-rw-r--r--   0        0        0      620 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/lax.py
+-rw-r--r--   0        0        0      407 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/operator.py
+-rw-r--r--   0        0        0     2044 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/operator.pyi
+-rw-r--r--   0        0        0        0 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/py.typed
+-rw-r--r--   0        0        0     1764 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_constants.py
+-rw-r--r--   0        0        0     7849 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_creation_functions.py
+-rw-r--r--   0        0        0      894 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_data_type_functions.py
+-rw-r--r--   0        0        0      124 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_dispatch.py
+-rw-r--r--   0        0        0     6645 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_elementwise_functions.py
+-rw-r--r--   0        0        0      293 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_indexing_functions.py
+-rw-r--r--   0        0        0      762 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_linear_algebra_functions.py
+-rw-r--r--   0        0        0     1722 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_manipulation_functions.py
+-rw-r--r--   0        0        0      778 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_searching_functions.py
+-rw-r--r--   0        0        0      636 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_set_functions.py
+-rw-r--r--   0        0        0      629 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_sorting_functions.py
+-rw-r--r--   0        0        0     1925 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_statistical_functions.py
+-rw-r--r--   0        0        0      575 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/_utility_functions.py
+-rw-r--r--   0        0        0     3453 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/fft.py
+-rw-r--r--   0        0        0     3726 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/array_api/linalg.py
+-rw-r--r--   0        0        0      532 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/__init__.py
+-rw-r--r--   0        0        0     9218 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_core.py
+-rw-r--r--   0        0        0     5767 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_creation_functions.py
+-rw-r--r--   0        0        0      106 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_dispatch.py
+-rw-r--r--   0        0        0     7533 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/_higher_order.py
+-rw-r--r--   0        0        0       60 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/fft.py
+-rw-r--r--   0        0        0       63 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/numpy/linalg.py
+-rw-r--r--   0        0        0       84 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/scipy/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/scipy/special.py
+-rw-r--r--   0        0        0     1925 2024-04-25 15:09:51.000000 quaxed-0.4/src/quaxed/scipy/special.pyi
+-rw-r--r--   0        0        0       21 2024-04-25 15:09:51.000000 quaxed-0.4/tests/__init__.py
+-rw-r--r--   0        0        0    38875 2024-04-25 15:09:51.000000 quaxed-0.4/tests/myarray.py
+-rw-r--r--   0        0        0      177 2024-04-25 15:09:51.000000 quaxed-0.4/tests/test_package.py
+-rw-r--r--   0        0        0       31 2024-04-25 15:09:51.000000 quaxed-0.4/tests/array_api/__init__.py
+-rw-r--r--   0        0        0     1710 2024-04-25 15:09:51.000000 quaxed-0.4/tests/array_api/test_jax.py
+-rw-r--r--   0        0        0    35919 2024-04-25 15:09:51.000000 quaxed-0.4/tests/array_api/test_myarray.py
+-rw-r--r--   0        0        0       27 2024-04-25 15:09:51.000000 quaxed-0.4/tests/numpy/__init__.py
+-rw-r--r--   0        0        0    50801 2024-04-25 15:09:51.000000 quaxed-0.4/tests/numpy/test_jax.py
+-rw-r--r--   0        0        0     2218 2024-04-25 15:09:51.000000 quaxed-0.4/.gitignore
+-rw-r--r--   0        0        0     1528 2024-04-25 15:09:51.000000 quaxed-0.4/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-25 15:09:51.000000 quaxed-0.4/README.md
+-rw-r--r--   0        0        0     4291 2024-04-25 15:09:51.000000 quaxed-0.4/pyproject.toml
+-rw-r--r--   0        0        0     3287 2024-04-25 15:09:51.000000 quaxed-0.4/PKG-INFO
```

### Comparing `quaxed-0.3.8/.pre-commit-config.yaml` & `quaxed-0.4/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,31 @@
   autofix_commit_msg: "style: pre-commit fixes"
   autoupdate_schedule: "monthly"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.21.3
+    rev: v3.24.0
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
 
   - repo: meta
     hooks:
       - id: check-useless-excludes
 
   - repo: https://github.com/scientific-python/cookie
-    rev: 2024.03.10
+    rev: 2024.04.23
     hooks:
       - id: sp-repo-review
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -43,22 +43,22 @@
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
@@ -74,15 +74,15 @@
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.9.0"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         files: src
         additional_dependencies:
           - pytest
         exclude: |
           (?x)^(
```

### Comparing `quaxed-0.3.8/noxfile.py` & `quaxed-0.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/.github/CONTRIBUTING.md` & `quaxed-0.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/.github/matchers/pylint.json` & `quaxed-0.4/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/.github/workflows/cd.yml` & `quaxed-0.4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/.github/workflows/ci.yml` & `quaxed-0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/docs/conf.py` & `quaxed-0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/__init__.py` & `quaxed-0.4/src/quaxed/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/_jax.py` & `quaxed-0.4/src/quaxed/_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/lax.py` & `quaxed-0.4/src/quaxed/lax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/operator.pyi` & `quaxed-0.4/src/quaxed/operator.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/array_api/__init__.py` & `quaxed-0.4/src/quaxed/array_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from jaxtyping import install_import_hook
 
 with install_import_hook("quaxed", None):
     from . import (
         _constants,
         _creation_functions,
         _data_type_functions,
+        _dispatch,
         _elementwise_functions,
         _indexing_functions,
         _linear_algebra_functions,
         _manipulation_functions,
         _searching_functions,
         _set_functions,
         _sorting_functions,
@@ -24,14 +25,15 @@
         _utility_functions,
         fft,
         linalg,
     )
     from ._constants import *
     from ._creation_functions import *
     from ._data_type_functions import *
+    from ._dispatch import *
     from ._elementwise_functions import *
     from ._indexing_functions import *
     from ._linear_algebra_functions import *
     from ._manipulation_functions import *
     from ._searching_functions import *
     from ._set_functions import *
     from ._sorting_functions import *
@@ -47,7 +49,8 @@
 __all__ += _linear_algebra_functions.__all__
 __all__ += _manipulation_functions.__all__
 __all__ += _searching_functions.__all__
 __all__ += _set_functions.__all__
 __all__ += _sorting_functions.__all__
 __all__ += _statistical_functions.__all__
 __all__ += _utility_functions.__all__
+__all__ += _dispatch.__all__
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_creation_functions.py` & `quaxed-0.4/src/quaxed/array_api/_creation_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 import jax
 import jax.numpy as jnp
 from jax import Device
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
+from quaxed._types import DType
+from quaxed._utils import quaxify
+
 from ._dispatch import dispatcher
-from ._types import DType
-from ._utils import quaxify
 
 T = TypeVar("T")
 
 # =============================================================================
 
 
 @dispatcher
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_data_type_functions.py` & `quaxed-0.4/src/quaxed/array_api/_data_type_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 __all__ = ["astype", "can_cast", "finfo", "iinfo", "isdtype", "result_type"]
 
 
 from jax.experimental import array_api
 from jax.experimental.array_api._data_type_functions import FInfo, IInfo
 from jaxtyping import ArrayLike
 
-from ._types import DType
-from ._utils import quaxify
+from quaxed._types import DType
+from quaxed._utils import quaxify
 
 
 @quaxify
 def astype(x: ArrayLike, dtype: DType, /, *, copy: bool = True) -> ArrayLike:
     return array_api.astype(x, dtype, copy=copy)
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_elementwise_functions.py` & `quaxed-0.4/src/quaxed/array_api/_elementwise_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ]
 
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def abs(x: ArrayLike, /) -> Value:
     return array_api.abs(x)
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_linear_algebra_functions.py` & `quaxed-0.4/src/quaxed/array_api/_linear_algebra_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from collections.abc import Sequence
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def matmul(x1: ArrayLike, x2: ArrayLike, /) -> Value:
     return array_api.matmul(x1, x2)
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_manipulation_functions.py` & `quaxed-0.4/src/quaxed/array_api/_manipulation_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "stack",
 ]
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def broadcast_arrays(*arrays: ArrayLike) -> list[Value]:
     return array_api.broadcast_arrays(*arrays)
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_searching_functions.py` & `quaxed-0.4/src/quaxed/array_api/_searching_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ["argmax", "argmin", "nonzero", "where"]
 
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def argmax(
     x: ArrayLike,
     /,
     *,
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_set_functions.py` & `quaxed-0.4/src/quaxed/array_api/_set_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ["unique_all", "unique_counts", "unique_inverse", "unique_values"]
 
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def unique_all(x: ArrayLike, /) -> tuple[Value, Value, Value, Value]:
     return array_api.unique_all(x)
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_statistical_functions.py` & `quaxed-0.4/src/quaxed/array_api/_statistical_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 __all__ = ["max", "mean", "min", "prod", "std", "sum", "var"]
 
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._types import DType
-from ._utils import quaxify
+from quaxed._types import DType
+from quaxed._utils import quaxify
 
 
 @quaxify
 def max(  # pylint: disable=redefined-builtin
     x: ArrayLike,
     /,
     *,
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_types.py` & `quaxed-0.4/src/quaxed/_types.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/array_api/_utility_functions.py` & `quaxed-0.4/src/quaxed/array_api/_utility_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __all__ = ["all", "any"]
 
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def all(
     x: ArrayLike,
     /,
     *,
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/fft.py` & `quaxed-0.4/src/quaxed/array_api/fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Literal
 
 from jax import Device
 from jax.experimental.array_api import fft as _jax_fft
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._utils import quaxify
+from quaxed._utils import quaxify
 
 
 @quaxify
 def fft(
     x: ArrayLike,
     /,
     *,
```

### Comparing `quaxed-0.3.8/src/quaxed/array_api/linalg.py` & `quaxed-0.4/src/quaxed/array_api/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from typing import Literal
 
 import jax.numpy as jnp
 from jax.experimental import array_api
 from jaxtyping import ArrayLike
 from quax import Value
 
-from ._types import DType
-from ._utils import quaxify
+from quaxed._types import DType
+from quaxed._utils import quaxify
 
 
 @quaxify
 def cholesky(x: ArrayLike, /, *, upper: bool = False) -> Value:
     return array_api.linalg.cholesky(x, upper=upper)
```

### Comparing `quaxed-0.3.8/src/quaxed/numpy/_core.py` & `quaxed-0.4/src/quaxed/numpy/_higher_order.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,26 @@
 """Quaxed :mod:`jax.numpy`."""
 
-__all__ = [
-    "allclose",
-    "array_equal",
-    "asarray",
-    "arctan2",
-    "cbrt",
-    "copy",
-    "cross",
-    "equal",
-    "exp2",
-    "expand_dims",
-    "greater",
-    "hypot",
-    "isclose",
-    "log",
-    "log10",
-    "matmul",
-    "moveaxis",
-    "power",
-    "squeeze",
-    "tan",
-    "trace",
-    "vectorize",
-]
+__all__ = ["vectorize"]
 
 import functools
 from collections.abc import Callable, Collection
 from typing import Any, TypeVar
 
 import jax
-import jax.numpy as jnp
 from jax._src.numpy.vectorize import (
     _apply_excluded,
     _check_output_dims,
     _parse_gufunc_signature,
     _parse_input_dimensions,
 )
-from quax import quaxify
-
-T = TypeVar("T")
-
-
-# ============================================================================
-# Helper functions
 
+from ._core import asarray, expand_dims, squeeze
 
-def _doc(jax_func: Callable[..., Any]) -> Callable[[T], T]:
-    """Copy docstrings from JAX functions."""
-
-    def transfer_doc(func: T) -> T:
-        """Copy docstrings from JAX functions."""
-        func.__doc__ = jax_func.__doc__
-        return func
-
-    return transfer_doc
-
-
-##############################################################################
-# Quaxified `jax.numpy` namespace
-
-
-allclose = quaxify(jnp.allclose)
-array_equal = quaxify(jnp.array_equal)
-asarray = quaxify(jnp.asarray)
-arctan2 = quaxify(jnp.arctan2)
-cbrt = quaxify(jnp.cbrt)
-copy = quaxify(jnp.copy)
-cross = quaxify(jnp.cross)
-equal = quaxify(jnp.equal)
-exp2 = quaxify(jnp.exp2)
-expand_dims = quaxify(jnp.expand_dims)
-greater = quaxify(jnp.greater)
-hypot = quaxify(jnp.hypot)
-isclose = quaxify(jnp.isclose)
-log = quaxify(jnp.log)
-log10 = quaxify(jnp.log10)
-matmul = quaxify(jnp.matmul)
-moveaxis = quaxify(jnp.moveaxis)
-power = quaxify(jnp.power)
-squeeze = quaxify(jnp.squeeze)
-tan = quaxify(jnp.tan)
-trace = quaxify(jnp.trace)
-
-
-# =====================================
-# `jax.numpy.vectorize`
+T = TypeVar("T")
 
 
 def vectorize(  # noqa: C901
     pyfunc: Callable[..., Any],
     *,
     excluded: Collection[int | str] = frozenset(),
     signature: str | None = None,
@@ -245,14 +176,15 @@
             else:
                 vectorized_func = jax.vmap(vectorized_func, in_axes)
         result = vectorized_func(*squeezed_args)
 
         if not dims_to_expand:
             out = result
         elif isinstance(result, tuple):
-            out = tuple(expand_dims(r, axis=dims_to_expand) for r in result)
+            dims_to_expand_ = tuple(dims_to_expand)
+            out = tuple(expand_dims(r, axis=dims_to_expand_) for r in result)
         else:
-            out = expand_dims(result, axis=dims_to_expand)
+            out = expand_dims(result, axis=tuple(dims_to_expand))
 
         return out
 
     return wrapped
```

### Comparing `quaxed-0.3.8/src/quaxed/scipy/special.py` & `quaxed-0.4/src/quaxed/scipy/special.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/src/quaxed/scipy/special.pyi` & `quaxed-0.4/src/quaxed/scipy/special.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/tests/myarray.py` & `quaxed-0.4/tests/myarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from jax import Device, lax
 from jax._src.lax.lax import DotDimensionNumbers, PrecisionLike
 from jax._src.lax.slicing import GatherDimensionNumbers, GatherScatterMode
 from jax._src.typing import DTypeLike, Shape
 from jaxtyping import ArrayLike
 from quax import ArrayValue, register
 
+from quaxed._types import DType
 from quaxed.array_api._dispatch import dispatcher
-from quaxed.array_api._types import DType
 
 
 class MyArray(ArrayValue):
     """A :class:`quax.ArrayValue` that is dense.
 
     This is different from :class:`quax.MyArray` only in that
     `quax` will not attempt to convert it to a JAX array.
```

### Comparing `quaxed-0.3.8/tests/array_api/test_jax.py` & `quaxed-0.4/tests/array_api/test_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/tests/array_api/test_myarray.py` & `quaxed-0.4/tests/array_api/test_myarray.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/.gitignore` & `quaxed-0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/LICENSE` & `quaxed-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/README.md` & `quaxed-0.4/README.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.3.8/pyproject.toml` & `quaxed-0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     "ANN101", # Missing type annotation for self in method
     "ANN401", # Dynamically typed expressions (typing.Any) are disallowed  # TODO
     "ARG001", # Unused function argument
     "COM812", # Missing trailing comma
     "D103",   # Missing docstring in public function  # TODO
     "D203",   # one-blank-line-before-class
     "D213",   # Multi-line docstring summary should start at the second line
+    "ISC001", # handled by formatter
     "ERA001", # Found commented-out code
     "F811",   # Redefinition of unused variable  <- plum
     "FIX002", # Line contains TODO, consider resolving the issue
     "PD011",  # Pandas
     "PYI041", # Use `float` instead of `int | float`
     "TD002",  # Missing author in TODO; try: `# TODO(<author_name>): .
     "TD003",  # Missing issue link on the line following this TODO
```

### Comparing `quaxed-0.3.8/PKG-INFO` & `quaxed-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quaxed
-Version: 0.3.8
+Version: 0.4
 Summary: Array-API JAX compatibility
 Project-URL: Homepage, https://github.com/GalacticDynamics/quaxed
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/quaxed/issues
 Project-URL: Discussions, https://github.com/GalacticDynamics/quaxed/discussions
 Project-URL: Changelog, https://github.com/GalacticDynamics/quaxed/releases
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License-File: LICENSE
```


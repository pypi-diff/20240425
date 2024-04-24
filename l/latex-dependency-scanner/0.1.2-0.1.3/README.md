# Comparing `tmp/latex_dependency_scanner-0.1.2.tar.gz` & `tmp/latex_dependency_scanner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_dependency_scanner-0.1.2.tar", last modified: Sun Oct  1 22:21:03 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `latex_dependency_scanner-0.1.2.tar` & `latex_dependency_scanner-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.224012 latex_dependency_scanner-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-01 22:21:03.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2023-10-01 22:20:53.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 22:21:03.228011 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-10-01 22:21:03.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-01 22:21:03.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-01 22:21:03.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-01 22:21:02.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-01 22:21:03.000000 latex_dependency_scanner-0.1.2/src/latex_dependency_scanner.egg-info/top_level.txt
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/_version.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/compile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/py.typed
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/scanner.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/README.md
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 latex_dependency_scanner-0.1.3/PKG-INFO
```

### Comparing `latex_dependency_scanner-0.1.2/LICENSE` & `latex_dependency_scanner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latex_dependency_scanner-0.1.2/PKG-INFO` & `latex_dependency_scanner-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: latex_dependency_scanner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Scan LaTeX documents for their dependencies.
-Home-page: https://github.com/pytask-dev/latex-dependency-scanner
-Author: Tobias Raabe
-Author-email: raabe@posteo.de
-License: MIT
+Project-URL: Homepage, https://github.com/pytask-dev/latex-dependency-scanner
 Project-URL: Changelog, https://github.com/pytask-dev/latex-dependency-scanner/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/pytask-dev/latex-dependency-scanner
 Project-URL: Github, https://github.com/pytask-dev/latex-dependency-scanner
 Project-URL: Tracker, https://github.com/pytask-dev/latex-dependency-scanner/issues
-Platform: any
+Author-email: Tobias Raabe <raabe@posteo.de>
+License: MIT
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Provides-Extra: test
+Requires-Dist: pytest-cov>=5.0.0; extra == 'test'
+Requires-Dist: pytest>=8.1.1; extra == 'test'
+Provides-Extra: typing
+Requires-Dist: mypy>=1.10.0; extra == 'typing'
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/latex-dependency-scanner)](https://pypi.org/project/latex-dependency-scanner)
 [![image](https://img.shields.io/conda/vn/conda-forge/latex-dependency-scanner.svg)](https://anaconda.org/conda-forge/latex-dependency-scanner)
 [![image](https://img.shields.io/conda/pn/conda-forge/latex-dependency-scanner.svg)](https://anaconda.org/conda-forge/latex-dependency-scanner)
 [![PyPI - License](https://img.shields.io/pypi/l/latex-dependency-scanner)](https://pypi.org/project/latex-dependency-scanner)
 [![image](https://img.shields.io/github/actions/workflow/status/pytask-dev/latex-dependency-scanner/main.yml?branch=main)](https://github.com/pytask-dev/latex-dependency-scanner/actions?query=branch%3Amain)
 [![image](https://codecov.io/gh/pytask-dev/latex-dependency-scanner/branch/main/graph/badge.svg)](https://app.codecov.io/gh/pytask-dev/latex-dependency-scanner)
```

### Comparing `latex_dependency_scanner-0.1.2/README.md` & `latex_dependency_scanner-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/compile.py` & `latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/compile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-"""This module provides the means to compile a LaTeX document to a desired location.
+"""Provides the means to compile a LaTeX document to a desired location.
 
 The function is mainly used in testing to validate the provided examples, but can also
 be used by users to compile their documents.
 
 """
+
 from __future__ import annotations
 
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from subprocess import CompletedProcess
 
-
 DEFAULT_OPTIONS = ["--pdf", "--interaction=nonstopmode", "--synctex=1", "--cd"]
 
 
 def compile_pdf(
     latex_document: Path,
     compiled_document: Path | None = None,
     args: list[str] | None = None,
 ) -> CompletedProcess[bytes]:
     """Generate a PDF from LaTeX document."""
     if shutil.which("latexmk") is None:
-        raise RuntimeError("'latexmk' must be on PATH to compile a LaTeX document.")
+        msg = "'latexmk' must be on PATH to compile a LaTeX document."
+        raise RuntimeError(msg)
 
     cmd = _prepare_cmd_options(latex_document, compiled_document, args)
     return subprocess.run(cmd, check=True)  # noqa: S603
 
 
 def _prepare_cmd_options(
     latex_document: Path,
```

### Comparing `latex_dependency_scanner-0.1.2/src/latex_dependency_scanner/scanner.py` & `latex_dependency_scanner-0.1.3/src/latex_dependency_scanner/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Includes the ability to scan a LaTeX document."""
+
 from __future__ import annotations
 
 import re
 from pathlib import Path
 from typing import Generator
 
-
 COMMON_TEX_EXTENSIONS = [".ltx", ".tex"]
 """List[str]: List of typical file extensions that contain latex"""
 
 
 COMMON_GRAPHICS_EXTENSIONS = [
     # Image formats.
     ".eps",
@@ -159,13 +159,15 @@
                             yield path_w_ext
 
                         # Stop loop, if a file has been found.
                         break
 
                 if not found_some_file:
                     possible_paths = (
-                        (relative_to / path).resolve().with_suffix(suffix)
-                        if suffix
-                        else (relative_to / path).resolve()
+                        (
+                            (relative_to / path).resolve().with_suffix(suffix)
+                            if suffix
+                            else (relative_to / path).resolve()
+                        )
                         for suffix in common_extensions
                     )
                     yield from possible_paths
```


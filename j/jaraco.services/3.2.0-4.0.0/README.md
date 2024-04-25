# Comparing `tmp/jaraco.services-3.2.0.tar.gz` & `tmp/jaraco_services-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.services-3.2.0.tar", last modified: Sat Jul 29 18:12:48 2023, max compression
+gzip compressed data, was "jaraco_services-4.0.0.tar", last modified: Thu Apr 25 06:55:18 2024, max compression
```

## Comparing `jaraco.services-3.2.0.tar` & `jaraco_services-4.0.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.518076 jaraco.services-3.2.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/jaraco/services/
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/jaraco/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/jaraco/services/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.526076 jaraco.services-3.2.0/jaraco.services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 18:12:48.000000 jaraco.services-3.2.0/jaraco.services.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:12:48.530076 jaraco.services-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-29 18:12:13.000000 jaraco.services-3.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.758756 jaraco_services-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.754756 jaraco_services-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.754756 jaraco_services-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-25 06:55:18.758756 jaraco_services-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.754756 jaraco_services-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.750756 jaraco_services-4.0.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.754756 jaraco_services-4.0.0/jaraco/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/jaraco/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/jaraco/services/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.754756 jaraco_services-4.0.0/jaraco.services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-25 06:55:18.000000 jaraco_services-4.0.0/jaraco.services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-25 06:55:18.000000 jaraco_services-4.0.0/jaraco.services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:55:18.000000 jaraco_services-4.0.0/jaraco.services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 06:55:18.000000 jaraco_services-4.0.0/jaraco.services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 06:55:18.000000 jaraco_services-4.0.0/jaraco.services.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:55:18.758756 jaraco_services-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:18.754756 jaraco_services-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-25 06:54:57.000000 jaraco_services-4.0.0/tox.ini
```

### Comparing `jaraco.services-3.2.0/.github/workflows/main.yml` & `jaraco_services-4.0.0/.github/workflows/main.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,99 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient. For tox, it must be one of
-  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
-  # in common is "1".
+  # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
-  # MyPy's color enforcement (must be a non-zero number)
-  MYPY_FORCE_COLOR: -42
-  # Recognized by the `py` package, dependency of `pytest` (must be "1")
-  PY_COLORS: 1
-  # Make tox-wrapped tools see color requests
-  TOX_TESTENV_PASSENV: >-
-    FORCE_COLOR
-    MYPY_FORCE_COLOR
-    NO_COLOR
-    PY_COLORS
-    PYTEST_THEME
-    PYTEST_THEME_MODE
 
   # Suppress noisy pip warnings
   PIP_DISABLE_PIP_VERSION_CHECK: 'true'
   PIP_NO_PYTHON_VERSION_WARNING: 'true'
   PIP_NO_WARN_SCRIPT_LOCATION: 'true'
 
-  # Disable the spinner, noise in GHA; TODO(webknjaz): Fix this upstream
-  # Must be "1".
-  TOX_PARALLEL_NO_SPINNER: 1
+  # Ensure tests can sense settings about the environment
+  TOX_OVERRIDE: >-
+    testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' || (matrix.python == '3.8' || matrix.python == '3.9') && matrix.platform == 'macos-latest' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox
 
-  docs:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
@@ -105,20 +104,19 @@
       contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.services-3.2.0/LICENSE` & `jaraco_services-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.services-3.2.0/NEWS.rst` & `jaraco_services-4.0.0/NEWS.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+v4.0.0
+======
+
+Features
+--------
+
+- Deprecated the PythonService.
+- Marked Guard and PortFree as deprecated.
+
+
+Deprecations and Removals
+-------------------------
+
+- Removed ServiceManager.
+- Removed deprecated 'Service.find_free_port'.
+- Removed deprecated 'port' parameter to PortFree.
+
+
 v3.2.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `jaraco.services-3.2.0/README.rst` & `jaraco_services-4.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.services.svg
    :target: https://pypi.org/project/jaraco.services
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.services.svg
 
-.. image:: https://github.com/jaraco/jaraco.services/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.services/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.services/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.services-3.2.0/docs/conf.py` & `jaraco_services-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.services-3.2.0/jaraco/services/__init__.py` & `jaraco_services-4.0.0/jaraco/services/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,44 @@
 """
 This module provides a Service base class for
 modeling management of a service, typically launched as a subprocess.
-
-The ServiceManager (deprecated)
-acts as a collection of interdependent services, can monitor which are
-running, and will start services on demand. The use case for ServiceManager
-has been superseded by the more elegant `pytest fixtures
-<https://pytest.org/latest/fixture.html>`_ model.
 """
 
 import os
 import sys
 import logging
 import time
 import re
 import datetime
 import functools
-import warnings
 import subprocess
 import urllib.request
-from typing import Set
+import warnings
 
 import path
 import portend
 from tempora.timing import Stopwatch
 from jaraco.classes import properties
 
 
 __all__ = [
-    'ServiceManager',
     'Guard',
     'HTTPStatus',
     'Subprocess',
-    'Dependable',
     'Service',
 ]
 
 
 log = logging.getLogger(__name__)
 
 
 class ServiceNotRunningError(Exception):
     pass
 
 
-class ServiceManager(list):
-    """
-    A class that manages services that may be required by some of the
-    unit tests. ServiceManager will start up daemon services as
-    subprocesses or threads and will stop them when requested or when
-    destroyed.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        msg = "ServiceManager is deprecated. Use fixtures instead."
-        warnings.warn(msg, DeprecationWarning)
-        self.failed = set()
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, type, value, tb):
-        self.stop_all()
-
-    @property
-    def running(self):
-        def is_running(p):
-            return p.is_running()
-
-        return filter(is_running, self)
-
-    def start(self, service):
-        """
-        Start the service, catching and logging exceptions
-        """
-        try:
-            map(self.start_class, service.depends)
-            if service.is_running():
-                return
-            if service in self.failed:
-                log.warning("%s previously failed to start", service)
-                return
-            service.start()
-        except Exception:
-            log.exception("Unable to start service %s", service)
-            self.failed.add(service)
-
-    def start_all(self):
-        "Start all services registered with this manager"
-        for service in self:
-            self.start(service)
-
-    def start_class(self, class_):
-        """
-        Start all services of a given class. If this manager doesn't already
-        have a service of that class, it constructs one and starts it.
-        """
-        matches = filter(lambda svc: isinstance(svc, class_), self)
-        if not matches:
-            svc = class_()
-            self.register(svc)
-            matches = [svc]
-        map(self.start, matches)
-        return matches
-
-    def register(self, service):
-        self.append(service)
-
-    def stop_class(self, class_):
-        "Stop all services of a given class"
-        matches = filter(lambda svc: isinstance(svc, class_), self)
-        map(self.stop, matches)
-
-    def stop(self, service):
-        for dep_class in service.depended_by:
-            self.stop_class(dep_class)
-        service.stop()
-
-    def stop_all(self):
-        # even though we can stop services in order by dependency, still
-        #  stop in reverse order as a reasonable heuristic.
-        map(self.stop, reversed(self.running))
-
-
 class Guard:
     """
     Prevent execution of a function unless arguments pass self.allowed()
 
     >>> class OnlyInts(Guard):
     ...     def allowed(self, *args, **kwargs):
     ...         return all(isinstance(arg, int) for arg in args)
@@ -140,14 +51,19 @@
     >>> the_func(1, '1') is None
     True
     """
 
     def __call__(self, func):
         @functools.wraps(func)
         def guarded(*args, **kwargs):
+            warnings.warn(
+                "Guard is deprecated. File an issue with jaraco.services if you encounter this message.",
+                DeprecationWarning,
+                stacklevel=3,
+            )
             res = self.allowed(*args, **kwargs)
             if res:
                 return func(*args, **kwargs)
 
         return guarded
 
     def allowed(self, *args, **kwargs):
@@ -157,34 +73,33 @@
 class HTTPStatus:
     """
     Mix-in for services that have an HTTP Service for checking the status
     """
 
     proto = 'http'
     status_path = '/_status/system'
-    __url = '{self.proto}://{host}:{self.port}{path}'
-    __err = 'Received status {err.code} from {self} on {host}:{self.port}'
 
     def build_url(self, path, host='localhost'):
-        return self.__url.format(**locals())
+        return f'{self.proto}://{host}:{self.port}{path}'
 
     def wait_for_http(self, host='localhost', timeout=15):
         timeout = datetime.timedelta(seconds=timeout)
         timer = Stopwatch()
         portend.occupied(host, self.port, timeout=timeout)
 
         url = self.build_url(self.status_path)
         while True:
             try:
                 conn = urllib.request.urlopen(url)
                 break
-            # comment below workaround for PyCQA/pyflakes#376
-            except urllib.error.HTTPError as err:  # noqa: F841
+            except urllib.error.HTTPError as err:
                 if timer.split() > timeout:
-                    raise ServiceNotRunningError(self.__err.format(**locals()))
+                    raise ServiceNotRunningError(
+                        f'Received status {err.code} from {self} on {host}:{self.port}'
+                    )
                 time.sleep(0.5)
         return conn.read()
 
 
 class Subprocess:
     """
     Mix-in to handle common subprocess handling
@@ -257,50 +172,24 @@
 
     def assert_running(self):
         process_running = self.process.returncode is None
         if not process_running:
             raise RuntimeError("Process terminated")
 
     class PortFree(Guard):
-        def __init__(self, port=None):
-            if port is not None:
-                warnings.warn(
-                    "Passing port to PortFree is deprecated", DeprecationWarning
-                )
-
         def allowed(self, service, *args, **kwargs):
             port_free = service.port_free(service.port)
             if not port_free:
                 log.warning("%s already running on port %s", service, service.port)
                 service.external = True
             return port_free
 
 
-class Dependable(type):
-    """
-    Metaclass to keep track of services which are depended on
-    by others.
-
-    When a class (cls) is created which depends on another
-    (dep), the other gets a reference to cls in its depended_by
-    attribute.
-    """
-
-    def __init__(cls, name, bases, attribs):
-        type.__init__(cls, name, bases, attribs)
-        # create a set in this class for dependent services to register
-        cls.depended_by = set()
-        for dep in cls.depends:
-            dep.depended_by.add(cls)
-
-
 class Service:
     "An abstract base class for services"
-    __metaclass__ = Dependable
-    depends: Set[str] = set()
 
     def start(self):
         log.info('Starting service %s', self)
 
     def is_running(self):
         return False
 
@@ -314,20 +203,14 @@
     def port_free(port, host='localhost'):
         try:
             portend.free(host, port, timeout=0.1)
         except portend.Timeout:
             return False
         return True
 
-    @staticmethod
-    def find_free_port():
-        msg = "Use portend.find_available_local_port"
-        warnings.warn(msg, DeprecationWarning, stacklevel=2)
-        return portend.find_available_local_port()
-
 
 class PythonService(Service, Subprocess):
     """
     A service created by installing a package_spec into an environment and
     invoking a command.
     """
 
@@ -377,14 +260,18 @@
 
     def install(self):
         installer = self.installer.split()
         cmd = [self.python, '-m'] + installer + [self.package_spec]
         subprocess.check_call(cmd, env=self._run_env)
 
     def start(self):
+        warnings.warn(
+            "PythonService is deprecated. "
+            "If anyone is still using it, please file an issue with jaraco.services."
+        )
         super().start()
         self.create_env()
         self.install()
         output = (self.env_path / 'output.txt').open('ab')
         self.process = subprocess.Popen(
             self.command, env=self._run_env, stdout=output, stderr=subprocess.STDOUT
         )
```

### Comparing `jaraco.services-3.2.0/jaraco/services/paths.py` & `jaraco_services-4.0.0/jaraco/services/paths.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,12 +45,11 @@
         """
         return filter(cls.is_valid_root, cls.candidate_paths)
 
     @classmethod
     def is_valid_root(cls, root):
         try:
             cmd = [os.path.join(root, cls.exe)] + cls.args
-            with open(os.path.devnull, 'r+', encoding='utf-8') as null:
-                subprocess.check_call(cmd, stdout=null)
+            subprocess.check_call(cmd, stdout=subprocess.DEVNULL)
         except OSError:
             return False
         return True
```

### Comparing `jaraco.services-3.2.0/jaraco.services.egg-info/SOURCES.txt` & `jaraco_services-4.0.0/jaraco.services.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .readthedocs.yaml
 LICENSE
 NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
+ruff.toml
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `jaraco.services-3.2.0/setup.cfg` & `jaraco_services-4.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-[metadata]
-name = jaraco.services
-author = Jason R. Coombs
-author_email = jaraco@jaraco.com
-description = Service orchestration and pytest plugins
-long_description = file:README.rst
-url = https://github.com/jaraco/jaraco.services
-classifiers = 
-	Development Status :: 5 - Production/Stable
-	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-
-[options]
-packages = find_namespace:
-include_package_data = true
-python_requires = >=3.8
-install_requires = 
-	portend
-	path
-	tempora
-	jaraco.classes
-
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
-
-[options.extras_require]
-testing = 
-	pytest >= 6
-	pytest-checkdocs >= 2.4
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
-	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
-	pytest-enabler >= 2.2
-	pytest-ruff
-docs = 
-	sphinx >= 3.5
-	jaraco.packaging >= 9.3
-	rst.linker >= 1.9
-	furo
-	sphinx-lint
-
-[options.entry_points]
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[build-system]
+requires = ["setuptools>=61.2", "setuptools_scm[toml]>=3.4.1"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "jaraco.services"
+authors = [
+	{ name = "Jason R. Coombs", email = "jaraco@jaraco.com" },
+]
+description = "Service orchestration and pytest plugins"
+readme = "README.rst"
+classifiers = [
+	"Development Status :: 5 - Production/Stable",
+	"Intended Audience :: Developers",
+	"License :: OSI Approved :: MIT License",
+	"Programming Language :: Python :: 3",
+	"Programming Language :: Python :: 3 :: Only",
+]
+requires-python = ">=3.8"
+dependencies = [
+	"portend",
+	"path",
+	"tempora",
+	"jaraco.classes",
+]
+dynamic = ["version"]
+
+[project.urls]
+Homepage = "https://github.com/jaraco/jaraco.services"
+
+[project.optional-dependencies]
+testing = [
+	# upstream
+	"pytest >= 6, != 8.1.*",
+	"pytest-checkdocs >= 2.4",
+	"pytest-cov",
+	"pytest-mypy",
+	"pytest-enabler >= 2.2",
+	"pytest-ruff >= 0.2.1",
+
+	# local
+]
+docs = [
+	# upstream
+	"sphinx >= 3.5",
+	"jaraco.packaging >= 9.3",
+	"rst.linker >= 1.9",
+	"furo",
+	"sphinx-lint",
 
+	# local
+]
+
+[tool.setuptools_scm]
```

### Comparing `jaraco.services-3.2.0/tests/test_services.py` & `jaraco_services-4.0.0/tests/test_services.py`

 * *Files identical despite different names*


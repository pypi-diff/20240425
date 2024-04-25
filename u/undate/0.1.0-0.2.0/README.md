# Comparing `tmp/undate-0.1.0.tar.gz` & `tmp/undate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undate-0.1.0.tar", last modified: Fri Mar  3 19:34:08 2023, max compression
+gzip compressed data, was "undate-0.2.0.tar", last modified: Thu Apr 25 19:43:00 2024, max compression
```

## Comparing `undate-0.1.0.tar` & `undate-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:34:08.130012 undate-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-03 19:33:57.000000 undate-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-03-03 19:34:08.130012 undate-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-03-03 19:33:57.000000 undate-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-03 19:33:57.000000 undate-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-03 19:34:08.130012 undate-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-03 19:33:57.000000 undate-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:34:08.126012 undate-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:34:08.130012 undate-0.1.0/src/undate/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-03 19:33:57.000000 undate-0.1.0/src/undate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:34:08.130012 undate-0.1.0/src/undate/dateformat/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-03 19:33:57.000000 undate-0.1.0/src/undate/dateformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-03 19:33:57.000000 undate-0.1.0/src/undate/dateformat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-03 19:33:57.000000 undate-0.1.0/src/undate/dateformat/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-03-03 19:33:57.000000 undate-0.1.0/src/undate/undate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:34:08.130012 undate-0.1.0/src/undate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-03-03 19:34:08.000000 undate-0.1.0/src/undate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-03 19:34:08.000000 undate-0.1.0/src/undate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 19:34:08.000000 undate-0.1.0/src/undate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-03 19:34:08.000000 undate-0.1.0/src/undate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 19:34:08.000000 undate-0.1.0/src/undate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:34:08.130012 undate-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-03 19:33:57.000000 undate-0.1.0/tests/test_undate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.347567 undate-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 19:42:56.000000 undate-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-25 19:43:00.347567 undate-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-25 19:42:56.000000 undate-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-25 19:42:56.000000 undate-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-25 19:43:00.351567 undate-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 19:42:56.000000 undate-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.343567 undate-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.343567 undate-0.2.0/src/undate/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.343567 undate-0.2.0/src/undate/dateformat/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.347567 undate-0.2.0/src/undate/dateformat/edtf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/edtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/edtf/edtf.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/edtf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/edtf/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/dateformat/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-25 19:42:56.000000 undate-0.2.0/src/undate/undate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.347567 undate-0.2.0/src/undate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-25 19:43:00.000000 undate-0.2.0/src/undate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 19:43:00.000000 undate-0.2.0/src/undate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:43:00.000000 undate-0.2.0/src/undate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-25 19:43:00.000000 undate-0.2.0/src/undate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 19:43:00.000000 undate-0.2.0/src/undate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:43:00.347567 undate-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16802 2024-04-25 19:42:56.000000 undate-0.2.0/tests/test_undate.py
```

### Comparing `undate-0.1.0/LICENSE.md` & `undate-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `undate-0.1.0/PKG-INFO` & `undate-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,11 @@
-Metadata-Version: 2.1
-Name: undate
-Version: 0.1.0
-Summary: "library for working with uncertain, fuzzy, or partially unknown dates and date intervals"
-Home-page: https://github.com/dh-tech/undate-python
-Author: DHTech
-Author-email: "dhtech.community@gmail.com"
-License: "Apache License, Version 2.0"
-Project-URL: Project Home, https://github.com/dh-tech/undate-python
-Project-URL: Bug Tracker, https://github.com/dh-tech/undate-python/issues
-Keywords: "dates dating uncertainty uncertain-dates unknown partially-known digital-humanities"
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE.md
-
 # undate-python
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 **undate** is a python library for working with uncertain or partially known dates.
 
 It was initially created as part of a [DH-Tech](https://dh-tech.github.io/) hackathon in November 2022.
 
 ---
 
@@ -86,20 +58,17 @@
 
 ## Setup and initialize git flow
 
 This repository uses [git-flow](https://github.com/nvie/gitflow) branching conventions:
 - **main** will always contain the most recent release
 - **develop** branch is the latest version of work in progress
 
-Pull requests should be made against the **develop** branch.
+Pull requests for new features should be made against the **develop** branch.
 
-It is recommended to install git flow (on OSX, use brew or ports, e.g.: `brew install git-flow`;
-on Ubuntu/Debian, `apt-get install git-flow`) and then initialize it in this repository
-via `git flow init` and accept the defaults.  Then you can use `git flow feature start`
-to create feature development branches.
+It is recommended to install git flow (on OSX, use brew or ports, e.g.: `brew install git-flow`; on Ubuntu/Debian, `apt-get install git-flow`) and then initialize it in this repository via `git flow init` and accept the defaults.  Then you can use `git flow feature start` to create feature development branches.
 
 Alternately, you can check out the develop branch (`git checkout develop`)
 and create your branches manually based on develop (`git checkout -b feature/xxx-name`).
 
 ### Set up Python environment
 Use a recent version of python 3.x; recommended to use a virtualenv, e.g.
 ```
@@ -123,41 +92,68 @@
 ### Run unit tests
 Tests can be run with either `tox` or `pytest`.
 
 To run all the tests in a single test file, use pytest and specify the path to the test: `pytest tests/test_dateformat/test_base.py`
 
 To test cases by name, use pytest: `pytest -k test_str`
 
+### Check python types
+
+Python typing is currently only enforced by a CI check action using `mypy`.
+To run mypy locally, first install mypy and the necessary typing libraries:
+```sh
+pip install mypy
+mypy --install-types
+```
+
+Once mypy is installed, run `mypy src/` to check.
+
+
 ### Create documentation
 
 ```sh
 tox -e docs
 ```
 
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center"><a href="https://github.com/ColeDCrawford"><img src="https://avatars.githubusercontent.com/u/16374762?v=4?s=100" width="100px;" alt="Cole Crawford"/><br /><sub><b>Cole Crawford</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=ColeDCrawford" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3AColeDCrawford" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=ColeDCrawford" title="Tests">⚠️</a></td>
-      <td align="center"><a href="http://rlskoeser.github.io"><img src="https://avatars.githubusercontent.com/u/691231?v=4?s=100" width="100px;" alt="Rebecca Sutton Koeser"/><br /><sub><b>Rebecca Sutton Koeser</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=rlskoeser" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3Arlskoeser" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=rlskoeser" title="Tests">⚠️</a></td>
-      <td align="center"><a href="https://github.com/robcast"><img src="https://avatars.githubusercontent.com/u/1488847?v=4?s=100" width="100px;" alt="Robert Casties"/><br /><sub><b>Robert Casties</b></sub></a><br /><a href="#data-robcast" title="Data">🔣</a></td>
-      <td align="center"><a href="https://github.com/jdamerow"><img src="https://avatars.githubusercontent.com/u/8881141?v=4?s=100" width="100px;" alt="Julia Damerow"/><br /><sub><b>Julia Damerow</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=jdamerow" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3Ajdamerow" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=jdamerow" title="Tests">⚠️</a> <a href="#eventOrganizing-jdamerow" title="Event Organizing">📋</a></td>
-      <td align="center"><a href="https://github.com/maltevogl"><img src="https://avatars.githubusercontent.com/u/20907912?v=4?s=100" width="100px;" alt="Malte Vogl"/><br /><sub><b>Malte Vogl</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=maltevogl" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3Amaltevogl" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=maltevogl" title="Tests">⚠️</a> <a href="https://github.com/dh-tech/undate-python/commits?author=maltevogl" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ColeDCrawford"><img src="https://avatars.githubusercontent.com/u/16374762?v=4?s=100" width="100px;" alt="Cole Crawford"/><br /><sub><b>Cole Crawford</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=ColeDCrawford" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3AColeDCrawford" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=ColeDCrawford" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://rlskoeser.github.io"><img src="https://avatars.githubusercontent.com/u/691231?v=4?s=100" width="100px;" alt="Rebecca Sutton Koeser"/><br /><sub><b>Rebecca Sutton Koeser</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=rlskoeser" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3Arlskoeser" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=rlskoeser" title="Tests">⚠️</a> <a href="#blog-rlskoeser" title="Blogposts">📝</a> <a href="#example-rlskoeser" title="Examples">💡</a> <a href="https://github.com/dh-tech/undate-python/commits?author=rlskoeser" title="Documentation">📖</a> <a href="#platform-rlskoeser" title="Packaging/porting to new platform">📦</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/robcast"><img src="https://avatars.githubusercontent.com/u/1488847?v=4?s=100" width="100px;" alt="Robert Casties"/><br /><sub><b>Robert Casties</b></sub></a><br /><a href="#data-robcast" title="Data">🔣</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jdamerow"><img src="https://avatars.githubusercontent.com/u/8881141?v=4?s=100" width="100px;" alt="Julia Damerow"/><br /><sub><b>Julia Damerow</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=jdamerow" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3Ajdamerow" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=jdamerow" title="Tests">⚠️</a> <a href="#eventOrganizing-jdamerow" title="Event Organizing">📋</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maltevogl"><img src="https://avatars.githubusercontent.com/u/20907912?v=4?s=100" width="100px;" alt="Malte Vogl"/><br /><sub><b>Malte Vogl</b></sub></a><br /><a href="https://github.com/dh-tech/undate-python/commits?author=maltevogl" title="Code">💻</a> <a href="https://github.com/dh-tech/undate-python/pulls?q=is%3Apr+reviewed-by%3Amaltevogl" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/dh-tech/undate-python/commits?author=maltevogl" title="Tests">⚠️</a> <a href="https://github.com/dh-tech/undate-python/commits?author=maltevogl" title="Documentation">📖</a></td>
     </tr>
   </tbody>
+  <tfoot>
+    <tr>
+      <td align="center" size="13px" colspan="7">
+        <img src="https://raw.githubusercontent.com/all-contributors/all-contributors-cli/1b8533af435da9854653492b1327a23a4dbd0a10/assets/logo-small.svg">
+          <a href="https://all-contributors.js.org/docs/en/bot/usage">Add your contributions</a>
+        </img>
+      </td>
+    </tr>
+  </tfoot>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
+
+
+### Related blog posts
+
+- [by Rebecca Sutton Koeser](#blog-rlskoeser)
+  - [Join me for a DHTech hackathon? It’s an un-date!](https://dh-tech.github.io/blog/2023-02-09-hackathon-summary/) 2023-02-09 on DHTech blog
```

### Comparing `undate-0.1.0/setup.cfg` & `undate-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,37 @@
 project_urls = 
 	Project Home = https://github.com/dh-tech/undate-python
 	Bug Tracker = https://github.com/dh-tech/undate-python/issues
 keywords = "dates dating uncertainty uncertain-dates unknown partially-known digital-humanities"
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 	Typing :: Typed
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	python-dateutil
+	lark
+
+[options.package_data]
+* = 
+	*.lark
 
 [options.extras_require]
 all = 
 	%(dev)s
 	%(test)s
 dev = 
 	black>=22.10.0
@@ -47,31 +52,31 @@
 	build
 	%(docs)s
 test = 
 	pytest>=7.2
 	pytest-ordering
 	pytest-cov
 docs = 
-	sphinx
+	sphinx<7.0.0
 	sphinx_rtd_theme
 	m2r2
 
 [options.packages.find]
 where = src
 
 [tox:tox]
-envlist = py38, py39, py310, py311
+envlist = py39, py310, py311, py312
 isolated_build = True
 
 [gh-actions]
 python = 
-	3.8: py38
 	3.9: py39
 	3.10: py310
 	3.11: py311
+	3.12: py312
 
 [pytest]
 minversion = 6.0
 addopts = -ra -q
 testpaths = 
 	tests
```

### Comparing `undate-0.1.0/src/undate/dateformat/base.py` & `undate-0.2.0/src/undate/dateformat/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 returned by :meth:`BaseDateFormat.available_formatters`
 
 """
 
 import importlib
 import logging
 import pkgutil
-from typing import Dict
+from typing import Dict, Type
 from functools import lru_cache  # functools.cache not available until 3.9
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseDateFormat:
@@ -37,19 +37,20 @@
         # undate param should be of type Union[Undate, UndateInterval] but can't add type hint here because of circular import
         # convert an undate or interval to string representation for this format
         raise NotImplementedError
 
     # cache import class method to ensure we only import once
     @classmethod
     @lru_cache
-    def import_formatters(cls):
+    def import_formatters(cls) -> int:
         """Import all undate.dateformat formatters
         so that they will be included in available formatters
         even if not explicitly imported. Only import once.
         returns the count of modules imported."""
+
         logger.debug("Loading formatters under undate.dateformat")
         import undate.dateformat
 
         # load packages under this path with curent package prefix
         formatter_path = undate.dateformat.__path__
         formatter_prefix = f"{undate.dateformat.__name__}."
 
@@ -61,11 +62,11 @@
             if not modname.endswith(".base"):
                 importlib.import_module(modname)
                 import_count += 1
 
         return import_count
 
     @classmethod
-    def available_formatters(cls) -> Dict[str, "BaseDateFormat"]:
+    def available_formatters(cls) -> Dict[str, Type["BaseDateFormat"]]:
         # ensure undate formatters are imported
         cls.import_formatters()
         return {c.name: c for c in cls.__subclasses__()}  # type: ignore
```

### Comparing `undate-0.1.0/src/undate/dateformat/iso8601.py` & `undate-0.2.0/src/undate/dateformat/iso8601.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,20 @@
         # TODO: what about invalid format?
         # could be YYYY, YYYY-MM, YYYY-MM-DD, --MM-DD for single date
         # or YYYY/YYYY (etc.) for an interval
         parts: List[str] = value.split("/")  # split in case we have a range
         if len(parts) == 1:
             return self._parse_single_date(parts[0])
         elif len(parts) == 2:
-            return UndateInterval(*[self._parse_single_date(p) for p in parts])
+            # date range; parse both parts and initialize an interval
+            start, end = [self._parse_single_date(p) for p in parts]
+            return UndateInterval(start, end)
+        else:
+            # more than two parts = unexpected input
+            raise ValueError
 
     def _parse_single_date(self, value: str) -> Undate:
         # split single iso date into parts; convert to int or None
         # special case: missing year
         date_parts: List[Union[int, None]] = []
         if value.startswith("--"):
             date_parts.append(None)  # year unknown
@@ -44,23 +49,22 @@
         return Undate(*date_parts)  # type: ignore
 
     def to_string(self, undate: Undate) -> str:
         # serialize to iso format for simplicity, for now
         date_parts: List[Union[str, None]] = []
         # for each part of the date that is known, generate the string format
         # then combine
-        for date_portion, known in undate.known_values.items():
-            if known:
+        # TODO: should error if we have year and day but no month
+        for date_portion, iso_format in self.iso_format.items():
+            if undate.is_known(date_portion):
                 # NOTE: datetime strftime for %Y for 3-digit year
                 # results in leading zero in some environments
                 # and not others; force year to always be 4 digits
                 if date_portion == "year":
                     date_parts.append("%04d" % undate.earliest.year)
                 else:
-                    date_parts.append(
-                        undate.earliest.strftime(self.iso_format[date_portion])
-                    )
+                    date_parts.append(undate.earliest.strftime(iso_format))
             elif date_portion == "year":
                 # if not known but this is year, add '-' for --MM-DD unknown year format
                 date_parts.append("-")
         # TODO: fix type error: "list[str | None]" is incompatible with "Iterable[str]"
         return "-".join(date_parts)  # type: ignore
```


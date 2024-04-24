# Comparing `tmp/hadolint_coatl-2.12.0.1rc1.tar.gz` & `tmp/hadolint_coatl-2.12.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadolint_coatl-2.12.0.1rc1.tar", last modified: Tue Mar 26 15:36:33 2024, max compression
+gzip compressed data, was "hadolint_coatl-2.12.0.2.tar", last modified: Wed Apr 24 22:17:22 2024, max compression
```

## Comparing `hadolint_coatl-2.12.0.1rc1.tar` & `hadolint_coatl-2.12.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 cesrom    (1000) cesrom    (1000)        0 2024-03-26 15:36:33.100855 hadolint_coatl-2.12.0.1rc1/
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)     1066 2024-03-25 23:47:04.000000 hadolint_coatl-2.12.0.1rc1/LICENSE
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)     1477 2024-03-26 15:36:33.100855 hadolint_coatl-2.12.0.1rc1/PKG-INFO
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)      693 2024-03-26 15:15:25.000000 hadolint_coatl-2.12.0.1rc1/README.md
-drwxr-xr-x   0 cesrom    (1000) cesrom    (1000)        0 2024-03-26 15:36:33.100855 hadolint_coatl-2.12.0.1rc1/hadolint_coatl.egg-info/
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)     1477 2024-03-26 15:36:33.000000 hadolint_coatl-2.12.0.1rc1/hadolint_coatl.egg-info/PKG-INFO
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)      203 2024-03-26 15:36:33.000000 hadolint_coatl-2.12.0.1rc1/hadolint_coatl.egg-info/SOURCES.txt
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)        1 2024-03-26 15:36:33.000000 hadolint_coatl-2.12.0.1rc1/hadolint_coatl.egg-info/dependency_links.txt
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)       11 2024-03-26 15:36:33.000000 hadolint_coatl-2.12.0.1rc1/hadolint_coatl.egg-info/top_level.txt
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)      410 2024-03-26 15:03:35.000000 hadolint_coatl-2.12.0.1rc1/pyproject.toml
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)     1932 2024-03-26 15:36:33.100855 hadolint_coatl-2.12.0.1rc1/setup.cfg
--rw-r--r--   0 cesrom    (1000) cesrom    (1000)      670 2024-03-26 00:50:27.000000 hadolint_coatl-2.12.0.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:17:22.714041 hadolint_coatl-2.12.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 22:17:18.000000 hadolint_coatl-2.12.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-24 22:17:22.714041 hadolint_coatl-2.12.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-24 22:17:18.000000 hadolint_coatl-2.12.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:17:22.714041 hadolint_coatl-2.12.0.2/hadolint_coatl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-24 22:17:22.000000 hadolint_coatl-2.12.0.2/hadolint_coatl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-24 22:17:22.000000 hadolint_coatl-2.12.0.2/hadolint_coatl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:17:22.000000 hadolint_coatl-2.12.0.2/hadolint_coatl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:17:22.000000 hadolint_coatl-2.12.0.2/hadolint_coatl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-24 22:17:18.000000 hadolint_coatl-2.12.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-24 22:17:22.714041 hadolint_coatl-2.12.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 22:17:18.000000 hadolint_coatl-2.12.0.2/setup.py
```

### Comparing `hadolint_coatl-2.12.0.1rc1/LICENSE` & `hadolint_coatl-2.12.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hadolint_coatl-2.12.0.1rc1/PKG-INFO` & `hadolint_coatl-2.12.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadolint_coatl
-Version: 2.12.0.1rc1
+Version: 2.12.0.2
 Summary: Python wrapper around invoking hadolint (https://github.com/hadolint/hadolint)
 Home-page: https://github.com/coatl-dev/hadolint-coatl
 Author: César Román
 Author-email: cesar@coatl.dev
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/cesarcoatl
 Project-URL: Source, https://github.com/coatl-dev/hadolint-coatl
@@ -15,15 +15,19 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hadolint-coatl
 
-A python wrapper to provide a pip-installable [hadolint] binary.
+[![PyPI - Version](https://img.shields.io/pypi/v/hadolint-coatl)](https://pypi.org/project/hadolint-coatl)
+[![Downloads](https://static.pepy.tech/badge/hadolint-coatl)](https://pepy.tech/project/hadolint-coatl)
+
+A python wrapper to provide a pip-installable [hadolint] binary. Inspired by
+[shellcheck-py].
 
 Internally this package provides a convenient way to download the pre-built
 hadolint binary for your particular platform.
 
 ### installation
 
 ```bash
@@ -38,15 +42,16 @@
 ### As a pre-commit hook
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
--   repo: https://github.com/coatl-dev/hadolint-coatl
-    rev: 2.12.0.1rc1
+  - repo: https://github.com/coatl-dev/hadolint-coatl
+    rev: 2.12.0.2
     hooks:
-    -   id: hadolint
+      - id: hadolint
 ```
 
 [hadolint]: https://github.com/hadolint/hadolint
 [pre-commit]: https://pre-commit.com
+[shellcheck-py]: https://github.com/shellcheck-py/shellcheck-py
```

### Comparing `hadolint_coatl-2.12.0.1rc1/README.md` & `hadolint_coatl-2.12.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # hadolint-coatl
 
-A python wrapper to provide a pip-installable [hadolint] binary.
+[![PyPI - Version](https://img.shields.io/pypi/v/hadolint-coatl)](https://pypi.org/project/hadolint-coatl)
+[![Downloads](https://static.pepy.tech/badge/hadolint-coatl)](https://pepy.tech/project/hadolint-coatl)
+
+A python wrapper to provide a pip-installable [hadolint] binary. Inspired by
+[shellcheck-py].
 
 Internally this package provides a convenient way to download the pre-built
 hadolint binary for your particular platform.
 
 ### installation
 
 ```bash
@@ -19,15 +23,16 @@
 ### As a pre-commit hook
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
--   repo: https://github.com/coatl-dev/hadolint-coatl
-    rev: 2.12.0.1rc1
+  - repo: https://github.com/coatl-dev/hadolint-coatl
+    rev: 2.12.0.2
     hooks:
-    -   id: hadolint
+      - id: hadolint
 ```
 
 [hadolint]: https://github.com/hadolint/hadolint
 [pre-commit]: https://pre-commit.com
+[shellcheck-py]: https://github.com/shellcheck-py/shellcheck-py
```

### Comparing `hadolint_coatl-2.12.0.1rc1/hadolint_coatl.egg-info/PKG-INFO` & `hadolint_coatl-2.12.0.2/hadolint_coatl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadolint_coatl
-Version: 2.12.0.1rc1
+Version: 2.12.0.2
 Summary: Python wrapper around invoking hadolint (https://github.com/hadolint/hadolint)
 Home-page: https://github.com/coatl-dev/hadolint-coatl
 Author: César Román
 Author-email: cesar@coatl.dev
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/cesarcoatl
 Project-URL: Source, https://github.com/coatl-dev/hadolint-coatl
@@ -15,15 +15,19 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hadolint-coatl
 
-A python wrapper to provide a pip-installable [hadolint] binary.
+[![PyPI - Version](https://img.shields.io/pypi/v/hadolint-coatl)](https://pypi.org/project/hadolint-coatl)
+[![Downloads](https://static.pepy.tech/badge/hadolint-coatl)](https://pepy.tech/project/hadolint-coatl)
+
+A python wrapper to provide a pip-installable [hadolint] binary. Inspired by
+[shellcheck-py].
 
 Internally this package provides a convenient way to download the pre-built
 hadolint binary for your particular platform.
 
 ### installation
 
 ```bash
@@ -38,15 +42,16 @@
 ### As a pre-commit hook
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
--   repo: https://github.com/coatl-dev/hadolint-coatl
-    rev: 2.12.0.1rc1
+  - repo: https://github.com/coatl-dev/hadolint-coatl
+    rev: 2.12.0.2
     hooks:
-    -   id: hadolint
+      - id: hadolint
 ```
 
 [hadolint]: https://github.com/hadolint/hadolint
 [pre-commit]: https://pre-commit.com
+[shellcheck-py]: https://github.com/shellcheck-py/shellcheck-py
```

### Comparing `hadolint_coatl-2.12.0.1rc1/setup.cfg` & `hadolint_coatl-2.12.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hadolint_coatl
-version = 2.12.0.1rc1
+version = 2.12.0.2
 description = Python wrapper around invoking hadolint (https://github.com/hadolint/hadolint)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/coatl-dev/hadolint-coatl
 author = César Román
 author_email = cesar@coatl.dev
 license = MIT
@@ -30,14 +30,19 @@
 	group = hadolint-binary
 	marker = sys_platform == "darwin" and platform_machine == "arm64"
 	marker = sys_platform == "darwin" and platform_machine == "x86_64"
 	url = https://github.com/hadolint/hadolint/releases/download/v2.12.0/hadolint-Darwin-x86_64
 	sha256 = 2a5b7afcab91645c39a7cebefcd835b865f7488e69be24567f433dfc3d41cd27
 	[hadolint]
 	group = hadolint-binary
+	marker = sys_platform == "linux" and platform_machine == "aarch64"
+	url = https://github.com/hadolint/hadolint/releases/download/v2.12.0/hadolint-Linux-arm64
+	sha256 = 5798551bf19f33951881f15eb238f90aef023f11e7ec7e9f4c37961cb87c5df6
+	[hadolint]
+	group = hadolint-binary
 	marker = sys_platform == "linux" and platform_machine == "x86_64"
 	url = https://github.com/hadolint/hadolint/releases/download/v2.12.0/hadolint-Linux-x86_64
 	sha256 = 56de6d5e5ec427e17b74fa48d51271c7fc0d61244bf5c90e828aab8362d55010
 	[hadolint.exe]
 	group = hadolint-binary
 	marker = sys_platform == "win32" and platform_machine == "AMD64"
 	marker = sys_platform == "win32" and platform_machine == "ARM64"
```

### Comparing `hadolint_coatl-2.12.0.1rc1/setup.py` & `hadolint_coatl-2.12.0.2/setup.py`

 * *Files identical despite different names*


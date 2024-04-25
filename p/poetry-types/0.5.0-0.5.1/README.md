# Comparing `tmp/poetry_types-0.5.0.tar.gz` & `tmp/poetry_types-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_types-0.5.0.tar", max compression
+gzip compressed data, was "poetry_types-0.5.1.tar", max compression
```

## Comparing `poetry_types-0.5.0.tar` & `poetry_types-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-08-23 09:23:20.808768 poetry_types-0.5.0/LICENSE
--rw-r--r--   0        0        0     1475 2023-08-23 09:23:20.808768 poetry_types-0.5.0/README.md
--rw-r--r--   0        0        0      145 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/commands/__init__.py
--rw-r--r--   0        0        0      981 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/commands/add_types.py
--rw-r--r--   0        0        0     8409 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/commands/base.py
--rw-r--r--   0        0        0     1076 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/commands/remove_types.py
--rw-r--r--   0        0        0     2750 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/commands/update_types.py
--rw-r--r--   0        0        0      163 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/packages_map.py
--rw-r--r--   0        0        0      544 2023-08-23 09:23:20.808768 poetry_types-0.5.0/poetry_types/poetry_types.py
--rw-r--r--   0        0        0     1142 2023-08-23 09:23:20.808768 poetry_types-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 poetry_types-0.5.0/setup.py
--rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 poetry_types-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-25 19:43:11.179648 poetry_types-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1459 2024-04-25 19:43:11.179648 poetry_types-0.5.1/README.md
+-rw-r--r--   0        0        0      145 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/commands/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/commands/add_types.py
+-rw-r--r--   0        0        0     8481 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/commands/base.py
+-rw-r--r--   0        0        0     1076 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/commands/remove_types.py
+-rw-r--r--   0        0        0     2750 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/commands/update_types.py
+-rw-r--r--   0        0        0      163 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/packages_map.py
+-rw-r--r--   0        0        0      544 2024-04-25 19:43:11.179648 poetry_types-0.5.1/poetry_types/poetry_types.py
+-rw-r--r--   0        0        0     1112 2024-04-25 19:43:11.179648 poetry_types-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2452 1970-01-01 00:00:00.000000 poetry_types-0.5.1/setup.py
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 poetry_types-0.5.1/PKG-INFO
```

### Comparing `poetry_types-0.5.0/LICENSE` & `poetry_types-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_types-0.5.0/README.md` & `poetry_types-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 - `poetry types add <package names>`
 - `poetry types remove <package names>`
 - `poetry types update <package names>`
 
 ## Usage examples
 
-- `poetry types add SQLAlchemy` adds `types-SQLAlchemy` to your project
-- `poetry types update` adds `types-SQLAlchemy` if `SQLAlchemy` is present, but not `types-SQLAlchemy`
-- `poetry types update` removes `types-SQLAlchemy` if `types-SQLAlchemy` is present, but not `SQLAlchemy`
+- `poetry types add openpyxl` adds `openpyxl` to your project
+- `poetry types update` adds `types-openpyxl` if `openpyxl` is present, but `types-openpyxl` is not
+- `poetry types update` removes `types-openpyxl` if `types-openpyxl` is present, but `openpyxl` is not
 
 ## Installation
 
 Run `poetry self add poetry-types` for global install or run `poetry add -D poetry-types` to use this plugin with your project.
 
 ## Usage with pre-commit
 
 ```yaml
 - repo: https://github.com/jvllmr/poetry-types
-  rev: v0.4.0
+  rev: v0.5.1
   hooks:
     - id: poetry-types
 ```
 
 ### poetry-types has to be skipped with pre-commit.ci
 
 ```yaml
```

### Comparing `poetry_types-0.5.0/poetry_types/commands/add_types.py` & `poetry_types-0.5.1/poetry_types/commands/add_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.5.0/poetry_types/commands/base.py` & `poetry_types-0.5.1/poetry_types/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,23 @@
 
     def pyproject_poetry_content(self):
         return self.pyproject_content()["tool"]["poetry"]
 
     @t.overload
     def get_types_section(
         self, create_if_not_exists: t.Literal[False]
-    ) -> tomlkit_items.Table | None:
-        ...
+    ) -> tomlkit_items.Table | None: ...
 
     @t.overload
-    def get_types_section(self) -> tomlkit_items.Table:
-        ...
+    def get_types_section(self) -> tomlkit_items.Table: ...
 
     @t.overload
     def get_types_section(
         self, create_if_not_exists: t.Literal[True]
-    ) -> tomlkit_items.Table:
-        ...
+    ) -> tomlkit_items.Table: ...
 
     def get_types_section(
         self, create_if_not_exists: bool = True
     ) -> tomlkit_items.Table:
         content = self.pyproject_content()
 
         try:
@@ -71,19 +68,23 @@
         return section
 
     def is_package_type_package_name(self, package: str):
         return package.startswith("types-") or package in PACKAGES_MAP.values()
 
     def convert_to_type_packages_names(self, packages: list[str]):
         return [
-            package
-            if package.startswith("types-")
-            else f"types-{package}"
-            if package not in PACKAGES_MAP
-            else PACKAGES_MAP[package]
+            (
+                package
+                if package.startswith("types-")
+                else (
+                    f"types-{package}"
+                    if package not in PACKAGES_MAP
+                    else PACKAGES_MAP[package]
+                )
+            )
             for package in packages
         ]
 
     def get_existing_type_packages(
         self, packages: list[str] | None = None, canonicalized=False
     ):
         """Filter packages in type section in pyproject.toml by names"""
```

### Comparing `poetry_types-0.5.0/poetry_types/commands/remove_types.py` & `poetry_types-0.5.1/poetry_types/commands/remove_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.5.0/poetry_types/commands/update_types.py` & `poetry_types-0.5.1/poetry_types/commands/update_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.5.0/poetry_types/poetry_types.py` & `poetry_types-0.5.1/poetry_types/poetry_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.5.0/pyproject.toml` & `poetry_types-0.5.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "poetry-types"
-version = "0.5.0"
+version = "0.5.1"
 description = "A poetry plugin that adds/removes type stubs as dependencies like the mypy --install-types command."
 authors = ["Jan Vollmer <jan@vllmr.dev>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/jvllmr/poetry-types"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = "^1.6"
-tomlkit = "^0.11.4"
-packaging = ">=21.3,<24.0"
+tomlkit = "<1.0"
+packaging = "<25.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.0"
-tox = "^3.0 ||^4.0"
-black = "^22.6.0 || ^23.0.0"
-ruff = "^0.0.270"
+pytest = "^8.0"
+tox = "^4.0"
+black = "<25.0.0"
+ruff = "<0.5.0"
 
 [tool.pyaphid]
 forbidden = ["print"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `poetry_types-0.5.0/setup.py` & `poetry_types-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['poetry_types', 'poetry_types.commands']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['packaging>=21.3,<24.0', 'poetry>=1.6,<2.0', 'tomlkit>=0.11.4,<0.12.0']
+['packaging<25.0', 'poetry>=1.6,<2.0', 'tomlkit<1.0']
 
 entry_points = \
 {'poetry.application.plugin': ['poetry-types = '
                                'poetry_types.poetry_types:PoetryTypes']}
 
 setup_kwargs = {
     'name': 'poetry-types',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'A poetry plugin that adds/removes type stubs as dependencies like the mypy --install-types command.',
-    'long_description': '# poetry-types\n\n[![PyPI version](https://badge.fury.io/py/poetry-types.svg)](https://badge.fury.io/py/poetry-types)\n[![GitHub license](https://img.shields.io/github/license/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/blob/master/LICENSE)\n[![GitHub issues](https://img.shields.io/github/issues/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/issues)\n![PyPI - Downloads](https://img.shields.io/pypi/dd/poetry-types)\n![Tests](https://github.com/jvllmr/poetry-types/actions/workflows/main.yml/badge.svg)\n\n## Description\n\nThis is a plugin to poetry for the upcoming poetry 1.2 plugin feature.\nIt installs/removes/updates typing stubs via following commands:\n\n- `poetry types add <package names>`\n- `poetry types remove <package names>`\n- `poetry types update <package names>`\n\n## Usage examples\n\n- `poetry types add SQLAlchemy` adds `types-SQLAlchemy` to your project\n- `poetry types update` adds `types-SQLAlchemy` if `SQLAlchemy` is present, but not `types-SQLAlchemy`\n- `poetry types update` removes `types-SQLAlchemy` if `types-SQLAlchemy` is present, but not `SQLAlchemy`\n\n## Installation\n\nRun `poetry self add poetry-types` for global install or run `poetry add -D poetry-types` to use this plugin with your project.\n\n## Usage with pre-commit\n\n```yaml\n- repo: https://github.com/jvllmr/poetry-types\n  rev: v0.4.0\n  hooks:\n    - id: poetry-types\n```\n\n### poetry-types has to be skipped with pre-commit.ci\n\n```yaml\nci:\n  skip: [poetry-types]\n```\n',
+    'long_description': '# poetry-types\n\n[![PyPI version](https://badge.fury.io/py/poetry-types.svg)](https://badge.fury.io/py/poetry-types)\n[![GitHub license](https://img.shields.io/github/license/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/blob/master/LICENSE)\n[![GitHub issues](https://img.shields.io/github/issues/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/issues)\n![PyPI - Downloads](https://img.shields.io/pypi/dd/poetry-types)\n![Tests](https://github.com/jvllmr/poetry-types/actions/workflows/main.yml/badge.svg)\n\n## Description\n\nThis is a plugin to poetry for the upcoming poetry 1.2 plugin feature.\nIt installs/removes/updates typing stubs via following commands:\n\n- `poetry types add <package names>`\n- `poetry types remove <package names>`\n- `poetry types update <package names>`\n\n## Usage examples\n\n- `poetry types add openpyxl` adds `openpyxl` to your project\n- `poetry types update` adds `types-openpyxl` if `openpyxl` is present, but `types-openpyxl` is not\n- `poetry types update` removes `types-openpyxl` if `types-openpyxl` is present, but `openpyxl` is not\n\n## Installation\n\nRun `poetry self add poetry-types` for global install or run `poetry add -D poetry-types` to use this plugin with your project.\n\n## Usage with pre-commit\n\n```yaml\n- repo: https://github.com/jvllmr/poetry-types\n  rev: v0.5.1\n  hooks:\n    - id: poetry-types\n```\n\n### poetry-types has to be skipped with pre-commit.ci\n\n```yaml\nci:\n  skip: [poetry-types]\n```\n',
     'author': 'Jan Vollmer',
     'author_email': 'jan@vllmr.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jvllmr/poetry-types',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `poetry_types-0.5.0/PKG-INFO` & `poetry_types-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: poetry-types
-Version: 0.5.0
+Version: 0.5.1
 Summary: A poetry plugin that adds/removes type stubs as dependencies like the mypy --install-types command.
 Home-page: https://github.com/jvllmr/poetry-types
 License: MIT
 Author: Jan Vollmer
 Author-email: jan@vllmr.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: packaging (>=21.3,<24.0)
+Requires-Dist: packaging (<25.0)
 Requires-Dist: poetry (>=1.6,<2.0)
-Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
+Requires-Dist: tomlkit (<1.0)
 Project-URL: Repository, https://github.com/jvllmr/poetry-types
 Description-Content-Type: text/markdown
 
 # poetry-types
 
 [![PyPI version](https://badge.fury.io/py/poetry-types.svg)](https://badge.fury.io/py/poetry-types)
 [![GitHub license](https://img.shields.io/github/license/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/blob/master/LICENSE)
@@ -36,27 +36,27 @@
 
 - `poetry types add <package names>`
 - `poetry types remove <package names>`
 - `poetry types update <package names>`
 
 ## Usage examples
 
-- `poetry types add SQLAlchemy` adds `types-SQLAlchemy` to your project
-- `poetry types update` adds `types-SQLAlchemy` if `SQLAlchemy` is present, but not `types-SQLAlchemy`
-- `poetry types update` removes `types-SQLAlchemy` if `types-SQLAlchemy` is present, but not `SQLAlchemy`
+- `poetry types add openpyxl` adds `openpyxl` to your project
+- `poetry types update` adds `types-openpyxl` if `openpyxl` is present, but `types-openpyxl` is not
+- `poetry types update` removes `types-openpyxl` if `types-openpyxl` is present, but `openpyxl` is not
 
 ## Installation
 
 Run `poetry self add poetry-types` for global install or run `poetry add -D poetry-types` to use this plugin with your project.
 
 ## Usage with pre-commit
 
 ```yaml
 - repo: https://github.com/jvllmr/poetry-types
-  rev: v0.4.0
+  rev: v0.5.1
   hooks:
     - id: poetry-types
 ```
 
 ### poetry-types has to be skipped with pre-commit.ci
 
 ```yaml
```


# Comparing `tmp/types-WTForms-3.1.0.20240311.tar.gz` & `tmp/types-WTForms-3.1.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-WTForms-3.1.0.20240311.tar", last modified: Mon Mar 11 02:18:13 2024, max compression
+gzip compressed data, was "types-WTForms-3.1.0.20240425.tar", last modified: Thu Apr 25 02:19:16 2024, max compression
```

## Comparing `types-WTForms-3.1.0.20240311.tar` & `types-WTForms-3.1.0.20240425.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/types_WTForms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/types_WTForms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-11 02:18:13.000000 types-WTForms-3.1.0.20240311/types_WTForms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/types_WTForms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/types_WTForms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/types_WTForms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/wtforms-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-11 02:18:12.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/wtforms-stubs/csrf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/csrf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/csrf/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/csrf/session.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/choices.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/form.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/numeric.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/fields/simple.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/form.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/meta.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/validators.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:13.024943 types-WTForms-3.1.0.20240311/wtforms-stubs/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/widgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-11 02:14:35.000000 types-WTForms-3.1.0.20240311/wtforms-stubs/widgets/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 02:19:15.000000 types-WTForms-3.1.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:15.000000 types-WTForms-3.1.0.20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-25 02:19:15.000000 types-WTForms-3.1.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:16.247086 types-WTForms-3.1.0.20240425/types_WTForms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-25 02:19:16.000000 types-WTForms-3.1.0.20240425/types_WTForms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-25 02:19:16.000000 types-WTForms-3.1.0.20240425/types_WTForms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:16.000000 types-WTForms-3.1.0.20240425/types_WTForms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 02:19:16.000000 types-WTForms-3.1.0.20240425/types_WTForms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 02:19:16.000000 types-WTForms-3.1.0.20240425/types_WTForms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/wtforms-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 02:19:15.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/wtforms-stubs/csrf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/csrf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/csrf/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/csrf/session.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/choices.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/form.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/numeric.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/fields/simple.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/form.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/meta.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:15.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/validators.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:16.251086 types-WTForms-3.1.0.20240425/wtforms-stubs/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/widgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-25 02:18:23.000000 types-WTForms-3.1.0.20240425/wtforms-stubs/widgets/core.pyi
```

### Comparing `types-WTForms-3.1.0.20240311/CHANGELOG.md` & `types-WTForms-3.1.0.20240425/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.1.0.20240425 (2024-04-25)
+
+Bump pyright to v1.1.360 (#11810)
+
 ## 3.1.0.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 3.1.0.20240301 (2024-03-01)
 
 Fix invalid noqa comments and poorly formatted type ignores (#11497)
```

### Comparing `types-WTForms-3.1.0.20240311/PKG-INFO` & `types-WTForms-3.1.0.20240425/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-WTForms
-Version: 3.1.0.20240311
+Version: 3.1.0.20240425
 Summary: Typing stubs for WTForms
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WTForms.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-WTForms` aims to provide accurate annotations
 for `WTForms==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WTForms. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-WTForms-3.1.0.20240311/setup.py` & `types-WTForms-3.1.0.20240425/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-WTForms` aims to provide accurate annotations
 for `WTForms==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WTForms. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.1.0.20240311",
+      version="3.1.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WTForms.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['MarkupSafe'],
       packages=['wtforms-stubs'],
-      package_data={'wtforms-stubs': ['__init__.pyi', 'csrf/__init__.pyi', 'csrf/core.pyi', 'csrf/session.pyi', 'fields/__init__.pyi', 'fields/choices.pyi', 'fields/core.pyi', 'fields/datetime.pyi', 'fields/form.pyi', 'fields/list.pyi', 'fields/numeric.pyi', 'fields/simple.pyi', 'form.pyi', 'i18n.pyi', 'meta.pyi', 'utils.pyi', 'validators.pyi', 'widgets/__init__.pyi', 'widgets/core.pyi', 'METADATA.toml']},
+      package_data={'wtforms-stubs': ['__init__.pyi', 'csrf/__init__.pyi', 'csrf/core.pyi', 'csrf/session.pyi', 'fields/__init__.pyi', 'fields/choices.pyi', 'fields/core.pyi', 'fields/datetime.pyi', 'fields/form.pyi', 'fields/list.pyi', 'fields/numeric.pyi', 'fields/simple.pyi', 'form.pyi', 'i18n.pyi', 'meta.pyi', 'utils.pyi', 'validators.pyi', 'widgets/__init__.pyi', 'widgets/core.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-WTForms-3.1.0.20240311/types_WTForms.egg-info/PKG-INFO` & `types-WTForms-3.1.0.20240425/types_WTForms.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-WTForms
-Version: 3.1.0.20240311
+Version: 3.1.0.20240425
 Summary: Typing stubs for WTForms
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/WTForms.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-WTForms` aims to provide accurate annotations
 for `WTForms==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/WTForms. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-WTForms-3.1.0.20240311/types_WTForms.egg-info/SOURCES.txt` & `types-WTForms-3.1.0.20240425/types_WTForms.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 types_WTForms.egg-info/requires.txt
 types_WTForms.egg-info/top_level.txt
 wtforms-stubs/METADATA.toml
 wtforms-stubs/__init__.pyi
 wtforms-stubs/form.pyi
 wtforms-stubs/i18n.pyi
 wtforms-stubs/meta.pyi
+wtforms-stubs/py.typed
 wtforms-stubs/utils.pyi
 wtforms-stubs/validators.pyi
 wtforms-stubs/csrf/__init__.pyi
 wtforms-stubs/csrf/core.pyi
 wtforms-stubs/csrf/session.pyi
 wtforms-stubs/fields/__init__.pyi
 wtforms-stubs/fields/choices.pyi
```

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/csrf/core.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/csrf/core.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/csrf/session.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/csrf/session.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/choices.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/choices.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/core.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/core.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/datetime.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/form.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/form.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 _BoundFormT = TypeVar("_BoundFormT", bound=BaseForm)
 
 class FormField(Field, Generic[_BoundFormT]):
     form_class: type[_BoundFormT]
     form: _BoundFormT
     separator: str
     def __init__(
-        self: FormField[_BoundFormT],
+        self: FormField[_BoundFormT],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         form_class: type[_BoundFormT],
         label: str | None = None,
         validators: None = None,
         separator: str = "-",
         *,
         description: str = "",
         id: str | None = None,
```

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/list.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/list.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     unbound_field: UnboundField[_BoundFieldT]
     min_entries: int
     max_entries: int | None
     last_index: int
     entries: list[_BoundFieldT]
     object_data: Iterable[Any]
     def __init__(
-        self: FieldList[_BoundFieldT],
+        self: FieldList[_BoundFieldT],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         # because of our workaround we need to accept Field as well
         unbound_field: UnboundField[_BoundFieldT] | _BoundFieldT,
         label: str | None = None,
         validators: tuple[_Validator[_FormT, _BoundFieldT], ...] | list[Any] | None = None,
         min_entries: int = 0,
         max_entries: int | None = None,
         separator: str = "-",
```

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/numeric.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/numeric.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/fields/simple.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/fields/simple.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/form.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/form.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/i18n.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/i18n.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/meta.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/meta.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/utils.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/validators.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/validators.pyi`

 * *Files identical despite different names*

### Comparing `types-WTForms-3.1.0.20240311/wtforms-stubs/widgets/core.pyi` & `types-WTForms-3.1.0.20240425/wtforms-stubs/widgets/core.pyi`

 * *Files identical despite different names*


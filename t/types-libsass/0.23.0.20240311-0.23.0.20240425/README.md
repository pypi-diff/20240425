# Comparing `tmp/types-libsass-0.23.0.20240311.tar.gz` & `tmp/types-libsass-0.23.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-libsass-0.23.0.20240311.tar", last modified: Mon Mar 11 02:17:23 2024, max compression
+gzip compressed data, was "types-libsass-0.23.0.20240425.tar", last modified: Thu Apr 25 02:19:19 2024, max compression
```

## Comparing `types-libsass-0.23.0.20240311.tar` & `types-libsass-0.23.0.20240425.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:23.113177 types-libsass-0.23.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-11 02:17:22.000000 types-libsass-0.23.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:17:22.000000 types-libsass-0.23.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-11 02:17:23.113177 types-libsass-0.23.0.20240311/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:23.113177 types-libsass-0.23.0.20240311/sass-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-11 02:17:22.000000 types-libsass-0.23.0.20240311/sass-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-03-11 02:17:22.000000 types-libsass-0.23.0.20240311/sass-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:23.113177 types-libsass-0.23.0.20240311/sassutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-11 02:17:22.000000 types-libsass-0.23.0.20240311/sassutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-libsass-0.23.0.20240311/sassutils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-11 02:14:35.000000 types-libsass-0.23.0.20240311/sassutils-stubs/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-11 02:14:35.000000 types-libsass-0.23.0.20240311/sassutils-stubs/distutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-11 02:14:35.000000 types-libsass-0.23.0.20240311/sassutils-stubs/wsgi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:17:23.113177 types-libsass-0.23.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-11 02:17:22.000000 types-libsass-0.23.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:23.113177 types-libsass-0.23.0.20240311/types_libsass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-11 02:17:23.000000 types-libsass-0.23.0.20240311/types_libsass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-11 02:17:23.000000 types-libsass-0.23.0.20240311/types_libsass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:17:23.000000 types-libsass-0.23.0.20240311/types_libsass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 02:17:23.000000 types-libsass-0.23.0.20240311/types_libsass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-11 02:17:23.000000 types-libsass-0.23.0.20240311/types_libsass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:19.759039 types-libsass-0.23.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 02:19:19.755039 types-libsass-0.23.0.20240425/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:19.755039 types-libsass-0.23.0.20240425/sass-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/sass-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/sass-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/sass-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:19.755039 types-libsass-0.23.0.20240425/sassutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/sassutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-libsass-0.23.0.20240425/sassutils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-25 02:18:23.000000 types-libsass-0.23.0.20240425/sassutils-stubs/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 02:18:23.000000 types-libsass-0.23.0.20240425/sassutils-stubs/distutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/sassutils-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-25 02:18:23.000000 types-libsass-0.23.0.20240425/sassutils-stubs/wsgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:19.759039 types-libsass-0.23.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:19.755039 types-libsass-0.23.0.20240425/types_libsass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/types_libsass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/types_libsass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/types_libsass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/types_libsass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 02:19:19.000000 types-libsass-0.23.0.20240425/types_libsass.egg-info/top_level.txt
```

### Comparing `types-libsass-0.23.0.20240311/CHANGELOG.md` & `types-libsass-0.23.0.20240425/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.23.0.20240425 (2024-04-25)
+
+Bump pyright to v1.1.360 (#11810)
+
 ## 0.23.0.20240311 (2024-03-11)
 
 Make stubtest pass on libsass/passlib/redis/tree-sitter if you're using Python 3.12 (#11561)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 0.23.0.20240109 (2024-01-09)
```

### Comparing `types-libsass-0.23.0.20240311/PKG-INFO` & `types-libsass-0.23.0.20240425/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-libsass
-Version: 0.23.0.20240311
+Version: 0.23.0.20240425
 Summary: Typing stubs for libsass
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/libsass.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-libsass` aims to provide accurate annotations
 for `libsass==0.23.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/libsass. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-libsass-0.23.0.20240311/sass-stubs/__init__.pyi` & `types-libsass-0.23.0.20240425/sass-stubs/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -156,20 +156,30 @@
     def __new__(cls, msg: str | bytes) -> Self: ...
 
 class SassMap(Mapping[_KT, _VT_co]):
     # copied from dict.__init__ in builtins.pyi, since it uses dict() internally
     @overload
     def __init__(self) -> None: ...
     @overload
-    def __init__(self: SassMap[str, _VT_co], **kwargs: _VT_co) -> None: ...
+    def __init__(self: SassMap[str, _VT_co], **kwargs: _VT_co) -> None: ...  # pyright: ignore[reportInvalidTypeVarUse]  #11780
     @overload
     def __init__(self, map: SupportsKeysAndGetItem[_KT, _VT_co], /) -> None: ...
     @overload
-    def __init__(self: SassMap[str, _VT_co], map: SupportsKeysAndGetItem[str, _VT_co], /, **kwargs: _VT_co) -> None: ...
+    def __init__(
+        self: SassMap[str, _VT_co],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
+        map: SupportsKeysAndGetItem[str, _VT_co],
+        /,
+        **kwargs: _VT_co,
+    ) -> None: ...
     @overload
     def __init__(self, iterable: Iterable[tuple[_KT, _VT_co]], /) -> None: ...
     @overload
-    def __init__(self: SassMap[str, _VT_co], iterable: Iterable[tuple[str, _VT_co]], /, **kwargs: _VT_co) -> None: ...
+    def __init__(
+        self: SassMap[str, _VT_co],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
+        iterable: Iterable[tuple[str, _VT_co]],
+        /,
+        **kwargs: _VT_co,
+    ) -> None: ...
     def __getitem__(self, key: _KT) -> _VT_co: ...
     def __iter__(self) -> Iterator[_KT]: ...
     def __len__(self) -> int: ...
     def __hash__(self) -> int: ...
```

### Comparing `types-libsass-0.23.0.20240311/sassutils-stubs/builder.pyi` & `types-libsass-0.23.0.20240425/sassutils-stubs/builder.pyi`

 * *Files identical despite different names*

### Comparing `types-libsass-0.23.0.20240311/sassutils-stubs/wsgi.pyi` & `types-libsass-0.23.0.20240425/sassutils-stubs/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `types-libsass-0.23.0.20240311/setup.py` & `types-libsass-0.23.0.20240425/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-libsass` aims to provide accurate annotations
 for `libsass==0.23.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/libsass. All fixes for
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
-      version="0.23.0.20240311",
+      version="0.23.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/libsass.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-setuptools'],
       packages=['sassutils-stubs', 'sass-stubs'],
-      package_data={'sassutils-stubs': ['__init__.pyi', 'builder.pyi', 'distutils.pyi', 'wsgi.pyi', 'METADATA.toml'], 'sass-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'sassutils-stubs': ['__init__.pyi', 'builder.pyi', 'distutils.pyi', 'wsgi.pyi', 'METADATA.toml', 'py.typed'], 'sass-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-libsass-0.23.0.20240311/types_libsass.egg-info/PKG-INFO` & `types-libsass-0.23.0.20240425/types_libsass.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-libsass
-Version: 0.23.0.20240311
+Version: 0.23.0.20240425
 Summary: Typing stubs for libsass
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/libsass.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-libsass` aims to provide accurate annotations
 for `libsass==0.23.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/libsass. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```


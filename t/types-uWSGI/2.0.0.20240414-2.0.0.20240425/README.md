# Comparing `tmp/types-uWSGI-2.0.0.20240414.tar.gz` & `tmp/types-uWSGI-2.0.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-uWSGI-2.0.0.20240414.tar", last modified: Sun Apr 14 03:12:24 2024, max compression
+gzip compressed data, was "types-uWSGI-2.0.0.20240425.tar", last modified: Thu Apr 25 02:19:02 2024, max compression
```

## Comparing `types-uWSGI-2.0.0.20240414.tar` & `types-uWSGI-2.0.0.20240425.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/uwsgi-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgi-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgi-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:02.075269 types-uWSGI-2.0.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-25 02:19:02.075269 types-uWSGI-2.0.0.20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:02.075269 types-uWSGI-2.0.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:02.075269 types-uWSGI-2.0.0.20240425/types_uWSGI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-25 02:19:02.000000 types-uWSGI-2.0.0.20240425/types_uWSGI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 02:19:02.000000 types-uWSGI-2.0.0.20240425/types_uWSGI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:02.000000 types-uWSGI-2.0.0.20240425/types_uWSGI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 02:19:02.000000 types-uWSGI-2.0.0.20240425/types_uWSGI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:02.075269 types-uWSGI-2.0.0.20240425/uwsgi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/uwsgi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/uwsgi-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/uwsgi-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:02.075269 types-uWSGI-2.0.0.20240425/uwsgidecorators-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/uwsgidecorators-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/uwsgidecorators-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:01.000000 types-uWSGI-2.0.0.20240425/uwsgidecorators-stubs/py.typed
```

### Comparing `types-uWSGI-2.0.0.20240414/CHANGELOG.md` & `types-uWSGI-2.0.0.20240425/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.0.0.20240425 (2024-04-25)
+
+Bump pyright to v1.1.360 (#11810)
+
+Disable uwsgi, pyaudio, jack-client stubtest on macOS (#11821)
+
 ## 2.0.0.20240414 (2024-04-14)
 
 uwsgi: remove unused allowlist entry (#11754)
 
 Also wow, some of the logs that come from uwsgi are quite interesting
 
 ## 2.0.0.20240311 (2024-03-11)
```

### Comparing `types-uWSGI-2.0.0.20240414/PKG-INFO` & `types-uWSGI-2.0.0.20240425/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-uWSGI
-Version: 2.0.0.20240414
+Version: 2.0.0.20240425
 Summary: Typing stubs for uWSGI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/uWSGI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/uWSGI. All fixes for
 types and metadata should be contributed there.
 
 Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b78de5712df6d3976e24cdebb2c2cedc9d780378` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-uWSGI-2.0.0.20240414/setup.py` & `types-uWSGI-2.0.0.20240425/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/uWSGI. All fixes for
 types and metadata should be contributed there.
 
 Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b78de5712df6d3976e24cdebb2c2cedc9d780378` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.20240414",
+      version="2.0.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/uWSGI.md",
```

### Comparing `types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/PKG-INFO` & `types-uWSGI-2.0.0.20240425/types_uWSGI.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-uWSGI
-Version: 2.0.0.20240414
+Version: 2.0.0.20240425
 Summary: Typing stubs for uWSGI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/uWSGI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/uWSGI. All fixes for
 types and metadata should be contributed there.
 
 Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b78de5712df6d3976e24cdebb2c2cedc9d780378` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-uWSGI-2.0.0.20240414/uwsgi-stubs/__init__.pyi` & `types-uWSGI-2.0.0.20240425/uwsgi-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/__init__.pyi` & `types-uWSGI-2.0.0.20240425/uwsgidecorators-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class postfork(Generic[_P, _T]):
     wid: int
     f: Callable[_P, _T] | None
     @overload
     def __init__(self: postfork[..., Any], f: int) -> None: ...
     @overload
-    def __init__(self: postfork[_P, _T], f: Callable[_P, _T]) -> None: ...
+    def __init__(self: postfork[_P, _T], f: Callable[_P, _T]) -> None: ...  # pyright: ignore[reportInvalidTypeVarUse]  #11780
     @overload
     def __call__(self, f: Callable[_P2, _T2], /) -> postfork[_P2, _T2]: ...
     @overload
     def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _T: ...
 
 class _spoolraw(Generic[_P, _SR]):
     f: Callable[_P, _SR]
@@ -66,15 +66,15 @@
 
 class mulefunc(Generic[_P, _T]):
     fname: str | None
     mule: int
     @overload
     def __init__(self: mulefunc[..., Any], f: int) -> None: ...
     @overload
-    def __init__(self: mulefunc[_P, _T], f: Callable[_P, _T]) -> None: ...
+    def __init__(self: mulefunc[_P, _T], f: Callable[_P, _T]) -> None: ...  # pyright: ignore[reportInvalidTypeVarUse]  #11780
     def real_call(self, *args: _P.args, **kwargs: _P.kwargs) -> None: ...
     @overload
     def __call__(self, f: Callable[_P2, _T2], /) -> mulefunc[_P2, _T2]: ...
     @overload
     def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _T: ...
 
 def mule_msg_dispatcher(message: bytes) -> Any: ...
```


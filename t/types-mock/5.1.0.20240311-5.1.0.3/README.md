# Comparing `tmp/types-mock-5.1.0.20240311.tar.gz` & `tmp/types-mock-5.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-mock-5.1.0.20240311.tar", last modified: Mon Mar 11 02:15:52 2024, max compression
+gzip compressed data, was "types-mock-5.1.0.3.tar", last modified: Fri Nov 24 02:18:41 2023, max compression
```

## Comparing `types-mock-5.1.0.20240311.tar` & `types-mock-5.1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:52.877592 types-mock-5.1.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-11 02:15:52.877592 types-mock-5.1.0.20240311/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:52.877592 types-mock-5.1.0.20240311/mock-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/mock-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-11 02:14:35.000000 types-mock-5.1.0.20240311/mock-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-11 02:14:35.000000 types-mock-5.1.0.20240311/mock-stubs/backports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-03-11 02:14:35.000000 types-mock-5.1.0.20240311/mock-stubs/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:15:52.877592 types-mock-5.1.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:52.877592 types-mock-5.1.0.20240311/types_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/types_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/types_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/types_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-11 02:15:52.000000 types-mock-5.1.0.20240311/types_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:41.748261 types-mock-5.1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-11-24 02:18:41.748261 types-mock-5.1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:41.748261 types-mock-5.1.0.3/mock-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/mock-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2023-11-24 02:17:58.000000 types-mock-5.1.0.3/mock-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-24 02:17:58.000000 types-mock-5.1.0.3/mock-stubs/backports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13483 2023-11-24 02:17:58.000000 types-mock-5.1.0.3/mock-stubs/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-24 02:18:41.748261 types-mock-5.1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 02:18:41.748261 types-mock-5.1.0.3/types_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/types_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/types_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/types_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-24 02:18:41.000000 types-mock-5.1.0.3/types_mock.egg-info/top_level.txt
```

### Comparing `types-mock-5.1.0.20240311/CHANGELOG.md` & `types-mock-5.1.0.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-## 5.1.0.20240311 (2024-03-11)
-
-Use PEP 570 syntax in third party stubs (#11554)
-
-## 5.1.0.20240106 (2024-01-06)
-
-Update typing_extensions imports in third-party stubs (#11245)
-
-Remove Python 3.7 branches (#11238)
-
 ## 5.1.0.3 (2023-11-24)
 
 Third-party stubs: remove unused `type: ignore`s (#11063)
 
 ## 5.1.0.2 (2023-09-02)
 
 Update `unittest.mock` to 3.12 (#10650)
```

### Comparing `types-mock-5.1.0.20240311/PKG-INFO` & `types-mock-5.1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: types-mock
-Version: 5.1.0.20240311
+Version: 5.1.0.3
 Summary: Typing stubs for mock
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for mock
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`mock`](https://github.com/testing-cabal/mock) package.
 It can be used by type-checking tools like
@@ -28,10 +28,10 @@
 This version of `types-mock` aims to provide accurate annotations
 for `mock==5.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
```

### Comparing `types-mock-5.1.0.20240311/mock-stubs/mock.pyi` & `types-mock-5.1.0.3/mock-stubs/mock.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from _typeshed import Incomplete
 from collections.abc import Callable, Coroutine, Iterable, Mapping, Sequence
 from contextlib import AbstractContextManager
 from types import TracebackType
-from typing import Any, ClassVar, Generic, Literal, TypeVar, overload
-from typing_extensions import ParamSpec, Self
+from typing import Any, ClassVar, Generic, TypeVar, overload
+from typing_extensions import Literal, ParamSpec, Self
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 _AF = TypeVar("_AF", bound=Callable[..., Coroutine[Any, Any, Any]])
 _T = TypeVar("_T")
 _TT = TypeVar("_TT", bound=type[Any])
 _R = TypeVar("_R")
 _P = ParamSpec("_P")
@@ -62,15 +62,15 @@
         value: Any = (),
         name: Incomplete | None = None,
         parent: Incomplete | None = None,
         two: bool = False,
         from_kall: bool = True,
     ) -> None: ...
     def __eq__(self, other: object) -> bool: ...
-    def __ne__(self, other: object, /) -> bool: ...
+    def __ne__(self, __other: object) -> bool: ...
     def __call__(self, *args: Any, **kwargs: Any) -> _Call: ...
     def __getattr__(self, attr: str) -> Any: ...
     @property
     def args(self) -> tuple[Any, ...]: ...
     @property
     def kwargs(self) -> dict[str, Any]: ...
     def call_list(self) -> _CallList: ...
@@ -200,15 +200,15 @@
     ) -> AbstractContextManager[tuple[tuple[Any, ...], dict[str, Any]]]: ...
     def get_original(self) -> tuple[Any, bool]: ...
     target: Any
     temp_original: Any
     is_local: bool
     def __enter__(self) -> _T: ...
     def __exit__(
-        self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: TracebackType | None, /
+        self, __exc_type: type[BaseException] | None, __exc_value: BaseException | None, __traceback: TracebackType | None
     ) -> None: ...
     def start(self) -> _T: ...
     def stop(self) -> None: ...
 
 class _patch_dict:
     in_dict: Any
     values: Any
```

### Comparing `types-mock-5.1.0.20240311/setup.py` & `types-mock-5.1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 This version of `types-mock` aims to provide accurate annotations
 for `mock==5.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
 '''.lstrip()
 
 setup(name=name,
-      version="5.1.0.20240311",
+      version="5.1.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['mock-stubs'],
       package_data={'mock-stubs': ['__init__.pyi', 'backports.pyi', 'mock.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
-      python_requires=">=3.8",
+      python_requires=">=3.7",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-mock-5.1.0.20240311/types_mock.egg-info/PKG-INFO` & `types-mock-5.1.0.3/types_mock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: types-mock
-Version: 5.1.0.20240311
+Version: 5.1.0.3
 Summary: Typing stubs for mock
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for mock
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`mock`](https://github.com/testing-cabal/mock) package.
 It can be used by type-checking tools like
@@ -28,10 +28,10 @@
 This version of `types-mock` aims to provide accurate annotations
 for `mock==5.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `81633e27097228a8a7eb0f963c62916ecea78abc` and was tested
+with mypy 1.7.1, pyright 1.1.334, and
+pytype 2023.11.21.
```


# Comparing `tmp/types-PyMySQL-1.1.0.1.tar.gz` & `tmp/types-PyMySQL-1.1.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyMySQL-1.1.0.1.tar", last modified: Thu Jul 20 15:20:05 2023, max compression
+gzip compressed data, was "types-PyMySQL-1.1.0.20240425.tar", last modified: Thu Apr 25 02:19:06 2024, max compression
```

## Comparing `types-PyMySQL-1.1.0.1.tar` & `types-PyMySQL-1.1.0.20240425.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.531992 types-PyMySQL-1.1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-20 15:20:05.531992 types-PyMySQL-1.1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.527992 types-PyMySQL-1.1.0.1/pymysql-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/charset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/connections.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.527992 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/CLIENT.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/COMMAND.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/CR.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/ER.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/FIELD_TYPE.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/FLAG.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/SERVER_STATUS.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/cursors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/err.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/times.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:05.531992 types-PyMySQL-1.1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.527992 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/pymysql-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/charset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/connections.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/CLIENT.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/COMMAND.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/CR.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/ER.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/FIELD_TYPE.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/FLAG.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/SERVER_STATUS.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/cursors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/err.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/times.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/top_level.txt
```

### Comparing `types-PyMySQL-1.1.0.1/CHANGELOG.md` & `types-PyMySQL-1.1.0.20240425/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.1.0.20240425 (2024-04-25)
+
+Bump pyright to v1.1.360 (#11810)
+
 ## 1.1.0.1 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 1.1.0.0 (2023-06-28)
```

### Comparing `types-PyMySQL-1.1.0.1/PKG-INFO` & `types-PyMySQL-1.1.0.20240425/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.1.0.1
+Version: 1.1.0.20240425
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for PyMySQL
 
-This is a PEP 561 type stub package for the `PyMySQL` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`PyMySQL`](https://github.com/PyMySQL/PyMySQL) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`PyMySQL`. The source for this package can be found at
+`PyMySQL`.
+
+This version of `types-PyMySQL` aims to provide accurate annotations
+for `PyMySQL==1.1.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyMySQL. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/__init__.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/connections.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/connections.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
         bind_address: Incomplete | None = None,
         binary_prefix: bool | None = False,
         program_name: Incomplete | None = None,
         server_public_key: bytes | None = None,
     ) -> None: ...
     @overload
     def __init__(
-        self: Connection[_C],  # different between overloads
+        # different between overloads:
+        self: Connection[_C],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         *,
         host: str | None = None,
         user: Incomplete | None = None,
         password: str = "",
         database: Incomplete | None = None,
         port: int = 0,
         unix_socket: Incomplete | None = None,
```

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/constants/COMMAND.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/COMMAND.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/constants/CR.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/CR.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/constants/ER.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/ER.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/converters.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/converters.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/cursors.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/cursors.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/pymysql-stubs/err.pyi` & `types-PyMySQL-1.1.0.20240425/pymysql-stubs/err.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.1/setup.py` & `types-PyMySQL-1.1.0.20240425/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 from setuptools import setup
 
 name = "types-PyMySQL"
 description = "Typing stubs for PyMySQL"
 long_description = '''
 ## Typing stubs for PyMySQL
 
-This is a PEP 561 type stub package for the `PyMySQL` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`PyMySQL`](https://github.com/PyMySQL/PyMySQL) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`PyMySQL`. The source for this package can be found at
+`PyMySQL`.
+
+This version of `types-PyMySQL` aims to provide accurate annotations
+for `PyMySQL==1.1.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyMySQL. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.1.0.1",
+      version="1.1.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pymysql-stubs'],
       package_data={'pymysql-stubs': ['__init__.pyi', 'charset.pyi', 'connections.pyi', 'constants/CLIENT.pyi', 'constants/COMMAND.pyi', 'constants/CR.pyi', 'constants/ER.pyi', 'constants/FIELD_TYPE.pyi', 'constants/FLAG.pyi', 'constants/SERVER_STATUS.pyi', 'constants/__init__.pyi', 'converters.pyi', 'cursors.pyi', 'err.pyi', 'times.pyi', 'util.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/PKG-INFO` & `types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.1.0.1
+Version: 1.1.0.20240425
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for PyMySQL
 
-This is a PEP 561 type stub package for the `PyMySQL` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`PyMySQL`](https://github.com/PyMySQL/PyMySQL) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`PyMySQL`. The source for this package can be found at
+`PyMySQL`.
+
+This version of `types-PyMySQL` aims to provide accurate annotations
+for `PyMySQL==1.1.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyMySQL. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
+pytype 2024.4.11.
```

### Comparing `types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/SOURCES.txt` & `types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pymysql-stubs/METADATA.toml
 pymysql-stubs/__init__.pyi
 pymysql-stubs/charset.pyi
 pymysql-stubs/connections.pyi
 pymysql-stubs/converters.pyi
 pymysql-stubs/cursors.pyi
 pymysql-stubs/err.pyi
+pymysql-stubs/py.typed
 pymysql-stubs/times.pyi
 pymysql-stubs/util.pyi
 pymysql-stubs/constants/CLIENT.pyi
 pymysql-stubs/constants/COMMAND.pyi
 pymysql-stubs/constants/CR.pyi
 pymysql-stubs/constants/ER.pyi
 pymysql-stubs/constants/FIELD_TYPE.pyi
```


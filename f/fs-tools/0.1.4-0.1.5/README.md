# Comparing `tmp/fs_tools-0.1.4.tar.gz` & `tmp/fs_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_tools-0.1.4.tar", last modified: Wed Apr 24 14:50:59 2024, max compression
+gzip compressed data, was "fs_tools-0.1.5.tar", last modified: Thu Apr 25 05:12:36 2024, max compression
```

## Comparing `fs_tools-0.1.4.tar` & `fs_tools-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.123947 fs_tools-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:50:59.123947 fs_tools-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-24 14:50:56.000000 fs_tools-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 14:50:59.123947 fs_tools-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.113947 fs_tools-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.113947 fs_tools-0.1.4/src/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      158 2024-04-24 14:47:14.000000 fs_tools-0.1.4/src/fs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-04-24 14:46:03.000000 fs_tools-0.1.4/src/fs/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1152 2024-04-24 14:50:46.000000 fs_tools-0.1.4/src/fs/compression.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1973 2024-04-24 14:19:34.000000 fs_tools-0.1.4/src/fs/io.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.4/src/fs/moving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      597 2024-04-24 14:14:26.000000 fs_tools-0.1.4/src/fs/paths.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.123947 fs_tools-0.1.4/src/fs_tools.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:36.394240 fs_tools-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-25 05:12:36.394240 fs_tools-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-25 05:12:33.000000 fs_tools-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 05:12:36.394240 fs_tools-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:36.384240 fs_tools-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:36.394240 fs_tools-0.1.5/src/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      166 2024-04-24 14:51:42.000000 fs_tools-0.1.5/src/fs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      288 2024-04-24 14:52:16.000000 fs_tools-0.1.5/src/fs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1152 2024-04-24 14:50:46.000000 fs_tools-0.1.5/src/fs/compression.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1971 2024-04-24 14:52:10.000000 fs_tools-0.1.5/src/fs/io.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.5/src/fs/moving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      654 2024-04-24 15:14:26.000000 fs_tools-0.1.5/src/fs/paths.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:36.394240 fs_tools-0.1.5/src/fs_tools.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-25 05:12:36.000000 fs_tools-0.1.5/src/fs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-25 05:12:36.000000 fs_tools-0.1.5/src/fs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 05:12:36.000000 fs_tools-0.1.5/src/fs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-25 05:12:36.000000 fs_tools-0.1.5/src/fs_tools.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-25 05:12:36.000000 fs_tools-0.1.5/src/fs_tools.egg-info/top_level.txt
```

### Comparing `fs_tools-0.1.4/pyproject.toml` & `fs_tools-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fs-tools"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple, exception-free filesystem tools"
 dependencies = [
   "haskellian"
 ]
```

### Comparing `fs_tools-0.1.4/src/fs/compression.py` & `fs_tools-0.1.5/src/fs/compression.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.4/src/fs/io.py` & `fs_tools-0.1.5/src/fs/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     ensure_path(path)
     with open(path, mode) as f:
       f.write(data)
       return Right(None)
   except OSError as e:
     return Left(e)
 
-def insert(path: str | Path, data: str | bytes, *, replace: bool = True) -> Either[FileExistsError | OSError, None]:
-  """Insert `data` to file at `path`. Returns `Left[FileExistsError]` if `replace is False` and the file exists"""
+def write(path: str | Path, data: str | bytes, *, replace: bool = True) -> Either[FileExistsError | OSError, None]:
+  """Write `data` to file at `path`. Returns `Left[FileExistsError]` if `replace is False` and the file exists"""
   access = 'w' if replace else 'x'
   mode = f'{access}b' if isinstance(data, bytes) else access
   try:
     ensure_path(path)
     with open(path, mode) as f:
       f.write(data)
       return Right(None)
```

### Comparing `fs_tools-0.1.4/src/fs/moving.py` & `fs_tools-0.1.5/src/fs/moving.py`

 * *Files identical despite different names*


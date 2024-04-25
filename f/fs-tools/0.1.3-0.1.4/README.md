# Comparing `tmp/fs_tools-0.1.3.tar.gz` & `tmp/fs_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_tools-0.1.3.tar", last modified: Wed Apr 24 14:47:18 2024, max compression
+gzip compressed data, was "fs_tools-0.1.4.tar", last modified: Wed Apr 24 14:50:59 2024, max compression
```

## Comparing `fs_tools-0.1.3.tar` & `fs_tools-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:47:18.803952 fs_tools-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:47:18.803952 fs_tools-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-24 14:47:16.000000 fs_tools-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 14:47:18.803952 fs_tools-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:47:18.803952 fs_tools-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:47:18.803952 fs_tools-0.1.3/src/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      158 2024-04-24 14:47:14.000000 fs_tools-0.1.3/src/fs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-04-24 14:46:03.000000 fs_tools-0.1.3/src/fs/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      928 2024-04-24 14:45:51.000000 fs_tools-0.1.3/src/fs/compression.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1973 2024-04-24 14:19:34.000000 fs_tools-0.1.3/src/fs/io.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.3/src/fs/moving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      597 2024-04-24 14:14:26.000000 fs_tools-0.1.3/src/fs/paths.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:47:18.803952 fs_tools-0.1.3/src/fs_tools.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:47:18.000000 fs_tools-0.1.3/src/fs_tools.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-24 14:47:18.000000 fs_tools-0.1.3/src/fs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 14:47:18.000000 fs_tools-0.1.3/src/fs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-24 14:47:18.000000 fs_tools-0.1.3/src/fs_tools.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 14:47:18.000000 fs_tools-0.1.3/src/fs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.123947 fs_tools-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:50:59.123947 fs_tools-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-24 14:50:56.000000 fs_tools-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 14:50:59.123947 fs_tools-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.113947 fs_tools-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.113947 fs_tools-0.1.4/src/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      158 2024-04-24 14:47:14.000000 fs_tools-0.1.4/src/fs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-04-24 14:46:03.000000 fs_tools-0.1.4/src/fs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1152 2024-04-24 14:50:46.000000 fs_tools-0.1.4/src/fs/compression.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1973 2024-04-24 14:19:34.000000 fs_tools-0.1.4/src/fs/io.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.4/src/fs/moving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      597 2024-04-24 14:14:26.000000 fs_tools-0.1.4/src/fs/paths.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:50:59.123947 fs_tools-0.1.4/src/fs_tools.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 14:50:59.000000 fs_tools-0.1.4/src/fs_tools.egg-info/top_level.txt
```

### Comparing `fs_tools-0.1.3/pyproject.toml` & `fs_tools-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fs-tools"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple, exception-free filesystem tools"
 dependencies = [
   "haskellian"
 ]
```

### Comparing `fs_tools-0.1.3/src/fs/compression.py` & `fs_tools-0.1.4/src/fs/compression.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from haskellian import Either, Left, Right
 from pathlib import Path
 
 def py_gzcompress(input: str | Path, output: str | Path | None = None):
   import shutil
   import gzip
   output = output or f'{input}.gz'
   with open(input, 'rb') as f_in:
@@ -10,19 +11,23 @@
       shutil.copyfileobj(f_in, f_out)
 
 def bash_gzcompress(input: str | Path, output: str | Path | None = None, *, keep: bool = True):
   output = output or f'{input}.gz'
   k = '-k' if keep else ''
   os.system(f'gzip {k} {input} -c > {output}')
 
-def gzcompress(input: str | Path, output: str | Path | None = None, *, keep: bool = True):
+def gzcompress(input: str | Path, output: str | Path | None = None, *, keep: bool = True) -> Either[OSError, None]:
   """Compress `input` to `output`.
   - Tries to use bash's `gzip`, otherwise defaults to python's `gzip`
   - Outputs to `f'{input}.gz'` if `output is None`
   - `keep`: whether to keep the `input` file
+  - Doesn't raise. Instead, it may return `Left[OSError]` if some' bad happens
   """
+  code = bash_gzcompress(input, output, keep=keep)
+  if code == 0:
+    return Right(None)
   try:
-    bash_gzcompress(input, output, keep=keep)
-  except:
     py_gzcompress(input, output)
     if not keep:
-      os.remove(input)
+      os.remove(input)
+  except OSError as e:
+    return Left(e)
```

### Comparing `fs_tools-0.1.3/src/fs/io.py` & `fs_tools-0.1.4/src/fs/io.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.3/src/fs/moving.py` & `fs_tools-0.1.4/src/fs/moving.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.3/src/fs/paths.py` & `fs_tools-0.1.4/src/fs/paths.py`

 * *Files identical despite different names*


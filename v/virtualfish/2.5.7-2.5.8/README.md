# Comparing `tmp/virtualfish-2.5.7.tar.gz` & `tmp/virtualfish-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualfish-2.5.7.tar", max compression
+gzip compressed data, was "virtualfish-2.5.8.tar", max compression
```

## Comparing `virtualfish-2.5.7.tar` & `virtualfish-2.5.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1103 2024-03-12 13:06:40.305723 virtualfish-2.5.7/LICENSE
--rw-r--r--   0        0        0     1758 2024-03-12 13:06:40.305723 virtualfish-2.5.7/README.md
--rw-r--r--   0        0        0     1397 2024-03-12 13:07:47.982115 virtualfish-2.5.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/__init__.py
--rw-r--r--   0        0        0      376 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/__main__.py
--rw-r--r--   0        0        0     3600 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/auto_activation.fish
--rw-r--r--   0        0        0      927 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/compat_aliases.fish
--rw-r--r--   0        0        0     3455 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/environment.fish
--rw-r--r--   0        0        0      797 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/global_requirements.fish
--rw-r--r--   0        0        0     1011 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/loader/__init__.py
--rw-r--r--   0        0        0     1051 2024-03-12 13:07:21.101962 virtualfish-2.5.7/virtualfish/loader/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2307 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/loader/cli.py
--rw-r--r--   0        0        0     1736 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/loader/installer.py
--rw-r--r--   0        0        0     4789 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/projects.fish
--rw-r--r--   0        0        0        0 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/__init__.py
--rw-r--r--   0        0        0      161 2024-03-12 13:07:21.101962 virtualfish-2.5.7/virtualfish/test/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      897 2024-03-12 13:07:21.101962 virtualfish-2.5.7/virtualfish/test/__pycache__/conftest.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     3424 2024-03-12 13:07:21.101962 virtualfish-2.5.7/virtualfish/test/__pycache__/repl.cpython-39.pyc
--rw-r--r--   0        0        0     1344 2024-03-12 13:07:21.201963 virtualfish-2.5.7/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     1130 2024-03-12 13:07:21.201963 virtualfish-2.5.7/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     1087 2024-03-12 13:07:21.201963 virtualfish-2.5.7/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     1369 2024-03-12 13:07:21.205963 virtualfish-2.5.7/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     1991 2024-03-12 13:07:21.209963 virtualfish-2.5.7/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0     1799 2024-03-12 13:07:21.209963 virtualfish-2.5.7/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-7.4.4.pyc
--rw-r--r--   0        0        0      364 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/conftest.py
--rw-r--r--   0        0        0      328 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/repl.fish
--rw-r--r--   0        0        0     3745 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/repl.py
--rw-r--r--   0        0        0      233 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/test_activate.py
--rw-r--r--   0        0        0      330 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/test_addpath.py
--rw-r--r--   0        0        0      193 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/test_deactivate.py
--rw-r--r--   0        0        0      489 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/test_loader.py
--rw-r--r--   0        0        0      405 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/test_repl.py
--rw-r--r--   0        0        0      368 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/test/test_rm.py
--rw-r--r--   0        0        0     1181 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/update_python.fish
--rw-r--r--   0        0        0    32719 2024-03-12 13:06:40.309723 virtualfish-2.5.7/virtualfish/virtual.fish
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 virtualfish-2.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-04-25 12:53:13.115721 virtualfish-2.5.8/LICENSE
+-rw-r--r--   0        0        0     1758 2024-04-25 12:53:13.119721 virtualfish-2.5.8/README.md
+-rw-r--r--   0        0        0     1397 2024-04-25 12:54:23.096047 virtualfish-2.5.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/__main__.py
+-rw-r--r--   0        0        0     3600 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/auto_activation.fish
+-rw-r--r--   0        0        0      927 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/compat_aliases.fish
+-rw-r--r--   0        0        0     3455 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/environment.fish
+-rw-r--r--   0        0        0      797 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/global_requirements.fish
+-rw-r--r--   0        0        0      993 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/loader/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/loader/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2307 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/loader/cli.py
+-rw-r--r--   0        0        0     1736 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/loader/installer.py
+-rw-r--r--   0        0        0     4789 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/projects.fish
+-rw-r--r--   0        0        0        0 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/test/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      897 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/test/__pycache__/conftest.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     3424 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/test/__pycache__/repl.cpython-39.pyc
+-rw-r--r--   0        0        0     1344 2024-04-25 12:54:01.615952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1130 2024-04-25 12:54:01.619952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1087 2024-04-25 12:54:01.619952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1369 2024-04-25 12:54:01.623952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1991 2024-04-25 12:54:01.627952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1799 2024-04-25 12:54:01.627952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0      364 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/conftest.py
+-rw-r--r--   0        0        0      328 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/repl.fish
+-rw-r--r--   0        0        0     3745 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/repl.py
+-rw-r--r--   0        0        0      233 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_activate.py
+-rw-r--r--   0        0        0      330 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_addpath.py
+-rw-r--r--   0        0        0      193 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_deactivate.py
+-rw-r--r--   0        0        0      489 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_loader.py
+-rw-r--r--   0        0        0      405 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_repl.py
+-rw-r--r--   0        0        0      368 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_rm.py
+-rw-r--r--   0        0        0     1181 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/update_python.fish
+-rw-r--r--   0        0        0    32704 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/virtual.fish
+-rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 virtualfish-2.5.8/PKG-INFO
```

### Comparing `virtualfish-2.5.7/LICENSE` & `virtualfish-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/README.md` & `virtualfish-2.5.8/README.md`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/pyproject.toml` & `virtualfish-2.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtualfish"
-version = "2.5.7"
+version = "2.5.8"
 description = "Fish shell tool for managing Python virtual environments"
 authors = ["Justin Mayer <entroP@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["fish", "shell", "python", "virtual", "environments", "virtualenv"]
 repository = "https://github.com/justinmayer/virtualfish"
 
@@ -18,15 +18,15 @@
 ]
 
 [tool.poetry.urls]
 "Documentation" = "https://virtualfish.readthedocs.org/"
 "Tracker" = "https://github.com/justinmayer/virtualfish/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 packaging = ">=21.3"
 pkgconfig = ">=1.5"
 psutil = ">=5.7"
 virtualenv = ">=20"
 
 [tool.poetry.dev-dependencies]
 black = ">=22"
```

### Comparing `virtualfish-2.5.7/virtualfish/auto_activation.fish` & `virtualfish-2.5.8/virtualfish/auto_activation.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/compat_aliases.fish` & `virtualfish-2.5.8/virtualfish/compat_aliases.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/environment.fish` & `virtualfish-2.5.8/virtualfish/environment.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/global_requirements.fish` & `virtualfish-2.5.8/virtualfish/global_requirements.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/loader/__init__.py` & `virtualfish-2.5.8/virtualfish/loader/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
 import os
 import sys
-import pkg_resources
-
+from importlib import metadata
 
 log = logging.getLogger(__name__)
 
 
 def load(plugins=(), full_install=True):
     try:
-        version = pkg_resources.get_distribution("virtualfish").version
+        version = metadata.version("virtualfish")
         commands = [f"set -g VIRTUALFISH_VERSION {version}"]
-    except pkg_resources.DistributionNotFound:
+    except metadata.PackageNotFoundError:
         commands = []
     base_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
     if full_install:
         commands += [
             f"set -g VIRTUALFISH_PYTHON_EXEC {sys.executable}",
             "source {}".format(os.path.join(base_path, "virtual.fish")),
```

### Comparing `virtualfish-2.5.7/virtualfish/loader/cli.py` & `virtualfish-2.5.8/virtualfish/loader/cli.py`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/loader/installer.py` & `virtualfish-2.5.8/virtualfish/loader/installer.py`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/projects.fish` & `virtualfish-2.5.8/virtualfish/projects.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/conftest.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/conftest.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 6c01 0000  a.......`S.el...
+00000000: 610d 0d0a 0000 0000 3952 2a66 6c01 0000  a.......9R*fl...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6406 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 6d0d 5a0d 0100 6506 6a0e 6407 6408  Z.m.Z...e.j.d.d.
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/repl.cpython-39.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/repl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 3745 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 a10e 0000  a.......`S.e....
+00000000: 610d 0d0a 0000 0000 3952 2a66 a10e 0000  a.......9R*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 fa00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6402 6c07 5a07 7a10 6401 6405  ..d.d.l.Z.z.d.d.
 00000070: 6c08 6d09 5a09 0100 5700 6e1e 0400 650a  l.m.Z...W.n...e.
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 233 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 e900 0000  a.......`S.e....
+00000000: 610d 0d0a 0000 0000 3952 2a66 e900 0000  a.......9R*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 8400 5a06  ..m.Z...d.d...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 000d 0000 000c 0000  ................
 00000070: 0043 0000 0073 3201 0000 7c00 a000 6401  .C...s2...|...d.
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 330 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 4a01 0000  a.......`S.eJ...
+00000000: 610d 0d0a 0000 0000 3952 2a66 4a01 0000  a.......9R*fJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 8400 5a06  ..m.Z...d.d...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 0009 0000 0007 0000  ................
 00000070: 0043 0000 0073 0a01 0000 7c00 6a00 9b00  .C...s....|.j...
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 c100 0000  a.......`S.e....
+00000000: 610d 0d0a 0000 0000 3952 2a66 c100 0000  a.......9R*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 8400 5a06  ..m.Z...d.d...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 000b 0000 000a 0000  ................
 00000070: 0043 0000 0073 d800 0000 7c00 a000 6401  .C...s....|...d.
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 489 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 e901 0000  a.......`S.e....
+00000000: 610d 0d0a 0000 0000 3952 2a66 e901 0000  a.......9R*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6506 6a0b 6406 6407  l.m.Z...e.j.d.d.
 00000070: 8400 8301 5a0c 6408 6409 8400 5a0d 640a  ....Z.d.d...Z.d.
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 405 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 9501 0000  a.......`S.e....
+00000000: 610d 0d0a 0000 0000 3952 2a66 9501 0000  a.......9R*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6506 6a09  d.d.l.m.Z...e.j.
 00000060: 6404 6405 8400 8301 5a0a 6406 6407 8400  d.d.....Z.d.d...
 00000070: 5a0b 6408 6409 8400 5a0c 640a 640b 8400  Z.d.d...Z.d.d...
```

### Comparing `virtualfish-2.5.7/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-7.4.4.pyc` & `virtualfish-2.5.8/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-8.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 12 13:06:40 2024 UTC, .py size: 368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6053 f065 7001 0000  a.......`S.ep...
+00000000: 610d 0d0a 0000 0000 3952 2a66 7001 0000  a.......9R*fp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 8400 5a07 6404 6405 8400 5a08  d.d...Z.d.d...Z.
 00000060: 6401 5300 2906 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000070: 0000 0000 0000 0000 000a 0000 000a 0000  ................
```

### Comparing `virtualfish-2.5.7/virtualfish/test/repl.py` & `virtualfish-2.5.8/virtualfish/test/repl.py`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/update_python.fish` & `virtualfish-2.5.8/virtualfish/update_python.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.7/virtualfish/virtual.fish` & `virtualfish-2.5.8/virtualfish/virtual.fish`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         end
         set -e _VF_TEMPORARY_ENV
     end
 end
 
 function __vf_addpath --description "Adds a path to sys.path in this virtualenv"
     if set -q VIRTUAL_ENV
-        set -l site_packages (eval "$VIRTUAL_ENV/bin/python -c 'import distutils.sysconfig; print(distutils.sysconfig.get_python_lib())'")
+        set -l site_packages (eval "$VIRTUAL_ENV/bin/python -c 'import sysconfig; print(sysconfig.get_path(\'platlib\'))'")
         set -l path_file $site_packages/_virtualenv_path_extensions.pth
 
         set -l remove 0
         if test $argv[1] = "-d"
             set remove 1
             set -e argv[1]
         end
```

### Comparing `virtualfish-2.5.7/PKG-INFO` & `virtualfish-2.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: virtualfish
-Version: 2.5.7
+Version: 2.5.8
 Summary: Fish shell tool for managing Python virtual environments
 Home-page: https://github.com/justinmayer/virtualfish
 License: MIT
 Keywords: fish,shell,python,virtual,environments,virtualenv
 Author: Justin Mayer
 Author-email: entroP@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Shells
 Requires-Dist: packaging (>=21.3)
```


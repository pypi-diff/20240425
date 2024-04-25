# Comparing `tmp/ensure_import-0.3.5.tar.gz` & `tmp/ensure_import-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensure_import-0.3.5.tar", max compression
+gzip compressed data, was "ensure_import-0.3.6.tar", max compression
```

## Comparing `ensure_import-0.3.5.tar` & `ensure_import-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-19 09:03:41.423240 ensure_import-0.3.5/LICENSE
--rw-r--r--   0        0        0     1797 2023-11-30 04:17:07.045757 ensure_import-0.3.5/README.md
--rw-r--r--   0        0        0     8710 2023-11-30 04:21:50.213387 ensure_import-0.3.5/ensure_import/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 12:36:42.801440 ensure_import-0.3.5/ensure_import/prepare.py
--rw-r--r--   0        0        0        0 2023-07-19 09:27:26.374548 ensure_import-0.3.5/ensure_import/py.typed
--rw-r--r--   0        0        0     1105 2023-11-30 04:11:57.714632 ensure_import-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 ensure_import-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 09:03:41.423240 ensure_import-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1796 2024-04-20 08:02:10.732314 ensure_import-0.3.6/README.md
+-rw-r--r--   0        0        0     9098 2024-04-24 02:38:22.161446 ensure_import-0.3.6/ensure_import/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-19 02:47:14.035579 ensure_import-0.3.6/ensure_import/prepare.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:27:26.374548 ensure_import-0.3.6/ensure_import/py.typed
+-rw-r--r--   0        0        0     1020 2024-04-24 02:39:42.999097 ensure_import-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 ensure_import-0.3.6/PKG-INFO
```

### Comparing `ensure_import-0.3.5/LICENSE` & `ensure_import-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ensure_import-0.3.5/README.md` & `ensure_import-0.3.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ensure_import
 
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/ensure_import.svg?style=for-the-badge)](https://pypi.python.org/pypi/ensure_import)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
+[![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/astral-sh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge)](https://github.com/pre-commit/pre-commit)
 
 Auto install third part packages by pip into virtual environment when import error.
 
 ## Install
 ```bash
 pip install ensure_import
```

### Comparing `ensure_import-0.3.5/ensure_import/__init__.py` & `ensure_import-0.3.6/ensure_import/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import importlib
 import importlib.metadata
 import logging
 import platform
 import re
+import shlex
 import subprocess
 import sys
 from contextlib import AbstractContextManager
 from functools import cached_property
 from pathlib import Path
 from typing import Dict, Final, List, Optional, Union
 
 logger = logging.getLogger(__name__)
 
 PathLike = Union[str, Path]
-__version__ = importlib.metadata.version("ensure_import")
+try:
+    __version__ = importlib.metadata.version("ensure_import")
+except importlib.metadata.PackageNotFoundError:
+    __version__ = "0.1.0"
+
 __all__ = ("__version__", "EnsureImport")
 
 
 class EnsureImport(AbstractContextManager):
     """Auto install modules if import error.
 
     Usage::
@@ -36,15 +41,16 @@
 
     mapping = {
         "multipart": "python-multipart",
         "tortoise": "tortoise-orm",
         "dotenv": "python-dotenv",
         "snap7": "python-snap7",
     }
-    retry: Final = 30
+    RETRY: Final = 30
+    retry = RETRY
     inited = False
     instances: Dict[str, "EnsureImport"] = {}
 
     @classmethod
     def reset(cls) -> None:
         cls.inited = False
         cls.instances.clear()
@@ -58,32 +64,34 @@
     def __init__(
         self,
         _sys_path: Optional[Union[PathLike, List[PathLike]]] = None,
         _workdir: Optional[PathLike] = None,
         _install: Optional[bool] = None,
         _no_venv: Optional[bool] = None,
         _exit=None,
+        _debug=False,
         **kwargs,
-    ):
+    ) -> None:
         """
-        :Param _sys_path: directory path to append to sys.path
-        :Param _workdir: working directory, default to Path.cwd
-        :Param _install: install by pip if module not found
-        :Param _no_venv: do not use `python -m venv venv` to create virtual environment
-        :Param _exit: whether call sys.exit when install error
-        :Param kwargs: package name mapping,  example: doten='python-dotenv'
+        :param _sys_path: directory path to append to sys.path
+        :param _workdir: working directory, default to Path.cwd
+        :param _install: install by pip if module not found
+        :param _no_venv: do not use `python -m venv venv` to create virtual environment
+        :param _exit: whether call sys.exit when install error
+        :param kwargs: package name mapping,  example: doten='python-dotenv'
         """
         if self.inited:
             return
         self._success = True
         self._mapping = kwargs
         self._trying = True
         self._tried = 0
         self._py_path = sys.executable
         self.inited = True
+        self._debug = _debug
         self._set_params(
             _sys_path,
             _workdir,
             _install,
             _no_venv,
             _exit,
         )
@@ -111,19 +119,15 @@
         self._no_venv = _no_venv
         if _exit is None:
             _exit = _sys_path is None
         self._exit = _exit
 
     @property
     def trying(self) -> bool:
-        if self._tried >= self.retry:
-            self._trying = False
-        else:
-            self._tried += 1
-        if self._trying:
+        if self._tried < self.RETRY and self._trying:
             return True
         self._trying = True
         return False
 
     def __bool__(self) -> bool:
         return self.trying
 
@@ -139,41 +143,45 @@
         self._clear_kw(packages)
         return self
 
     @property
     def ok(self) -> bool:
         return self._success
 
-    def extend_paths(self, p: Union[PathLike, List[PathLike]]) -> None:
+    def extend_paths(self, p: Union[PathLike, List[PathLike]]) -> bool:
         if isinstance(p, (str, Path)):
             if isinstance(p, str):
                 if (_p := Path(p)).is_file():
                     p = _p.parent.as_posix()
             else:
                 if p.is_file():
                     p = p.parent
                 p = p.as_posix()
             if p not in sys.path:
                 sys.path.append(p)
+                return True
+            return False
         elif isinstance(p, (list, set, tuple)):
-            for i in p:
-                self.extend_paths(i)
+            return any(self.extend_paths(i) for i in p)
         else:
             raise TypeError(f"Expected: str/Path/List/Set/Tuple\nGot: {type(p)}")
 
     def __exit__(self, exc_type, exc_value, traceback):
         if isinstance(exc_value, ImportError):
+            self._tried += 1
             if (p := self._sys_path) is None:
-                if self._tried < self.retry:
+                if self._tried < self.RETRY:
                     self._success = False
                     self.run(exc_value)
                     return True
             else:
-                if self._tried <= 1:
-                    self.extend_paths(p)
+                if self._tried <= 2:
+                    if not self.extend_paths(p):
+                        if self._debug:
+                            logger.warning(f"{p} already in sys.path")
                     return True
         else:
             self._trying = False
             self._success = True
 
     def run(self, e) -> None:
         modules = re.findall(r"'([a-zA-Z][0-9a-zA-Z_]+)'", str(e))
@@ -191,15 +199,15 @@
         return hasattr(sys, "real_prefix") or (
             hasattr(sys, "base_prefix") and sys.base_prefix != sys.prefix
         )
 
     @staticmethod
     def run_and_echo(cmd: str) -> int:
         logger.info(f"--> Executing shell command:\n {cmd}")
-        return subprocess.call(cmd, shell=True)
+        return subprocess.call(shlex.split(cmd))
 
     @staticmethod
     def log_error(action: str) -> None:
         logger.error(f"ERROR: failed to {action}")
 
     @classmethod
     def is_poetry_project(cls, dirpath: Path) -> bool:
@@ -211,15 +219,15 @@
         else:
             return False
         cmd = "poetry run python -m pip --version"
         return cls.check_shell(cmd)
 
     @staticmethod
     def check_shell(cmd: str) -> bool:
-        return subprocess.run(cmd, shell=True, stderr=subprocess.DEVNULL).returncode == 0
+        return subprocess.call(shlex.split(cmd), stderr=subprocess.DEVNULL) == 0
 
     @staticmethod
     def get_poetry_py_path() -> Path:
         cmd = "poetry env info --path"
         r = subprocess.run(cmd.split(), capture_output=True)
         return Path(r.stdout.strip().decode())
 
@@ -227,14 +235,23 @@
     def workdir(self) -> Path:
         if self._workdir is None:
             self._workdir = Path.cwd()
         elif self._workdir.is_file():
             self._workdir = self._workdir.parent
         return self._workdir
 
+    @staticmethod
+    def is_module_installed(name: str) -> bool:
+        try:
+            importlib.import_module(name)
+        except ImportError:
+            return False
+        else:
+            return True
+
     def install_and_extend_sys_path(self, *packages) -> int:
         py: Union[str, Path] = Path(sys.executable)
         depends = " ".join(packages)
         if not self._no_venv and not self.is_venv():
             if self.is_poetry_project(self.workdir):
                 p = self.get_poetry_py_path()
                 py = "poetry run python"
@@ -248,19 +265,15 @@
                     py = p / "Scripts" / "python.exe"
                 else:
                     py = p / "bin/python"
             if (lib := list(p.rglob("site-packages"))[0].as_posix()) not in sys.path:
                 sys.path.append(lib)
                 if not self.check_shell(f"{py} -c 'import ensure_import'"):
                     sys.path.append(Path(__file__).parent.parent.as_posix())
-                try:
-                    importlib.import_module(packages[0])
-                except ImportError:
-                    ...
-                else:
+                if self.is_module_installed(packages[0]):
                     return 0
             if self._install:
                 self.run_and_echo(f"{py} -m pip install --upgrade pip")
         if self._install and self.run_and_echo(f"{py} -m pip install {depends}"):
             self.log_error(f"install {depends}")
             return 2
         return 0
```

### Comparing `ensure_import-0.3.5/PKG-INFO` & `ensure_import-0.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensure-import
-Version: 0.3.5
+Version: 0.3.6
 Summary: Auto install third part packages by pip into virtual environment when import error.
 Home-page: https://github.com/waketzheng/ensure_import
 License: MIT
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # ensure_import
 
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/ensure_import.svg?style=for-the-badge)](https://pypi.python.org/pypi/ensure_import)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
+[![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/astral-sh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge)](https://github.com/pre-commit/pre-commit)
 
 Auto install third part packages by pip into virtual environment when import error.
 
 ## Install
 ```bash
 pip install ensure_import
```


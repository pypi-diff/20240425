# Comparing `tmp/datalad-installer-1.0.4.tar.gz` & `tmp/datalad_installer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad-installer-1.0.4.tar", last modified: Fri Feb 16 18:13:46 2024, max compression
+gzip compressed data, was "datalad_installer-1.0.5.tar", last modified: Thu Apr 25 16:46:01 2024, max compression
```

## Comparing `datalad-installer-1.0.4.tar` & `datalad_installer-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:13:46.107886 datalad-installer-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-02-16 18:13:34.000000 datalad-installer-1.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23835 2024-02-16 18:13:46.107886 datalad-installer-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-16 18:13:46.107886 datalad-installer-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:13:46.103886 datalad-installer-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:13:46.107886 datalad-installer-1.0.4/src/datalad_installer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23835 2024-02-16 18:13:46.000000 datalad-installer-1.0.4/src/datalad_installer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-16 18:13:46.000000 datalad-installer-1.0.4/src/datalad_installer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:13:46.000000 datalad-installer-1.0.4/src/datalad_installer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-16 18:13:46.000000 datalad-installer-1.0.4/src/datalad_installer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 18:13:46.000000 datalad-installer-1.0.4/src/datalad_installer.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   108073 2024-02-16 18:13:37.000000 datalad-installer-1.0.4/src/datalad_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:13:46.107886 datalad-installer-1.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:13:46.103886 datalad-installer-1.0.4/test/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:13:46.107886 datalad-installer-1.0.4/test/data/parse-links/
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/test/data/parse-links/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/test/data/parse-links/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/test/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-16 18:13:08.000000 datalad-installer-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:46:01.629973 datalad_installer-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-25 16:45:57.000000 datalad_installer-1.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23835 2024-04-25 16:46:01.629973 datalad_installer-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 16:46:01.629973 datalad_installer-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:46:01.625973 datalad_installer-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:46:01.629973 datalad_installer-1.0.5/src/datalad_installer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23835 2024-04-25 16:46:01.000000 datalad_installer-1.0.5/src/datalad_installer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-25 16:46:01.000000 datalad_installer-1.0.5/src/datalad_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:46:01.000000 datalad_installer-1.0.5/src/datalad_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 16:46:01.000000 datalad_installer-1.0.5/src/datalad_installer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 16:46:01.000000 datalad_installer-1.0.5/src/datalad_installer.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108222 2024-04-25 16:45:57.000000 datalad_installer-1.0.5/src/datalad_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:46:01.629973 datalad_installer-1.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:46:01.625973 datalad_installer-1.0.5/test/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:46:01.629973 datalad_installer-1.0.5/test/data/parse-links/
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/test/data/parse-links/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/test/data/parse-links/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/test/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-25 16:45:44.000000 datalad_installer-1.0.5/tox.ini
```

### Comparing `datalad-installer-1.0.4/CHANGELOG.md` & `datalad_installer-1.0.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+# v1.0.5 (Thu Apr 25 2024)
+
+#### 🐛 Bug Fix
+
+- Make compatible with arm64 brew, test on older and latest macos, strip away no longer needed windows test env exclusion [#197](https://github.com/datalad/datalad-installer/pull/197) ([@yarikoptic](https://github.com/yarikoptic))
+
+#### 🏠 Internal
+
+- Progress auto to 11.1.6 to avoid "not an integer" bug in auto [#198](https://github.com/datalad/datalad-installer/pull/198) ([@yarikoptic](https://github.com/yarikoptic))
+
+#### 🧪 Tests
+
+- Skip `--dev-pip` test on Python 3.7 [#195](https://github.com/datalad/datalad-installer/pull/195) ([@jwodder](https://github.com/jwodder))
+
+#### Authors: 2
+
+- John T. Wodder II ([@jwodder](https://github.com/jwodder))
+- Yaroslav Halchenko ([@yarikoptic](https://github.com/yarikoptic))
+
+---
+
 # v1.0.4 (Fri Feb 16 2024)
 
 #### 🐛 Bug Fix
 
 - Always provide -y   to apt-get install [#194](https://github.com/datalad/datalad-installer/pull/194) ([@yarikoptic](https://github.com/yarikoptic))
 - Handle lack of Link header when paginating [#188](https://github.com/datalad/datalad-installer/pull/188) ([@jwodder](https://github.com/jwodder))
```

### Comparing `datalad-installer-1.0.4/LICENSE` & `datalad_installer-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/PKG-INFO` & `datalad_installer-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-installer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Installation script for Datalad and related components
 Home-page: https://github.com/datalad/datalad-installer
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Maintainer: John Thorvald Wodder II
 Maintainer-email: datalad-installer@varonathe.org
 License: MIT
```

### Comparing `datalad-installer-1.0.4/README.rst` & `datalad_installer-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/run-tests.sh` & `datalad_installer-1.0.5/run-tests.sh`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/setup.cfg` & `datalad_installer-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/src/datalad_installer.egg-info/PKG-INFO` & `datalad_installer-1.0.5/src/datalad_installer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-installer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Installation script for Datalad and related components
 Home-page: https://github.com/datalad/datalad-installer
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Maintainer: John Thorvald Wodder II
 Maintainer-email: datalad-installer@varonathe.org
 License: MIT
```

### Comparing `datalad-installer-1.0.4/src/datalad_installer.py` & `datalad_installer-1.0.5/src/datalad_installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 .. _git-annex: https://git-annex.branchable.com
 
 Visit <https://github.com/datalad/datalad-installer> for more information.
 """
 
 from __future__ import annotations
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 __author__ = "The DataLad Team and Contributors"
 __author_email__ = "team@datalad.org"
 __license__ = "MIT"
 __url__ = "https://github.com/datalad/datalad-installer"
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Iterator
 from contextlib import contextmanager, suppress
 import ctypes
 from dataclasses import InitVar, dataclass, field
 from email import policy
 from email.headerregistry import ContentTypeHeader
 from enum import Enum
-from functools import total_ordering
+from functools import lru_cache, total_ordering
 from getopt import GetoptError, getopt
 from html.parser import HTMLParser
 from http.client import HTTPMessage
 from itertools import groupby
 import json
 import logging
 from operator import attrgetter
@@ -1608,16 +1608,17 @@
             log.error(
                 "brew command failed; printing diagnostic output for reporting issue"
             )
             runcmd("brew", "config")
             runcmd("brew", "doctor")
             raise
         ### TODO: Handle variations in this path (Is it "$(brew --prefix)/bin"?)
-        log.debug("Installed program directory: /usr/local/bin")
-        return Path("/usr/local/bin")
+        bin_dir = get_brew_bin_dir()
+        log.debug("Installed program directory: %s", bin_dir)
+        return bin_dir
 
     def assert_supported_system(self, **_kwargs: Any) -> None:
         if shutil.which("brew") is None:
             raise MethodNotSupportedError("brew command not found")
 
 
 @DataladComponent.register_installer
@@ -2957,14 +2958,19 @@
         for _ in range(5):
             if os.path.exists(path):
                 return True
             sleep(1)
     return os.path.exists(path)
 
 
+@lru_cache()
+def get_brew_bin_dir() -> Path:
+    return Path(readcmd("brew", "--prefix").rstrip(os.linesep)) / "bin"
+
+
 def parse_links(html: str, base_url: Optional[str] = None) -> list[Link]:
     """
     Parse the source of an HTML page and return a list of all hyperlinks found
     on it.
 
     This function does not support encoding declarations embedded in HTML, and
     it has limited ability to deal with invalid HTML.
```

### Comparing `datalad-installer-1.0.4/test/conftest.py` & `datalad_installer-1.0.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/test/data/parse-links/sample.html` & `datalad_installer-1.0.5/test/data/parse-links/sample.html`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/test/data/parse-links/sample.json` & `datalad_installer-1.0.5/test/data/parse-links/sample.json`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/test/test_install.py` & `datalad_installer-1.0.5/test/test_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
     )
     assert r == 0
     assert (venv_path / bin_path("python")).exists()
     assert (venv_path / bin_path("datalad")).exists()
 
 
 @pytest.mark.skipif(
-    sys.version_info[:2] < (3, 7), reason="dev pip no longer supports Python < 3.7"
+    sys.version_info[:2] < (3, 8), reason="dev pip no longer supports Python < 3.8"
 )
 def test_install_venv_dev_pip_datalad(tmp_path: Path) -> None:
     venv_path = tmp_path / "venv"
     r = main(
         [
             "datalad_installer.py",
             "venv",
@@ -409,15 +409,25 @@
 @pytest.mark.skipif(
     not ON_MACOS or shutil.which("brew") is None, reason="requires macOS with Homebrew"
 )
 def test_install_git_annex_brew(mocker: MockerFixture) -> None:
     spy = mocker.spy(datalad_installer, "runcmd")
     r = main(["datalad_installer.py", "git-annex", "-m", "brew"])
     assert r == 0
-    assert spy.call_args_list[-1] == mocker.call("brew", "install", "git-annex")
+
+    # where to look for the "brew install" invocation
+    target_index = -1
+    # we might have checked also for the brew --prefix
+    if spy.call_args_list[-1] == mocker.call(
+        "brew", "--prefix", stdout=-1, universal_newlines=True
+    ):
+        target_index -= 1
+    assert spy.call_args_list[target_index] == mocker.call(
+        "brew", "install", "git-annex"
+    )
     assert shutil.which("git-annex") is not None
 
 
 @pytest.mark.ghauth_required
 @pytest.mark.parametrize(
     "ostype,ext",
     [
```

### Comparing `datalad-installer-1.0.4/test/test_options.py` & `datalad_installer-1.0.5/test/test_options.py`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/test/test_util.py` & `datalad_installer-1.0.5/test/test_util.py`

 * *Files identical despite different names*

### Comparing `datalad-installer-1.0.4/tox.ini` & `datalad_installer-1.0.5/tox.ini`

 * *Files identical despite different names*


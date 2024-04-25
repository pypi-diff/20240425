# Comparing `tmp/c4t-1.2.0.tar.gz` & `tmp/c4t-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4t-1.2.0.tar", last modified: Tue Sep 19 10:11:33 2023, max compression
+gzip compressed data, was "c4t-1.2.3.tar", last modified: Thu Apr 25 11:15:28 2024, max compression
```

## Comparing `c4t-1.2.0.tar` & `c4t-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2023-09-19 10:11:33.152605 c4t-1.2.0/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1063 2023-09-13 10:14:04.000000 c4t-1.2.0/LICENSE
--rw-r--r--   0 pairin    (1000) pairin    (1000)     5116 2023-09-19 10:11:33.152605 c4t-1.2.0/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)     3989 2023-09-19 10:10:09.000000 c4t-1.2.0/README.md
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1745 2023-09-19 10:10:09.000000 c4t-1.2.0/pyproject.toml
--rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2023-09-19 10:11:33.152605 c4t-1.2.0/setup.cfg
--rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2023-09-13 10:14:04.000000 c4t-1.2.0/setup.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2023-09-19 10:11:33.142605 c4t-1.2.0/src/
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2023-09-19 10:11:33.142605 c4t-1.2.0/src/c4t/
--rw-r--r--   0 pairin    (1000) pairin    (1000)    13073 2023-09-19 10:10:09.000000 c4t-1.2.0/src/c4t/__init__.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1409 2023-09-19 10:06:36.000000 c4t-1.2.0/src/c4t/cli.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2023-09-19 10:11:33.142605 c4t-1.2.0/src/c4t.egg-info/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     5116 2023-09-19 10:11:33.000000 c4t-1.2.0/src/c4t.egg-info/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)      279 2023-09-19 10:11:33.000000 c4t-1.2.0/src/c4t.egg-info/SOURCES.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2023-09-19 10:11:33.000000 c4t-1.2.0/src/c4t.egg-info/dependency_links.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       36 2023-09-19 10:11:33.000000 c4t-1.2.0/src/c4t.egg-info/entry_points.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)      105 2023-09-19 10:11:33.000000 c4t-1.2.0/src/c4t.egg-info/requires.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        4 2023-09-19 10:11:33.000000 c4t-1.2.0/src/c4t.egg-info/top_level.txt
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2023-09-19 10:11:33.152605 c4t-1.2.0/tests/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     2978 2023-09-19 10:10:09.000000 c4t-1.2.0/tests/tests.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.615374 c4t-1.2.3/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1063 2024-03-16 17:32:43.000000 c4t-1.2.3/LICENSE
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     6275 2024-04-25 11:15:28.615374 c4t-1.2.3/PKG-INFO
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     4620 2024-03-29 00:26:43.000000 c4t-1.2.3/README.md
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     2117 2024-03-29 00:26:43.000000 c4t-1.2.3/pyproject.toml
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-25 11:15:28.615374 c4t-1.2.3/setup.cfg
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-03-16 17:32:43.000000 c4t-1.2.3/setup.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/src/
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/src/c4t/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)    13339 2024-03-29 00:26:43.000000 c4t-1.2.3/src/c4t/__init__.py
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1409 2024-03-16 17:32:43.000000 c4t-1.2.3/src/c4t/cli.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/src/c4t.egg-info/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     6275 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/PKG-INFO
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      279 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/SOURCES.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/dependency_links.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       36 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/entry_points.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      245 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/requires.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)        4 2024-04-25 11:15:28.000000 c4t-1.2.3/src/c4t.egg-info/top_level.txt
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-25 11:15:28.605374 c4t-1.2.3/tests/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     2941 2024-03-29 00:26:43.000000 c4t-1.2.3/tests/tests.py
```

### Comparing `c4t-1.2.0/LICENSE` & `c4t-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `c4t-1.2.0/PKG-INFO` & `c4t-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.2.0
+Version: 1.2.3
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: wget>=3.2
-Provides-Extra: dev
-Requires-Dist: build==0.10.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
-Requires-Dist: bumpver>=2023.1126; extra == "dev"
+Provides-Extra: lint
+Requires-Dist: mypy>=1.9.0; extra == "lint"
+Requires-Dist: types-requests>=2.31.0.20240311; extra == "lint"
+Requires-Dist: ruff>=0.3.4; extra == "lint"
 Provides-Extra: test
 Requires-Dist: selenium>=4.12.0; extra == "test"
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Provides-Extra: package
+Requires-Dist: build==0.10.0; extra == "package"
+Requires-Dist: twine>=4.0.2; extra == "package"
+Provides-Extra: dev
+Requires-Dist: bumpver>=2023.1126; extra == "dev"
+Requires-Dist: c4t[lint]; extra == "dev"
+Requires-Dist: c4t[test]; extra == "dev"
+Requires-Dist: c4t[package]; extra == "dev"
 
-# c4t: Chrome for Testing - v1.2.0
+[![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
+![PyPI - Version](https://img.shields.io/pypi/v/c4t)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
+![PyPI - Format](https://img.shields.io/pypi/format/c4t)
+![PyPI - License](https://img.shields.io/pypi/l/c4t)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+# c4t: Chrome for Testing - v1.2.3
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.0/README.md` & `c4t-1.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-# c4t: Chrome for Testing - v1.2.0
+[![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
+![PyPI - Version](https://img.shields.io/pypi/v/c4t)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
+![PyPI - Format](https://img.shields.io/pypi/format/c4t)
+![PyPI - License](https://img.shields.io/pypi/l/c4t)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+# c4t: Chrome for Testing - v1.2.3
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.0/pyproject.toml` & `c4t-1.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c4t"
-version = "1.2.0"
+version = "1.2.3"
 authors = [
   { name="p4irin", email="139928764+p4irin@users.noreply.github.com" },
 ]
 description = "Install Chrome for Testing assets."
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -17,47 +17,63 @@
 dependencies = [
   "requests >= 2.31.0",
   "wget >= 3.2",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: POSIX :: Linux",
     "Intended Audience :: Developers",    
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",    
     "License :: OSI Approved :: MIT License",    
 ]
 
 [project.optional-dependencies]
-dev = [
-  "build == 0.10.0",
-  "twine >= 4.0.2",
-  "bumpver >= 2023.1126",
+lint = [
+  "mypy >= 1.9.0",
+  "types-requests >= 2.31.0.20240311",
+  "ruff >= 0.3.4",
 ]
 test = [
   "selenium >= 4.12.0",
+  "pytest >= 8.1.1",
+  "pytest-cov >= 4.1.0",
+]
+package = [
+  "build == 0.10.0",
+  "twine >= 4.0.2",
+]
+dev = [
+  "bumpver >= 2023.1126",
+  "c4t[lint]",
+  "c4t[test]",
+  "c4t[package]",
 ]
 
 [project.scripts]
 c4t = "c4t.cli:cli"
 
 [project.urls]
 "Homepage" = "https://github.com/p4irin/c4t"
 "Bug Tracker" = "https://github.com/p4irin/c4t/issues"
 
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+
 [tool.bumpver]
-current_version = "1.2.0"
+current_version = "1.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
@@ -72,7 +88,13 @@
 "tests/tests.py" = [
   "^__version__ = '{version}'$",
 ]
 "README.md" = [
   " - v{version}$",
 ]
 
+
+[tool.mypy]
+
+[[tool.mypy.overrides]]
+module = "wget"
+ignore_missing_imports = true
```

### Comparing `c4t-1.2.0/setup.py` & `c4t-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `c4t-1.2.0/src/c4t/__init__.py` & `c4t-1.2.3/src/c4t/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     browser.close()
     browser.quit()
 """
 
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.2.0'
+__version__ = '1.2.3'
 
 
 import requests
 import os
 import json
 import wget
 import zipfile
@@ -145,15 +145,20 @@
 
         Args:
             files: Files that should have their execute bit on.
             for_binary: The binary the files are related to.
         """
 
         for file in files:
-            os.chmod(f'{self._installation_path_of(for_binary)}/{file}', 0o755)
+            try:
+                os.chmod(f'{self._installation_path_of(for_binary)}/{file}', 0o755)
+            except FileNotFoundError:
+                # Some files were removed from the Chrome zip download
+                # Just move on to the next file
+                continue
 
     def _download(
             self,
             binary: Literal['chrome', 'chromedriver'],
             for_platform: str,
             from_url: str
         ) -> str:
@@ -182,14 +187,30 @@
         try:
             wget.download(from_url, self._download_dir)
             print('\n')
         except Exception as e:
             print(f'wget threw Exception {e}')
             raise e
         return binary_zip_file
+    
+    def extract_zip_with_permissions(self, zip_file: str, destination: str):
+        """Extract zip file and keep file permissions
+        
+        zipfile doesn't keep file permissions
+
+        Args:
+            zip_file: Relative path from working directory to the zip file
+            destination: Relative path from working directory
+        """
+        with zipfile.ZipFile(zip_file, 'r') as zip_ref:
+            for member in zip_ref.infolist():
+                zip_ref.extract(member, destination)
+                file_name = f'{destination}/{member.filename}'
+                permissions = member.external_attr >> 16
+                os.chmod(file_name, permissions)    
 
     def _unzip(
             self,
             binary: Literal['chrome', 'chromedriver'],
             from_zip_file: str,
             for_platform: str='linux64'
         ) -> None:
@@ -203,18 +224,17 @@
         """
 
         print(f'Unzipping {from_zip_file}')
         binary_path = f'{self._download_dir}/{binary}-{for_platform}/{binary}'
         if os.path.isfile(binary_path):
             print(f'{from_zip_file} already unzipped. Skipping')
         else:
-            with zipfile.ZipFile(
-                    f'{self._download_dir}/{from_zip_file}'
-                 ) as zfh:
-                zfh.extractall(f'{self._download_dir}')
+            self.extract_zip_with_permissions(
+                f'{self._download_dir}/{from_zip_file}', f'{self._download_dir}'
+            )
 
     def _create_symlink(
             self,
             to_binary: Literal['chrome', 'chromedriver'],
             version: str,
             for_platform: str='linux64'
         ) -> None:
@@ -347,35 +367,20 @@
 
         self._unzip(
             binary='chrome', 
             from_zip_file=chrome_zip_file,
             for_platform='linux64'
         )
 
-        chrome_files_to_make_executable = [
-            "chrome", "chrome_crashpad_handler", "chrome_sandbox",
-            "chrome-wrapper", "libEGL.so", "libGLESv2.so",
-            "libvk_swiftshader.so", "libvulkan.so.1", "nacl_helper",
-            "nacl_helper_bootstrap", "nacl_irt_x86_64.nexe", "xdg-mime",
-            "xdg-settings"
-        ]
-
-        # zipfile doesn't preserve file permissions
-        self._make_executable(
-            chrome_files_to_make_executable, for_binary='chrome'
-        )
-
         self._unzip(
             binary='chromedriver',
             from_zip_file=chromedriver_zip_file,
             for_platform='linux64'
         )
 
-        self._make_executable(['chromedriver'], for_binary='chromedriver')
-
         self._create_symlink(
             to_binary='chrome',
             version=version,
             for_platform='linux64'
         )
 
         self._create_symlink(
```

### Comparing `c4t-1.2.0/src/c4t/cli.py` & `c4t-1.2.3/src/c4t/cli.py`

 * *Files identical despite different names*

### Comparing `c4t-1.2.0/src/c4t.egg-info/PKG-INFO` & `c4t-1.2.3/src/c4t.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.2.0
+Version: 1.2.3
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: wget>=3.2
-Provides-Extra: dev
-Requires-Dist: build==0.10.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
-Requires-Dist: bumpver>=2023.1126; extra == "dev"
+Provides-Extra: lint
+Requires-Dist: mypy>=1.9.0; extra == "lint"
+Requires-Dist: types-requests>=2.31.0.20240311; extra == "lint"
+Requires-Dist: ruff>=0.3.4; extra == "lint"
 Provides-Extra: test
 Requires-Dist: selenium>=4.12.0; extra == "test"
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Provides-Extra: package
+Requires-Dist: build==0.10.0; extra == "package"
+Requires-Dist: twine>=4.0.2; extra == "package"
+Provides-Extra: dev
+Requires-Dist: bumpver>=2023.1126; extra == "dev"
+Requires-Dist: c4t[lint]; extra == "dev"
+Requires-Dist: c4t[test]; extra == "dev"
+Requires-Dist: c4t[package]; extra == "dev"
 
-# c4t: Chrome for Testing - v1.2.0
+[![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
+![PyPI - Version](https://img.shields.io/pypi/v/c4t)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
+![PyPI - Format](https://img.shields.io/pypi/format/c4t)
+![PyPI - License](https://img.shields.io/pypi/l/c4t)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+# c4t: Chrome for Testing - v1.2.3
 
 Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
```

### Comparing `c4t-1.2.0/tests/tests.py` & `c4t-1.2.3/tests/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import unittest
 import os
 import time
-from shutil import rmtree
 from selenium.webdriver import ChromeOptions, ChromeService, Chrome
 import c4t
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.2.0'
+__version__ = '1.2.3'
 
 
 class C4tTests(unittest.TestCase):
 
     class _TestData:
         specific_version_of_assets = '116.0.5794.0'
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.assets_dir = './assets'
-        rmtree(cls.assets_dir) if os.path.exists(cls.assets_dir) else None
         cls.chrome_options = ChromeOptions()
         cls.chrome_options.binary_location = c4t.location.chrome
+        cls.chrome_options.add_argument('--no-sandbox')
+        cls.chrome_options.add_argument('--headless')        
         cls.chrome_service = ChromeService(
             executable_path=c4t.location.chromedriver
         )
 
     def setUp(self) -> None:
         pass
 
     def tearDown(self) -> None:
         pass
 
     @classmethod
     def tearDownClass(cls) -> None:
-        rmtree(cls.assets_dir) if os.path.exists(cls.assets_dir) else None
-
+        pass
+    
     def verify_chrome_for_testing_version_with_selenium(
             self, expected_version: str
         ):
 
         browser = Chrome(
             options=self.chrome_options, service=self.chrome_service
         )
@@ -50,15 +50,15 @@
         )
         browser.quit()    
 
     def test_001_installation_of_default_latest_stable_version(self):            
         assets = c4t.Assets()
         self.assertTrue(os.path.isdir(self.assets_dir))
         assets.install()
-        self.assertTrue(type(assets.active_version) == str)
+        self.assertTrue(isinstance(assets.active_version, str))
         self.assertTrue(
             os.path.exists(
                 f'{self.assets_dir}/{assets.active_version}/chrome-linux64/chrome'
             )
         )
         self.assertTrue(
             os.path.exists(
```


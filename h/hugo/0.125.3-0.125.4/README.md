# Comparing `tmp/hugo-0.125.3.tar.gz` & `tmp/hugo-0.125.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugo-0.125.3.tar", last modified: Mon Apr 22 18:03:14 2024, max compression
+gzip compressed data, was "hugo-0.125.4.tar", last modified: Thu Apr 25 14:21:37 2024, max compression
```

## Comparing `hugo-0.125.3.tar` & `hugo-0.125.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:03:14.028431 hugo-0.125.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-22 18:03:09.000000 hugo-0.125.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-22 18:03:09.000000 hugo-0.125.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-22 18:03:09.000000 hugo-0.125.3/LICENSE-hugo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 18:03:09.000000 hugo-0.125.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-22 18:03:14.028431 hugo-0.125.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19810 2024-04-22 18:03:09.000000 hugo-0.125.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-22 18:03:09.000000 hugo-0.125.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:03:14.028431 hugo-0.125.3/hugo/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-22 18:03:09.000000 hugo-0.125.3/hugo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:03:14.028431 hugo-0.125.3/hugo/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 18:03:09.000000 hugo-0.125.3/hugo/binaries/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-22 18:03:09.000000 hugo-0.125.3/hugo/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-22 18:03:09.000000 hugo-0.125.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-22 18:03:14.032431 hugo-0.125.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-04-22 18:03:09.000000 hugo-0.125.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:37.134593 hugo-0.125.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-25 14:21:32.000000 hugo-0.125.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-25 14:21:32.000000 hugo-0.125.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 14:21:32.000000 hugo-0.125.4/LICENSE-hugo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 14:21:32.000000 hugo-0.125.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-25 14:21:37.134593 hugo-0.125.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19810 2024-04-25 14:21:32.000000 hugo-0.125.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-25 14:21:32.000000 hugo-0.125.4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:37.134593 hugo-0.125.4/hugo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 14:21:32.000000 hugo-0.125.4/hugo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:37.134593 hugo-0.125.4/hugo/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 14:21:32.000000 hugo-0.125.4/hugo/binaries/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-25 14:21:32.000000 hugo-0.125.4/hugo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 14:21:32.000000 hugo-0.125.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 14:21:37.138593 hugo-0.125.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-04-25 14:21:32.000000 hugo-0.125.4/setup.py
```

### Comparing `hugo-0.125.3/CODE_OF_CONDUCT.md` & `hugo-0.125.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.3/LICENSE` & `hugo-0.125.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hugo-0.125.3/LICENSE-hugo.txt` & `hugo-0.125.4/LICENSE-hugo.txt`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 The Hugo Authors.
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `hugo-0.125.3/PKG-INFO` & `hugo-0.125.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.125.3
+Version: 0.125.4
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.125.3/README.md` & `hugo-0.125.4/README.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.3/SECURITY.md` & `hugo-0.125.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.3/hugo/cli.py` & `hugo-0.125.4/hugo/cli.py`

 * *Files identical despite different names*

### Comparing `hugo-0.125.3/pyproject.toml` & `hugo-0.125.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hugo-0.125.3/setup.py` & `hugo-0.125.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import Command, Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from wheel.bdist_wheel import bdist_wheel
 
 # ------ Hugo build configuration and constants ------------------------------------
 
-HUGO_VERSION = "0.125.3"
+HUGO_VERSION = "0.125.4"
 # The Go toolchain will download the tarball into the hugo_cache/ directory.
 # We will point the build command to that location to build Hugo from source
 HUGO_CACHE_DIR = "hugo_cache"
 FILE_EXT = (
     ".exe" if (sys.platform == "win32" or os.environ.get("GOOS") == "windows") else ""
 )
 # The vendor name is used to set the vendorInfo variable in the Hugo binary
```


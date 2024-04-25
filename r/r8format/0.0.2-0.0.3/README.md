# Comparing `tmp/r8format-0.0.2.tar.gz` & `tmp/r8format-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r8format-0.0.2.tar", last modified: Tue Apr 23 10:53:27 2024, max compression
+gzip compressed data, was "r8format-0.0.3.tar", last modified: Thu Apr 25 07:32:55 2024, max compression
```

## Comparing `r8format-0.0.2.tar` & `r8format-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,57 @@
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.597995 r8format-0.0.2/
--rw-r--r--   0 cjs       (1765) cjs       (1765)     4396 2024-04-23 10:53:27.593995 r8format-0.0.2/PKG-INFO
--rw-r-----   0 cjs       (1765) cjs       (1765)     4160 2024-04-23 08:53:57.000000 r8format-0.0.2/README.md
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/bastok/
--rw-r-----   0 cjs       (1765) cjs       (1765)     1464 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/blines.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/bastok/charset/
--rw-r-----   0 cjs       (1765) cjs       (1765)     6822 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/charset/__init__.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     5844 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/charset/msx.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/bastok/cli/
--rwxr-x---   0 cjs       (1765) cjs       (1765)     3527 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/cli/basdump.py
--rwxr-x---   0 cjs       (1765) cjs       (1765)     1165 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/cli/blines.py
--rwxr-x---   0 cjs       (1765) cjs       (1765)     2264 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/cli/detok.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/bastok/detok/
--rw-r-----   0 cjs       (1765) cjs       (1765)    28656 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/detok/msx2.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     9042 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/bastok/tlines.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/binary/
--rw-r-----   0 cjs       (1765) cjs       (1765)      152 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/__init__.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.589995 r8format-0.0.2/psrc/binary/cli/
--rwxr-x---   0 cjs       (1765) cjs       (1765)     2926 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/cli/msx_dasm.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     3414 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/memimage.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     5441 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/symtab.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.593995 r8format-0.0.2/psrc/binary/tool/
--rw-r-----   0 cjs       (1765) cjs       (1765)       82 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/tool/__init__.py
--rw-r-----   0 cjs       (1765) cjs       (1765)    11413 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/tool/asl.py
--rw-r-----   0 cjs       (1765) cjs       (1765)    13158 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/binary/tool/asxxxx.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.593995 r8format-0.0.2/psrc/cmtconv/
--rw-r-----   0 cjs       (1765) cjs       (1765)      242 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/analyze.py
--rw-r-----   0 cjs       (1765) cjs       (1765)    20766 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/audio.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     6517 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/bytestream.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.593995 r8format-0.0.2/psrc/cmtconv/cli/
--rwxr-x---   0 cjs       (1765) cjs       (1765)    12247 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/cli/analyze_cmt.py
--rwxr-x---   0 cjs       (1765) cjs       (1765)     2522 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/cli/cmtconv.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     2010 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/formats.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     4804 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/logging.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.593995 r8format-0.0.2/psrc/cmtconv/platform/
--rw-r-----   0 cjs       (1765) cjs       (1765)    14253 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/platform/fm7.py
--rw-r-----   0 cjs       (1765) cjs       (1765)    20059 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/platform/jr200.py
--rw-r-----   0 cjs       (1765) cjs       (1765)    16545 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/platform/mb6885.py
--rw-r-----   0 cjs       (1765) cjs       (1765)    12946 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/platform/pc8001.py
--rw-r-----   0 cjs       (1765) cjs       (1765)     8509 2024-04-23 08:53:57.000000 r8format-0.0.2/psrc/cmtconv/platform/tk85.py
-drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-23 10:53:27.593995 r8format-0.0.2/psrc/r8format.egg-info/
--rw-r--r--   0 cjs       (1765) cjs       (1765)     4396 2024-04-23 10:53:27.000000 r8format-0.0.2/psrc/r8format.egg-info/PKG-INFO
--rw-r-----   0 cjs       (1765) cjs       (1765)      932 2024-04-23 10:53:27.000000 r8format-0.0.2/psrc/r8format.egg-info/SOURCES.txt
--rw-r-----   0 cjs       (1765) cjs       (1765)        1 2024-04-23 10:53:27.000000 r8format-0.0.2/psrc/r8format.egg-info/dependency_links.txt
--rw-r-----   0 cjs       (1765) cjs       (1765)      228 2024-04-23 10:53:27.000000 r8format-0.0.2/psrc/r8format.egg-info/entry_points.txt
--rw-r-----   0 cjs       (1765) cjs       (1765)       22 2024-04-23 10:53:27.000000 r8format-0.0.2/psrc/r8format.egg-info/top_level.txt
--rw-r-----   0 cjs       (1765) cjs       (1765)      787 2024-04-23 10:52:05.000000 r8format-0.0.2/pyproject.toml
--rw-r-----   0 cjs       (1765) cjs       (1765)       38 2024-04-23 10:53:27.597995 r8format-0.0.2/setup.cfg
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.718347 r8format-0.0.3/
+-rw-r--r--   0 cjs       (1765) cjs       (1765)     4460 2024-04-25 07:32:55.718347 r8format-0.0.3/PKG-INFO
+-rw-r-----   0 cjs       (1765) cjs       (1765)     4224 2024-04-23 11:14:34.000000 r8format-0.0.3/README.md
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.710347 r8format-0.0.3/doc/
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1585 2024-04-25 07:31:23.000000 r8format-0.0.3/doc/CHANGELOG.md
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1011 2024-04-23 15:42:43.000000 r8format-0.0.3/doc/TODO.md
+-rw-r-----   0 cjs       (1765) cjs       (1765)     7734 2024-04-23 08:53:57.000000 r8format-0.0.3/doc/bastok.md
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1240 2024-04-23 08:53:57.000000 r8format-0.0.3/doc/cmtconv.md
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1354 2024-04-23 14:08:31.000000 r8format-0.0.3/doc/release.md
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.710347 r8format-0.0.3/psrc/
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/bastok/
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1464 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/blines.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/bastok/charset/
+-rw-r-----   0 cjs       (1765) cjs       (1765)     6822 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/charset/__init__.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     5844 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/charset/msx.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/bastok/cli/
+-rwxr-x---   0 cjs       (1765) cjs       (1765)     3527 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/cli/basdump.py
+-rwxr-x---   0 cjs       (1765) cjs       (1765)     1165 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/cli/blines.py
+-rwxr-x---   0 cjs       (1765) cjs       (1765)     2264 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/cli/detok.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/bastok/detok/
+-rw-r-----   0 cjs       (1765) cjs       (1765)    28656 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/detok/msx2.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     9042 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/bastok/tlines.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/binary/
+-rw-r-----   0 cjs       (1765) cjs       (1765)      152 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/__init__.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/binary/cli/
+-rwxr-x---   0 cjs       (1765) cjs       (1765)     2926 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/cli/msx_dasm.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     3414 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/memimage.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     5441 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/symtab.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/binary/tool/
+-rw-r-----   0 cjs       (1765) cjs       (1765)       82 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/tool/__init__.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)    11413 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/tool/asl.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)    13158 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/binary/tool/asxxxx.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/cmtconv/
+-rw-r-----   0 cjs       (1765) cjs       (1765)      242 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/analyze.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)    20766 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/audio.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     6517 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/bytestream.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.714347 r8format-0.0.3/psrc/cmtconv/cli/
+-rwxr-x---   0 cjs       (1765) cjs       (1765)    12247 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/cli/analyze_cmt.py
+-rwxr-x---   0 cjs       (1765) cjs       (1765)     2522 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/cli/cmtconv.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     2010 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/formats.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     4804 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/logging.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.718347 r8format-0.0.3/psrc/cmtconv/platform/
+-rw-r-----   0 cjs       (1765) cjs       (1765)    14253 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/platform/fm7.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)    20059 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/platform/jr200.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)    16545 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/platform/mb6885.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)    12946 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/platform/pc8001.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     8509 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/cmtconv/platform/tk85.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)       72 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/conftest.py
+-rw-r-----   0 cjs       (1765) cjs       (1765)     9410 2024-04-23 08:53:57.000000 r8format-0.0.3/psrc/pytest_pt.py
+drwxr-x---   0 cjs       (1765) cjs       (1765)        0 2024-04-25 07:32:55.718347 r8format-0.0.3/psrc/r8format.egg-info/
+-rw-r--r--   0 cjs       (1765) cjs       (1765)     4460 2024-04-25 07:32:55.000000 r8format-0.0.3/psrc/r8format.egg-info/PKG-INFO
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1040 2024-04-25 07:32:55.000000 r8format-0.0.3/psrc/r8format.egg-info/SOURCES.txt
+-rw-r-----   0 cjs       (1765) cjs       (1765)        1 2024-04-25 07:32:55.000000 r8format-0.0.3/psrc/r8format.egg-info/dependency_links.txt
+-rw-r-----   0 cjs       (1765) cjs       (1765)      228 2024-04-25 07:32:55.000000 r8format-0.0.3/psrc/r8format.egg-info/entry_points.txt
+-rw-r-----   0 cjs       (1765) cjs       (1765)       32 2024-04-25 07:32:55.000000 r8format-0.0.3/psrc/r8format.egg-info/top_level.txt
+-rw-r-----   0 cjs       (1765) cjs       (1765)     1311 2024-04-25 07:30:19.000000 r8format-0.0.3/pyproject.toml
+-rw-r-----   0 cjs       (1765) cjs       (1765)       38 2024-04-25 07:32:55.718347 r8format-0.0.3/setup.cfg
```

### Comparing `r8format-0.0.2/PKG-INFO` & `r8format-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r8format
-Version: 0.0.2
+Version: 0.0.3
 Summary: Retrocomputing 8-bit file format manipulation tools
 Author-email: "Curt J. Sampson" <cjs@cynic.net>, Stuart Croy <stuartcroy@mac.com>
 Description-Content-Type: text/markdown
 
 r8format - Tools for Manipulating and Converting Retro-8-bit File Formats
 =========================================================================
 
@@ -14,23 +14,24 @@
 
 #### Installation
 
 This is a [PyPA] package than can be built/installed with any compliant
 tool, such as Pip. We suggest you install it in a virtualenv, but this
 isn't necessary. Typical methods of installation include:
 
+    #   Install the most recent release from PyPI
+    pip install r8format        # https://pypi.org/project/r8format/
+
     #   Install the latest version directly from GitHub.
     pip install git+https://github.com/mc68-net/r8format.git
 
     #   Install local copy of the repo in editable form.
     #   You almost certainly want to be using a virtual environment for this.
     pip install -q -e ./r8format
 
-A [PyPI] package is planned.
-
 On Linux, the top-level `./Test` script in the repo will run both the
 unit and functional (command-line) tests. This has been tested only
 under Linux, but will likely work under Windows as well.
 
 If you have a need to run this on a platform that isn't working, please
 contact the authors (below) for support.
 
@@ -104,15 +105,14 @@
 - Curt J. Sampson <cjs@cynic.net> (GitHub:[0cjs] Discord:`0cjs`)
 - Stuart Croy (GitHub:[croys])
 
 
 
 <!-------------------------------------------------------------------->
 [PyPA]: https://packaging.python.org/en/latest/specifications/
-[PyPI]: https://pypi.org/
 
 <!-- Programs -->
 [bt]: ./doc/bastok.md
 [cc]: ./doc/cmtconv.md
 
 <!-- Support and Authors -->
 [0cjs]: https://github.com/0cjs
```

### Comparing `r8format-0.0.2/README.md` & `r8format-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 #### Installation
 
 This is a [PyPA] package than can be built/installed with any compliant
 tool, such as Pip. We suggest you install it in a virtualenv, but this
 isn't necessary. Typical methods of installation include:
 
+    #   Install the most recent release from PyPI
+    pip install r8format        # https://pypi.org/project/r8format/
+
     #   Install the latest version directly from GitHub.
     pip install git+https://github.com/mc68-net/r8format.git
 
     #   Install local copy of the repo in editable form.
     #   You almost certainly want to be using a virtual environment for this.
     pip install -q -e ./r8format
 
-A [PyPI] package is planned.
-
 On Linux, the top-level `./Test` script in the repo will run both the
 unit and functional (command-line) tests. This has been tested only
 under Linux, but will likely work under Windows as well.
 
 If you have a need to run this on a platform that isn't working, please
 contact the authors (below) for support.
 
@@ -97,15 +98,14 @@
 - Curt J. Sampson <cjs@cynic.net> (GitHub:[0cjs] Discord:`0cjs`)
 - Stuart Croy (GitHub:[croys])
 
 
 
 <!-------------------------------------------------------------------->
 [PyPA]: https://packaging.python.org/en/latest/specifications/
-[PyPI]: https://pypi.org/
 
 <!-- Programs -->
 [bt]: ./doc/bastok.md
 [cc]: ./doc/cmtconv.md
 
 <!-- Support and Authors -->
 [0cjs]: https://github.com/0cjs
```

### Comparing `r8format-0.0.2/psrc/bastok/blines.py` & `r8format-0.0.3/psrc/bastok/blines.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/charset/__init__.py` & `r8format-0.0.3/psrc/bastok/charset/__init__.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/charset/msx.py` & `r8format-0.0.3/psrc/bastok/charset/msx.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/cli/basdump.py` & `r8format-0.0.3/psrc/bastok/cli/basdump.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/cli/blines.py` & `r8format-0.0.3/psrc/bastok/cli/blines.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/cli/detok.py` & `r8format-0.0.3/psrc/bastok/cli/detok.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/detok/msx2.py` & `r8format-0.0.3/psrc/bastok/detok/msx2.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/bastok/tlines.py` & `r8format-0.0.3/psrc/bastok/tlines.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/binary/cli/msx_dasm.py` & `r8format-0.0.3/psrc/binary/cli/msx_dasm.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/binary/memimage.py` & `r8format-0.0.3/psrc/binary/memimage.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/binary/symtab.py` & `r8format-0.0.3/psrc/binary/symtab.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/binary/tool/asl.py` & `r8format-0.0.3/psrc/binary/tool/asl.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/binary/tool/asxxxx.py` & `r8format-0.0.3/psrc/binary/tool/asxxxx.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/audio.py` & `r8format-0.0.3/psrc/cmtconv/audio.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/bytestream.py` & `r8format-0.0.3/psrc/cmtconv/bytestream.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/cli/analyze_cmt.py` & `r8format-0.0.3/psrc/cmtconv/cli/analyze_cmt.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/cli/cmtconv.py` & `r8format-0.0.3/psrc/cmtconv/cli/cmtconv.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/formats.py` & `r8format-0.0.3/psrc/cmtconv/formats.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/logging.py` & `r8format-0.0.3/psrc/cmtconv/logging.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/platform/fm7.py` & `r8format-0.0.3/psrc/cmtconv/platform/fm7.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/platform/jr200.py` & `r8format-0.0.3/psrc/cmtconv/platform/jr200.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/platform/mb6885.py` & `r8format-0.0.3/psrc/cmtconv/platform/mb6885.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/platform/pc8001.py` & `r8format-0.0.3/psrc/cmtconv/platform/pc8001.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/cmtconv/platform/tk85.py` & `r8format-0.0.3/psrc/cmtconv/platform/tk85.py`

 * *Files identical despite different names*

### Comparing `r8format-0.0.2/psrc/r8format.egg-info/PKG-INFO` & `r8format-0.0.3/psrc/r8format.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r8format
-Version: 0.0.2
+Version: 0.0.3
 Summary: Retrocomputing 8-bit file format manipulation tools
 Author-email: "Curt J. Sampson" <cjs@cynic.net>, Stuart Croy <stuartcroy@mac.com>
 Description-Content-Type: text/markdown
 
 r8format - Tools for Manipulating and Converting Retro-8-bit File Formats
 =========================================================================
 
@@ -14,23 +14,24 @@
 
 #### Installation
 
 This is a [PyPA] package than can be built/installed with any compliant
 tool, such as Pip. We suggest you install it in a virtualenv, but this
 isn't necessary. Typical methods of installation include:
 
+    #   Install the most recent release from PyPI
+    pip install r8format        # https://pypi.org/project/r8format/
+
     #   Install the latest version directly from GitHub.
     pip install git+https://github.com/mc68-net/r8format.git
 
     #   Install local copy of the repo in editable form.
     #   You almost certainly want to be using a virtual environment for this.
     pip install -q -e ./r8format
 
-A [PyPI] package is planned.
-
 On Linux, the top-level `./Test` script in the repo will run both the
 unit and functional (command-line) tests. This has been tested only
 under Linux, but will likely work under Windows as well.
 
 If you have a need to run this on a platform that isn't working, please
 contact the authors (below) for support.
 
@@ -104,15 +105,14 @@
 - Curt J. Sampson <cjs@cynic.net> (GitHub:[0cjs] Discord:`0cjs`)
 - Stuart Croy (GitHub:[croys])
 
 
 
 <!-------------------------------------------------------------------->
 [PyPA]: https://packaging.python.org/en/latest/specifications/
-[PyPI]: https://pypi.org/
 
 <!-- Programs -->
 [bt]: ./doc/bastok.md
 [cc]: ./doc/cmtconv.md
 
 <!-- Support and Authors -->
 [0cjs]: https://github.com/0cjs
```

### Comparing `r8format-0.0.2/psrc/r8format.egg-info/SOURCES.txt` & `r8format-0.0.3/psrc/r8format.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 README.md
 pyproject.toml
+doc/CHANGELOG.md
+doc/TODO.md
+doc/bastok.md
+doc/cmtconv.md
+doc/release.md
+psrc/conftest.py
+psrc/pytest_pt.py
 psrc/bastok/blines.py
 psrc/bastok/tlines.py
 psrc/bastok/charset/__init__.py
 psrc/bastok/charset/msx.py
 psrc/bastok/cli/basdump.py
 psrc/bastok/cli/blines.py
 psrc/bastok/cli/detok.py
```


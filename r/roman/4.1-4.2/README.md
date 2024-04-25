# Comparing `tmp/roman-4.1.tar.gz` & `tmp/roman-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roman-4.1.tar", last modified: Fri May 26 08:25:05 2023, max compression
+gzip compressed data, was "roman-4.2.tar", last modified: Thu Apr 25 05:25:07 2024, max compression
```

## Comparing `roman-4.1.tar` & `roman-4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-26 08:25:05.000000 roman-4.1/
--rw-r--r--   0 jens       (501) staff       (20)     1017 2023-05-26 08:23:27.000000 roman-4.1/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      804 2023-04-20 08:26:38.000000 roman-4.1/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       30 2023-05-26 08:23:02.000000 roman-4.1/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2023-05-26 08:23:02.000000 roman-4.1/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      196 2023-04-20 08:26:38.000000 roman-4.1/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)     4238 2023-05-26 08:25:05.000000 roman-4.1/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1148 2021-11-02 08:52:53.000000 roman-4.1/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      423 2023-05-26 08:25:05.000000 roman-4.1/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2203 2023-05-26 08:23:36.000000 roman-4.1/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-26 08:25:05.000000 roman-4.1/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)     4238 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      325 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)       38 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        6 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-25 13:53:40.000000 roman-4.1/src/roman.egg-info/zip-safe
--rw-r--r--   0 jens       (501) staff       (20)     4280 2023-05-26 08:23:02.000000 roman-4.1/src/roman.py
--rw-r--r--   0 jens       (501) staff       (20)     3293 2023-05-26 08:23:02.000000 roman-4.1/src/tests.py
--rw-r--r--   0 jens       (501) staff       (20)     1425 2023-04-20 08:26:38.000000 roman-4.1/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-25 05:25:07.993183 roman-4.2/
+-rw-r--r--   0 jens       (501) staff       (20)     1215 2024-04-25 05:23:20.000000 roman-4.2/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2024-04-25 05:19:16.000000 roman-4.2/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       30 2023-05-26 08:23:02.000000 roman-4.2/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2023-05-26 08:23:02.000000 roman-4.2/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      196 2024-04-25 05:19:16.000000 roman-4.2/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)     3605 2024-04-25 05:25:07.993134 roman-4.2/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1148 2021-11-02 08:52:53.000000 roman-4.2/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      389 2024-04-25 05:25:07.993421 roman-4.2/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2303 2024-04-25 05:23:31.000000 roman-4.2/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-25 05:25:07.992277 roman-4.2/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-25 05:25:07.992974 roman-4.2/src/roman.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)     3605 2024-04-25 05:25:07.000000 roman-4.2/src/roman.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      325 2024-04-25 05:25:07.000000 roman-4.2/src/roman.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-04-25 05:25:07.000000 roman-4.2/src/roman.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       37 2024-04-25 05:25:07.000000 roman-4.2/src/roman.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        6 2024-04-25 05:25:07.000000 roman-4.2/src/roman.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-25 13:53:40.000000 roman-4.2/src/roman.egg-info/zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)     4108 2024-04-25 05:18:32.000000 roman-4.2/src/roman.py
+-rw-r--r--   0 jens       (501) staff       (20)     3293 2023-05-26 08:23:02.000000 roman-4.2/src/tests.py
+-rw-r--r--   0 jens       (501) staff       (20)     1901 2024-04-25 05:19:16.000000 roman-4.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `roman-4.1/CHANGES.rst` & `roman-4.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Change log
 ==========
 
+4.2 (2024-04-25)
+----------------
+
+- Remove overlooked mentions of the Python 2.1.1 license
+  (`#17 <https://github.com/zopefoundation/roman/issues/17>`_)
+
+- Add support for Python 3.12 and 3.13.
+
+
 4.1 (2023-05-26)
 ----------------
 
 - Change license to the Zope Public License (ZPL) version 2.1
   (`#15 <https://github.com/zopefoundation/roman/issues/15>`_)
```

### Comparing `roman-4.1/CONTRIBUTING.md` & `roman-4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `roman-4.1/LICENSE.txt` & `roman-4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roman-4.1/README.rst` & `roman-4.2/README.rst`

 * *Files identical despite different names*

### Comparing `roman-4.1/setup.py` & `roman-4.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 desc = ('{}\n\n{}'.format(open('README.rst').read(),
                           open('CHANGES.rst').read()))
 
 setup(
     name='roman',
-    version='4.1',
+    version='4.2',
     author="Mark Pilgrim",
     maintainer="Zope Foundation and Contributors",
     maintainer_email="zope-dev@zope.dev",
     description="Integer to Roman numerals converter",
     long_description=desc,
     long_description_content_type='text/x-rst',
     license="ZPL 2.1",
@@ -35,14 +35,16 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
         'Natural Language :: English',
         'Operating System :: OS Independent',
     ],
```

### Comparing `roman-4.1/src/roman.py` & `roman-4.2/src/roman.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 __version__ = "1.4"
 __date__ = "8 August 2001"
 __copyright__ = """Copyright (c) 2001 Mark Pilgrim
 
 This program is part of "Dive Into Python", a free Python tutorial for
 experienced programmers.  Visit http://diveintopython.org/ for the
 latest version.
-
-This program is free software; you can redistribute it and/or modify
-it under the terms of the Python 2.1.1 license, available at
-http://www.python.org/2.1.1/license.html
 """
 
 import argparse
 import re
 import sys
```

### Comparing `roman-4.1/src/tests.py` & `roman-4.2/src/tests.py`

 * *Files identical despite different names*


# Comparing `tmp/Geode_Background-7.9.8-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Background-7.9.8rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 3221972 bytes, number of entries: 16
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-25 00:20 geode_background/__init__.py
--rw-r--r--  2.0 unx      191 b- defN 24-Apr-25 00:20 geode_background/brep.py
--rw-r--r--  2.0 unx      192 b- defN 24-Apr-25 00:20 geode_background/solid.py
--rw-r--r--  2.0 unx      196 b- defN 24-Apr-25 00:20 geode_background/surface.py
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-25 00:21 geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-25 00:21 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-25 00:21 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-25 00:21 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   155192 b- defN 24-Apr-25 00:21 geode_background/lib64/libGeode-Background_brep.so
--rwxr-xr-x  2.0 unx   109008 b- defN 24-Apr-25 00:21 geode_background/lib64/libGeode-Background_common.so
--rwxr-xr-x  2.0 unx  3420848 b- defN 24-Apr-25 00:21 geode_background/lib64/libGeode-Background_solid.so
--rwxr-xr-x  2.0 unx  3235312 b- defN 24-Apr-25 00:21 geode_background/lib64/libGeode-Background_surface.so
--rw-r--r--  2.0 unx     1057 b- defN 24-Apr-25 00:21 Geode_Background-7.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 24-Apr-25 00:21 Geode_Background-7.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-25 00:21 Geode_Background-7.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1661 b- defN 24-Apr-25 00:21 Geode_Background-7.9.8.dist-info/RECORD
-16 files, 7412943 bytes uncompressed, 3219150 bytes compressed:  56.6%
+Zip file size: 4725539 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      216 b- defN 24-Apr-24 09:02 geode_background/__init__.py
+-rw-rw-rw-  2.0 fat      199 b- defN 24-Apr-24 09:02 geode_background/brep.py
+-rw-rw-rw-  2.0 fat      199 b- defN 24-Apr-24 09:02 geode_background/solid.py
+-rw-rw-rw-  2.0 fat      203 b- defN 24-Apr-24 09:02 geode_background/surface.py
+-rw-rw-rw-  2.0 fat  3766784 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_brep.dll
+-rw-rw-rw-  2.0 fat    53248 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_common.dll
+-rw-rw-rw-  2.0 fat  3963392 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_solid.dll
+-rw-rw-rw-  2.0 fat  3811328 b- defN 24-Apr-24 09:03 geode_background/bin/Geode-Background_surface.dll
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-24 09:03 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1104 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1601 b- defN 24-Apr-24 09:03 Geode_Background-7.9.8rc1.dist-info/RECORD
+16 files, 12100151 bytes uncompressed, 4722837 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -6,44 +6,44 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_brep.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_common.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_solid.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_surface.dll
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_brep.so
+Filename: geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_common.so
+Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_solid.so
+Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_surface.so
+Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Background-7.9.8.dist-info/METADATA
+Filename: Geode_Background-7.9.8rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.9.8.dist-info/WHEEL
+Filename: Geode_Background-7.9.8rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.9.8.dist-info/top_level.txt
+Filename: Geode_Background-7.9.8rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.9.8.dist-info/RECORD
+Filename: Geode_Background-7.9.8rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,5 +1,8 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-from .surface import *
-from .solid import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .surface import *
+from .solid import *
+from .brep import *
```

## geode_background/brep.py

```diff
@@ -1,10 +1,10 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_brep import *
-
-BackgroundBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_brep import *
+
+BackgroundBRepLibrary.initialize()
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

## Comparing `Geode_Background-7.9.8.dist-info/METADATA` & `Geode_Background-7.9.8rc1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 2.1
-Name: Geode-Background
-Version: 7.9.8
-Summary: Geode-solutions OpenGeode module for building background meshes
-Home-page: https://github.com/Geode-solutions/Geode-Background
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common ==31.*,>=31.0.8
-Requires-Dist: opengeode-core ==14.*,>=14.19.2
-
-<h1 align="center">Background<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Module to generate background meshes and background models for OpenGeode</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Background_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Background_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Background_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Background_private.svg" alt="Version">
-</p>
+Metadata-Version: 2.1
+Name: Geode-Background
+Version: 7.9.8rc1
+Summary: Geode-solutions OpenGeode module for building background meshes
+Home-page: https://github.com/Geode-solutions/Geode-Background
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common ==31.*,>=31.0.8
+Requires-Dist: opengeode-core ==14.*,>=14.19.2
+
+<h1 align="center">Background<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Module to generate background meshes and background models for OpenGeode</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Background_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Background_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Background_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Background_private.svg" alt="Version">
+</p>
+
+
```


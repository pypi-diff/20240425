# Comparing `tmp/cirq-1.4.0.dev20240419073809-py3-none-any.whl.zip` & `tmp/cirq-1.4.0.dev20240425182738-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8341 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 24-Apr-19 07:38 cirq-1.4.0.dev20240419073809.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-19 07:38 cirq-1.4.0.dev20240419073809.dist-info/LICENSE
--rw-r--r--  2.0 unx     7832 b- defN 24-Apr-19 07:38 cirq-1.4.0.dev20240419073809.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 07:38 cirq-1.4.0.dev20240419073809.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-19 07:38 cirq-1.4.0.dev20240419073809.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 24-Apr-19 07:38 cirq-1.4.0.dev20240419073809.dist-info/RECORD
-6 files, 20137 bytes uncompressed, 7303 bytes compressed:  63.7%
+Zip file size: 8340 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 24-Apr-25 18:27 cirq-1.4.0.dev20240425182738.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-25 18:27 cirq-1.4.0.dev20240425182738.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7832 b- defN 24-Apr-25 18:27 cirq-1.4.0.dev20240425182738.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 18:27 cirq-1.4.0.dev20240425182738.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 18:27 cirq-1.4.0.dev20240425182738.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 24-Apr-25 18:27 cirq-1.4.0.dev20240425182738.dist-info/RECORD
+6 files, 20137 bytes uncompressed, 7302 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.4.0.dev20240419073809.dist-info/AUTHORS
+Filename: cirq-1.4.0.dev20240425182738.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.4.0.dev20240419073809.dist-info/LICENSE
+Filename: cirq-1.4.0.dev20240425182738.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.4.0.dev20240419073809.dist-info/METADATA
+Filename: cirq-1.4.0.dev20240425182738.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.4.0.dev20240419073809.dist-info/WHEEL
+Filename: cirq-1.4.0.dev20240425182738.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.4.0.dev20240419073809.dist-info/top_level.txt
+Filename: cirq-1.4.0.dev20240425182738.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.4.0.dev20240419073809.dist-info/RECORD
+Filename: cirq-1.4.0.dev20240425182738.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.4.0.dev20240419073809.dist-info/LICENSE` & `cirq-1.4.0.dev20240425182738.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.4.0.dev20240419073809.dist-info/METADATA` & `cirq-1.4.0.dev20240425182738.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.4.0.dev20240419073809
+Version: 1.4.0.dev20240425182738
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt ==1.4.0.dev20240419073809
-Requires-Dist: cirq-core ==1.4.0.dev20240419073809
-Requires-Dist: cirq-ft ==1.4.0.dev20240419073809
-Requires-Dist: cirq-google ==1.4.0.dev20240419073809
-Requires-Dist: cirq-ionq ==1.4.0.dev20240419073809
-Requires-Dist: cirq-pasqal ==1.4.0.dev20240419073809
-Requires-Dist: cirq-rigetti ==1.4.0.dev20240419073809
-Requires-Dist: cirq-web ==1.4.0.dev20240419073809
+Requires-Dist: cirq-aqt ==1.4.0.dev20240425182738
+Requires-Dist: cirq-core ==1.4.0.dev20240425182738
+Requires-Dist: cirq-ft ==1.4.0.dev20240425182738
+Requires-Dist: cirq-google ==1.4.0.dev20240425182738
+Requires-Dist: cirq-ionq ==1.4.0.dev20240425182738
+Requires-Dist: cirq-pasqal ==1.4.0.dev20240425182738
+Requires-Dist: cirq-rigetti ==1.4.0.dev20240425182738
+Requires-Dist: cirq-web ==1.4.0.dev20240425182738
 Provides-Extra: dev_env
 Requires-Dist: mypy ==1.2.0 ; extra == 'dev_env'
 Requires-Dist: types-backports ==0.1.3 ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf ~=3.20 ; extra == 'dev_env'
 Requires-Dist: types-requests ==2.28.1 ; extra == 'dev_env'
 Requires-Dist: types-setuptools ==62.6.1 ; extra == 'dev_env'
```

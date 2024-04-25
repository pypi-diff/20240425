# Comparing `tmp/composabl_api_dev-0.8.0.dev43-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/composabl_api_dev-0.8.0.dev44-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 757664 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-23 20:17 composabl_api_dev-0.8.0.dev43.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-23 20:17 composabl_api_dev.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-23 20:17 composabl_api/
--rw-r--r--  2.0 unx     1684 b- defN 24-Apr-23 20:17 composabl_api_dev-0.8.0.dev43.dist-info/METADATA
--rw-rw-r--  2.0 unx      593 b- defN 24-Apr-23 20:17 composabl_api_dev-0.8.0.dev43.dist-info/RECORD
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-23 20:17 composabl_api_dev-0.8.0.dev43.dist-info/top_level.txt
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-23 20:17 composabl_api_dev-0.8.0.dev43.dist-info/WHEEL
--rwxr-xr-x  2.0 unx    84656 b- defN 24-Apr-23 20:17 composabl_api/__init__.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx  2820608 b- defN 24-Apr-23 20:17 composabl_api/nocode.cpython-311-x86_64-linux-gnu.so
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:40 composabl_api_dev.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:40 composabl_api/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:40 composabl_api_dev-0.8.0.dev44.dist-info/
+-rwxr-xr-x  2.0 unx    84656 b- defN 24-Apr-25 15:40 composabl_api/__init__.cpython-311-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  2820608 b- defN 24-Apr-25 15:40 composabl_api/nocode.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1684 b- defN 24-Apr-25 15:40 composabl_api_dev-0.8.0.dev44.dist-info/METADATA
+-rw-rw-r--  2.0 unx      593 b- defN 24-Apr-25 15:40 composabl_api_dev-0.8.0.dev44.dist-info/RECORD
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-25 15:40 composabl_api_dev-0.8.0.dev44.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-25 15:40 composabl_api_dev-0.8.0.dev44.dist-info/WHEEL
 9 files, 2907707 bytes uncompressed, 756208 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: composabl_api_dev-0.8.0.dev43.dist-info/
-Comment: 
-
 Filename: composabl_api_dev.libs/
 Comment: 
 
 Filename: composabl_api/
 Comment: 
 
-Filename: composabl_api_dev-0.8.0.dev43.dist-info/METADATA
+Filename: composabl_api_dev-0.8.0.dev44.dist-info/
+Comment: 
+
+Filename: composabl_api/__init__.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: composabl_api_dev-0.8.0.dev43.dist-info/RECORD
+Filename: composabl_api/nocode.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: composabl_api_dev-0.8.0.dev43.dist-info/top_level.txt
+Filename: composabl_api_dev-0.8.0.dev44.dist-info/METADATA
 Comment: 
 
-Filename: composabl_api_dev-0.8.0.dev43.dist-info/WHEEL
+Filename: composabl_api_dev-0.8.0.dev44.dist-info/RECORD
 Comment: 
 
-Filename: composabl_api/__init__.cpython-311-x86_64-linux-gnu.so
+Filename: composabl_api_dev-0.8.0.dev44.dist-info/top_level.txt
 Comment: 
 
-Filename: composabl_api/nocode.cpython-311-x86_64-linux-gnu.so
+Filename: composabl_api_dev-0.8.0.dev44.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## Comparing `composabl_api_dev-0.8.0.dev43.dist-info/METADATA` & `composabl_api_dev-0.8.0.dev44.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composabl-api-dev
-Version: 0.8.0.dev43
+Version: 0.8.0.dev44
 Summary: the Composabl API
 Author-email: Composabl <info@composabl.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: cython
 Requires-Dist: ruff
 Requires-Dist: simple-term-menu
```

## Comparing `composabl_api_dev-0.8.0.dev43.dist-info/RECORD` & `composabl_api_dev-0.8.0.dev44.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-composabl_api_dev-0.8.0.dev43.dist-info/METADATA,sha256=XM1mJouGOpzXqXnp-nnsKNerCZ4CHGiJxMWawVf5zDA,1684
-composabl_api_dev-0.8.0.dev43.dist-info/RECORD,,
-composabl_api_dev-0.8.0.dev43.dist-info/top_level.txt,sha256=bxdD4xIxmo1HURkgiI6n1Rl2HZ5q-3i3JrHx8uS8lHc,14
-composabl_api_dev-0.8.0.dev43.dist-info/WHEEL,sha256=-7Vwsd-KuPOtdyxdAC8drxF7lN4th9mKINh8g6MaZ9k,152
 composabl_api/__init__.cpython-311-x86_64-linux-gnu.so,sha256=kIaEfB0zis76I_hQymVbvdS8t0Po9fLRIlkX_8ReFbc,84656
 composabl_api/nocode.cpython-311-x86_64-linux-gnu.so,sha256=XpQ7U7F62XWQk2Ycl5AbanTTR7o5bxftskvdSe3N72s,2820608
+composabl_api_dev-0.8.0.dev44.dist-info/METADATA,sha256=CIHDkpVfJkknHtOpXeloQewnBzgGFyzfnCpmOVMshws,1684
+composabl_api_dev-0.8.0.dev44.dist-info/RECORD,,
+composabl_api_dev-0.8.0.dev44.dist-info/top_level.txt,sha256=bxdD4xIxmo1HURkgiI6n1Rl2HZ5q-3i3JrHx8uS8lHc,14
+composabl_api_dev-0.8.0.dev44.dist-info/WHEEL,sha256=-7Vwsd-KuPOtdyxdAC8drxF7lN4th9mKINh8g6MaZ9k,152
```


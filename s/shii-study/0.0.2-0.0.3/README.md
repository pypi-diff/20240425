# Comparing `tmp/shii_study-0.0.2-py2.py3-none-any.whl.zip` & `tmp/shii_study-0.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 3182 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 shii/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 shii/src/__init__.py
--rw-r--r--  2.0 unx       17 b- defN 80-Jan-01 00:00 shii/src/shii/__init__.py
--rw-r--r--  2.0 unx     2975 b- defN 80-Jan-01 00:00 shii/src/shii/study.py
--rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      612 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/RECORD
-8 files, 4519 bytes uncompressed, 2106 bytes compressed:  53.4%
+Zip file size: 3107 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 80-Jan-01 00:00 shii/__init__.py
+-rw-r--r--  2.0 unx       17 b- defN 80-Jan-01 00:00 shii/src/__init__.py
+-rw-r--r--  2.0 unx     2975 b- defN 80-Jan-01 00:00 shii/src/study.py
+-rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      529 b- defN 80-Jan-01 00:00 shii_study-0.0.3.dist-info/RECORD
+7 files, 4533 bytes uncompressed, 2167 bytes compressed:  52.2%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: shii/__init__.py
 Comment: 
 
 Filename: shii/src/__init__.py
 Comment: 
 
-Filename: shii/src/shii/__init__.py
+Filename: shii/src/study.py
 Comment: 
 
-Filename: shii/src/shii/study.py
+Filename: shii_study-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: shii_study-0.0.2.dist-info/METADATA
+Filename: shii_study-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: shii_study-0.0.2.dist-info/WHEEL
+Filename: shii_study-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: shii_study-0.0.2.dist-info/top_level.txt
-Comment: 
-
-Filename: shii_study-0.0.2.dist-info/RECORD
+Filename: shii_study-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shii/__init__.py

```diff
@@ -0,0 +1,7 @@
+00000000: 6672 6f6d 2073 7263 2e73 7475 6479 2069  from src.study i
+00000010: 6d70 6f72 7420 7374 7564 792c 2073 7475  mport study, stu
+00000020: 6479 5f72 6574 7572 6e5f 7465 7874 2c20  dy_return_text, 
+00000030: 6e6f 5f73 7475 6479 5f72 6574 7572 6e5f  no_study_return_
+00000040: 7465 7874 2c20 7374 7564 795f 7361 790a  text, study_say.
+00000050: 7665 7273 696f 6e20 3d20 2730 2e30 2e33  version = '0.0.3
+00000060: 27                                       '
```

## shii/src/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 7665 7273 696f 6e20 3d20 2730 2e30 2e33  version = '0.0.3
+00000010: 27                                       '
```

## Comparing `shii/src/shii/study.py` & `shii/src/study.py`

 * *Files identical despite different names*

## Comparing `shii_study-0.0.2.dist-info/METADATA` & `shii_study-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shii_study
-Version: 0.0.2
+Version: 0.0.3
 Summary: PYPI tutorial package creation written by Boran
 Home-page: https://github.com/boranloves/shii
 Author: boran
 Author-email: boran <boran@shii.me>
 Project-URL: Homepage, https://github.com/boranloves/shii
 Project-URL: Issues, https://github.com/boranloves/shii
 Classifier: Programming Language :: Python :: 3
```


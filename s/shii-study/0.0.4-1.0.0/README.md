# Comparing `tmp/shii_study-0.0.4-py2.py3-none-any.whl.zip` & `tmp/shii_study-1.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3150 bytes, number of entries: 7
--rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 shii/__init__.py
+Zip file size: 3148 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 shii/__init__.py
 -rw-r--r--  2.0 unx       17 b- defN 80-Jan-01 00:00 shii/src/__init__.py
 -rw-r--r--  2.0 unx     2975 b- defN 80-Jan-01 00:00 shii/src/study.py
--rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 80-Jan-01 00:00 shii_study-0.0.4.dist-info/RECORD
-7 files, 4630 bytes uncompressed, 2210 bytes compressed:  52.3%
+-rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 80-Jan-01 00:00 shii_study-1.0.0.dist-info/RECORD
+7 files, 4641 bytes uncompressed, 2208 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: shii/src/__init__.py
 Comment: 
 
 Filename: shii/src/study.py
 Comment: 
 
-Filename: shii_study-0.0.4.dist-info/METADATA
+Filename: shii_study-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: shii_study-0.0.4.dist-info/WHEEL
+Filename: shii_study-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: shii_study-0.0.4.dist-info/top_level.txt
+Filename: shii_study-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: shii_study-0.0.4.dist-info/RECORD
+Filename: shii_study-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shii/__init__.py

```diff
@@ -1,3 +1,3 @@
-from shii.src.study import study, study_return_text, no_study_return_text, study_say
+from shii.src.study import study, study_return_text, no_study_return_text, study_say, del_study
 __all__ = ['study', 'study_return_text', 'study_say', 'no_study_return_text', 'del_study']
-version = '0.0.4'
+version = '1.0.0'
```

## shii/src/__init__.py

```diff
@@ -1 +1 @@
-version = '0.0.4'
+version = '1.0.0'
```

## Comparing `shii_study-0.0.4.dist-info/METADATA` & `shii_study-1.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shii_study
-Version: 0.0.4
+Version: 1.0.0
 Summary: PYPI tutorial package creation written by Boran
 Home-page: https://github.com/boranloves/shii
 Author: boran
 Author-email: boran <boran@shii.me>
 Project-URL: Homepage, https://github.com/boranloves/shii
 Project-URL: Issues, https://github.com/boranloves/shii
 Classifier: Programming Language :: Python :: 3
```


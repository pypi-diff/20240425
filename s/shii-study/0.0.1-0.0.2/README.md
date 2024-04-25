# Comparing `tmp/shii_study-0.0.1-py2.py3-none-any.whl.zip` & `tmp/shii_study-0.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 3034 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 src/__init__.py
--rw-r--r--  2.0 unx       17 b- defN 80-Jan-01 00:00 src/shii/__init__.py
--rw-r--r--  2.0 unx     2975 b- defN 80-Jan-01 00:00 src/shii/study.py
--rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 80-Jan-01 00:00 shii_study-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      527 b- defN 80-Jan-01 00:00 shii_study-0.0.1.dist-info/RECORD
-7 files, 4433 bytes uncompressed, 2096 bytes compressed:  52.7%
+Zip file size: 3182 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 shii/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 shii/src/__init__.py
+-rw-r--r--  2.0 unx       17 b- defN 80-Jan-01 00:00 shii/src/shii/__init__.py
+-rw-r--r--  2.0 unx     2975 b- defN 80-Jan-01 00:00 shii/src/shii/study.py
+-rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      612 b- defN 80-Jan-01 00:00 shii_study-0.0.2.dist-info/RECORD
+8 files, 4519 bytes uncompressed, 2106 bytes compressed:  53.4%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: src/__init__.py
+Filename: shii/__init__.py
 Comment: 
 
-Filename: src/shii/__init__.py
+Filename: shii/src/__init__.py
 Comment: 
 
-Filename: src/shii/study.py
+Filename: shii/src/shii/__init__.py
 Comment: 
 
-Filename: shii_study-0.0.1.dist-info/METADATA
+Filename: shii/src/shii/study.py
 Comment: 
 
-Filename: shii_study-0.0.1.dist-info/WHEEL
+Filename: shii_study-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: shii_study-0.0.1.dist-info/top_level.txt
+Filename: shii_study-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: shii_study-0.0.1.dist-info/RECORD
+Filename: shii_study-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: shii_study-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `src/shii/study.py` & `shii/src/shii/study.py`

 * *Files identical despite different names*

## Comparing `shii_study-0.0.1.dist-info/METADATA` & `shii_study-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shii_study
-Version: 0.0.1
+Version: 0.0.2
 Summary: PYPI tutorial package creation written by Boran
 Home-page: https://github.com/boranloves/shii
 Author: boran
 Author-email: boran <boran@shii.me>
 Project-URL: Homepage, https://github.com/boranloves/shii
 Project-URL: Issues, https://github.com/boranloves/shii
 Classifier: Programming Language :: Python :: 3
```

## Comparing `shii_study-0.0.1.dist-info/RECORD` & `shii_study-0.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-src/shii/__init__.py,sha256=9VhSGV5ZyHfm_vUuUbVSBg_WEobb2WyqcGP5JyQEU-I,17
-src/shii/study.py,sha256=lCWrybj2GY7bVsymRiriTid7j1-75ZNKtU8DmTCm3Zg,2975
-shii_study-0.0.1.dist-info/METADATA,sha256=qCXxj52uD87Fecesw7CO55V3FtCXwZYdNSjpLRkFeKo,800
-shii_study-0.0.1.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-shii_study-0.0.1.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
-shii_study-0.0.1.dist-info/RECORD,,
+shii/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+shii/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+shii/src/shii/__init__.py,sha256=bSqyoeHAucSckl5v3a66CYITyf4PbXqIe37V9U9tp9g,17
+shii/src/shii/study.py,sha256=lCWrybj2GY7bVsymRiriTid7j1-75ZNKtU8DmTCm3Zg,2975
+shii_study-0.0.2.dist-info/METADATA,sha256=5C0RHENuWPBpSb-MIVaojGENkQ5wpkyC1eh4CJZ4tpA,800
+shii_study-0.0.2.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+shii_study-0.0.2.dist-info/top_level.txt,sha256=xSjQX0HJSMT8sgtMRf6vWT1kRi8g03W9l-ttA6Mmbgk,5
+shii_study-0.0.2.dist-info/RECORD,,
```


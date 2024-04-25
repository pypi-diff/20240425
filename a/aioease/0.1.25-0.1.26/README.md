# Comparing `tmp/aioease-0.1.25-py3-none-any.whl.zip` & `tmp/aioease-0.1.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4016 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       25 b- defN 24-Apr-11 19:27 aioease/__init__.py
+Zip file size: 4029 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       40 b- defN 24-Apr-25 16:50 aioease/__init__.py
 -rw-rw-rw-  2.0 fat     3375 b- defN 24-Apr-18 20:43 aioease/main.py
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-18 20:44 aioease-0.1.25.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2776 b- defN 24-Apr-18 20:44 aioease-0.1.25.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 20:44 aioease-0.1.25.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-18 20:44 aioease-0.1.25.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      536 b- defN 24-Apr-18 20:44 aioease-0.1.25.dist-info/RECORD
-7 files, 7884 bytes uncompressed, 3066 bytes compressed:  61.1%
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-25 16:51 aioease-0.1.26.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2776 b- defN 24-Apr-25 16:51 aioease-0.1.26.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 16:51 aioease-0.1.26.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-25 16:51 aioease-0.1.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      536 b- defN 24-Apr-25 16:51 aioease-0.1.26.dist-info/RECORD
+7 files, 7899 bytes uncompressed, 3079 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: aioease/__init__.py
 Comment: 
 
 Filename: aioease/main.py
 Comment: 
 
-Filename: aioease-0.1.25.dist-info/LICENSE
+Filename: aioease-0.1.26.dist-info/LICENSE
 Comment: 
 
-Filename: aioease-0.1.25.dist-info/METADATA
+Filename: aioease-0.1.26.dist-info/METADATA
 Comment: 
 
-Filename: aioease-0.1.25.dist-info/WHEEL
+Filename: aioease-0.1.26.dist-info/WHEEL
 Comment: 
 
-Filename: aioease-0.1.25.dist-info/top_level.txt
+Filename: aioease-0.1.26.dist-info/top_level.txt
 Comment: 
 
-Filename: aioease-0.1.25.dist-info/RECORD
+Filename: aioease-0.1.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aioease/__init__.py

```diff
@@ -1 +1 @@
-from .main import execute
+from .main import execute_async_requests
```

## Comparing `aioease-0.1.25.dist-info/LICENSE` & `aioease-0.1.26.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aioease-0.1.25.dist-info/METADATA` & `aioease-0.1.26.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioease
-Version: 0.1.25
+Version: 0.1.26
 Summary: A simple and easy way to use asyncio & aiohttp libraries.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp >=3
 Requires-Dist: aiolimiter >=1
 
 # AIOEase
```

## Comparing `aioease-0.1.25.dist-info/RECORD` & `aioease-0.1.26.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-aioease/__init__.py,sha256=a6rCsJjLbHO6rDXGUt6aNY0p4pdXPLsraOCXS1b3ebU,25
+aioease/__init__.py,sha256=lR0Hcyx-Ish3yNCWyPpv71wJ9AF-wpXQBSScxoXXHA0,40
 aioease/main.py,sha256=Uk1nWU6HyTp6M55onVZeJCMuZ_Ip9eFF8egNQ5mwy0c,3375
-aioease-0.1.25.dist-info/LICENSE,sha256=KUfCP2RRTQeOp21tGhWgyQC88-Awp1f53UWHBJhbqw4,1072
-aioease-0.1.25.dist-info/METADATA,sha256=wa30PHZBXRiJAB6B1e4vH1zUNZQBrwJW10b04TO8kWg,2776
-aioease-0.1.25.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aioease-0.1.25.dist-info/top_level.txt,sha256=YC746SLK75mF2jnE3ENkKxCYhsK-teH2V1nl1BmrGO4,8
-aioease-0.1.25.dist-info/RECORD,,
+aioease-0.1.26.dist-info/LICENSE,sha256=KUfCP2RRTQeOp21tGhWgyQC88-Awp1f53UWHBJhbqw4,1072
+aioease-0.1.26.dist-info/METADATA,sha256=YfFnTFYv8-Di3pwdJjoe3k3_b4PyW54bDCxap2ZO80Q,2776
+aioease-0.1.26.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aioease-0.1.26.dist-info/top_level.txt,sha256=YC746SLK75mF2jnE3ENkKxCYhsK-teH2V1nl1BmrGO4,8
+aioease-0.1.26.dist-info/RECORD,,
```


# Comparing `tmp/etiq_spark-1.5.1rc3-cp39-cp39-win_amd64.whl.zip` & `tmp/etiq_spark-1.6.0rc0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 442085 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1318400 b- defN 23-Nov-28 14:45 etiq/spark.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1317 b- defN 23-Nov-28 14:45 etiq/spark.pyi
--rw-rw-rw-  2.0 fat     2078 b- defN 23-Nov-28 14:45 etiq_spark-1.5.1rc3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Nov-28 14:45 etiq_spark-1.5.1rc3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Nov-28 14:43 etiq_spark-1.5.1rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      481 b- defN 23-Nov-28 14:45 etiq_spark-1.5.1rc3.dist-info/RECORD
-6 files, 1322375 bytes uncompressed, 441217 bytes compressed:  66.6%
+Zip file size: 440900 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat  1313280 b- defN 24-Apr-25 14:37 etiq/spark.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1317 b- defN 24-Apr-25 14:37 etiq/spark.pyi
+-rw-rw-rw-  2.0 fat     2078 b- defN 24-Apr-25 14:37 etiq_spark-1.6.0rc0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 24-Apr-25 14:37 etiq_spark-1.6.0rc0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-25 14:36 etiq_spark-1.6.0rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      481 b- defN 24-Apr-25 14:37 etiq_spark-1.6.0rc0.dist-info/RECORD
+6 files, 1317255 bytes uncompressed, 440032 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: etiq/spark.cp39-win_amd64.pyd
 Comment: 
 
 Filename: etiq/spark.pyi
 Comment: 
 
-Filename: etiq_spark-1.5.1rc3.dist-info/METADATA
+Filename: etiq_spark-1.6.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: etiq_spark-1.5.1rc3.dist-info/WHEEL
+Filename: etiq_spark-1.6.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: etiq_spark-1.5.1rc3.dist-info/top_level.txt
+Filename: etiq_spark-1.6.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: etiq_spark-1.5.1rc3.dist-info/RECORD
+Filename: etiq_spark-1.6.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `etiq_spark-1.5.1rc3.dist-info/METADATA` & `etiq_spark-1.6.0rc0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etiq-spark
-Version: 1.5.1rc3
+Version: 1.6.0rc0
 Summary: This is an optional, extension to the etiq library to provide spark datasets
 Author-email: ETIQ AI <devops@etiq.ai>
 Project-URL: homepage, https://etiq.ai
 Keywords: ai,bias,etiq,fairness
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: etiq ==1.5.1rc3
+Requires-Dist: etiq ==1.6.0rc0
 Requires-Dist: pyspark[pandas_on_spark] >=3.3.2
 
 # ETIQ AI
 
 Etiq helps companies test and monitor ML models. For data science & ML teams,
 Etiq tests ML algorithms, identifying issues and preventing accuracy loss in
 both building & production stages. Etiq helps identify the following issue
```


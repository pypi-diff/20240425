# Comparing `tmp/amazon_kclpy-2.1.3.tar.gz` & `tmp/amazon_kclpy-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_kclpy-2.1.3.tar", last modified: Tue Aug  8 21:09:00 2023, max compression
+gzip compressed data, was "amazon_kclpy-2.1.4.tar", last modified: Wed Apr 24 23:20:02 2024, max compression
```

## Comparing `amazon_kclpy-2.1.3.tar` & `amazon_kclpy-2.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)    10142 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/LICENSE.txt
--rw-r--r--   0 brenplyn (23167224) amazon     (100)       72 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/MANIFEST.in
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      114 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/NOTICE.txt
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      351 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/PKG-INFO
--rw-r--r--   0 brenplyn (23167224) amazon     (100)    17612 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/README.md
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.746161 amazon_kclpy-2.1.3/amazon_kclpy/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      827 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/__init__.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      781 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/checkpoint_error.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     1839 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/dispatch.py
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy/jars/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/jars/__init__.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)    12498 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/kcl.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)    13819 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/messages.py
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy/v2/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      820 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v2/__init__.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     5308 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v2/processor.py
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy/v3/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      820 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v3/__init__.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     5583 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/amazon_kclpy/v3/processor.py
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      351 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/PKG-INFO
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      776 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/SOURCES.txt
--rw-r--r--   0 brenplyn (23167224) amazon     (100)        1 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/dependency_links.txt
--rw-r--r--   0 brenplyn (23167224) amazon     (100)        1 2023-08-08 20:54:13.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/not-zip-safe
--rw-r--r--   0 brenplyn (23167224) amazon     (100)       14 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/requires.txt
--rw-r--r--   0 brenplyn (23167224) amazon     (100)       53 2023-08-08 21:09:00.000000 amazon_kclpy-2.1.3/amazon_kclpy.egg-info/top_level.txt
--rw-r--r--   0 brenplyn (23167224) amazon     (100)    14135 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/pom.xml
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/samples/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     2741 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/__init__.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     7176 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/amazon_kclpy_helper.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     4755 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/sample.properties
--rwxr-xr-x   0 brenplyn (23167224) amazon     (100)     6915 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/sample_kclpy_app.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     5706 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/samples/sample_kinesis_wordputter.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)      104 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/setup.cfg
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     8728 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/setup.py
-drwxr-xr-x   0 brenplyn (23167224) amazon     (100)        0 2023-08-08 21:09:00.750161 amazon_kclpy-2.1.3/test/
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     3791 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/test/test_amazon_kclpy.py
--rw-r--r--   0 brenplyn (23167224) amazon     (100)     3925 2023-08-08 20:47:08.000000 amazon_kclpy-2.1.3/test/test_amazon_kclpy_input_output_integration.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    10142 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/LICENSE.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)       72 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/MANIFEST.in
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      114 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/NOTICE.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      351 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/PKG-INFO
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    18562 2024-04-23 23:03:52.000000 amazon_kclpy-2.1.4/README.md
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      827 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      781 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/checkpoint_error.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     1839 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/dispatch.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/jars/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)        0 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/jars/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    12498 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/kcl.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    13819 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/messages.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/v2/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      820 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v2/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     5308 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v2/processor.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy/v3/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      820 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v3/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     5583 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/amazon_kclpy/v3/processor.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      351 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/PKG-INFO
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      776 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)        1 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)        1 2024-04-23 21:56:05.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/not-zip-safe
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)       14 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/requires.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)       53 2024-04-24 23:20:02.000000 amazon_kclpy-2.1.4/amazon_kclpy.egg-info/top_level.txt
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)    14133 2024-04-23 23:03:52.000000 amazon_kclpy-2.1.4/pom.xml
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/samples/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     2741 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/__init__.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     7176 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/amazon_kclpy_helper.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     4755 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/sample.properties
+-rwxr-xr-x   0 vvilo    (25800068) amazon     (100)     6915 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/sample_kclpy_app.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     5706 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/samples/sample_kinesis_wordputter.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)      104 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/setup.cfg
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     8728 2024-04-23 23:03:52.000000 amazon_kclpy-2.1.4/setup.py
+drwxr-xr-x   0 vvilo    (25800068) amazon     (100)        0 2024-04-24 23:20:02.241019 amazon_kclpy-2.1.4/test/
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     3791 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/test/test_amazon_kclpy.py
+-rw-r--r--   0 vvilo    (25800068) amazon     (100)     3926 2024-04-04 20:08:10.000000 amazon_kclpy-2.1.4/test/test_amazon_kclpy_input_output_integration.py
```

### Comparing `amazon_kclpy-2.1.3/LICENSE.txt` & `amazon_kclpy-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/README.md` & `amazon_kclpy-2.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -142,14 +142,23 @@
 * The [Amazon KCL for Java][kinesis-github]
 * The [Amazon KCL for Ruby][amazon-kinesis-ruby-github]
 * The [Amazon Kinesis Documentation][amazon-kinesis-docs]
 * The [Amazon Kinesis Forum][kinesis-forum]
 
 ## Release Notes
 
+### Release 2.1.4 (April 23, 2024)
+* Upgraded KCL and KCL-Multilang dependencies from 2.5.2 to 2.5.8 [PR #239](https://github.com/awslabs/amazon-kinesis-client-python/pull/239)
+* Upgraded ion-java from 1.5.1 to 1.11.4 [PR #243](https://github.com/awslabs/amazon-kinesis-client-python/pull/243)
+* Upgraded logback version from 1.3.0 to 1.3.12 [PR #242](https://github.com/awslabs/amazon-kinesis-client-python/pull/242)
+* Upgraded io.netty dependency from 4.1.86.Final to 4.1.94.Final [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
+* Upgraded Google Guava dependency from 32.0.0-jre to 32.1.1-jre [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
+* Upgraded jackson-databind from 2.13.4 to 2.13.5 [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
+* Upgraded protobuf-java from 3.21.5 to 3.21.7 [PR #234](https://github.com/awslabs/amazon-kinesis-client-python/pull/234)
+
 ### Release 2.1.3 (August 8, 2023)
 * Added the ability to specify STS endpoint and region [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/230)
 * Upgraded KCL and KCL-Multilang Dependencies from 2.5.1 to 2.5.2 [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/230)
 
 ### Release 2.1.2 (June 29, 2023)
 * Added the ability to pass in streamArn to multilang Daemon [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/221)
 * Upgraded KCL and KCL-Multilang Dependencies from 2.4.4 to 2.5.1 [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/221)
```

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/__init__.py` & `amazon_kclpy-2.1.4/amazon_kclpy/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/checkpoint_error.py` & `amazon_kclpy-2.1.4/amazon_kclpy/checkpoint_error.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/dispatch.py` & `amazon_kclpy-2.1.4/amazon_kclpy/dispatch.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/kcl.py` & `amazon_kclpy-2.1.4/amazon_kclpy/kcl.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/messages.py` & `amazon_kclpy-2.1.4/amazon_kclpy/messages.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/v2/__init__.py` & `amazon_kclpy-2.1.4/amazon_kclpy/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/v2/processor.py` & `amazon_kclpy-2.1.4/amazon_kclpy/v2/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/v3/__init__.py` & `amazon_kclpy-2.1.4/amazon_kclpy/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy/v3/processor.py` & `amazon_kclpy-2.1.4/amazon_kclpy/v3/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/amazon_kclpy.egg-info/SOURCES.txt` & `amazon_kclpy-2.1.4/amazon_kclpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/pom.xml` & `amazon_kclpy-2.1.4/pom.xml`

 * *Files 1% similar despite different names*

#### Comparing `amazon_kclpy-2.1.3/pom.xml` & `amazon_kclpy-2.1.4/pom.xml`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <properties>
     <awssdk.version>2.19.2</awssdk.version>
     <aws-java-sdk.version>1.12.370</aws-java-sdk.version>
-    <kcl.version>2.5.2</kcl.version>
-    <netty.version>4.1.86.Final</netty.version>
+    <kcl.version>2.5.8</kcl.version>
+    <netty.version>4.1.108.Final</netty.version>
     <netty-reactive.version>2.0.6</netty-reactive.version>
-    <fasterxml-jackson.version>2.13.4</fasterxml-jackson.version>
-    <logback.version>1.3.0</logback.version>
+    <fasterxml-jackson.version>2.13.5</fasterxml-jackson.version>
+    <logback.version>1.3.12</logback.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>software.amazon.kinesis</groupId>
       <artifactId>amazon-kinesis-client-multilang</artifactId>
       <version>${kcl.version}</version>
     </dependency>
@@ -205,15 +205,15 @@
       <groupId>org.reactivestreams</groupId>
       <artifactId>reactive-streams</artifactId>
       <version>1.0.3</version>
     </dependency>
     <dependency>
       <groupId>com.google.guava</groupId>
       <artifactId>guava</artifactId>
-      <version>32.0.0-jre</version>
+      <version>32.1.1-jre</version>
     </dependency>
     <dependency>
       <groupId>com.google.code.findbugs</groupId>
       <artifactId>jsr305</artifactId>
       <version>3.0.2</version>
     </dependency>
     <dependency>
@@ -235,15 +235,15 @@
       <groupId>org.codehaus.mojo</groupId>
       <artifactId>animal-sniffer-annotations</artifactId>
       <version>1.20</version>
     </dependency>
     <dependency>
       <groupId>com.google.protobuf</groupId>
       <artifactId>protobuf-java</artifactId>
-      <version>3.21.5</version>
+      <version>3.21.7</version>
     </dependency>
     <dependency>
       <groupId>org.apache.commons</groupId>
       <artifactId>commons-lang3</artifactId>
       <version>3.12.0</version>
     </dependency>
     <dependency>
@@ -303,17 +303,17 @@
     </dependency>
     <dependency>
       <groupId>com.amazonaws</groupId>
       <artifactId>aws-java-sdk-sts</artifactId>
       <version>${aws-java-sdk.version}</version>
     </dependency>
     <dependency>
-      <groupId>software.amazon.ion</groupId>
+      <groupId>com.amazon.ion</groupId>
       <artifactId>ion-java</artifactId>
-      <version>1.5.1</version>
+      <version>1.11.4</version>
     </dependency>
     <dependency>
       <groupId>software.amazon.glue</groupId>
       <artifactId>schema-registry-serde</artifactId>
       <version>1.1.13</version>
     </dependency>
     <dependency>
```

### Comparing `amazon_kclpy-2.1.3/samples/__init__.py` & `amazon_kclpy-2.1.4/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/samples/amazon_kclpy_helper.py` & `amazon_kclpy-2.1.4/samples/amazon_kclpy_helper.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/samples/sample.properties` & `amazon_kclpy-2.1.4/samples/sample.properties`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/samples/sample_kclpy_app.py` & `amazon_kclpy-2.1.4/samples/sample_kclpy_app.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/samples/sample_kinesis_wordputter.py` & `amazon_kclpy-2.1.4/samples/sample_kinesis_wordputter.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/setup.py` & `amazon_kclpy-2.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #
 # Will retrieve the configured jars from maven and then advise the user
 # to rerun the install command.
 #
 
 PACKAGE_NAME = 'amazon_kclpy'
 JAR_DIRECTORY = os.path.join(PACKAGE_NAME, 'jars')
-PACKAGE_VERSION = '2.1.3'
+PACKAGE_VERSION = '2.1.4'
 PYTHON_REQUIREMENTS = [
     'boto',
     # argparse is part of python2.7 but must be declared for python2.6
     'argparse',
 ]
 REMOTE_MAVEN_PACKAGES_FILE = 'pom.xml'
```

### Comparing `amazon_kclpy-2.1.3/test/test_amazon_kclpy.py` & `amazon_kclpy-2.1.4/test/test_amazon_kclpy.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.3/test/test_amazon_kclpy_input_output_integration.py` & `amazon_kclpy-2.1.4/test/test_amazon_kclpy_input_output_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     {"action": "status", "responseFor": "processRecords"},
     {"action": "checkpoint", "sequenceNumber": None, "subSequenceNumber": None},
     {"action": "status", "responseFor": "shardEnded"}
 ]
 
 
 def _strip_all_whitespace(s):
-    return re.sub('\s*', '', s)
+    return re.sub('\\s*', '', s)
 
 
 test_shard_id = "shardId-123"
 test_sequence_number = "456"
 
 test_input_messages = [
     {"action": "initialize", "shardId": test_shard_id, "sequenceNumber": test_sequence_number, "subSequenceNumber": 0},
```


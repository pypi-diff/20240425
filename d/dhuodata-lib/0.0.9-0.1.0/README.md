# Comparing `tmp/dhuodata-lib-0.0.9.zip` & `tmp/dhuodata-lib-0.1.0.zip`

## zipinfo {}

```diff
@@ -1,28 +1,27 @@
-Zip file size: 12077 bytes, number of entries: 26
-drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:13 dhuodata-lib-0.0.9/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:13 dhuodata-lib-0.0.9/tests/
--rw-rw-r--  2.0 unx     2528 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/PKG-INFO
--rw-rw-r--  2.0 unx      863 b- defN 24-Apr-24 19:12 dhuodata-lib-0.0.9/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/setup.cfg
--rw-rw-r--  2.0 unx     2346 b- defN 24-Apr-16 15:35 dhuodata-lib-0.0.9/README.md
-drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuolib/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuolib/oci_tools/
--rw-rw-r--  2.0 unx      711 b- defN 24-Apr-24 15:14 dhuodata-lib-0.0.9/src/dhuolib/validations.py
--rw-rw-r--  2.0 unx      261 b- defN 24-Apr-23 13:50 dhuodata-lib-0.0.9/src/dhuolib/auth.py
--rw-rw-r--  2.0 unx     1087 b- defN 24-Apr-23 13:51 dhuodata-lib-0.0.9/src/dhuolib/services.py
--rw-rw-r--  2.0 unx      358 b- defN 24-Apr-23 13:51 dhuodata-lib-0.0.9/src/dhuolib/config.py
--rw-rw-r--  2.0 unx      758 b- defN 24-Apr-24 15:22 dhuodata-lib-0.0.9/src/dhuolib/predict.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 15:35 dhuodata-lib-0.0.9/src/dhuolib/__init__.py
--rw-rw-r--  2.0 unx      141 b- defN 24-Apr-23 13:51 dhuodata-lib-0.0.9/src/dhuolib/worker.py
--rw-rw-r--  2.0 unx     3863 b- defN 24-Apr-24 16:16 dhuodata-lib-0.0.9/src/dhuolib/clients.py
--rw-rw-r--  2.0 unx      716 b- defN 24-Apr-24 15:22 dhuodata-lib-0.0.9/src/dhuolib/oci_tools/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 15:52 dhuodata-lib-0.0.9/src/dhuolib/oci_tools/__init__.py
--rw-rw-r--  2.0 unx        1 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     2528 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      489 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      128 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-24 19:13 dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     3466 b- defN 24-Apr-24 17:10 dhuodata-lib-0.0.9/tests/test_dhuolib.py
-26 files, 20290 bytes uncompressed, 7973 bytes compressed:  60.7%
+Zip file size: 10907 bytes, number of entries: 25
+drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:30 dhuodata-lib-0.1.0/
+drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:30 dhuodata-lib-0.1.0/dhuodata_lib.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:30 dhuodata-lib-0.1.0/src/
+-rw-rw-r--  2.0 unx     2528 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/PKG-INFO
+-rw-rw-r--  2.0 unx      847 b- defN 24-Apr-24 19:29 dhuodata-lib-0.1.0/setup.py
+-rw-rw-r--  2.0 unx       38 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/setup.cfg
+-rw-rw-r--  2.0 unx     2346 b- defN 24-Apr-16 15:35 dhuodata-lib-0.1.0/README.md
+-rw-rw-r--  2.0 unx        1 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     2528 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      463 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      128 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        4 b- defN 24-Apr-24 19:30 dhuodata-lib-0.1.0/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:30 dhuodata-lib-0.1.0/src/dhuolib/
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-24 15:48 dhuodata-lib-0.1.0/src/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 24-Apr-24 19:30 dhuodata-lib-0.1.0/src/dhuolib/oci_tools/
+-rw-rw-r--  2.0 unx      711 b- defN 24-Apr-24 15:14 dhuodata-lib-0.1.0/src/dhuolib/validations.py
+-rw-rw-r--  2.0 unx      261 b- defN 24-Apr-23 13:50 dhuodata-lib-0.1.0/src/dhuolib/auth.py
+-rw-rw-r--  2.0 unx     1087 b- defN 24-Apr-23 13:51 dhuodata-lib-0.1.0/src/dhuolib/services.py
+-rw-rw-r--  2.0 unx      358 b- defN 24-Apr-23 13:51 dhuodata-lib-0.1.0/src/dhuolib/config.py
+-rw-rw-r--  2.0 unx      758 b- defN 24-Apr-24 15:22 dhuodata-lib-0.1.0/src/dhuolib/predict.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 15:35 dhuodata-lib-0.1.0/src/dhuolib/__init__.py
+-rw-rw-r--  2.0 unx      141 b- defN 24-Apr-23 13:51 dhuodata-lib-0.1.0/src/dhuolib/worker.py
+-rw-rw-r--  2.0 unx     3863 b- defN 24-Apr-24 16:16 dhuodata-lib-0.1.0/src/dhuolib/clients.py
+-rw-rw-r--  2.0 unx      716 b- defN 24-Apr-24 15:22 dhuodata-lib-0.1.0/src/dhuolib/oci_tools/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 15:52 dhuodata-lib-0.1.0/src/dhuolib/oci_tools/__init__.py
+25 files, 16778 bytes uncompressed, 6989 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -1,79 +1,76 @@
-Filename: dhuodata-lib-0.0.9/
+Filename: dhuodata-lib-0.1.0/
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/
+Filename: dhuodata-lib-0.1.0/dhuodata_lib.egg-info/
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/tests/
+Filename: dhuodata-lib-0.1.0/src/
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/PKG-INFO
+Filename: dhuodata-lib-0.1.0/PKG-INFO
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/setup.py
+Filename: dhuodata-lib-0.1.0/setup.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/setup.cfg
+Filename: dhuodata-lib-0.1.0/setup.cfg
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/README.md
+Filename: dhuodata-lib-0.1.0/README.md
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/
+Filename: dhuodata-lib-0.1.0/dhuodata_lib.egg-info/dependency_links.txt
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/
+Filename: dhuodata-lib-0.1.0/dhuodata_lib.egg-info/PKG-INFO
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/oci_tools/
+Filename: dhuodata-lib-0.1.0/dhuodata_lib.egg-info/SOURCES.txt
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/validations.py
+Filename: dhuodata-lib-0.1.0/dhuodata_lib.egg-info/requires.txt
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/auth.py
+Filename: dhuodata-lib-0.1.0/dhuodata_lib.egg-info/top_level.txt
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/services.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/config.py
+Filename: dhuodata-lib-0.1.0/src/__init__.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/predict.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/oci_tools/
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/__init__.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/validations.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/worker.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/auth.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/clients.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/services.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/oci_tools/utils.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/config.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuolib/oci_tools/__init__.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/predict.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/dependency_links.txt
+Filename: dhuodata-lib-0.1.0/src/dhuolib/__init__.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/PKG-INFO
+Filename: dhuodata-lib-0.1.0/src/dhuolib/worker.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/SOURCES.txt
+Filename: dhuodata-lib-0.1.0/src/dhuolib/clients.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/requires.txt
+Filename: dhuodata-lib-0.1.0/src/dhuolib/oci_tools/utils.py
 Comment: 
 
-Filename: dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/top_level.txt
-Comment: 
-
-Filename: dhuodata-lib-0.0.9/tests/test_dhuolib.py
+Filename: dhuodata-lib-0.1.0/src/dhuolib/oci_tools/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `dhuodata-lib-0.0.9/PKG-INFO` & `dhuodata-lib-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.9
+Version: 0.1.0
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```

## Comparing `dhuodata-lib-0.0.9/setup.py` & `dhuodata-lib-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.0.9",
+    version="0.1.0",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    packages=find_packages(include=["src", "src.*"]),
     platforms="any",
 )
```

## Comparing `dhuodata-lib-0.0.9/README.md` & `dhuodata-lib-0.1.0/README.md`

 * *Files identical despite different names*

## Comparing `dhuodata-lib-0.0.9/src/dhuolib/validations.py` & `dhuodata-lib-0.1.0/src/dhuolib/validations.py`

 * *Files identical despite different names*

## Comparing `dhuodata-lib-0.0.9/src/dhuolib/services.py` & `dhuodata-lib-0.1.0/src/dhuolib/services.py`

 * *Files identical despite different names*

## Comparing `dhuodata-lib-0.0.9/src/dhuolib/predict.py` & `dhuodata-lib-0.1.0/src/dhuolib/predict.py`

 * *Files identical despite different names*

## Comparing `dhuodata-lib-0.0.9/src/dhuolib/clients.py` & `dhuodata-lib-0.1.0/src/dhuolib/clients.py`

 * *Files identical despite different names*

## Comparing `dhuodata-lib-0.0.9/src/dhuolib/oci_tools/utils.py` & `dhuodata-lib-0.1.0/src/dhuolib/oci_tools/utils.py`

 * *Files identical despite different names*

## Comparing `dhuodata-lib-0.0.9/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata-lib-0.1.0/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.0.9
+Version: 0.1.0
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
```


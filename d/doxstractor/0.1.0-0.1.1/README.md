# Comparing `tmp/doxstractor-0.1.0.tar.gz` & `tmp/doxstractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxstractor-0.1.0.tar", last modified: Wed Apr 17 14:51:09 2024, max compression
+gzip compressed data, was "doxstractor-0.1.1.tar", last modified: Thu Apr 25 13:13:52 2024, max compression
```

## Comparing `doxstractor-0.1.0.tar` & `doxstractor-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-17 14:51:09.614617 doxstractor-0.1.0/
--rw-r--r--   0 jannesklaas   (501) staff       (20)    11356 2024-04-13 17:47:21.000000 doxstractor-0.1.0/LICENSE.md
--rw-r--r--   0 jannesklaas   (501) staff       (20)     7244 2024-04-17 14:51:09.614435 doxstractor-0.1.0/PKG-INFO
--rw-r--r--   0 jannesklaas   (501) staff       (20)     6645 2024-04-17 14:16:37.000000 doxstractor-0.1.0/README.md
-drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-17 14:51:09.609837 doxstractor-0.1.0/doxstractor/
--rw-r--r--   0 jannesklaas   (501) staff       (20)      295 2024-04-17 13:46:09.000000 doxstractor-0.1.0/doxstractor/__init__.py
-drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-17 14:51:09.612103 doxstractor-0.1.0/doxstractor/extractors/
--rw-r--r--   0 jannesklaas   (501) staff       (20)      142 2024-04-16 10:20:48.000000 doxstractor-0.1.0/doxstractor/extractors/__init__.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     1587 2024-04-17 14:30:18.000000 doxstractor-0.1.0/doxstractor/extractors/base.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     3300 2024-04-17 14:30:57.000000 doxstractor-0.1.0/doxstractor/extractors/category.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     2225 2024-04-17 14:25:12.000000 doxstractor-0.1.0/doxstractor/extractors/numeric.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     1886 2024-04-17 14:24:19.000000 doxstractor-0.1.0/doxstractor/extractors/text.py
-drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-17 14:51:09.613602 doxstractor-0.1.0/doxstractor/models/
--rw-r--r--   0 jannesklaas   (501) staff       (20)      229 2024-04-17 13:46:00.000000 doxstractor-0.1.0/doxstractor/models/__init__.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     4258 2024-04-17 14:35:54.000000 doxstractor-0.1.0/doxstractor/models/anthropic.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     1071 2024-04-17 13:50:19.000000 doxstractor-0.1.0/doxstractor/models/base.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     1561 2024-04-17 13:49:22.000000 doxstractor-0.1.0/doxstractor/models/mock.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     1185 2024-04-17 14:40:28.000000 doxstractor-0.1.0/doxstractor/models/transformers_classify.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     2694 2024-04-17 14:39:38.000000 doxstractor-0.1.0/doxstractor/models/transformers_qa.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     3566 2024-04-17 14:45:34.000000 doxstractor-0.1.0/doxstractor/nodes.py
--rw-r--r--   0 jannesklaas   (501) staff       (20)     3960 2024-04-12 13:51:50.000000 doxstractor-0.1.0/doxstractor/utils.py
-drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-17 14:51:09.614222 doxstractor-0.1.0/doxstractor.egg-info/
--rw-r--r--   0 jannesklaas   (501) staff       (20)     7244 2024-04-17 14:51:09.000000 doxstractor-0.1.0/doxstractor.egg-info/PKG-INFO
--rw-r--r--   0 jannesklaas   (501) staff       (20)      660 2024-04-17 14:51:09.000000 doxstractor-0.1.0/doxstractor.egg-info/SOURCES.txt
--rw-r--r--   0 jannesklaas   (501) staff       (20)        1 2024-04-17 14:51:09.000000 doxstractor-0.1.0/doxstractor.egg-info/dependency_links.txt
--rw-r--r--   0 jannesklaas   (501) staff       (20)       39 2024-04-17 14:51:09.000000 doxstractor-0.1.0/doxstractor.egg-info/requires.txt
--rw-r--r--   0 jannesklaas   (501) staff       (20)       12 2024-04-17 14:51:09.000000 doxstractor-0.1.0/doxstractor.egg-info/top_level.txt
--rw-r--r--   0 jannesklaas   (501) staff       (20)      866 2024-04-17 14:45:58.000000 doxstractor-0.1.0/pyproject.toml
--rw-r--r--   0 jannesklaas   (501) staff       (20)       38 2024-04-17 14:51:09.614658 doxstractor-0.1.0/setup.cfg
-drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-17 14:51:09.613922 doxstractor-0.1.0/tests/
--rw-r--r--   0 jannesklaas   (501) staff       (20)     1830 2024-04-17 13:48:50.000000 doxstractor-0.1.0/tests/test_nodes.py
+drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-25 13:13:52.091550 doxstractor-0.1.1/
+-rw-r--r--   0 jannesklaas   (501) staff       (20)    11356 2024-04-13 17:47:21.000000 doxstractor-0.1.1/LICENSE.md
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     7244 2024-04-25 13:13:52.091359 doxstractor-0.1.1/PKG-INFO
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     6645 2024-04-17 14:16:37.000000 doxstractor-0.1.1/README.md
+drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-25 13:13:52.083907 doxstractor-0.1.1/doxstractor/
+-rw-r--r--   0 jannesklaas   (501) staff       (20)      318 2024-04-25 13:02:22.000000 doxstractor-0.1.1/doxstractor/__init__.py
+drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-25 13:13:52.087003 doxstractor-0.1.1/doxstractor/extractors/
+-rw-r--r--   0 jannesklaas   (501) staff       (20)      142 2024-04-16 10:20:48.000000 doxstractor-0.1.1/doxstractor/extractors/__init__.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     1587 2024-04-17 14:30:18.000000 doxstractor-0.1.1/doxstractor/extractors/base.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     3300 2024-04-17 14:30:57.000000 doxstractor-0.1.1/doxstractor/extractors/category.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     2225 2024-04-17 14:25:12.000000 doxstractor-0.1.1/doxstractor/extractors/numeric.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     1886 2024-04-17 14:24:19.000000 doxstractor-0.1.1/doxstractor/extractors/text.py
+drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-25 13:13:52.090440 doxstractor-0.1.1/doxstractor/models/
+-rw-r--r--   0 jannesklaas   (501) staff       (20)      282 2024-04-25 13:02:02.000000 doxstractor-0.1.1/doxstractor/models/__init__.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     4258 2024-04-17 14:35:54.000000 doxstractor-0.1.1/doxstractor/models/anthropic.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     1071 2024-04-17 13:50:19.000000 doxstractor-0.1.1/doxstractor/models/base.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     2321 2024-04-25 13:06:55.000000 doxstractor-0.1.1/doxstractor/models/huggingface_endpoints.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     1561 2024-04-17 13:49:22.000000 doxstractor-0.1.1/doxstractor/models/mock.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     1185 2024-04-17 14:40:28.000000 doxstractor-0.1.1/doxstractor/models/transformers_classify.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     2694 2024-04-17 14:39:38.000000 doxstractor-0.1.1/doxstractor/models/transformers_qa.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     3566 2024-04-17 14:45:34.000000 doxstractor-0.1.1/doxstractor/nodes.py
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     3960 2024-04-12 13:51:50.000000 doxstractor-0.1.1/doxstractor/utils.py
+drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-25 13:13:52.091141 doxstractor-0.1.1/doxstractor.egg-info/
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     7244 2024-04-25 13:13:52.000000 doxstractor-0.1.1/doxstractor.egg-info/PKG-INFO
+-rw-r--r--   0 jannesklaas   (501) staff       (20)      704 2024-04-25 13:13:52.000000 doxstractor-0.1.1/doxstractor.egg-info/SOURCES.txt
+-rw-r--r--   0 jannesklaas   (501) staff       (20)        1 2024-04-25 13:13:52.000000 doxstractor-0.1.1/doxstractor.egg-info/dependency_links.txt
+-rw-r--r--   0 jannesklaas   (501) staff       (20)       39 2024-04-25 13:13:52.000000 doxstractor-0.1.1/doxstractor.egg-info/requires.txt
+-rw-r--r--   0 jannesklaas   (501) staff       (20)       12 2024-04-25 13:13:52.000000 doxstractor-0.1.1/doxstractor.egg-info/top_level.txt
+-rw-r--r--   0 jannesklaas   (501) staff       (20)      866 2024-04-25 13:07:06.000000 doxstractor-0.1.1/pyproject.toml
+-rw-r--r--   0 jannesklaas   (501) staff       (20)       38 2024-04-25 13:13:52.091590 doxstractor-0.1.1/setup.cfg
+drwxr-xr-x   0 jannesklaas   (501) staff       (20)        0 2024-04-25 13:13:52.090812 doxstractor-0.1.1/tests/
+-rw-r--r--   0 jannesklaas   (501) staff       (20)     1830 2024-04-17 13:48:50.000000 doxstractor-0.1.1/tests/test_nodes.py
```

### Comparing `doxstractor-0.1.0/LICENSE.md` & `doxstractor-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/PKG-INFO` & `doxstractor-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doxstractor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Doxstractor extracts strutured data from text in an easily configurable way.
 Author: Jannes Klaas
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/JannesKlaas/doxstractor
 Project-URL: Issues, https://github.com/JannesKlaas/doxstractor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `doxstractor-0.1.0/README.md` & `doxstractor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/extractors/base.py` & `doxstractor-0.1.1/doxstractor/extractors/base.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/extractors/category.py` & `doxstractor-0.1.1/doxstractor/extractors/category.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/extractors/numeric.py` & `doxstractor-0.1.1/doxstractor/extractors/numeric.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/extractors/text.py` & `doxstractor-0.1.1/doxstractor/extractors/text.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/models/anthropic.py` & `doxstractor-0.1.1/doxstractor/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/models/base.py` & `doxstractor-0.1.1/doxstractor/models/base.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/models/mock.py` & `doxstractor-0.1.1/doxstractor/models/mock.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/models/transformers_classify.py` & `doxstractor-0.1.1/doxstractor/models/transformers_classify.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/models/transformers_qa.py` & `doxstractor-0.1.1/doxstractor/models/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/nodes.py` & `doxstractor-0.1.1/doxstractor/nodes.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor/utils.py` & `doxstractor-0.1.1/doxstractor/utils.py`

 * *Files identical despite different names*

### Comparing `doxstractor-0.1.0/doxstractor.egg-info/PKG-INFO` & `doxstractor-0.1.1/doxstractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doxstractor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Doxstractor extracts strutured data from text in an easily configurable way.
 Author: Jannes Klaas
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/JannesKlaas/doxstractor
 Project-URL: Issues, https://github.com/JannesKlaas/doxstractor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `doxstractor-0.1.0/doxstractor.egg-info/SOURCES.txt` & `doxstractor-0.1.1/doxstractor.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 doxstractor/extractors/base.py
 doxstractor/extractors/category.py
 doxstractor/extractors/numeric.py
 doxstractor/extractors/text.py
 doxstractor/models/__init__.py
 doxstractor/models/anthropic.py
 doxstractor/models/base.py
+doxstractor/models/huggingface_endpoints.py
 doxstractor/models/mock.py
 doxstractor/models/transformers_classify.py
 doxstractor/models/transformers_qa.py
 tests/test_nodes.py
```

### Comparing `doxstractor-0.1.0/pyproject.toml` & `doxstractor-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools>=65.5.1"]       # PEP 518 specifications
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "doxstractor"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Jannes Klaas" }]
 
 description = "Doxstractor extracts strutured data from text in an easily configurable way."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["anthropic==0.25.1", "transformers==4.39.3"]
 license = { text = "Apache Software License (Apache 2.0)" }
```

### Comparing `doxstractor-0.1.0/tests/test_nodes.py` & `doxstractor-0.1.1/tests/test_nodes.py`

 * *Files identical despite different names*


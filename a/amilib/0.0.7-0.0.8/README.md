# Comparing `tmp/amilib-0.0.7.tar.gz` & `tmp/amilib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amilib-0.0.7.tar", last modified: Tue Apr 23 07:59:02 2024, max compression
+gzip compressed data, was "dist/amilib-0.0.8.tar", last modified: Thu Apr 25 01:40:44 2024, max compression
```

## Comparing `amilib-0.0.7.tar` & `amilib-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.018311 amilib-0.0.7/
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.0.7/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-23 07:59:02.018166 amilib-0.0.7/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)       76 2024-04-16 00:05:01.000000 amilib-0.0.7/README.md
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.012909 amilib-0.0.7/amilib/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.0.7/amilib/ami_csv.py
--rw-r--r--   0 pm286      (503) staff       (20)   168064 2024-04-18 06:54:59.000000 amilib-0.0.7/amilib/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    16455 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     8504 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    81920 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_pdf_libs.py
--rw-r--r--   0 pm286      (503) staff       (20)     4976 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/amidriver.py
--rw-r--r--   0 pm286      (503) staff       (20)    49270 2024-04-23 07:57:44.000000 amilib-0.0.7/amilib/amix.py
--rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/bbox.py
--rw-r--r--   0 pm286      (503) staff       (20)    14085 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-04-23 05:05:15.000000 amilib-0.0.7/amilib/headless_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.000000 amilib-0.0.7/amilib/html_extra.py
--rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/html_generator.py
--rw-r--r--   0 pm286      (503) staff       (20)    48143 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/html_marker.py
--rw-r--r--   0 pm286      (503) staff       (20)    27194 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/pdf_args.py
--rw-r--r--   0 pm286      (503) staff       (20)    36799 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    54474 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.013953 amilib-0.0.7/amilib.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      846 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)      125 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-23 07:59:02.018353 amilib-0.0.7/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     1651 2024-04-23 07:57:44.000000 amilib-0.0.7/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.017972 amilib-0.0.7/test/
--rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.0.7/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.0.7/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)    21400 2024-04-23 04:51:55.000000 amilib-0.0.7/test/test_headless.py
--rw-r--r--   0 pm286      (503) staff       (20)   120176 2024-04-23 06:41:05.000000 amilib-0.0.7/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    80007 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.000000 amilib-0.0.7/test/test_stat.py
--rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10541 2024-04-18 07:00:37.000000 amilib-0.0.7/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.000000 amilib-0.0.7/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-25 01:40:44.088764 amilib-0.0.8/
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.0.8/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-25 01:40:44.088629 amilib-0.0.8/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)       76 2024-04-16 00:05:01.000000 amilib-0.0.8/README.md
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-25 01:40:44.086003 amilib-0.0.8/amilib/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.0.8/amilib/ami_csv.py
+-rw-r--r--   0 pm286      (503) staff       (20)   168064 2024-04-18 06:54:59.000000 amilib-0.0.8/amilib/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16455 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8504 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    81920 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/ami_pdf_libs.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4976 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/amidriver.py
+-rw-r--r--   0 pm286      (503) staff       (20)    49310 2024-04-25 01:40:16.000000 amilib-0.0.8/amilib/amix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/bbox.py
+-rw-r--r--   0 pm286      (503) staff       (20)    14085 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-04-23 05:05:15.000000 amilib-0.0.8/amilib/headless_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.000000 amilib-0.0.8/amilib/html_extra.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/html_generator.py
+-rw-r--r--   0 pm286      (503) staff       (20)    48143 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/html_marker.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27194 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/pdf_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)    36799 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    54474 2024-04-16 00:05:01.000000 amilib-0.0.8/amilib/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-25 01:40:44.086799 amilib-0.0.8/amilib.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      846 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)      125 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-25 01:40:43.000000 amilib-0.0.8/amilib.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-25 01:40:44.088811 amilib-0.0.8/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     1651 2024-04-25 01:40:35.000000 amilib-0.0.8/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-25 01:40:44.088405 amilib-0.0.8/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.0.8/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.0.8/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)    21400 2024-04-23 04:51:55.000000 amilib-0.0.8/test/test_headless.py
+-rw-r--r--   0 pm286      (503) staff       (20)   120176 2024-04-23 06:41:05.000000 amilib-0.0.8/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.0.8/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    80007 2024-04-16 00:05:02.000000 amilib-0.0.8/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.000000 amilib-0.0.8/test/test_stat.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.0.8/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10541 2024-04-18 07:00:37.000000 amilib-0.0.8/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.0.8/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.000000 amilib-0.0.8/test/test_xml.py
```

### Comparing `amilib-0.0.7/LICENSE` & `amilib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/PKG-INFO` & `amilib-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.7
+Version: 0.0.8
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.7/amilib/ami_bib.py` & `amilib-0.0.8/amilib/ami_bib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/ami_html.py` & `amilib-0.0.8/amilib/ami_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/ami_integrate.py` & `amilib-0.0.8/amilib/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/ami_nlp.py` & `amilib-0.0.8/amilib/ami_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/ami_pdf_libs.py` & `amilib-0.0.8/amilib/ami_pdf_libs.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/ami_svg.py` & `amilib-0.0.8/amilib/ami_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/ami_util.py` & `amilib-0.0.8/amilib/ami_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/amidriver.py` & `amilib-0.0.8/amilib/amidriver.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/amix.py` & `amilib-0.0.8/amilib/amix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1152,14 +1152,15 @@
         version = '0.0.1a3'  # 2024-03-27
         version = '0.0.1'  # 2024-04-03
         version = '0.0.2'  # 2024-04-04
         version = '0.0.3'  # 2024-04-19
         # had to revert here I think
         version = '0.0.6'  # 2024-04-19
         version = '0.0.7'  # 2024-04-23
+        version = '0.0.8'  # 2024-04-23
 
         # logging.warn(f"VERSION {version}")
         return version
 
 
 class AmiLibArgs(AbstractArgs):
     """Parse args to analyze, edit and annotate HTML"""
```

### Comparing `amilib-0.0.7/amilib/bbox.py` & `amilib-0.0.8/amilib/bbox.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/file_lib.py` & `amilib-0.0.8/amilib/file_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/headless_lib.py` & `amilib-0.0.8/amilib/headless_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/html_extra.py` & `amilib-0.0.8/amilib/html_extra.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/html_generator.py` & `amilib-0.0.8/amilib/html_generator.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/html_marker.py` & `amilib-0.0.8/amilib/html_marker.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/pdf_args.py` & `amilib-0.0.8/amilib/pdf_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/util.py` & `amilib-0.0.8/amilib/util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/wikimedia.py` & `amilib-0.0.8/amilib/wikimedia.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib/xml_lib.py` & `amilib-0.0.8/amilib/xml_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/amilib.egg-info/PKG-INFO` & `amilib-0.0.8/amilib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.7
+Version: 0.0.8
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.7/amilib.egg-info/SOURCES.txt` & `amilib-0.0.8/amilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/setup.py` & `amilib-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'scikit-learn',
 
 ]
 
 setup(
     name='amilib',
     url='https://github.com/petermr/amilib',
-    version='0.0.7',
+    version='0.0.8',
     description='document download, cleaning, managemenr',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `amilib-0.0.7/test/test_all.py` & `amilib-0.0.8/test/test_all.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_file.py` & `amilib-0.0.8/test/test_file.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_headless.py` & `amilib-0.0.8/test/test_headless.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_html.py` & `amilib-0.0.8/test/test_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_nlp.py` & `amilib-0.0.8/test/test_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_pdf.py` & `amilib-0.0.8/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_stat.py` & `amilib-0.0.8/test/test_stat.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_svg.py` & `amilib-0.0.8/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_util.py` & `amilib-0.0.8/test/test_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_wikidata.py` & `amilib-0.0.8/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.7/test/test_xml.py` & `amilib-0.0.8/test/test_xml.py`

 * *Files identical despite different names*

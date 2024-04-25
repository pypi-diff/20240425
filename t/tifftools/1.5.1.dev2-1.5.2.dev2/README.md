# Comparing `tmp/tifftools-1.5.1.dev2.tar.gz` & `tmp/tifftools-1.5.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifftools-1.5.1.dev2.tar", last modified: Wed Apr 24 19:10:27 2024, max compression
+gzip compressed data, was "tifftools-1.5.2.dev2.tar", last modified: Thu Apr 25 17:37:02 2024, max compression
```

## Comparing `tifftools-1.5.1.dev2.tar` & `tifftools-1.5.2.dev2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.748515 tifftools-1.5.1.dev2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.740515 tifftools-1.5.1.dev2/.circleci/
--rw-r--r--   0 root         (0) root         (0)     4029 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      596 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1633 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     3764 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)      549 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8830 2024-04-24 19:10:27.748515 tifftools-1.5.1.dev2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7969 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/README.rst
--rw-r--r--   0 root         (0) root         (0)      424 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/codecov.yml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 19:10:27.748515 tifftools-1.5.1.dev2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tests/data/
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_datatype.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_double_reference.tif
--rw-r--r--   0 root         (0) root         (0)      653 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_header1.tif
--rw-r--r--   0 root         (0) root         (0)      815 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_header2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_ifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      360 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      616 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_jpeg2.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_strip_offset.tif
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_subifd_offset.tif
--rw-r--r--   0 root         (0) root         (0)      653 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_tag_offset.tif
--rw-r--r--   0 root         (0) root         (0)      641 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/bad_unicode.tif
--rw-r--r--   0 root         (0) root         (0)      616 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/good_jpeg.tif
--rw-r--r--   0 root         (0) root         (0)      453 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/data/good_single.tif
--rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_constants.py
--rw-r--r--   0 root         (0) root         (0)     4616 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_dump.py
--rw-r--r--   0 root         (0) root         (0)     2608 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)      848 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_options.py
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_path_or_fobj.py
--rw-r--r--   0 root         (0) root         (0)     1943 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_read_tiff.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_readme.py
--rw-r--r--   0 root         (0) root         (0)     5557 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_set.py
--rw-r--r--   0 root         (0) root         (0)     3992 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)     9822 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tests/test_write_tiff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tifftools/
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/__main__.py
--rw-r--r--   0 root         (0) root         (0)    31419 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/commands.py
--rw-r--r--   0 root         (0) root         (0)    67608 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/constants.py
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/path_or_fobj.py
--rwxr-xr-x   0 root         (0) root         (0)    33650 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tifftools/tifftools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:10:27.744515 tifftools-1.5.1.dev2/tifftools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8830 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:10:22.000000 tifftools-1.5.1.dev2/tifftools.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 19:10:27.000000 tifftools-1.5.1.dev2/tifftools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1595 2024-04-24 19:10:08.000000 tifftools-1.5.1.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:37:02.521138 tifftools-1.5.2.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:37:02.517138 tifftools-1.5.2.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     4029 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      596 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3857 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)      549 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8830 2024-04-25 17:37:02.521138 tifftools-1.5.2.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7969 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      424 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 17:37:02.521138 tifftools-1.5.2.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:37:02.517138 tifftools-1.5.2.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:37:02.521138 tifftools-1.5.2.dev2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_datatype.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_double_reference.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_header1.tif
+-rw-r--r--   0 root         (0) root         (0)      815 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_header2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_ifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      360 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_jpeg2.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_strip_offset.tif
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_subifd_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      653 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_tag_offset.tif
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/bad_unicode.tif
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/good_jpeg.tif
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/data/good_single.tif
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_constants.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_dump.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_options.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_path_or_fobj.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_read_tiff.py
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_set.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)    10802 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tests/test_write_tiff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:37:02.521138 tifftools-1.5.2.dev2/tifftools/
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    31419 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/commands.py
+-rw-r--r--   0 root         (0) root         (0)    67608 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/constants.py
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/path_or_fobj.py
+-rwxr-xr-x   0 root         (0) root         (0)    33265 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tifftools/tifftools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:37:02.521138 tifftools-1.5.2.dev2/tifftools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8830 2024-04-25 17:37:02.000000 tifftools-1.5.2.dev2/tifftools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-25 17:37:02.000000 tifftools-1.5.2.dev2/tifftools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:37:02.000000 tifftools-1.5.2.dev2/tifftools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-25 17:37:02.000000 tifftools-1.5.2.dev2/tifftools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:36:56.000000 tifftools-1.5.2.dev2/tifftools.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 17:37:02.000000 tifftools-1.5.2.dev2/tifftools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-04-25 17:36:41.000000 tifftools-1.5.2.dev2/tox.ini
```

### Comparing `tifftools-1.5.1.dev2/.circleci/config.yml` & `tifftools-1.5.2.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/.gitignore` & `tifftools-1.5.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/.pre-commit-config.yaml` & `tifftools-1.5.2.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/CHANGELOG.md` & `tifftools-1.5.2.dev2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change Log
 
+## Version 1.5.2
+
+### Improvements
+- Simplify the deduplication code ([#94](../../pull/94))
+
 ## Version 1.5.1
 
 ### Improvements
 - Speed up deduplication process ([#93](../../pull/93))
 
 ## Version 1.5.0
```

### Comparing `tifftools-1.5.1.dev2/LICENSE` & `tifftools-1.5.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/PKG-INFO` & `tifftools-1.5.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.5.1.dev2
+Version: 1.5.2.dev2
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.5.1.dev2/README.rst` & `tifftools-1.5.2.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/setup.py` & `tifftools-1.5.2.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_datatype.tif` & `tifftools-1.5.2.dev2/tests/data/bad_datatype.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_double_reference.tif` & `tifftools-1.5.2.dev2/tests/data/bad_double_reference.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_header1.tif` & `tifftools-1.5.2.dev2/tests/data/bad_header1.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_header2.tif` & `tifftools-1.5.2.dev2/tests/data/bad_header2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_jpeg2.tif` & `tifftools-1.5.2.dev2/tests/data/bad_jpeg2.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_subifd_offset.tif` & `tifftools-1.5.2.dev2/tests/data/bad_subifd_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_tag_offset.tif` & `tifftools-1.5.2.dev2/tests/data/bad_tag_offset.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/bad_unicode.tif` & `tifftools-1.5.2.dev2/tests/data/bad_unicode.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/data/good_jpeg.tif` & `tifftools-1.5.2.dev2/tests/data/good_jpeg.tif`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/datastore.py` & `tifftools-1.5.2.dev2/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_constants.py` & `tifftools-1.5.2.dev2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_dump.py` & `tifftools-1.5.2.dev2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_main.py` & `tifftools-1.5.2.dev2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_options.py` & `tifftools-1.5.2.dev2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_path_or_fobj.py` & `tifftools-1.5.2.dev2/tests/test_path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_read_tiff.py` & `tifftools-1.5.2.dev2/tests/test_read_tiff.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_readme.py` & `tifftools-1.5.2.dev2/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_set.py` & `tifftools-1.5.2.dev2/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_split.py` & `tifftools-1.5.2.dev2/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tests/test_write_tiff.py` & `tifftools-1.5.2.dev2/tests/test_write_tiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,39 @@
     assert len(open(destpath, 'rb').read().split(uniqueString)) == 3
     dest2path = tmp_path / 'sample2.tiff'
     tifftools.write_tiff(info, dest2path, dedup=True)
     assert len(open(dest2path, 'rb').read().split(uniqueString)) == 2
     info2 = tifftools.read_tiff(dest2path)
     dest3path = tmp_path / 'sample3.tiff'
     tifftools.write_tiff(info2, dest3path)
-    assert open(destpath, 'rb').read() == open(dest3path, 'rb').read()
+    assert len(open(dest3path, 'rb').read().split(uniqueString)) == 3
+
+
+def test_write_with_dedup_and_ifdsfirst(tmp_path):
+    path = os.path.join(os.path.dirname(__file__), 'data', 'good_single.tif')
+    info = tifftools.read_tiff(path)
+    uniqueString = b'UNIQUESTRING'
+    info['ifds'][0]['tags'][23456] = {
+        'datatype': tifftools.Datatype.UNDEFINED,
+        'data': uniqueString
+    }
+    info['ifds'][0]['tags'][23457] = {
+        'datatype': tifftools.Datatype.UNDEFINED,
+        'data': uniqueString
+    }
+    destpath = tmp_path / 'sample.tiff'
+    tifftools.write_tiff(info, destpath)
+    assert len(open(destpath, 'rb').read().split(uniqueString)) == 3
+    dest2path = tmp_path / 'sample2.tiff'
+    tifftools.write_tiff(info, dest2path, dedup=True, ifdsFirst=True)
+    assert len(open(dest2path, 'rb').read().split(uniqueString)) == 2
+    info2 = tifftools.read_tiff(dest2path)
+    dest3path = tmp_path / 'sample3.tiff'
+    tifftools.write_tiff(info2, dest3path)
+    assert len(open(dest3path, 'rb').read().split(uniqueString)) == 3
 
 
 def test_write_bytecount_data(tmp_path):
     path = os.path.join(os.path.dirname(__file__), 'data', 'good_single.tif')
     info = tifftools.read_tiff(path)
     # Just use data from within the file itself; an actual sample file with
     # compression 6 and defined Q, AC, and DC tables would be better.
```

### Comparing `tifftools-1.5.1.dev2/tifftools/__init__.py` & `tifftools-1.5.2.dev2/tifftools/__init__.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tifftools/commands.py` & `tifftools-1.5.2.dev2/tifftools/commands.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tifftools/constants.py` & `tifftools-1.5.2.dev2/tifftools/constants.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tifftools/path_or_fobj.py` & `tifftools-1.5.2.dev2/tifftools/path_or_fobj.py`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tifftools/tifftools.py` & `tifftools-1.5.2.dev2/tifftools/tifftools.py`

 * *Files 2% similar despite different names*

```diff
@@ -701,59 +701,57 @@
     if len(offsets) != len(lengths):
         raise TifftoolsError('Offsets and byte counts do not correspond.')
     destOffsets = [0] * len(offsets)
     # We preserve the order of the chunks from the original file
     offsetList = sorted([(offset, idx) for idx, offset in enumerate(offsets)])
     olidx = 0
     lastOffset = lastLength = lastOffsetIdx = None
+    blocks = []
+    desttell = dest.tell()
     while olidx < len(offsetList):
         offset, idx = offsetList[olidx]
         length = lengths[idx]
         if offset and check_offset(srclen, offset, length):
             # if a block repeats a previous block, continue the pattern
             if lastOffset == offset and lastLength == length:
                 destOffsets[idx] = destOffsets[lastOffsetIdx]
                 olidx += 1
                 continue
             lastOffset, lastLength, lastOffsetIdx = offset, length, idx
-            src.seek(offset)
-            destOffsets[idx] = dest.tell()
-            tells = {'idx': [idx], 'pos': destOffsets[idx], 'offset': offset}
-            # Group reads when possible; the biggest overhead is in the actual
-            # read call
-            while (not dedup and olidx + 1 < len(offsetList) and
-                   offsetList[olidx + 1][0] == offsetList[olidx][0] + lengths[idx] and
-                   check_offset(srclen, offsetList[olidx + 1][0],
-                                lengths[offsetList[olidx + 1][1]])):
-                destOffsets[offsetList[olidx + 1][1]] = destOffsets[idx] + lengths[idx]
-                tells['idx'].append(offsetList[olidx + 1][1])
-                olidx += 1
-                offset, idx = offsetList[olidx]
-                length += lengths[idx]
+            destOffsets[idx] = desttell
             if dedup:
                 hashkey = (hash(getattr(src, 'name', src)), offset)
                 if hashkey in dedup['hashlog']:
                     h = dedup['hashlog'][hashkey]
                 else:
                     readlen = length
                     h = hashlib.new(_DEDUP_HASH_METHOD)
+                    src.seek(offset)
                     while readlen:
                         data = src.read(min(readlen, COPY_CHUNKSIZE))
                         h.update(data)
                         readlen -= len(data)
                     h = h.digest()
                     dedup['hashlog'][hashkey] = h
                 if h in dedup['hashes']:
                     hpos = dedup['hashes'][h]
-                    for tidx in tells['idx']:
-                        destOffsets[tidx] = destOffsets[tidx] - tells['pos'] + hpos
+                    destOffsets[idx] = hpos
                     dedup['reused'] += 1
                     length = 0
                 else:
-                    dedup['hashes'][h] = tells['pos']
-                    src.seek(tells['offset'])
-            while length:
-                data = src.read(min(length, COPY_CHUNKSIZE))
-                dest.write(data)
-                length -= len(data)
+                    dedup['hashes'][h] = destOffsets[idx]
+            # Group reads when possible; the biggest overhead is in the actual
+            # read call
+            if length:
+                if len(blocks) and offset == blocks[-1][0] + blocks[-1][1]:
+                    blocks[-1] = (blocks[-1][0], blocks[-1][1] + length)
+                else:
+                    blocks.append((offset, length))
+                desttell += length
         olidx += 1
+    for offset, length in blocks:
+        src.seek(offset)
+        while length:
+            data = src.read(min(length, COPY_CHUNKSIZE))
+            dest.write(data)
+            length -= len(data)
     return destOffsets
```

### Comparing `tifftools-1.5.1.dev2/tifftools.egg-info/PKG-INFO` & `tifftools-1.5.2.dev2/tifftools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifftools
-Version: 1.5.1.dev2
+Version: 1.5.2.dev2
 Summary: Pure python tiff tools to handle all tags and IFDs.
 Home-page: https://github.com/DigitalSlideArchive/tifftools
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: tiff
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tifftools-1.5.1.dev2/tifftools.egg-info/SOURCES.txt` & `tifftools-1.5.2.dev2/tifftools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tifftools-1.5.1.dev2/tox.ini` & `tifftools-1.5.2.dev2/tox.ini`

 * *Files identical despite different names*


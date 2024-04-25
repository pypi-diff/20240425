# Comparing `tmp/janus_swi-1.1.4.tar.gz` & `tmp/janus_swi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_swi-1.1.4.tar", last modified: Thu Feb 22 15:29:51 2024, max compression
+gzip compressed data, was "janus_swi-1.2.0.tar", last modified: Thu Apr 25 09:50:41 2024, max compression
```

## Comparing `janus_swi-1.1.4.tar` & `janus_swi-1.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.735834 janus_swi-1.1.4/
--rw-r--r--   0 janw      (1000) janw      (1000)       83 2023-09-03 11:56:51.000000 janus_swi-1.1.4/.gitignore
--rw-r--r--   0 janw      (1000) janw      (1000)     1840 2024-02-02 10:15:19.000000 janus_swi-1.1.4/CMakeLists.txt
--rw-r--r--   0 janw      (1000) janw      (1000)     6657 2024-02-22 15:29:51.735834 janus_swi-1.1.4/PKG-INFO
--rw-r--r--   0 janw      (1000) janw      (1000)     6125 2023-12-08 12:29:10.000000 janus_swi-1.1.4/README.md
--rw-r--r--   0 janw      (1000) janw      (1000)        6 2024-02-22 15:28:34.000000 janus_swi-1.1.4/VERSION
--rw-r--r--   0 janw      (1000) janw      (1000)       82 2024-02-02 10:15:19.000000 janus_swi-1.1.4/config.h.cmake
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.731834 janus_swi-1.1.4/examples/
--rw-r--r--   0 janw      (1000) janw      (1000)      443 2023-08-03 15:55:23.000000 janus_swi-1.1.4/examples/SpaCY.md
--rw-r--r--   0 janw      (1000) janw      (1000)      394 2023-08-03 15:55:23.000000 janus_swi-1.1.4/examples/spacy.pl
--rw-r--r--   0 janw      (1000) janw      (1000)      200 2023-10-16 09:41:10.000000 janus_swi-1.1.4/examples/trains.py
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.731834 janus_swi-1.1.4/gen/
--rw-r--r--   0 janw      (1000) janw      (1000)      726 2023-09-07 10:01:02.000000 janus_swi-1.1.4/gen/janus.bbl
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.735834 janus_swi-1.1.4/janus/
--rw-r--r--   0 janw      (1000) janw      (1000)      925 2023-09-03 12:39:21.000000 janus_swi-1.1.4/janus/__init__.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1261 2023-11-09 16:44:28.000000 janus_swi-1.1.4/janus/_find_swipl.py
--rw-r--r--   0 janw      (1000) janw      (1000)     4634 2023-11-08 13:09:52.000000 janus_swi-1.1.4/janus/hash.c
--rw-r--r--   0 janw      (1000) janw      (1000)    57119 2024-01-10 12:43:29.000000 janus_swi-1.1.4/janus/janus.c
--rw-r--r--   0 janw      (1000) janw      (1000)    43116 2024-02-02 10:19:12.000000 janus_swi-1.1.4/janus/janus.pl
--rw-r--r--   0 janw      (1000) janw      (1000)    19808 2024-02-22 15:28:40.000000 janus_swi-1.1.4/janus/janus.py
--rw-r--r--   0 janw      (1000) janw      (1000)      113 2023-09-03 11:56:51.000000 janus_swi-1.1.4/janus/janus_swi.py
--rw-r--r--   0 janw      (1000) janw      (1000)    16978 2024-01-10 12:48:05.000000 janus_swi-1.1.4/janus/mod_swipl.c
--rw-r--r--   0 janw      (1000) janw      (1000)    56542 2024-01-13 13:25:41.000000 janus_swi-1.1.4/janus.doc
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.735834 janus_swi-1.1.4/janus_swi.egg-info/
--rw-r--r--   0 janw      (1000) janw      (1000)     6657 2024-02-22 15:29:51.000000 janus_swi-1.1.4/janus_swi.egg-info/PKG-INFO
--rw-r--r--   0 janw      (1000) janw      (1000)      915 2024-02-22 15:29:51.000000 janus_swi-1.1.4/janus_swi.egg-info/SOURCES.txt
--rw-r--r--   0 janw      (1000) janw      (1000)        1 2024-02-22 15:29:51.000000 janus_swi-1.1.4/janus_swi.egg-info/dependency_links.txt
--rw-r--r--   0 janw      (1000) janw      (1000)       10 2024-02-22 15:29:51.000000 janus_swi-1.1.4/janus_swi.egg-info/top_level.txt
--rw-r--r--   0 janw      (1000) janw      (1000)      589 2023-09-19 08:05:44.000000 janus_swi-1.1.4/pyproject.toml
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.735834 janus_swi-1.1.4/scripts/
--rwxr-xr-x   0 janw      (1000) janw      (1000)     1582 2023-12-15 13:16:39.000000 janus_swi-1.1.4/scripts/newversion
--rwxrwxr-x   0 janw      (1000) janw      (1000)      310 2023-12-17 16:29:23.000000 janus_swi-1.1.4/scripts/pypi-upload
--rw-r--r--   0 janw      (1000) janw      (1000)       38 2024-02-22 15:29:51.735834 janus_swi-1.1.4/setup.cfg
--rw-r--r--   0 janw      (1000) janw      (1000)     1651 2024-02-22 15:28:40.000000 janus_swi-1.1.4/setup.py
--rw-r--r--   0 janw      (1000) janw      (1000)    14859 2024-01-10 17:13:51.000000 janus_swi-1.1.4/test_janus.pl
--rw-r--r--   0 janw      (1000) janw      (1000)     8218 2024-01-16 08:48:38.000000 janus_swi-1.1.4/test_xsb_janus.pl
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.735834 janus_swi-1.1.4/tests/
--rw-r--r--   0 janw      (1000) janw      (1000)       28 2023-09-07 07:25:25.000000 janus_swi-1.1.4/tests/baseclasses.py
--rw-r--r--   0 janw      (1000) janw      (1000)     5706 2023-11-01 16:45:15.000000 janus_swi-1.1.4/tests/bench.pl
--rw-r--r--   0 janw      (1000) janw      (1000)     3870 2023-11-25 15:01:40.000000 janus_swi-1.1.4/tests/demo.py
--rw-r--r--   0 janw      (1000) janw      (1000)      275 2023-12-20 20:35:11.000000 janus_swi-1.1.4/tests/dog.py
--rw-rw-r--   0 janw      (1000) janw      (1000)      170 2023-07-28 09:08:08.000000 janus_swi-1.1.4/tests/russel.pl
--rw-r--r--   0 janw      (1000) janw      (1000)      586 2023-10-16 09:28:16.000000 janus_swi-1.1.4/tests/threads.py
--rw-r--r--   0 janw      (1000) janw      (1000)      188 2023-10-16 09:41:10.000000 janus_swi-1.1.4/tests/while.py
-drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-02-22 15:29:51.735834 janus_swi-1.1.4/xsb_tests/
--rw-r--r--   0 janw      (1000) janw      (1000)     2101 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/Person.py
--rw-r--r--   0 janw      (1000) janw      (1000)     2256 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/jintf.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1322 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/kwargs.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1286 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/numpexamp.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1946 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/returnVal.py
--rw-r--r--   0 janw      (1000) janw      (1000)      568 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/sample.json
--rw-r--r--   0 janw      (1000) janw      (1000)     1824 2023-09-07 07:29:42.000000 janus_swi-1.1.4/xsb_tests/stressTest.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1338 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/sumlist3.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1320 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/test_err.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1685 2023-09-07 07:30:23.000000 janus_swi-1.1.4/xsb_tests/test_stress.pl
--rw-r--r--   0 janw      (1000) janw      (1000)     1289 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/testc.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1400 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/tupInList.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1260 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/tupletest.py
--rw-r--r--   0 janw      (1000) janw      (1000)     1392 2023-09-03 11:56:51.000000 janus_swi-1.1.4/xsb_tests/variadic.py
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.498338 janus_swi-1.2.0/
+-rw-r--r--   0 janw      (1000) janw      (1000)       83 2024-01-26 10:35:59.000000 janus_swi-1.2.0/.gitignore
+-rw-r--r--   0 janw      (1000) janw      (1000)     2180 2024-04-25 09:27:30.000000 janus_swi-1.2.0/CMakeLists.txt
+-rw-r--r--   0 janw      (1000) janw      (1000)     6657 2024-04-25 09:50:41.498338 janus_swi-1.2.0/PKG-INFO
+-rw-r--r--   0 janw      (1000) janw      (1000)     6125 2024-01-26 10:35:59.000000 janus_swi-1.2.0/README.md
+-rw-r--r--   0 janw      (1000) janw      (1000)        6 2024-04-25 09:49:12.000000 janus_swi-1.2.0/VERSION
+-rw-r--r--   0 janw      (1000) janw      (1000)       82 2024-01-26 10:35:59.000000 janus_swi-1.2.0/config.h.cmake
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.494338 janus_swi-1.2.0/examples/
+-rw-r--r--   0 janw      (1000) janw      (1000)      443 2024-01-26 10:35:59.000000 janus_swi-1.2.0/examples/SpaCY.md
+-rw-r--r--   0 janw      (1000) janw      (1000)      394 2024-01-26 10:35:59.000000 janus_swi-1.2.0/examples/spacy.pl
+-rw-r--r--   0 janw      (1000) janw      (1000)      200 2024-01-26 10:35:59.000000 janus_swi-1.2.0/examples/trains.py
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.494338 janus_swi-1.2.0/gen/
+-rw-r--r--   0 janw      (1000) janw      (1000)      726 2024-01-26 10:35:59.000000 janus_swi-1.2.0/gen/janus.bbl
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.494338 janus_swi-1.2.0/janus/
+-rw-r--r--   0 janw      (1000) janw      (1000)      925 2024-01-26 10:35:59.000000 janus_swi-1.2.0/janus/__init__.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1261 2024-01-26 10:35:59.000000 janus_swi-1.2.0/janus/_find_swipl.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     4634 2024-01-26 10:35:59.000000 janus_swi-1.2.0/janus/hash.c
+-rw-r--r--   0 janw      (1000) janw      (1000)    58067 2024-04-25 09:27:30.000000 janus_swi-1.2.0/janus/janus.c
+-rw-r--r--   0 janw      (1000) janw      (1000)    45100 2024-04-05 07:29:17.000000 janus_swi-1.2.0/janus/janus.pl
+-rw-r--r--   0 janw      (1000) janw      (1000)    19808 2024-04-25 09:49:23.000000 janus_swi-1.2.0/janus/janus.py
+-rw-r--r--   0 janw      (1000) janw      (1000)      113 2024-01-26 10:35:59.000000 janus_swi-1.2.0/janus/janus_swi.py
+-rw-r--r--   0 janw      (1000) janw      (1000)    17119 2024-04-05 07:29:17.000000 janus_swi-1.2.0/janus/mod_swipl.c
+-rw-r--r--   0 janw      (1000) janw      (1000)    56534 2024-04-25 09:27:30.000000 janus_swi-1.2.0/janus.doc
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.498338 janus_swi-1.2.0/janus_swi.egg-info/
+-rw-r--r--   0 janw      (1000) janw      (1000)     6657 2024-04-25 09:50:41.000000 janus_swi-1.2.0/janus_swi.egg-info/PKG-INFO
+-rw-r--r--   0 janw      (1000) janw      (1000)      915 2024-04-25 09:50:41.000000 janus_swi-1.2.0/janus_swi.egg-info/SOURCES.txt
+-rw-r--r--   0 janw      (1000) janw      (1000)        1 2024-04-25 09:50:41.000000 janus_swi-1.2.0/janus_swi.egg-info/dependency_links.txt
+-rw-r--r--   0 janw      (1000) janw      (1000)       10 2024-04-25 09:50:41.000000 janus_swi-1.2.0/janus_swi.egg-info/top_level.txt
+-rw-r--r--   0 janw      (1000) janw      (1000)      589 2024-01-26 10:35:59.000000 janus_swi-1.2.0/pyproject.toml
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.498338 janus_swi-1.2.0/scripts/
+-rwxr-xr-x   0 janw      (1000) janw      (1000)     1582 2024-01-26 10:35:59.000000 janus_swi-1.2.0/scripts/newversion
+-rwxr-xr-x   0 janw      (1000) janw      (1000)      310 2024-01-26 10:35:59.000000 janus_swi-1.2.0/scripts/pypi-upload
+-rw-r--r--   0 janw      (1000) janw      (1000)       38 2024-04-25 09:50:41.498338 janus_swi-1.2.0/setup.cfg
+-rw-r--r--   0 janw      (1000) janw      (1000)     1651 2024-04-25 09:49:23.000000 janus_swi-1.2.0/setup.py
+-rw-r--r--   0 janw      (1000) janw      (1000)    14859 2024-01-26 10:35:59.000000 janus_swi-1.2.0/test_janus.pl
+-rw-r--r--   0 janw      (1000) janw      (1000)     8218 2024-01-26 10:35:59.000000 janus_swi-1.2.0/test_xsb_janus.pl
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.498338 janus_swi-1.2.0/tests/
+-rw-r--r--   0 janw      (1000) janw      (1000)       28 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/baseclasses.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     5706 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/bench.pl
+-rw-r--r--   0 janw      (1000) janw      (1000)     3870 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/demo.py
+-rw-r--r--   0 janw      (1000) janw      (1000)      275 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/dog.py
+-rw-r--r--   0 janw      (1000) janw      (1000)      170 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/russel.pl
+-rw-r--r--   0 janw      (1000) janw      (1000)      586 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/threads.py
+-rw-r--r--   0 janw      (1000) janw      (1000)      188 2024-01-26 10:35:59.000000 janus_swi-1.2.0/tests/while.py
+drwxr-xr-x   0 janw      (1000) janw      (1000)        0 2024-04-25 09:50:41.498338 janus_swi-1.2.0/xsb_tests/
+-rw-r--r--   0 janw      (1000) janw      (1000)     2101 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/Person.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     2256 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/jintf.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1322 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/kwargs.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1286 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/numpexamp.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1946 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/returnVal.py
+-rw-r--r--   0 janw      (1000) janw      (1000)      568 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/sample.json
+-rw-r--r--   0 janw      (1000) janw      (1000)     1824 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/stressTest.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1338 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/sumlist3.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1320 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/test_err.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1685 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/test_stress.pl
+-rw-r--r--   0 janw      (1000) janw      (1000)     1289 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/testc.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1400 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/tupInList.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1260 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/tupletest.py
+-rw-r--r--   0 janw      (1000) janw      (1000)     1392 2024-01-26 10:35:59.000000 janus_swi-1.2.0/xsb_tests/variadic.py
```

### Comparing `janus_swi-1.1.4/CMakeLists.txt` & `janus_swi-1.2.0/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 cmake_minimum_required(VERSION 3.16)
 project(swipl-swipy)
 
 include("../cmake/PrologPackage.cmake")
 
 if(CMAKE_BUILD_TYPE STREQUAL "Debug" OR CMAKE_BUILD_TYPE STREQUAL "Sanitize")
   message("Trying to find debug version of Python")
+  set(PYTHON_PREFER_DEBUG ON)
   set(Python_FIND_ABI "ON" "ANY" "ANY")
 endif()
 
 # Note: allows for -DCPYTHON_VERSION="3.11;EXACT" to demand an exact
 # version of CPython.  Used by the Macports Portfile to ensure the
 # requested dependency and the version used are the same.
 if(NOT CPYTHON_VERSION)
@@ -17,14 +18,22 @@
 endif()
 
 find_package(Python ${CPYTHON_VERSION} COMPONENTS Interpreter Development)
 if(CMAKE_VERSION VERSION_LESS 3.18 AND Python_Development_FOUND)
   set(Python_Development.Embed_FOUND ON)
 endif()
 
+if(NOT Python_Development.Embed_FOUND AND PYTHON_PREFER_DEBUG)
+  set(Python_FIND_ABI "ANY" "ANY" "ANY")
+  find_package(Python ${CPYTHON_VERSION} COMPONENTS Interpreter Development)
+  if(CMAKE_VERSION VERSION_LESS 3.18 AND Python_Development_FOUND)
+    set(Python_Development.Embed_FOUND ON)
+  endif()
+endif()
+
 if(Python_Development.Embed_FOUND)
 
 set(PYTHON_FILES janus.py janus_swi.py)
 prepend(PYTHON_FILES janus/ ${PYTHON_FILES})
 
 # For some reason linking to python3.lib claims python311.lib does
 # not exist when using MSVC.   The link command seems correct.
```

### Comparing `janus_swi-1.1.4/PKG-INFO` & `janus_swi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus_swi
-Version: 1.1.4
+Version: 1.2.0
 Summary: Janus library to call SWI-Prolog
 Home-page: https://github.com/SWI-Prolog/packages-swipy
 Author: Jan Wielemaker
 Author-email: Jan Wielemaker <jan@swi-prolog.org>
 License: BSD-2-Clause
 Project-URL: Homepage, https://www.swi-prolog.org
 Project-URL: Documentation, https://www.swi-prolog.org/pldoc/package/janus
```

### Comparing `janus_swi-1.1.4/README.md` & `janus_swi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/gen/janus.bbl` & `janus_swi-1.2.0/gen/janus.bbl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/janus/__init__.py` & `janus_swi-1.2.0/janus/__init__.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/janus/_find_swipl.py` & `janus_swi-1.2.0/janus/_find_swipl.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/janus/hash.c` & `janus_swi-1.2.0/janus/hash.c`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/janus/janus.c` & `janus_swi-1.2.0/janus/janus.c`

 * *Files 0% similar despite different names*

```diff
@@ -388,40 +388,62 @@
     }
   }
 
   return FALSE;
 }
 
 static htable *py_module_table = NULL;
+static PL_option_t import_options[] =
+{ PL_OPTION("as", OPT_ATOM),
+  PL_OPTIONS_END
+};
+
 
 static int
-py_register_module(term_t name, PyObject **mod, int flags)
-{ PyObject *idobj;
-  atom_t id;
+py_register_module(term_t name, term_t options, PyObject **mod, int flags)
+{ PyObject *idobj = NULL;
+  int rc = FALSE;
 
   if ( !py_module_table )
     py_module_table = py_new_hashmap();
 
-  if ( get_py_name(name, &idobj, flags) &&
-       PL_get_atom(name, &id) )
-  { PyObject *m = check_error(PyImport_Import(idobj));
+  if ( get_py_name(name, &idobj, flags) )
+  { PyObject *m;
+    atom_t as = 0;
+
+    if ( options )
+    { if ( !PL_scan_options(options, 0, "py_import_options", import_options,
+			    &as) )
+	goto out;
+      if ( as && py_lookup_hashmap(py_module_table, as) )
+      { term_t as_term;
+	rc = ((as_term=PL_new_term_ref()) &&
+	      PL_put_atom(as_term, as) &&
+	      PL_permission_error("import_as", "py_module", as_term));
+	goto out;
+      }
+    }
+    if ( !as && !PL_get_atom_ex(name, &as) )
+      goto out;
 
-    Py_DECREF(idobj);
+    m = check_error(PyImport_Import(idobj));
     if ( m )
     { PyObject *old = NULL;
       if ( mod )
 	*mod = m;
-      int rc = py_add_hashmap(py_module_table, id, m, &old);
+      rc = py_add_hashmap(py_module_table, as, m, &old);
       if ( old )
 	Py_DECREF(old);
-      return rc;
-    }
+    } else
+      rc = FALSE;
   }
 
-  return FALSE;
+out:
+  Py_CLEAR(idobj);
+  return rc;
 }
 
 
 static int
 get_py_module(term_t name, PyObject **mod)
 { atom_t id;
 
@@ -439,15 +461,15 @@
       py_module_table = py_new_hashmap();
 
     if ( (obj=py_lookup_hashmap(py_module_table, id)) )
     { Py_INCREF(obj);
       *mod = obj;
       return TRUE;
     } else
-    { if ( py_register_module(name, mod, 0) )
+    { if ( py_register_module(name, 0, mod, 0) )
       { Py_INCREF(*mod);
 	return TRUE;
       }
     }
   }
 
   return FALSE;
@@ -457,15 +479,29 @@
 static foreign_t
 py_update_module_cache(term_t name)
 { int rc;
   py_gil_state state;
 
   if ( !py_gil_ensure(&state) )
     return FALSE;
-  rc = py_register_module(name, NULL, CVT_EXCEPTION);
+  rc = py_register_module(name, 0, NULL, CVT_EXCEPTION);
+  py_gil_release(state);
+
+  return rc;
+}
+
+
+static foreign_t
+py_import(term_t spec, term_t options)
+{ py_gil_state state;
+  int rc;
+
+  if ( !py_gil_ensure(&state) )
+    return FALSE;
+  rc = py_register_module(spec, options, NULL, CVT_EXCEPTION);
   py_gil_release(state);
 
   return rc;
 }
 
 
 static PyObject *
@@ -996,37 +1032,42 @@
 		 /*******************************
 		 *       PROLOG -> PYTHON       *
 		 *******************************/
 
 static int
 py_add_to_dict(term_t key, term_t value, void *closure)
 { PyObject *py_dict = closure;
-  PyObject *py_value;
+  PyObject *py_value = NULL;
+  PyObject *py_key = NULL;
   char *s;
   int rc;
 
-  if ( !py_from_prolog(value, &py_value) )
-    return 1;				/* error */
+  if ( py_from_prolog(value, &py_value) )
+  { if ( PL_get_chars(key, &s, CVT_ATOM) )
+    { rc = PyDict_SetItemString(py_dict, s, py_value);
+    } else
+    { if ( py_from_prolog(key, &py_key) )
+      { rc = PyDict_SetItem(py_dict, py_key, py_value);
+      } else
+      { rc = 1;
+	goto out;		/* not a Python error */
+      }
+    }
 
-  if ( PL_get_chars(key, &s, CVT_ATOM) )
-  { rc = PyDict_SetItemString(py_dict, s, py_value);
+    if ( rc != 0 )
+      check_error(py_value);
   } else
-  { PyObject *py_key;
-
-    if ( !py_from_prolog(key, &py_key) )
-      return 1;
-    rc = PyDict_SetItem(py_dict, py_key, py_value);
+  { rc = 1;
   }
 
-  if ( rc != 0 )
-  { check_error(py_value);
-    return 1;
-  }
+out:
+  Py_CLEAR(py_value);
+  Py_CLEAR(py_key);
 
-  return 0;
+  return rc;
 }
 
 
 static int
 add_prolog_key_value_to_dict(PyObject *py_dict, term_t tuple,
 			     term_t key, term_t value)
 { if ( PL_is_functor(tuple, FUNCTOR_key_value2) ) /* Key:Value */
@@ -2470,14 +2511,15 @@
 
 #define REGISTER(name, arity, func, flags) \
         PL_register_foreign_in_module("janus", name, arity, func, flags)
 #define NDET PL_FA_NONDETERMINISTIC
 
   REGISTER("py_initialize_",	     3,	py_initialize_,		0);
   REGISTER("py_finalize",	     0,	py_finalize,		0);
+  REGISTER("py_import_",	     2, py_import,		0);
   REGISTER("py_call",		     1,	py_call1,		0);
   REGISTER("py_call",		     2,	py_call2,		0);
   REGISTER("py_call",		     3,	py_call3,		0);
   REGISTER("py_iter",		     2,	py_iter2,		NDET);
   REGISTER("py_iter",		     3,	py_iter3,		NDET);
   REGISTER("py_setattr",	     3, py_setattr,		0);
   REGISTER("py_run",		     5,	py_run,			0);
```

### Comparing `janus_swi-1.1.4/janus/janus.pl` & `janus_swi-1.2.0/janus/janus.pl`

 * *Files 4% similar despite different names*

```diff
@@ -68,28 +68,29 @@
             py_obj_dir/2,               % +ObjRef, -List (deprecated)
             py_obj_dict/2,              % +ObjRef, -Dict (deprecated)
             py_type/2,			% +ObjRef, -Type:atom
             py_isinstance/2,            % +ObjRef, +Type
             py_module_exists/1,         % +Module
             py_hasattr/2,               % +Module, ?Symbol
 
+            py_import/2,                % +Spec, +Options
             py_module/2,                % +Module:atom, +Source:string
 
             py_initialize/3,            % +Program, +Argv, +Options
             py_lib_dirs/1,              % -Dirs
             py_add_lib_dir/1,           % +Dir
             py_add_lib_dir/2,           % +Dir,+Where
 
             op(200, fy, @),             % @constant
             op(50,  fx, #)              % #Value
           ]).
 :- meta_predicate py_with_gil(0).
 
 :- use_module(library(apply_macros), []).
-:- autoload(library(lists), [append/3, member/2, append/2]).
+:- autoload(library(lists), [append/3, member/2, append/2, last/2]).
 :- autoload(library(apply),
             [maplist/2, exclude/3, maplist/3, convlist/3, partition/4]).
 :- autoload(library(error), [must_be/2, domain_error/2]).
 :- autoload(library(dicts), [dict_keys/2]).
 :- autoload(library(option), [dict_options/2, select_option/4, option/2]).
 :- autoload(library(prolog_code), [comma_list/2]).
 :- autoload(library(readutil), [read_line_to_string/2, read_file_to_string/3]).
@@ -731,14 +732,59 @@
     (   atom(ModuleOrObj)
     ->  py_call(ModuleOrObj:'__name__'), % force loading
         py_call(hasattr(eval(sys:modules:'__getitem__'(ModuleOrObj)), Name), @true)
     ;   py_call(hasattr(ModuleOrObj, Name), @true)
     ).
 
 
+%!  py_import(+Spec, +Options) is det.
+%
+%   Import a Python module.  Janus   imports  modules automatically when
+%   referred in py_call/2 and  related   predicates.  Importing a module
+%   implies  the  module  is  loaded   using  Python's  ``__import__()``
+%   built-in and added to a table  that   maps  Prolog atoms to imported
+%   modules. This predicate explicitly imports a module and allows it to
+%   be associated with a different  name.   This  is  useful for loading
+%   _nested modules_, i.e., a specific module   from a Python package as
+%   well as for  avoiding  conflicts.  For   example,  with  the  Python
+%   `selenium` package installed, we can do in Python:
+%
+%       >>> from selenium import webdriver
+%       >>> browser = webdriver.Chrome()
+%
+%   Without this predicate, we can do
+%
+%       ?- py_call('selenium.webdriver':'Chrome'(), Chrome).
+%
+%   For a single call this is  fine,   but  for making multiple calls it
+%   gets cumbersome.  With this predicate we can write this.
+%
+%       ?- py_import('selenium.webdriver', []).
+%       ?- py_call(webdriver:'Chrome'(), Chrome).
+%
+%   By default, the imported module  is   associated  to an atom created
+%   from the last segment of the dotted   name. Below we use an explicit
+%   name.
+%
+%       ?- py_import('selenium.webdriver', [as(browser)]).
+%       ?- py_call(browser:'Chrome'(), Chrome).
+%
+%   @error  permission_error(import_as,  py_module,  As)   if  there  is
+%   already a module associated with As.
+
+py_import(Spec, Options) :-
+    option(as(_), Options),
+    !,
+    py_import_(Spec, Options).
+py_import(Spec, Options) :-
+    split_string(Spec, ".", "", Parts),
+    last(Parts, Last),
+    atom_string(As, Last),
+    py_import_(Spec, [as(As)|Options]).
+
 %!  py_module(+Module:atom, +Source:string) is det.
 %
 %   Load Source into the Python module Module.   This  is intended to be
 %   used together with the `string` _quasi quotation_ that supports long
 %   strings in SWI-Prolog.   For example:
 %
 %   ```
@@ -1252,14 +1298,18 @@
 
 prolog:error_message(python_error(Class, Value)) -->
     { py_str(Value, Message)
     },
     [ 'Python ', ansi(code, "'~w'", [Class]), ':', nl,
       '  ~w'-[Message]
     ].
+prolog:error_message(permission_error(import_as, py_module, As)) -->
+    [ 'Janus: No permission to import a module as ', ansi(code, '~q', As),
+      ': module exists.'
+    ].
 
 prolog:message_context(context(_, PythonCtx)) -->
     { nonvar(PythonCtx),
       PythonCtx = python_stack(Stack),
       current_prolog_flag(py_backtrace, true),
       py_is_object(Stack),
       !,
```

### Comparing `janus_swi-1.1.4/janus/janus.py` & `janus_swi-1.2.0/janus/janus.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 if not hasattr(_swipl, 'call'):
     raise RuntimeError(f"Loaded wrong module '_swipl' from {_swipl.__file__}")
 
 ################################################################
 # Versions
 
 # 10000*major + 100*minor + patch
-version_num=10104
+version_num=10200
 
 def version_str(num=version_num):
     """
     Return Janus version as major.minor.patch
     """
     return f"{num//10000}.{num%10000//100}.{num%100}"
```

### Comparing `janus_swi-1.1.4/janus/mod_swipl.c` & `janus_swi-1.2.0/janus/mod_swipl.c`

 * *Files 1% similar despite different names*

```diff
@@ -492,15 +492,22 @@
 
   switch(rc)
   { case PL_S_LAST:
       PL_cut_query(qid);
       done = TRUE;
       /*FALLTHROUGH*/
     case PL_S_TRUE:
-      py_from_prolog(av+2, &out);
+      if ( !py_from_prolog(av+2, &out) )
+      { term_t ex = PL_exception(0);
+
+	assert(ex);
+	ex = PL_copy_term_ref(ex);
+	PL_clear_exception();
+	Py_SetPrologError(ex);
+      }
       break;
     case PL_S_FALSE:
       out = PyBool_FromLong(0);
       PL_cut_query(qid);
       done = TRUE;
       break;
     case PL_S_EXCEPTION:
```

### Comparing `janus_swi-1.1.4/janus.doc` & `janus_swi-1.2.0/janus.doc`

 * *Files 0% similar despite different names*

```diff
@@ -624,15 +624,15 @@
 
 \textbf{Failure to close a query typically leaves SWI-Prolog in an
 inconsistent state and further interaction with Prolog is likely to
 crash the process}.  Future versions may improve on that.
 
 
 \begin{description}
-  \cfunction{dict}{janus.query_once}{query, bindings=\{{}\}, keep=False,
+  \cfunction{dict}{janus.query_once}{query, inputs=\{{}\}, keep=False,
 			            truth_vals=TruthVals.PLAIN_TRUTHVALS}
 Call \arg{query} using \arg{bindings} as once/1, returning a dict with
 the resulting bindings. If \arg{bindings} is omitted, no variables are
 bound. The \arg{keep} parameter determines whether or not Prolog
 discards all backtrackable changes.  By default, such changes are
 discarded and as a result, changes to backtrackable global variables
 are lost.  Using \const{True}, such changes are preserved.
@@ -665,15 +665,15 @@
 queries (\cfuncref{janus.cmd}{}) or queries with leading ground
 arguments followed by a single output variable.
 
 \begin{tags}
 \tag{Compatibility} PIP.
 \end{tags}
 
-    \cfunction{dict}{janus.once}{query, bindings=\{{}\}, keep=False,
+    \cfunction{dict}{janus.once}{query, inputs=\{{}\}, keep=False,
 			         truth_vals=TruthVals.PLAIN_TRUTHVALS}
     \jargon{Deprecated}.  Renamed to \cfuncref{janus.query_once}{}.
 
     \cfunction{Any}{janus.apply_once}{module, predicate, *input, fail=obj}
     \jargon{Functional notation} style calling of a deterministic Prolog
     predicate.  This calls \term{module:predicate}{Input \ldots, Output}, where
     \arg{Input} are the Python \arg{input} arguments converted to
@@ -768,25 +768,25 @@
 
 Class \cfuncref{janus.query}{} is similar to the
 \cfuncref{janus.query_once}{} function, but it returns a Python
 \jargon{iterator} that allows for iterating over the answers to a
 non-deterministic Prolog predicate.
 
 \begin{description}
-   \cfunction{query}{janus.query}{query, bindings=\{{}\}, keep=False}
+   \cfunction{query}{janus.query}{query, inputs=\{{}\}, keep=False}
    As \cfuncref{janus.query_once}{}, returning an \jargon{iterator} that
    provides an answer dict as \cfuncref{janus.query_once}{} for each answer
    to \arg{query}.  Answers never have \const{truth} \const{False}.
    See discussion above.
 
 \begin{tags}
 \tag{Compatibility} PIP.  The \const{keep} is a SWI-Prolog extension.
 \end{tags}
 
-   \cfunction{Query}{janus.Query}{query, bindings=\{{}\}, keep=False}
+   \cfunction{Query}{janus.Query}{query, inputs=\{{}\}, keep=False}
    \jargon{Deprecated}.  This class was renamed to \cfuncref{janus.query}.
 
    \cfunction{dict{|}None}{janus.query.next}{}
    Explicitly ask for the next solution of the iterator.  Normally,
    using the \ctype{query} as an iterator is to be preferred.  See
    discussion above.
```

### Comparing `janus_swi-1.1.4/janus_swi.egg-info/PKG-INFO` & `janus_swi-1.2.0/janus_swi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus_swi
-Version: 1.1.4
+Version: 1.2.0
 Summary: Janus library to call SWI-Prolog
 Home-page: https://github.com/SWI-Prolog/packages-swipy
 Author: Jan Wielemaker
 Author-email: Jan Wielemaker <jan@swi-prolog.org>
 License: BSD-2-Clause
 Project-URL: Homepage, https://www.swi-prolog.org
 Project-URL: Documentation, https://www.swi-prolog.org/pldoc/package/janus
```

### Comparing `janus_swi-1.1.4/janus_swi.egg-info/SOURCES.txt` & `janus_swi-1.2.0/janus_swi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/pyproject.toml` & `janus_swi-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/scripts/newversion` & `janus_swi-1.2.0/scripts/newversion`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/setup.py` & `janus_swi-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     link_args.append(f'-Wl,-rpath={props["PLLIBDIR"]},--enable-new-dtags')
 elif ( sys.platform == 'darwin' ):
     link_args.append(f'-Wl,-rpath,{props["PLLIBDIR"]}')
 elif ( sys.platform == 'win32' ):
     PLLIB="libswipl"
 
 setup(name='janus_swi',
-      version='1.1.4',
+      version='1.2.0',
       description="Janus library to call SWI-Prolog",
       author="Jan Wielemaker",
       author_email="jan@swi-prolog.org",
       url="https://github.com/SWI-Prolog/packages-swipy",
       license="BSD-2",
       packages=['janus_swi'],
       package_dir={"janus_swi":"janus"},
```

### Comparing `janus_swi-1.1.4/test_janus.pl` & `janus_swi-1.2.0/test_janus.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/test_xsb_janus.pl` & `janus_swi-1.2.0/test_xsb_janus.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/tests/bench.pl` & `janus_swi-1.2.0/tests/bench.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/tests/demo.py` & `janus_swi-1.2.0/tests/demo.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/tests/threads.py` & `janus_swi-1.2.0/tests/threads.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/Person.py` & `janus_swi-1.2.0/xsb_tests/Person.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/jintf.py` & `janus_swi-1.2.0/xsb_tests/jintf.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/kwargs.py` & `janus_swi-1.2.0/xsb_tests/kwargs.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/numpexamp.py` & `janus_swi-1.2.0/xsb_tests/numpexamp.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/returnVal.py` & `janus_swi-1.2.0/xsb_tests/returnVal.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/sample.json` & `janus_swi-1.2.0/xsb_tests/sample.json`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/stressTest.py` & `janus_swi-1.2.0/xsb_tests/stressTest.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/sumlist3.py` & `janus_swi-1.2.0/xsb_tests/sumlist3.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/test_err.py` & `janus_swi-1.2.0/xsb_tests/test_err.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/test_stress.pl` & `janus_swi-1.2.0/xsb_tests/test_stress.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/testc.py` & `janus_swi-1.2.0/xsb_tests/testc.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/tupInList.py` & `janus_swi-1.2.0/xsb_tests/tupInList.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/tupletest.py` & `janus_swi-1.2.0/xsb_tests/tupletest.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.1.4/xsb_tests/variadic.py` & `janus_swi-1.2.0/xsb_tests/variadic.py`

 * *Files identical despite different names*


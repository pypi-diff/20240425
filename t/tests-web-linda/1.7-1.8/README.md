# Comparing `tmp/tests_web_linda-1.7.tar.gz` & `tmp/tests_web_linda-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tests_web_linda-1.7.tar", last modified: Thu Apr 25 15:30:06 2024, max compression
+gzip compressed data, was "tests_web_linda-1.8.tar", last modified: Thu Apr 25 15:31:50 2024, max compression
```

## Comparing `tests_web_linda-1.7.tar` & `tests_web_linda-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 15:30:06.589468 tests_web_linda-1.7/
--rw-rw-rw-   0        0        0       45 2024-04-25 15:29:10.000000 tests_web_linda-1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      413 2024-04-25 15:30:06.589468 tests_web_linda-1.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 15:30:06.589468 tests_web_linda-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1355 2024-04-25 15:29:19.000000 tests_web_linda-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:30:06.535567 tests_web_linda-1.7/tests_web_linda/
--rw-rw-rw-   0        0        0      101 2024-04-25 15:09:14.000000 tests_web_linda-1.7/tests_web_linda/__init__.py
--rw-rw-rw-   0        0        0     1240 2024-04-25 15:13:09.000000 tests_web_linda-1.7/tests_web_linda/main.py
--rw-rw-rw-   0        0        0       19 2024-04-25 15:29:16.000000 tests_web_linda-1.7/tests_web_linda/version.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:30:06.585206 tests_web_linda-1.7/tests_web_linda.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      335 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 15:31:50.735754 tests_web_linda-1.8/
+-rw-rw-rw-   0        0        0       45 2024-04-25 15:29:10.000000 tests_web_linda-1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      413 2024-04-25 15:31:50.735754 tests_web_linda-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:31:50.739999 tests_web_linda-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2024-04-25 15:31:41.000000 tests_web_linda-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:31:50.702578 tests_web_linda-1.8/tests_web_linda/
+-rw-rw-rw-   0        0        0      113 2024-04-25 15:31:20.000000 tests_web_linda-1.8/tests_web_linda/__init__.py
+-rw-rw-rw-   0        0        0     1240 2024-04-25 15:13:09.000000 tests_web_linda-1.8/tests_web_linda/main.py
+-rw-rw-rw-   0        0        0       19 2024-04-25 15:31:46.000000 tests_web_linda-1.8/tests_web_linda/version.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:31:50.735754 tests_web_linda-1.8/tests_web_linda.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-04-25 15:31:50.000000 tests_web_linda-1.8/tests_web_linda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-25 15:31:50.000000 tests_web_linda-1.8/tests_web_linda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:31:50.000000 tests_web_linda-1.8/tests_web_linda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-25 15:31:50.000000 tests_web_linda-1.8/tests_web_linda.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      335 2024-04-25 15:31:50.000000 tests_web_linda-1.8/tests_web_linda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 15:31:50.000000 tests_web_linda-1.8/tests_web_linda.egg-info/top_level.txt
```

### Comparing `tests_web_linda-1.7/setup.py` & `tests_web_linda-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 setup(
     name='tests_web_linda',
-    version='1.7',
+    version='1.8',
     description='A simple functional test library using Selenium and Chrome driver',
     author='Linda Lopez',
     packages=find_packages(),
     include_package_data=True, #Esto hace que setuptools lea el archivo MANIFEST.in
     package_data={
         'tests_web_linda': ['app/*'],
     },
```

### Comparing `tests_web_linda-1.7/tests_web_linda/main.py` & `tests_web_linda-1.8/tests_web_linda/main.py`

 * *Files identical despite different names*


# Comparing `tmp/tests_web_linda-1.6.tar.gz` & `tmp/tests_web_linda-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tests_web_linda-1.6.tar", last modified: Thu Apr 25 15:25:57 2024, max compression
+gzip compressed data, was "tests_web_linda-1.7.tar", last modified: Thu Apr 25 15:30:06 2024, max compression
```

## Comparing `tests_web_linda-1.6.tar` & `tests_web_linda-1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 15:25:57.398465 tests_web_linda-1.6/
--rw-rw-rw-   0        0        0       59 2024-04-24 16:36:39.000000 tests_web_linda-1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      413 2024-04-25 15:25:57.397386 tests_web_linda-1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 15:25:57.398465 tests_web_linda-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1355 2024-04-25 15:25:48.000000 tests_web_linda-1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:25:57.347323 tests_web_linda-1.6/tests_web_linda/
--rw-rw-rw-   0        0        0      101 2024-04-25 15:09:14.000000 tests_web_linda-1.6/tests_web_linda/__init__.py
--rw-rw-rw-   0        0        0     1240 2024-04-25 15:13:09.000000 tests_web_linda-1.6/tests_web_linda/main.py
--rw-rw-rw-   0        0        0       19 2024-04-25 15:25:53.000000 tests_web_linda-1.6/tests_web_linda/version.py
-drwxrwxrwx   0        0        0        0 2024-04-25 15:25:57.392550 tests_web_linda-1.6/tests_web_linda.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-25 15:25:57.000000 tests_web_linda-1.6/tests_web_linda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-25 15:25:57.000000 tests_web_linda-1.6/tests_web_linda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 15:25:57.000000 tests_web_linda-1.6/tests_web_linda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-25 15:25:57.000000 tests_web_linda-1.6/tests_web_linda.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      335 2024-04-25 15:25:57.000000 tests_web_linda-1.6/tests_web_linda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 15:25:57.000000 tests_web_linda-1.6/tests_web_linda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 15:30:06.589468 tests_web_linda-1.7/
+-rw-rw-rw-   0        0        0       45 2024-04-25 15:29:10.000000 tests_web_linda-1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      413 2024-04-25 15:30:06.589468 tests_web_linda-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:30:06.589468 tests_web_linda-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2024-04-25 15:29:19.000000 tests_web_linda-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:30:06.535567 tests_web_linda-1.7/tests_web_linda/
+-rw-rw-rw-   0        0        0      101 2024-04-25 15:09:14.000000 tests_web_linda-1.7/tests_web_linda/__init__.py
+-rw-rw-rw-   0        0        0     1240 2024-04-25 15:13:09.000000 tests_web_linda-1.7/tests_web_linda/main.py
+-rw-rw-rw-   0        0        0       19 2024-04-25 15:29:16.000000 tests_web_linda-1.7/tests_web_linda/version.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:30:06.585206 tests_web_linda-1.7/tests_web_linda.egg-info/
+-rw-rw-rw-   0        0        0      413 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      335 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 15:30:06.000000 tests_web_linda-1.7/tests_web_linda.egg-info/top_level.txt
```

### Comparing `tests_web_linda-1.6/setup.py` & `tests_web_linda-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 setup(
     name='tests_web_linda',
-    version='1.6',
+    version='1.7',
     description='A simple functional test library using Selenium and Chrome driver',
     author='Linda Lopez',
     packages=find_packages(),
     include_package_data=True, #Esto hace que setuptools lea el archivo MANIFEST.in
     package_data={
         'tests_web_linda': ['app/*'],
     },
```

### Comparing `tests_web_linda-1.6/tests_web_linda/main.py` & `tests_web_linda-1.7/tests_web_linda/main.py`

 * *Files identical despite different names*


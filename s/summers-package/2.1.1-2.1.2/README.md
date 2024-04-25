# Comparing `tmp/summers_package-2.1.1.tar.gz` & `tmp/summers_package-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summers_package-2.1.1.tar", last modified: Thu Apr 25 10:15:47 2024, max compression
+gzip compressed data, was "summers_package-2.1.2.tar", last modified: Thu Apr 25 15:47:19 2024, max compression
```

## Comparing `summers_package-2.1.1.tar` & `summers_package-2.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 10:15:47.213500 summers_package-2.1.1/
--rw-rw-rw-   0        0        0     1098 2024-04-25 07:54:50.000000 summers_package-2.1.1/License.txt
--rw-rw-rw-   0        0        0      806 2024-04-25 10:15:47.210036 summers_package-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-04-25 08:29:30.000000 summers_package-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 10:15:47.214508 summers_package-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-04-25 10:12:06.000000 summers_package-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:15:47.162191 summers_package-2.1.1/summers_package/
--rw-rw-rw-   0        0        0      114 2024-04-24 19:55:40.000000 summers_package-2.1.1/summers_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:15:47.207032 summers_package-2.1.1/summers_package.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-25 10:15:46.000000 summers_package-2.1.1/summers_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-25 10:15:46.000000 summers_package-2.1.1/summers_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 10:15:46.000000 summers_package-2.1.1/summers_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 10:15:46.000000 summers_package-2.1.1/summers_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 15:47:19.344200 summers_package-2.1.2/
+-rw-rw-rw-   0        0        0     1098 2024-04-25 07:54:50.000000 summers_package-2.1.2/License.txt
+-rw-rw-rw-   0        0        0     1309 2024-04-25 15:47:19.342201 summers_package-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2024-04-25 15:46:05.000000 summers_package-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:47:19.345200 summers_package-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-04-25 15:46:50.000000 summers_package-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:47:19.313202 summers_package-2.1.2/summers_package/
+-rw-rw-rw-   0        0        0      114 2024-04-24 19:55:40.000000 summers_package-2.1.2/summers_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:47:19.340199 summers_package-2.1.2/summers_package.egg-info/
+-rw-rw-rw-   0        0        0     1309 2024-04-25 15:47:19.000000 summers_package-2.1.2/summers_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-04-25 15:47:19.000000 summers_package-2.1.2/summers_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:47:19.000000 summers_package-2.1.2/summers_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 15:47:19.000000 summers_package-2.1.2/summers_package.egg-info/top_level.txt
```

### Comparing `summers_package-2.1.1/License.txt` & `summers_package-2.1.2/License.txt`

 * *Files identical despite different names*

### Comparing `summers_package-2.1.1/setup.py` & `summers_package-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh: 
 	long_description = fh.read() 
 
 setuptools.setup( 
 	name="summers_package", 
 
-	version="2.1.1", 
+	version="2.1.2", 
 
 	author="Ansh Gupta", 
 
 	author_email="Ansh.Gupta@iiitb.ac.in", 
 
 	description="For doing calculations like Addition, Multiplication and Subtraction",
```


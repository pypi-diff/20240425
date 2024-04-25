# Comparing `tmp/turbodinwriter-0.2.1.tar.gz` & `tmp/turbodinwriter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbodinwriter-0.2.1.tar", last modified: Thu Mar  7 23:51:24 2024, max compression
+gzip compressed data, was "turbodinwriter-0.3.1.tar", last modified: Thu Apr 25 17:39:25 2024, max compression
```

## Comparing `turbodinwriter-0.2.1.tar` & `turbodinwriter-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-07 23:51:24.247446 turbodinwriter-0.2.1/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-07 23:22:46.000000 turbodinwriter-0.2.1/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      531 2024-03-07 23:51:24.247273 turbodinwriter-0.2.1/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-07 23:22:46.000000 turbodinwriter-0.2.1/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      599 2024-03-07 23:51:22.000000 turbodinwriter-0.2.1/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-03-07 23:51:24.247481 turbodinwriter-0.2.1/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-07 23:51:24.244834 turbodinwriter-0.2.1/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-07 23:51:24.245525 turbodinwriter-0.2.1/src/turbodinwriter/
--rw-r--r--   0 robertdegen   (501) staff       (20)   224382 2024-03-07 23:22:08.000000 turbodinwriter-0.2.1/src/turbodinwriter/__init__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-07 23:51:24.247105 turbodinwriter-0.2.1/src/turbodinwriter.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      531 2024-03-07 23:51:24.000000 turbodinwriter-0.2.1/src/turbodinwriter.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      272 2024-03-07 23:51:24.000000 turbodinwriter-0.2.1/src/turbodinwriter.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-03-07 23:51:24.000000 turbodinwriter-0.2.1/src/turbodinwriter.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       19 2024-03-07 23:51:24.000000 turbodinwriter-0.2.1/src/turbodinwriter.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       15 2024-03-07 23:51:24.000000 turbodinwriter-0.2.1/src/turbodinwriter.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 17:39:25.615818 turbodinwriter-0.3.1/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-07 23:22:46.000000 turbodinwriter-0.3.1/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      553 2024-04-25 17:39:25.615635 turbodinwriter-0.3.1/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-03-07 23:22:46.000000 turbodinwriter-0.3.1/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      613 2024-04-25 17:39:23.000000 turbodinwriter-0.3.1/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-25 17:39:25.615861 turbodinwriter-0.3.1/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 17:39:25.612060 turbodinwriter-0.3.1/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 17:39:25.612710 turbodinwriter-0.3.1/src/turbodinwriter/
+-rw-r--r--   0 robertdegen   (501) staff       (20)   224382 2024-03-07 23:22:08.000000 turbodinwriter-0.3.1/src/turbodinwriter/__init__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 17:39:25.615451 turbodinwriter-0.3.1/src/turbodinwriter.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      553 2024-04-25 17:39:25.000000 turbodinwriter-0.3.1/src/turbodinwriter.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      272 2024-04-25 17:39:25.000000 turbodinwriter-0.3.1/src/turbodinwriter.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-25 17:39:25.000000 turbodinwriter-0.3.1/src/turbodinwriter.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       26 2024-04-25 17:39:25.000000 turbodinwriter-0.3.1/src/turbodinwriter.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       15 2024-04-25 17:39:25.000000 turbodinwriter-0.3.1/src/turbodinwriter.egg-info/top_level.txt
```

### Comparing `turbodinwriter-0.2.1/PKG-INFO` & `turbodinwriter-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: turbodinwriter
-Version: 0.2.1
+Version: 0.3.1
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: qrcode
 Requires-Dist: reportlab
 Requires-Dist: tabulate
 
 TODO
```

### Comparing `turbodinwriter-0.2.1/pyproject.toml` & `turbodinwriter-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "turbodinwriter"
-version = "0.2.1"
+version = "0.3.1"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "qrcode",
     "reportlab",
     "tabulate"
 ]
 
 [project.urls]
 Homepage = "https://github.com/turbo-bert"
 Issues = "https://github.com/turbo-bert"
```

### Comparing `turbodinwriter-0.2.1/src/turbodinwriter/__init__.py` & `turbodinwriter-0.3.1/src/turbodinwriter/__init__.py`

 * *Files identical despite different names*

### Comparing `turbodinwriter-0.2.1/src/turbodinwriter.egg-info/PKG-INFO` & `turbodinwriter-0.3.1/src/turbodinwriter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: turbodinwriter
-Version: 0.2.1
+Version: 0.3.1
 Summary: A small example package
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert
 Project-URL: Issues, https://github.com/turbo-bert
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: qrcode
 Requires-Dist: reportlab
 Requires-Dist: tabulate
 
 TODO
```


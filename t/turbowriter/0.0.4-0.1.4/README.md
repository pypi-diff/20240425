# Comparing `tmp/turbowriter-0.0.4.tar.gz` & `tmp/turbowriter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbowriter-0.0.4.tar", last modified: Tue Mar 12 18:02:56 2024, max compression
+gzip compressed data, was "turbowriter-0.1.4.tar", last modified: Thu Apr 25 19:46:22 2024, max compression
```

## Comparing `turbowriter-0.0.4.tar` & `turbowriter-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-12 18:02:56.662995 turbowriter-0.0.4/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2023-12-13 18:26:58.000000 turbowriter-0.0.4/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      527 2024-03-12 18:02:56.662825 turbowriter-0.0.4/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2023-12-13 18:26:58.000000 turbowriter-0.0.4/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      595 2024-03-12 18:02:41.000000 turbowriter-0.0.4/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-03-12 18:02:56.663030 turbowriter-0.0.4/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-12 18:02:56.660682 turbowriter-0.0.4/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-12 18:02:56.661381 turbowriter-0.0.4/src/turbowriter/
--rw-r--r--   0 robertdegen   (501) staff       (20)    21457 2024-03-12 18:01:19.000000 turbowriter-0.0.4/src/turbowriter/__init__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-03-12 18:02:56.662654 turbowriter-0.0.4/src/turbowriter.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      527 2024-03-12 18:02:56.000000 turbowriter-0.0.4/src/turbowriter.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      254 2024-03-12 18:02:56.000000 turbowriter-0.0.4/src/turbowriter.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-03-12 18:02:56.000000 turbowriter-0.0.4/src/turbowriter.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       18 2024-03-12 18:02:56.000000 turbowriter-0.0.4/src/turbowriter.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       12 2024-03-12 18:02:56.000000 turbowriter-0.0.4/src/turbowriter.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 19:46:22.722320 turbowriter-0.1.4/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2023-12-13 18:26:58.000000 turbowriter-0.1.4/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      572 2024-04-25 19:46:22.722130 turbowriter-0.1.4/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2023-12-13 18:26:58.000000 turbowriter-0.1.4/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      624 2024-04-25 19:46:20.000000 turbowriter-0.1.4/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-25 19:46:22.722358 turbowriter-0.1.4/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 19:46:22.720117 turbowriter-0.1.4/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 19:46:22.720820 turbowriter-0.1.4/src/turbowriter/
+-rw-r--r--   0 robertdegen   (501) staff       (20)    21457 2024-03-12 18:01:19.000000 turbowriter-0.1.4/src/turbowriter/__init__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-25 19:46:22.721956 turbowriter-0.1.4/src/turbowriter.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      572 2024-04-25 19:46:22.000000 turbowriter-0.1.4/src/turbowriter.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      254 2024-04-25 19:46:22.000000 turbowriter-0.1.4/src/turbowriter.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-25 19:46:22.000000 turbowriter-0.1.4/src/turbowriter.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       33 2024-04-25 19:46:22.000000 turbowriter-0.1.4/src/turbowriter.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       12 2024-04-25 19:46:22.000000 turbowriter-0.1.4/src/turbowriter.egg-info/top_level.txt
```

### Comparing `turbowriter-0.0.4/PKG-INFO` & `turbowriter-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: turbowriter
-Version: 0.0.4
+Version: 0.1.4
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
+Requires-Dist: Pillow
+Requires-Dist: qrcode
 Requires-Dist: reportlab
-Requires-Dist: turboqr
+Requires-Dist: tabulate
 
 TODO
```

### Comparing `turbowriter-0.0.4/pyproject.toml` & `turbowriter-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "turbowriter"
-version = "0.0.4"
+version = "0.1.4"
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
+    "Pillow",
+    "qrcode",
     "reportlab",
-    "turboqr"
+    "tabulate"
 ]
 
 [project.urls]
 Homepage = "https://github.com/turbo-bert"
 Issues = "https://github.com/turbo-bert"
```

### Comparing `turbowriter-0.0.4/src/turbowriter/__init__.py` & `turbowriter-0.1.4/src/turbowriter/__init__.py`

 * *Files identical despite different names*

### Comparing `turbowriter-0.0.4/src/turbowriter.egg-info/PKG-INFO` & `turbowriter-0.1.4/src/turbowriter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: turbowriter
-Version: 0.0.4
+Version: 0.1.4
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
+Requires-Dist: Pillow
+Requires-Dist: qrcode
 Requires-Dist: reportlab
-Requires-Dist: turboqr
+Requires-Dist: tabulate
 
 TODO
```


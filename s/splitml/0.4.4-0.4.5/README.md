# Comparing `tmp/splitml-0.4.4.tar.gz` & `tmp/splitml-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitml-0.4.4.tar", last modified: Mon Mar 18 19:12:09 2024, max compression
+gzip compressed data, was "splitml-0.4.5.tar", last modified: Thu Apr 25 15:01:40 2024, max compression
```

## Comparing `splitml-0.4.4.tar` & `splitml-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:12:09.611626 splitml-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-18 19:12:00.000000 splitml-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-18 19:12:09.611626 splitml-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-18 19:12:00.000000 splitml-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-18 19:12:00.000000 splitml-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 19:12:09.611626 splitml-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:12:09.611626 splitml-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:12:09.611626 splitml-0.4.4/src/splitml/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-18 19:12:00.000000 splitml-0.4.4/src/splitml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-18 19:12:00.000000 splitml-0.4.4/src/splitml/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-18 19:12:00.000000 splitml-0.4.4/src/splitml/groupers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-03-18 19:12:00.000000 splitml-0.4.4/src/splitml/splitml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-18 19:12:00.000000 splitml-0.4.4/src/splitml/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:12:09.611626 splitml-0.4.4/src/splitml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-18 19:12:09.000000 splitml-0.4.4/src/splitml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-18 19:12:09.000000 splitml-0.4.4/src/splitml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:12:09.000000 splitml-0.4.4/src/splitml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-18 19:12:09.000000 splitml-0.4.4/src/splitml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 19:12:09.000000 splitml-0.4.4/src/splitml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.044650 splitml-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 15:01:31.000000 splitml-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-25 15:01:40.044650 splitml-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-25 15:01:31.000000 splitml-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 15:01:31.000000 splitml-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:01:40.044650 splitml-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.040650 splitml-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.040650 splitml-0.4.5/src/splitml/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/groupers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/html_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/splitml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 15:01:31.000000 splitml-0.4.5/src/splitml/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:40.044650 splitml-0.4.5/src/splitml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:01:40.000000 splitml-0.4.5/src/splitml.egg-info/top_level.txt
```

### Comparing `splitml-0.4.4/LICENSE` & `splitml-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `splitml-0.4.4/PKG-INFO` & `splitml-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.4.4
+Version: 0.4.5
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `splitml-0.4.4/README.md` & `splitml-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `splitml-0.4.4/pyproject.toml` & `splitml-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "splitml"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
     { name="Hansimov" },
 ]
 description = "Split Markup Language (HTML and Markdown) to Groups and Nodes"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `splitml-0.4.4/src/splitml/constants.py` & `splitml-0.4.5/src/splitml/constants.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.4/src/splitml/groupers.py` & `splitml-0.4.5/src/splitml/groupers.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.4/src/splitml/stats.py` & `splitml-0.4.5/src/splitml/stats.py`

 * *Files identical despite different names*

### Comparing `splitml-0.4.4/src/splitml.egg-info/PKG-INFO` & `splitml-0.4.5/src/splitml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitml
-Version: 0.4.4
+Version: 0.4.5
 Summary: Split Markup Language (HTML and Markdown) to Groups and Nodes
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/splitml
 Project-URL: Issues, https://github.com/Hansimov/splitml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


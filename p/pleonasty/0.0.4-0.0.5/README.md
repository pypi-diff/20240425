# Comparing `tmp/pleonasty-0.0.4.tar.gz` & `tmp/pleonasty-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pleonasty-0.0.4.tar", last modified: Fri Mar 29 00:32:18 2024, max compression
+gzip compressed data, was "pleonasty-0.0.5.tar", last modified: Thu Apr 25 19:23:07 2024, max compression
```

## Comparing `pleonasty-0.0.4.tar` & `pleonasty-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 00:32:18.767248 pleonasty-0.0.4/
--rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1385 2024-03-29 00:32:18.767248 pleonasty-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.4/README.MD
--rw-rw-rw-   0        0        0      830 2024-03-29 00:30:05.000000 pleonasty-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 00:32:18.767248 pleonasty-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 00:32:18.761314 pleonasty-0.0.4/src/
--rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:32:18.766246 pleonasty-0.0.4/src/pleonasty.egg-info/
--rw-rw-rw-   0        0        0     1385 2024-03-29 00:32:18.000000 pleonasty-0.0.4/src/pleonasty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-03-29 00:32:18.000000 pleonasty-0.0.4/src/pleonasty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 00:32:18.000000 pleonasty-0.0.4/src/pleonasty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-03-29 00:32:18.000000 pleonasty-0.0.4/src/pleonasty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-29 00:32:18.000000 pleonasty-0.0.4/src/pleonasty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14614 2024-03-29 00:30:39.000000 pleonasty-0.0.4/src/pleonasty.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:23:07.203661 pleonasty-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1385 2024-04-25 19:23:07.202661 pleonasty-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.5/README.MD
+-rw-rw-rw-   0        0        0      830 2024-04-25 19:22:09.000000 pleonasty-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 19:23:07.204659 pleonasty-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 19:23:07.166143 pleonasty-0.0.5/src/
+-rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:23:07.196658 pleonasty-0.0.5/src/pleonasty.egg-info/
+-rw-rw-rw-   0        0        0     1385 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-25 19:23:07.000000 pleonasty-0.0.5/src/pleonasty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14643 2024-04-25 19:21:42.000000 pleonasty-0.0.5/src/pleonasty.py
```

### Comparing `pleonasty-0.0.4/LICENSE` & `pleonasty-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.4/PKG-INFO` & `pleonasty-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.4/README.MD` & `pleonasty-0.0.5/README.MD`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.4/pyproject.toml` & `pleonasty-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 
 name = "pleonasty"
 
-version = "0.0.4"
+version = "0.0.5"
 
 authors = [
   { name="Ryan L. Boyd", email="ryan@ryanboyd.io" },
 ]
 
 description = "A very simple abstraction for LLMs to get single responses to a given input."
```

### Comparing `pleonasty-0.0.4/src/pleonasty.egg-info/PKG-INFO` & `pleonasty-0.0.5/src/pleonasty.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.4/src/pleonasty.py` & `pleonasty-0.0.5/src/pleonasty.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,16 @@
                                  start_time=start_time,
                                  stop_time=stop_time)
 
         return
 
     def batch_analyze_to_csv(self,
                              texts: list,
-                             text_metadata: dict,
-                             csv_output_location: str,
+                             text_metadata: dict = {},
+                             csv_output_location: str = "AnalysisResults.csv",
                              append_to_existing_csv: bool = False,
                              output_encoding: str = "utf-8-sig",
                              max_seq_length: int = 4096,
                              temperature: float = 0.3,
                              top_k: int = 10,
                              ) -> None:
```


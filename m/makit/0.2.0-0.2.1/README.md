# Comparing `tmp/makit-0.2.0.tar.gz` & `tmp/makit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makit-0.2.0.tar", last modified: Tue Apr 23 13:15:48 2024, max compression
+gzip compressed data, was "makit-0.2.1.tar", last modified: Thu Apr 25 14:59:59 2024, max compression
```

## Comparing `makit-0.2.0.tar` & `makit-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 13:15:48.626664 makit-0.2.0/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2024-04-23 09:01:38.000000 makit-0.2.0/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       36 2024-04-23 09:05:36.000000 makit-0.2.0/MANIFEST.in
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-23 13:15:48.626664 makit-0.2.0/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      494 2024-04-23 10:54:16.000000 makit-0.2.0/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 13:15:48.626664 makit-0.2.0/makeit/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       50 2024-04-23 09:07:05.000000 makit-0.2.0/makeit/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       68 2024-04-23 09:07:11.000000 makit-0.2.0/makeit/__main__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      540 2024-04-23 13:14:19.000000 makit-0.2.0/makeit/main.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1700 2024-04-23 13:14:47.000000 makit-0.2.0/makeit/make.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 09:05:06.000000 makit-0.2.0/makeit/py.typed
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2916 2024-04-23 13:11:27.000000 makit-0.2.0/makeit/tui.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2024-04-23 13:14:55.000000 makit-0.2.0/makeit/version.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 13:15:48.626664 makit-0.2.0/makit.egg-info/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-23 13:15:48.000000 makit-0.2.0/makit.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      362 2024-04-23 13:15:48.000000 makit-0.2.0/makit.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2024-04-23 13:15:48.000000 makit-0.2.0/makit.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       69 2024-04-23 13:15:48.000000 makit-0.2.0/makit.egg-info/entry_points.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-23 13:15:48.000000 makit-0.2.0/makit.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        7 2024-04-23 13:15:48.000000 makit-0.2.0/makit.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      822 2024-04-23 13:14:59.000000 makit-0.2.0/pyproject.toml
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-23 09:02:06.000000 makit-0.2.0/requirements.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 13:15:48.626664 makit-0.2.0/setup.cfg
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 09:04:45.000000 makit-0.2.0/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-25 14:59:59.060247 makit-0.2.1/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2024-04-23 09:01:38.000000 makit-0.2.1/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       36 2024-04-23 09:05:36.000000 makit-0.2.1/MANIFEST.in
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-25 14:59:59.060247 makit-0.2.1/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      494 2024-04-23 10:54:16.000000 makit-0.2.1/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-25 14:59:59.060247 makit-0.2.1/makeit/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       50 2024-04-23 09:07:05.000000 makit-0.2.1/makeit/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       68 2024-04-23 09:07:11.000000 makit-0.2.1/makeit/__main__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      540 2024-04-23 13:14:19.000000 makit-0.2.1/makeit/main.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1773 2024-04-25 13:17:26.000000 makit-0.2.1/makeit/make.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 09:05:06.000000 makit-0.2.1/makeit/py.typed
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2916 2024-04-23 13:11:27.000000 makit-0.2.1/makeit/tui.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2024-04-25 14:59:26.000000 makit-0.2.1/makeit/version.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-25 14:59:59.060247 makit-0.2.1/makit.egg-info/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-25 14:59:59.000000 makit-0.2.1/makit.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      362 2024-04-25 14:59:59.000000 makit-0.2.1/makit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2024-04-25 14:59:59.000000 makit-0.2.1/makit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       69 2024-04-25 14:59:59.000000 makit-0.2.1/makit.egg-info/entry_points.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-25 14:59:59.000000 makit-0.2.1/makit.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        7 2024-04-25 14:59:59.000000 makit-0.2.1/makit.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      822 2024-04-25 14:59:28.000000 makit-0.2.1/pyproject.toml
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-23 09:02:06.000000 makit-0.2.1/requirements.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-25 14:59:59.060247 makit-0.2.1/setup.cfg
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 09:04:45.000000 makit-0.2.1/setup.py
```

### Comparing `makit-0.2.0/LICENSE` & `makit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makit-0.2.0/PKG-INFO` & `makit-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interactive Makefile step picker
 Author-email: igrek51 <igrek51.dev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/igrek51/makeit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: makit Version: 0.2.0 Summary: Interactive Makefile
+Metadata-Version: 2.1 Name: makit Version: 0.2.1 Summary: Interactive Makefile
 step picker Author-email: igrek51
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/igrek51/
 makeit Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual==0.57.1 # Makeit
 **makeit** is an interactive Makefile runner.
```

### Comparing `makit-0.2.0/makeit/main.py` & `makit-0.2.1/makeit/main.py`

 * *Files identical despite different names*

### Comparing `makit-0.2.0/makeit/make.py` & `makit-0.2.1/makeit/make.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,22 @@
     assert makefile_path.is_file(), "'Makefile' not found"
     lines: list[str] = makefile_path.read_text(encoding='utf-8').splitlines()
     lines = [l for l in lines if l]
     return _parse_makefile_lines(lines)
 
 
 def _parse_makefile_lines(lines: list[str]) -> list[MakeStep]:
-    step_header_regex = re.compile(r'^(\w+):( .+)?$')
-    step_code_regex = re.compile(r'^(\t|\s+)(.+)')
+    step_header_regex = re.compile(r'^([a-zA-Z0-9_\-\.]+):( .+)?$')
+    step_code_regex = re.compile(r'^(\s+)(.+)')
     steps: list[MakeStep] = []
     current_step: MakeStep | None = None
     for i, line in enumerate(lines):
         if match := step_header_regex.match(line):
+            if line.startswith('.'):
+                continue
             dependencies = (match.group(2) or '').strip()
             current_step = MakeStep(
                 name=match.group(1),
                 dependencies=dependencies if dependencies else None,
                 code=[],
                 raw_lines=[line],
                 comment=None,
```

### Comparing `makit-0.2.0/makeit/tui.py` & `makit-0.2.1/makeit/tui.py`

 * *Files identical despite different names*

### Comparing `makit-0.2.0/makit.egg-info/PKG-INFO` & `makit-0.2.1/makit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interactive Makefile step picker
 Author-email: igrek51 <igrek51.dev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/igrek51/makeit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: makit Version: 0.2.0 Summary: Interactive Makefile
+Metadata-Version: 2.1 Name: makit Version: 0.2.1 Summary: Interactive Makefile
 step picker Author-email: igrek51
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/igrek51/
 makeit Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual==0.57.1 # Makeit
 **makeit** is an interactive Makefile runner.
```

### Comparing `makit-0.2.0/pyproject.toml` & `makit-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "makit"
-version = "0.2.0"  # also in makeit/version.py
+version = "0.2.1"  # also in makeit/version.py
 description = "Interactive Makefile step picker"
 license = {text = "MIT"}
 authors = [
     { name = "igrek51", email = "igrek51.dev@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```


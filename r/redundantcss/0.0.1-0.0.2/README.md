# Comparing `tmp/redundantcss-0.0.1.tar.gz` & `tmp/redundantcss-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "redundantcss-0.0.2.tar", last modified: Thu Apr 25 01:37:29 2024, max compression
```

## Comparing `redundantcss-0.0.1.tar` & `redundantcss-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redundantcss-0.0.1/redundantcss/__init__.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 redundantcss-0.0.1/redundantcss/redundantcss.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 redundantcss-0.0.1/redundantcss/validateArgs.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 redundantcss-0.0.1/LICENSE
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 redundantcss-0.0.1/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 redundantcss-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 redundantcss-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 01:37:29.578086 redundantcss-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2024-04-24 22:32:51.000000 redundantcss-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1957 2024-04-25 01:37:29.577088 redundantcss-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1330 2024-04-25 00:40:00.000000 redundantcss-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 01:37:29.559072 redundantcss-0.0.2/redundantcss/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:32:51.000000 redundantcss-0.0.2/redundantcss/__init__.py
+-rw-rw-rw-   0        0        0     4583 2024-04-25 00:40:24.000000 redundantcss-0.0.2/redundantcss/redundantcss.py
+-rw-rw-rw-   0        0        0      705 2024-04-24 22:32:51.000000 redundantcss-0.0.2/redundantcss/validateArgs.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:37:29.576095 redundantcss-0.0.2/redundantcss.egg-info/
+-rw-rw-rw-   0        0        0     1957 2024-04-25 01:37:29.000000 redundantcss-0.0.2/redundantcss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-25 01:37:29.000000 redundantcss-0.0.2/redundantcss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 01:37:29.000000 redundantcss-0.0.2/redundantcss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-25 01:37:29.000000 redundantcss-0.0.2/redundantcss.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-25 01:37:29.000000 redundantcss-0.0.2/redundantcss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-25 01:37:29.000000 redundantcss-0.0.2/redundantcss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 01:37:29.579085 redundantcss-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2024-04-25 00:39:52.000000 redundantcss-0.0.2/setup.py
```

### Comparing `redundantcss-0.0.1/redundantcss/redundantcss.py` & `redundantcss-0.0.2/redundantcss/redundantcss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import sys
 from pathlib import Path
 import os
 
-from validateArgs import parse_classes, check_folder_contents
+from redundantcss.validateArgs import parse_classes, check_folder_contents
 
 def main():
     usage = """
 USAGE: python redundantcss.py 'stylesheet_path' 'template_path_or_template_paths'
 
 Description:
   This script analyzes a stylesheet and identifies redundant CSS rules not used by the templates provided.
```

### Comparing `redundantcss-0.0.1/redundantcss/validateArgs.py` & `redundantcss-0.0.2/redundantcss/validateArgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from bs4 import BeautifulSoup
 
 def parse_classes(html_sheet):
     classes = set()
     content = html_sheet.read()
     soup = BeautifulSoup(content, 'html.parser')
     elements_with_class = soup.find_all(class_=True)
```

### Comparing `redundantcss-0.0.1/LICENSE` & `redundantcss-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redundantcss-0.0.1/README.md` & `redundantcss-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # RedundantCSS
-#### Video Demo: Coming soon
 
 ### **Contents:**
 - [Description](#description)
 - [Installation](#installation)
 - [Usage](#usage)
 
 ## **Description:**
 This script analyzes a stylesheet and identifies redundant CSS classes not used by the templates provided. The script prints the names of all unused classes to the terminal, at which point you can go to the stylesheet and delete unused classes.
 <br>
 
 **COMING IN V2:** Remove the manual aspect of removing the CSS and give user the option for this process to be done automatically.
 <hr>
 
 ## **Installation:**
-**COMING SOON**
+    pip install redundantcss
 
 <hr>
 
 ## **Usage:**
-    python3 redundantcss.py 'stylesheet_path' 'template_path_or_template_paths'
+    redundantcss 'stylesheet_path' 'template_path_or_template_paths'
+
+or
+
+    redundantcss 'stylesheet_path' 'template_path_or_template_paths'
 
 Arguments:
   - 'stylesheet_path': Path to the CSS stylesheet to be analyzed.
   - 'template_path_or_template_paths': Path to a folder containing HTML templates or paths to individual template files.
 
 Examples:
   1. Analyze a single template:
```


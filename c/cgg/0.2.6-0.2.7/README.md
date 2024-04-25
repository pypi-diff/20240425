# Comparing `tmp/cgg-0.2.6.tar.gz` & `tmp/cgg-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgg-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cgg-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cgg-0.2.6.tar` & `cgg-0.2.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.6/LICENSE
--rw-r--r--   0        0        0     3972 2024-04-19 05:24:13.254176 cgg-0.2.6/README.md
--rw-r--r--   0        0        0      742 2024-04-19 05:29:39.720815 cgg-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5186 2024-04-19 05:14:14.191290 cgg-0.2.6/src/cgg/__init__.py
--rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 cgg-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4066 2024-04-25 00:36:15.159266 cgg-0.2.7/README.md
+-rw-r--r--   0        0        0      742 2024-04-25 00:32:11.783810 cgg-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5490 2024-04-25 00:31:01.107926 cgg-0.2.7/src/cgg/__init__.py
+-rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 cgg-0.2.7/PKG-INFO
```

### Comparing `cgg-0.2.6/LICENSE` & `cgg-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cgg-0.2.6/README.md` & `cgg-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -116,13 +116,20 @@
 ```
 cgg vc
 ```
 Or by (recognizor p):
 ```
 cgg vp
 ```
-
+Or by (online recognizor c):
+```
+cgg oc
+```
+Or by (online recognizor p):
+```
+cgg op
+```
 #### website
 Click [gguf.us](https://gguf.us) or launch it straight from console by:
 ```
 cgg us
 ```
```

### Comparing `cgg-0.2.6/pyproject.toml` & `cgg-0.2.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "cgg"
 authors = [{name = "calcuis", email = "info@calcu.io"}]
 description = "cgg is a short form of call gguf model/file; cgg is a cmd-based app built on gguf-connector, which allows users interacting with large language model (i.e., chatgpt) via a simple command without coding a long long syntax"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version"]
-dependencies = ["gguf-connector >=0.7.28"]
+dependencies = ["gguf-connector >=0.7.31"]
 
 [project.urls]
 Homepage = "https://github.com/calcuis/cgg"
 Issues = "https://github.com/calcuis/cgg/issues"
 
 [project.scripts]
 cgg = "cgg.__init__:__init__"
```

### Comparing `cgg-0.2.6/src/cgg/__init__.py` & `cgg-0.2.7/src/cgg/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # !/usr/bin/env python3
 
-__version__="0.2.6"
+__version__="0.2.7"
 
 import argparse, json, os.path, urllib.request
 from rich.progress import Progress
 # rich (refined) ###########################################################################
 def get_file_size(url):
     with urllib.request.urlopen(url) as response:
         size = int(response.headers['Content-Length'])
@@ -73,14 +73,16 @@
     subparsers.add_parser('gpp', help='gpp connector')
     subparsers.add_parser('c', help='c connector')
     subparsers.add_parser('g', help='g connector')
     subparsers.add_parser('r', help='metadata reader')
     subparsers.add_parser('s', help='sample GGUF list (internet required)')
     subparsers.add_parser('pc', help='pdf analyzor c')
     subparsers.add_parser('pp', help='pdf analyzor p')
+    subparsers.add_parser('oc', help='wav recognizor c (internet required)')
+    subparsers.add_parser('op', help='wav recognizor p (internet required)')
     subparsers.add_parser('vc', help='wav recognizor c')
     subparsers.add_parser('vp', help='wav recognizor p')
     subparsers.add_parser('us', help='launch to gguf.us')
     args = parser.parse_args()
     # if statement below
     if args.subcommand == 'clone':
         clone_file(args.url)
@@ -91,14 +93,18 @@
         print("Please select a GGUF file to download:")
         extract_names(json_data)
         handle_user_input(json_data)
     elif args.subcommand == 'us':
         from gguf_connector import w
     elif args.subcommand == 'r':
         from gguf_connector import r
+    elif args.subcommand == 'oc':
+        from gguf_connector import cg
+    elif args.subcommand == 'op':
+        from gguf_connector import pg
     elif args.subcommand == 'vc':
         from gguf_connector import cs
     elif args.subcommand == 'vp':
         from gguf_connector import ps
     elif args.subcommand == 'pc':
         from gguf_connector import cp
     elif args.subcommand == 'pp':
```

### Comparing `cgg-0.2.6/PKG-INFO` & `cgg-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cgg
-Version: 0.2.6
+Version: 0.2.7
 Summary: cgg is a short form of call gguf model/file; cgg is a cmd-based app built on gguf-connector, which allows users interacting with large language model (i.e., chatgpt) via a simple command without coding a long long syntax
 Author-email: calcuis <info@calcu.io>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: gguf-connector >=0.7.28
+Requires-Dist: gguf-connector >=0.7.31
 Project-URL: Homepage, https://github.com/calcuis/cgg
 Project-URL: Issues, https://github.com/calcuis/cgg/issues
 
 ### GGUF caller
 
 [<img src="https://raw.githubusercontent.com/calcuis/cgg/master/cgg.gif" width="128" height="128">](https://github.com/calcuis/cgg)
 [![Static Badge](https://img.shields.io/badge/cgg-release-blue?logo=github)](https://github.com/calcuis/cgg/releases)
@@ -127,13 +127,20 @@
 ```
 cgg vc
 ```
 Or by (recognizor p):
 ```
 cgg vp
 ```
-
+Or by (online recognizor c):
+```
+cgg oc
+```
+Or by (online recognizor p):
+```
+cgg op
+```
 #### website
 Click [gguf.us](https://gguf.us) or launch it straight from console by:
 ```
 cgg us
 ```
```


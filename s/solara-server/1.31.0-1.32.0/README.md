# Comparing `tmp/solara_server-1.31.0.tar.gz` & `tmp/solara_server-1.32.0.tar.gz`

## Comparing `solara_server-1.31.0.tar` & `solara_server-1.32.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 solara_server-1.31.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_server-1.31.0/LICENSE
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_server-1.31.0/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solara_server-1.31.0/pyproject.toml
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 solara_server-1.31.0/PKG-INFO
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 solara_server-1.32.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 solara_server-1.32.0/LICENSE
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 solara_server-1.32.0/README.md
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solara_server-1.32.0/pyproject.toml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 solara_server-1.32.0/PKG-INFO
```

### Comparing `solara_server-1.31.0/.gitignore` & `solara_server-1.32.0/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -78,12 +78,12 @@
 
 # output file from the docs
 build/
 
 ./tmp
 ./examples
 node_modules
-packages/assets/cdn
-packages/assets/dist/*
+packages/solara-assets/cdn
+packages/solara-assets/dist/*
 
 solara-env
 states
```

### Comparing `solara_server-1.31.0/LICENSE` & `solara_server-1.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solara_server-1.31.0/pyproject.toml` & `solara_server-1.32.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "solara-server"
 readme = "README.md"
 authors = [{name = "Maarten A. Breddels", email = "maartenbreddels@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "1.31.0"
+version = "1.32.0"
 dynamic = ["description"]
 dependencies = [
     "solara-ui",
     "jinja2",
     "click>=7.1.0",
     "rich_click",
     "filelock",
```

### Comparing `solara_server-1.31.0/PKG-INFO` & `solara_server-1.32.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solara-server
-Version: 1.31.0
+Version: 1.32.0
 Dynamic: Summary
 Project-URL: Home, https://www.github.com/widgetti/solara
 Project-URL: Documentation, https://solara.dev
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Maarten A. Breddels
```


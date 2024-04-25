# Comparing `tmp/dir2prompt-1.0.7.tar.gz` & `tmp/dir2prompt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dir2prompt-1.0.7.tar", last modified: Thu Apr 25 17:14:06 2024, max compression
+gzip compressed data, was "dir2prompt-1.0.8.tar", last modified: Thu Apr 25 18:49:59 2024, max compression
```

## Comparing `dir2prompt-1.0.7.tar` & `dir2prompt-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 17:14:06.295281 dir2prompt-1.0.7/
--rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.7/LICENSE
--rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 17:14:06.295062 dir2prompt-1.0.7/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 15:53:20.000000 dir2prompt-1.0.7/README.md
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 17:14:06.294823 dir2prompt-1.0.7/dir2prompt.egg-info/
--rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 17:14:06.000000 dir2prompt-1.0.7/dir2prompt.egg-info/PKG-INFO
--rw-r--r--   0 mkieffer   (501) staff       (20)      248 2024-04-25 17:14:06.000000 dir2prompt-1.0.7/dir2prompt.egg-info/SOURCES.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 17:14:06.000000 dir2prompt-1.0.7/dir2prompt.egg-info/dependency_links.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)       37 2024-04-25 17:14:06.000000 dir2prompt-1.0.7/dir2prompt.egg-info/entry_points.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)        4 2024-04-25 17:14:06.000000 dir2prompt-1.0.7/dir2prompt.egg-info/top_level.txt
--rw-r--r--   0 mkieffer   (501) staff       (20)     1250 2024-04-25 17:13:56.000000 dir2prompt-1.0.7/pyproject.toml
--rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 17:14:06.295333 dir2prompt-1.0.7/setup.cfg
-drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 17:14:06.294432 dir2prompt-1.0.7/src/
--rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:25.000000 dir2prompt-1.0.7/src/__init__.py
--rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.7/src/config.json
--rw-r--r--   0 mkieffer   (501) staff       (20)     7916 2024-04-25 16:39:29.000000 dir2prompt-1.0.7/src/d2p.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 18:49:59.735705 dir2prompt-1.0.8/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1069 2024-04-02 23:08:45.000000 dir2prompt-1.0.8/LICENSE
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 18:49:59.735471 dir2prompt-1.0.8/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)     4322 2024-04-25 15:53:20.000000 dir2prompt-1.0.8/README.md
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 18:49:59.734146 dir2prompt-1.0.8/dir2prompt/
+-rw-r--r--   0 mkieffer   (501) staff       (20)        0 2024-04-25 16:44:25.000000 dir2prompt-1.0.8/dir2prompt/__init__.py
+-rw-r--r--   0 mkieffer   (501) staff       (20)      978 2024-04-02 23:57:47.000000 dir2prompt-1.0.8/dir2prompt/config.json
+-rw-r--r--   0 mkieffer   (501) staff       (20)     7923 2024-04-25 18:46:36.000000 dir2prompt-1.0.8/dir2prompt/d2p.py
+drwxr-xr-x   0 mkieffer   (501) staff       (20)        0 2024-04-25 18:49:59.735175 dir2prompt-1.0.8/dir2prompt.egg-info/
+-rw-r--r--   0 mkieffer   (501) staff       (20)     6550 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/PKG-INFO
+-rw-r--r--   0 mkieffer   (501) staff       (20)      269 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)        1 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       44 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/entry_points.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)       11 2024-04-25 18:49:59.000000 dir2prompt-1.0.8/dir2prompt.egg-info/top_level.txt
+-rw-r--r--   0 mkieffer   (501) staff       (20)     1271 2024-04-25 17:32:20.000000 dir2prompt-1.0.8/pyproject.toml
+-rw-r--r--   0 mkieffer   (501) staff       (20)       38 2024-04-25 18:49:59.735753 dir2prompt-1.0.8/setup.cfg
```

### Comparing `dir2prompt-1.0.7/LICENSE` & `dir2prompt-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.7/PKG-INFO` & `dir2prompt-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dir2prompt-1.0.7/README.md` & `dir2prompt-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.7/dir2prompt.egg-info/PKG-INFO` & `dir2prompt-1.0.8/dir2prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dir2prompt
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate prompts for long-context LLMs using the content in your directory
 Author-email: Max Kieffer <wkieffer@ufl.edu>
 License: MIT License
         
         Copyright (c) 2024 mkieffer1107
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dir2prompt-1.0.7/pyproject.toml` & `dir2prompt-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dir2prompt"
-version = "1.0.7"
+version = "1.0.8"
 license = {file = "LICENSE"}
 authors = [
   { name="Max Kieffer", email="wkieffer@ufl.edu" },
 ]
 description = "Generate prompts for long-context LLMs using the content in your directory"
 readme = "README.md"
 requires-python = ">=3.6"
@@ -35,12 +35,12 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/mkieffer1107/dir2prompt"
 Issues = "https://github.com/mkieffer1107/dir2prompt/issues"
 
 [tool.setuptools]
-packages = ["src"]
-package-data = {"src" = ["config.json"]}
+packages = ["dir2prompt"]
+package-data = {"dir2prompt" = ["config.json"]}
 
 [project.scripts]
-d2p = "src.d2p:main"
+d2p = "dir2prompt.d2p:main"
```

### Comparing `dir2prompt-1.0.7/src/config.json` & `dir2prompt-1.0.8/dir2prompt/config.json`

 * *Files identical despite different names*

### Comparing `dir2prompt-1.0.7/src/d2p.py` & `dir2prompt-1.0.8/dir2prompt/d2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             dir_name = os.path.basename(os.getcwd()) 
         else:
             dir_name = os.path.basename(args.dir)
         args.outfile = f"{dir_name}_prompt"
 
     # set the default config file path 
     if args.config is None:
-        args.config = str(files("src").joinpath("config.json"))
+        args.config = str(files("dir2prompt").joinpath("config.json"))
     return args
 
 
 def main():
     args = parse_options()
 
     config = load_config(args.config)
```


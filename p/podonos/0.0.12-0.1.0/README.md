# Comparing `tmp/podonos-0.0.12.tar.gz` & `tmp/podonos-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podonos-0.0.12.tar", last modified: Sun Apr 14 08:40:48 2024, max compression
+gzip compressed data, was "podonos-0.1.0.tar", last modified: Thu Apr 25 06:46:38 2024, max compression
```

## Comparing `podonos-0.0.12.tar` & `podonos-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-14 08:40:48.002005 podonos-0.0.12/
--rw-r--r--   0 soohyun    (501) staff       (20)     1063 2024-04-14 07:16:47.000000 podonos-0.0.12/LICENSE
--rw-r--r--   0 soohyun    (501) staff       (20)     3130 2024-04-14 08:40:48.001822 podonos-0.0.12/PKG-INFO
--rw-r--r--   0 soohyun    (501) staff       (20)      997 2024-04-14 07:16:47.000000 podonos-0.0.12/README.md
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-14 08:40:48.000635 podonos-0.0.12/podonos/
--rw-r--r--   0 soohyun    (501) staff       (20)       82 2024-04-14 08:18:03.000000 podonos-0.0.12/podonos/__init__.py
--rw-r--r--   0 soohyun    (501) staff       (20)    18924 2024-04-14 08:36:02.000000 podonos-0.0.12/podonos/sdk.py
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-14 08:40:48.001631 podonos-0.0.12/podonos.egg-info/
--rw-r--r--   0 soohyun    (501) staff       (20)     3130 2024-04-14 08:40:47.000000 podonos-0.0.12/podonos.egg-info/PKG-INFO
--rw-r--r--   0 soohyun    (501) staff       (20)      221 2024-04-14 08:40:47.000000 podonos-0.0.12/podonos.egg-info/SOURCES.txt
--rw-r--r--   0 soohyun    (501) staff       (20)        1 2024-04-14 08:40:47.000000 podonos-0.0.12/podonos.egg-info/dependency_links.txt
--rw-r--r--   0 soohyun    (501) staff       (20)       19 2024-04-14 08:40:47.000000 podonos-0.0.12/podonos.egg-info/requires.txt
--rw-r--r--   0 soohyun    (501) staff       (20)        8 2024-04-14 08:40:47.000000 podonos-0.0.12/podonos.egg-info/top_level.txt
--rw-r--r--   0 soohyun    (501) staff       (20)      975 2024-04-14 08:17:57.000000 podonos-0.0.12/pyproject.toml
--rw-r--r--   0 soohyun    (501) staff       (20)       38 2024-04-14 08:40:48.002041 podonos-0.0.12/setup.cfg
+drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-25 06:46:38.959521 podonos-0.1.0/
+-rw-r--r--   0 soohyun    (501) staff       (20)     1063 2024-04-14 07:16:47.000000 podonos-0.1.0/LICENSE
+-rw-r--r--   0 soohyun    (501) staff       (20)     3129 2024-04-25 06:46:38.959299 podonos-0.1.0/PKG-INFO
+-rw-r--r--   0 soohyun    (501) staff       (20)      997 2024-04-14 07:16:47.000000 podonos-0.1.0/README.md
+drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-25 06:46:38.957934 podonos-0.1.0/podonos/
+-rw-r--r--   0 soohyun    (501) staff       (20)       81 2024-04-25 05:35:37.000000 podonos-0.1.0/podonos/__init__.py
+-rw-r--r--   0 soohyun    (501) staff       (20)     1980 2024-04-23 03:57:37.000000 podonos-0.1.0/podonos/audio_meta.py
+-rw-r--r--   0 soohyun    (501) staff       (20)      398 2024-04-25 06:32:35.000000 podonos-0.1.0/podonos/constant.py
+-rw-r--r--   0 soohyun    (501) staff       (20)      118 2024-04-22 06:38:27.000000 podonos-0.1.0/podonos/default_config.py
+-rw-r--r--   0 soohyun    (501) staff       (20)      210 2024-04-22 06:38:27.000000 podonos-0.1.0/podonos/eval_name.py
+-rw-r--r--   0 soohyun    (501) staff       (20)     9955 2024-04-23 07:35:47.000000 podonos-0.1.0/podonos/evaluator.py
+-rw-r--r--   0 soohyun    (501) staff       (20)     7242 2024-04-25 06:29:56.000000 podonos-0.1.0/podonos/sdk.py
+-rw-r--r--   0 soohyun    (501) staff       (20)     2398 2024-04-25 06:31:21.000000 podonos-0.1.0/podonos/version.py
+drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-25 06:46:38.959077 podonos-0.1.0/podonos.egg-info/
+-rw-r--r--   0 soohyun    (501) staff       (20)     3129 2024-04-25 06:46:38.000000 podonos-0.1.0/podonos.egg-info/PKG-INFO
+-rw-r--r--   0 soohyun    (501) staff       (20)      368 2024-04-25 06:46:38.000000 podonos-0.1.0/podonos.egg-info/SOURCES.txt
+-rw-r--r--   0 soohyun    (501) staff       (20)        1 2024-04-25 06:46:38.000000 podonos-0.1.0/podonos.egg-info/dependency_links.txt
+-rw-r--r--   0 soohyun    (501) staff       (20)       19 2024-04-25 06:46:38.000000 podonos-0.1.0/podonos.egg-info/requires.txt
+-rw-r--r--   0 soohyun    (501) staff       (20)        8 2024-04-25 06:46:38.000000 podonos-0.1.0/podonos.egg-info/top_level.txt
+-rw-r--r--   0 soohyun    (501) staff       (20)      974 2024-04-25 06:38:37.000000 podonos-0.1.0/pyproject.toml
+-rw-r--r--   0 soohyun    (501) staff       (20)       38 2024-04-25 06:46:38.959565 podonos-0.1.0/setup.cfg
+drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-25 06:46:38.958848 podonos-0.1.0/tests/
+-rw-r--r--   0 soohyun    (501) staff       (20)     3589 2024-04-22 06:38:27.000000 podonos-0.1.0/tests/test_sdk.py
```

### Comparing `podonos-0.0.12/LICENSE` & `podonos-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podonos-0.0.12/PKG-INFO` & `podonos-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podonos
-Version: 0.0.12
+Version: 0.1.0
 Summary: Managed evaluation for audio & speech
 Author-email: Soohyun Bae <sb@podonos.com>
 License: MIT License
         
         Copyright (c) 2024 Podonos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `podonos-0.0.12/README.md` & `podonos-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `podonos-0.0.12/podonos.egg-info/PKG-INFO` & `podonos-0.1.0/podonos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podonos
-Version: 0.0.12
+Version: 0.1.0
 Summary: Managed evaluation for audio & speech
 Author-email: Soohyun Bae <sb@podonos.com>
 License: MIT License
         
         Copyright (c) 2024 Podonos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `podonos-0.0.12/pyproject.toml` & `podonos-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "podonos"
-version = "0.0.12"
+version = "0.1.0"
 description = "Managed evaluation for audio & speech"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     {name = "Soohyun Bae", email = "sb@podonos.com"}
 ]
 requires-python = ">=3.8"
```


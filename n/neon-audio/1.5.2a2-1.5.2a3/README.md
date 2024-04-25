# Comparing `tmp/neon-audio-1.5.2a2.tar.gz` & `tmp/neon-audio-1.5.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-audio-1.5.2a2.tar", last modified: Tue Mar 12 19:15:15 2024, max compression
+gzip compressed data, was "neon-audio-1.5.2a3.tar", last modified: Thu Apr 25 16:29:46 2024, max compression
```

## Comparing `neon-audio-1.5.2a2.tar` & `neon-audio-1.5.2a3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:15:15.634476 neon-audio-1.5.2a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-12 19:15:15.634476 neon-audio-1.5.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:15:15.630476 neon-audio-1.5.2a2/neon_audio/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:15:15.630476 neon-audio-1.5.2a2/neon_audio/tts/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/tts/neon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/neon_audio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:15:15.630476 neon-audio-1.5.2a2/neon_audio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:15:15.000000 neon-audio-1.5.2a2/neon_audio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 19:15:15.634476 neon-audio-1.5.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:15:15.630476 neon-audio-1.5.2a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/tests/api_method_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:15:15.630476 neon-audio-1.5.2a2/tests/test_objects/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/tests/test_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-03-12 19:15:11.000000 neon-audio-1.5.2a2/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:46.580854 neon-audio-1.5.2a3/neon_audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/neon_audio/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/tts/neon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/neon_audio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/neon_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:46.000000 neon-audio-1.5.2a3/neon_audio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/tests/api_method_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:46.584854 neon-audio-1.5.2a3/tests/test_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/tests/test_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-25 16:29:42.000000 neon-audio-1.5.2a3/tests/unit_tests.py
```

### Comparing `neon-audio-1.5.2a2/LICENSE.md` & `neon-audio-1.5.2a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/PKG-INFO` & `neon-audio-1.5.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.5.2a2
+Version: 1.5.2a3
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.5.2a2/README.md` & `neon-audio-1.5.2a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/__init__.py` & `neon-audio-1.5.2a3/neon_audio/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/__main__.py` & `neon-audio-1.5.2a3/neon_audio/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/cli.py` & `neon-audio-1.5.2a3/neon_audio/cli.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/service.py` & `neon-audio-1.5.2a3/neon_audio/service.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/tts/__init__.py` & `neon-audio-1.5.2a3/neon_audio/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/tts/neon.py` & `neon-audio-1.5.2a3/neon_audio/tts/neon.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio/utils.py` & `neon-audio-1.5.2a3/neon_audio/utils.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/neon_audio.egg-info/PKG-INFO` & `neon-audio-1.5.2a3/neon_audio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.5.2a2
+Version: 1.5.2a3
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.5.2a2/neon_audio.egg-info/SOURCES.txt` & `neon-audio-1.5.2a3/neon_audio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/setup.py` & `neon-audio-1.5.2a3/setup.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/tests/__init__.py` & `neon-audio-1.5.2a3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/tests/api_method_tests.py` & `neon-audio-1.5.2a3/tests/api_method_tests.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/tests/test_objects/__init__.py` & `neon-audio-1.5.2a3/tests/test_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a2/tests/unit_tests.py` & `neon-audio-1.5.2a3/tests/unit_tests.py`

 * *Files identical despite different names*


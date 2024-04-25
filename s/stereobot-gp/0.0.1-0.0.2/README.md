# Comparing `tmp/stereobot_gp-0.0.1.tar.gz` & `tmp/stereobot_gp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stereobot_gp-0.0.1.tar", last modified: Thu Apr 25 04:21:00 2024, max compression
+gzip compressed data, was "stereobot_gp-0.0.2.tar", last modified: Thu Apr 25 11:05:25 2024, max compression
```

## Comparing `stereobot_gp-0.0.1.tar` & `stereobot_gp-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 04:21:00.931059 stereobot_gp-0.0.1/
--rw-rw-rw-   0        0        0      562 2024-04-25 04:21:00.930059 stereobot_gp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-04-24 18:15:15.000000 stereobot_gp-0.0.1/README.md
--rw-rw-rw-   0        0        0      612 2024-04-25 04:20:44.000000 stereobot_gp-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 04:21:00.932060 stereobot_gp-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 04:21:00.921059 stereobot_gp-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 04:21:00.925058 stereobot_gp-0.0.1/src/stereo_gp/
--rw-rw-rw-   0        0        0        0 2024-04-24 21:57:38.000000 stereobot_gp-0.0.1/src/stereo_gp/__init__.py
--rw-rw-rw-   0        0        0    16381 2024-04-25 04:16:06.000000 stereobot_gp-0.0.1/src/stereo_gp/stereo_gp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 04:21:00.930059 stereobot_gp-0.0.1/src/stereobot_gp.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-25 04:21:00.000000 stereobot_gp-0.0.1/src/stereobot_gp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-25 04:21:00.000000 stereobot_gp-0.0.1/src/stereobot_gp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 04:21:00.000000 stereobot_gp-0.0.1/src/stereobot_gp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-25 04:21:00.000000 stereobot_gp-0.0.1/src/stereobot_gp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 11:05:25.626405 stereobot_gp-0.0.2/
+-rw-rw-rw-   0        0        0     2391 2024-04-25 11:05:25.625404 stereobot_gp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2024-04-25 10:57:39.000000 stereobot_gp-0.0.2/README.md
+-rw-rw-rw-   0        0        0      612 2024-04-25 11:05:13.000000 stereobot_gp-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 11:05:25.626405 stereobot_gp-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 11:05:25.616402 stereobot_gp-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 11:05:25.619403 stereobot_gp-0.0.2/src/stereo_gp/
+-rw-rw-rw-   0        0        0        0 2024-04-24 21:57:38.000000 stereobot_gp-0.0.2/src/stereo_gp/__init__.py
+-rw-rw-rw-   0        0        0    16589 2024-04-25 10:47:56.000000 stereobot_gp-0.0.2/src/stereo_gp/stereo_gp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:05:25.624405 stereobot_gp-0.0.2/src/stereobot_gp.egg-info/
+-rw-rw-rw-   0        0        0     2391 2024-04-25 11:05:25.000000 stereobot_gp-0.0.2/src/stereobot_gp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-04-25 11:05:25.000000 stereobot_gp-0.0.2/src/stereobot_gp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 11:05:25.000000 stereobot_gp-0.0.2/src/stereobot_gp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 11:05:25.000000 stereobot_gp-0.0.2/src/stereobot_gp.egg-info/top_level.txt
```

### Comparing `stereobot_gp-0.0.1/pyproject.toml` & `stereobot_gp-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stereobot_gp"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Gabriela Pinheiro", email="gpinheiro2812@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stereobot_gp-0.0.1/src/stereo_gp/stereo_gp.py` & `stereobot_gp-0.0.2/src/stereo_gp/stereo_gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import cohere
 import time 
 
 class Classifier:
     def __init__(self, API_KEY, trial_key=False) -> None:
+        """
+        API_KEY: Cohere API Key
+        trial_key: boolean to indicate if the the API Key is a free trial key, if True the ratelimit will be respected by the accuracy evaluation
+        """
+
         self.co = cohere.Client(API_KEY)
         self.trial_key = trial_key
     
     def classify(self, passage) -> str:
         """
         Function that receives a passage to be classified by the Stereobot and returns the generated label.
         """
```


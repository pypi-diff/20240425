# Comparing `tmp/npiai-0.0.2.dev2.tar.gz` & `tmp/npiai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai-0.0.2.dev2.tar", max compression
+gzip compressed data, was "npiai-0.0.3.tar", max compression
```

## Comparing `npiai-0.0.2.dev2.tar` & `npiai-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-18 05:31:48.474805 npiai-0.0.2.dev2/README.md
--rw-r--r--   0        0        0      151 2024-04-20 00:39:52.418936 npiai-0.0.2.dev2/npiai/__init__.py
--rw-r--r--   0        0        0      132 2024-04-20 00:26:15.294019 npiai-0.0.2.dev2/npiai/app/__init__.py
--rw-r--r--   0        0        0      510 2024-04-20 00:09:40.569381 npiai-0.0.2.dev2/npiai/app/google.py
--rw-r--r--   0        0        0     1090 2024-04-20 00:09:40.565760 npiai-0.0.2.dev2/npiai/app/human_feedback.py
--rw-r--r--   0        0        0       57 2024-04-20 00:26:15.289527 npiai-0.0.2.dev2/npiai/core/__init__.py
--rw-r--r--   0        0        0     6106 2024-04-20 00:09:40.560265 npiai-0.0.2.dev2/npiai/core/base.py
--rw-r--r--   0        0        0      371 2024-04-20 01:05:08.872951 npiai-0.0.2.dev2/pyproject.toml
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 npiai-0.0.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 05:31:48.474805 npiai-0.0.3/README.md
+-rw-r--r--   0        0        0      151 2024-04-20 00:39:52.418936 npiai-0.0.3/npiai/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-20 00:26:15.294019 npiai-0.0.3/npiai/app/__init__.py
+-rw-r--r--   0        0        0      282 2024-04-24 22:25:36.766045 npiai-0.0.3/npiai/app/browser.py
+-rw-r--r--   0        0        0      278 2024-04-24 22:20:47.884237 npiai-0.0.3/npiai/app/discord.py
+-rw-r--r--   0        0        0      277 2024-04-24 22:20:06.679823 npiai-0.0.3/npiai/app/github.py
+-rw-r--r--   0        0        0      510 2024-04-20 00:09:40.569381 npiai-0.0.3/npiai/app/google.py
+-rw-r--r--   0        0        0     1064 2024-04-24 22:19:56.249598 npiai-0.0.3/npiai/app/human_feedback.py
+-rw-r--r--   0        0        0      279 2024-04-24 22:20:30.694448 npiai-0.0.3/npiai/app/twitter.py
+-rw-r--r--   0        0        0       57 2024-04-20 00:26:15.289527 npiai-0.0.3/npiai/core/__init__.py
+-rw-r--r--   0        0        0     6106 2024-04-20 00:09:40.560265 npiai-0.0.3/npiai/core/base.py
+-rw-r--r--   0        0        0      312 2024-04-24 22:31:35.055119 npiai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 npiai-0.0.3/PKG-INFO
```

### Comparing `npiai-0.0.2.dev2/npiai/app/human_feedback.py` & `npiai-0.0.3/npiai/app/human_feedback.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from npiai.core.base import App
 from npiai_proto import api_pb2
 
 
 class ConsoleFeedback(App):
 
-    def __init__(self, npi_endpoint: str = None):
+    def __init__(self):
         super().__init__(
             app_name="console_feedback",
             app_type=api_pb2.AppType.APP_UNKNOWN,
         )
 
     def schema(self):
         return {
```

### Comparing `npiai-0.0.2.dev2/npiai/core/base.py` & `npiai-0.0.3/npiai/core/base.py`

 * *Files identical despite different names*


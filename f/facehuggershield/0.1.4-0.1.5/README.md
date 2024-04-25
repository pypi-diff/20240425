# Comparing `tmp/facehuggershield-0.1.4.tar.gz` & `tmp/facehuggershield-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facehuggershield-0.1.4.tar", last modified: Wed Apr 24 02:43:57 2024, max compression
+gzip compressed data, was "facehuggershield-0.1.5.tar", last modified: Thu Apr 25 17:41:07 2024, max compression
```

## Comparing `facehuggershield-0.1.4.tar` & `facehuggershield-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:57.701946 facehuggershield-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:43:51.000000 facehuggershield-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:43:57.701946 facehuggershield-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:43:51.000000 facehuggershield-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:43:57.701946 facehuggershield-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 02:43:51.000000 facehuggershield-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:57.697946 facehuggershield-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:57.701946 facehuggershield-0.1.4/src/facehuggershield/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:51.000000 facehuggershield-0.1.4/src/facehuggershield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 02:43:51.000000 facehuggershield-0.1.4/src/facehuggershield/huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:57.701946 facehuggershield-0.1.4/src/facehuggershield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:43:57.000000 facehuggershield-0.1.4/src/facehuggershield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 02:43:57.000000 facehuggershield-0.1.4/src/facehuggershield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:43:57.000000 facehuggershield-0.1.4/src/facehuggershield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 02:43:57.000000 facehuggershield-0.1.4/src/facehuggershield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 02:43:57.000000 facehuggershield-0.1.4/src/facehuggershield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:41:07.769612 facehuggershield-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-25 17:41:07.769612 facehuggershield-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:41:07.769612 facehuggershield-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:41:07.765612 facehuggershield-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:41:07.769612 facehuggershield-0.1.5/src/facehuggershield/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/src/facehuggershield/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:41:07.769612 facehuggershield-0.1.5/src/facehuggershield/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/src/facehuggershield/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/src/facehuggershield/huggingface/set_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-25 17:41:03.000000 facehuggershield-0.1.5/src/facehuggershield/huggingface/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:41:07.769612 facehuggershield-0.1.5/src/facehuggershield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-25 17:41:07.000000 facehuggershield-0.1.5/src/facehuggershield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 17:41:07.000000 facehuggershield-0.1.5/src/facehuggershield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:41:07.000000 facehuggershield-0.1.5/src/facehuggershield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 17:41:07.000000 facehuggershield-0.1.5/src/facehuggershield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 17:41:07.000000 facehuggershield-0.1.5/src/facehuggershield.egg-info/top_level.txt
```

### Comparing `facehuggershield-0.1.4/LICENSE` & `facehuggershield-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.4/PKG-INFO` & `facehuggershield-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defendatron==0.1.1
+Requires-Dist: defendatron==0.1.3
 
 # Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
```

### Comparing `facehuggershield-0.1.4/README.md` & `facehuggershield-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.4/setup.py` & `facehuggershield-0.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="facehuggershield",
-    version="0.1.4",
+    version="0.1.5",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
     url="https://github.com/Capsize-Games/facehuggershield",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "defendatron==0.1.1",
+        "defendatron==0.1.3",
     ],
     dependency_links=[
     ],
 )
```

### Comparing `facehuggershield-0.1.4/src/facehuggershield/huggingface.py` & `facehuggershield-0.1.5/src/facehuggershield/huggingface/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import defendatron
+from facehuggershield.huggingface.set_environment_variables import set_huggingface_environment_variables
 
 print("Activating facehugger shield...")
-defendatron.activate(
+def activate(
     nullscream_blacklist=[
         "huggingface_hub.commands",
         "huggingface_hub.templates",
         "huggingface_hub._commit_api",
         "huggingface_hub._commit_scheduler",
         "huggingface_hub._infernece_endpoints",
         "huggingface_hub._login",
@@ -22,15 +23,34 @@
         "huggingface_hub.repocard",
         "huggingface_hub.repocard_data",
         "huggingface_hub.utils._gitcredential",
         "huggingface_hub.utils._headers",
         "huggingface_hub.utils._headers",
         "huggingface_hub.utils._telemetry",
         "transformers.utils.hub.PushToHubMixin",
+        "transformers.tools.agents",
     ],
     nullscream_whitelist=[
-        "huggingface_hub.utils",
+        # "huggingface_hub.utils",
+        "transformers.models.whisper",
+        "transformers.models.whisper.modeling_whisper",
+        "transformers.models.whisper",
     ],
+    nullscream_function_blacklist=[],
     activate_shadowlogger=True,
     activate_darklock=True,
     activate_nullscream=True,
-)
+    show_stdout=True
+):
+    set_huggingface_environment_variables(
+        allow_downloads=False,
+
+    )
+    defendatron.activate(
+        nullscream_blacklist=nullscream_blacklist,
+        nullscream_whitelist=nullscream_whitelist,
+        nullscream_function_blacklist=nullscream_function_blacklist,
+        activate_shadowlogger=activate_shadowlogger,
+        activate_darklock=activate_darklock,
+        activate_nullscream=activate_nullscream,
+        show_stdout=show_stdout
+    )
```

### Comparing `facehuggershield-0.1.4/src/facehuggershield.egg-info/PKG-INFO` & `facehuggershield-0.1.5/src/facehuggershield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defendatron==0.1.1
+Requires-Dist: defendatron==0.1.3
 
 # Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
```


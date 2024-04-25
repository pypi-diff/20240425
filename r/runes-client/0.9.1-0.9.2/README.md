# Comparing `tmp/runes-client-0.9.1.tar.gz` & `tmp/runes-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-client-0.9.1.tar", last modified: Thu Apr 18 00:03:54 2024, max compression
+gzip compressed data, was "runes-client-0.9.2.tar", last modified: Thu Apr 25 00:36:14 2024, max compression
```

## Comparing `runes-client-0.9.1.tar` & `runes-client-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.008017 runes-client-0.9.1/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.9.1/LICENSE.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)     7947 2024-04-18 00:03:54.007737 runes-client-0.9.1/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)     7408 2024-04-17 23:56:47.000000 runes-client-0.9.1/README.md
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.004276 runes-client-0.9.1/runes_client/
--rw-r--r--   0 stevehiehn   (501) staff       (20)      663 2024-04-12 18:49:27.000000 runes-client-0.9.1/runes_client/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    10334 2024-04-12 04:09:34.000000 runes-client-0.9.1/runes_client/api_client.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.9.1/runes_client/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    38952 2024-04-12 19:19:52.000000 runes-client-0.9.1/runes_client/core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/decorators.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/dn_tracer.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/file_uploader.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.005526 runes-client-0.9.1/runes_client/output/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/output/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6818 2024-04-08 05:37:47.000000 runes-client-0.9.1/runes_client/output/results_handler.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.006211 runes-client-0.9.1/runes_client/utils/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/utils/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/utils/audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.9.1/runes_client/utils/file_type_classifier.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.007512 runes-client-0.9.1/runes_client.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     7947 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-18 00:03:53.000000 runes-client-0.9.1/runes_client.egg-info/top_level.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-18 00:03:54.008063 runes-client-0.9.1/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-18 00:00:22.000000 runes-client-0.9.1/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-18 00:03:54.007286 runes-client-0.9.1/tests/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.9.1/tests/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.9.1/tests/test_audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.9.1/tests/test_core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.9.1/tests/test_registration.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.9.1/tests/test_results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 00:36:14.563538 runes-client-0.9.2/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.9.2/LICENSE.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7974 2024-04-25 00:36:14.563325 runes-client-0.9.2/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7426 2024-04-18 17:41:49.000000 runes-client-0.9.2/README.md
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 00:36:14.559170 runes-client-0.9.2/runes_client/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      663 2024-04-12 18:49:27.000000 runes-client-0.9.2/runes_client/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    10334 2024-04-12 04:09:34.000000 runes-client-0.9.2/runes_client/api_client.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.9.2/runes_client/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    38952 2024-04-12 19:19:52.000000 runes-client-0.9.2/runes_client/core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.9.2/runes_client/decorators.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.9.2/runes_client/dn_tracer.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.9.2/runes_client/file_uploader.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 00:36:14.560613 runes-client-0.9.2/runes_client/output/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.9.2/runes_client/output/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-04-25 00:34:32.000000 runes-client-0.9.2/runes_client/output/results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 00:36:14.561346 runes-client-0.9.2/runes_client/utils/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.9.2/runes_client/utils/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.9.2/runes_client/utils/audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      654 2024-04-25 00:34:47.000000 runes-client-0.9.2/runes_client/utils/file_type_classifier.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 00:36:14.562819 runes-client-0.9.2/runes_client.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     7974 2024-04-25 00:36:14.000000 runes-client-0.9.2/runes_client.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-25 00:36:14.000000 runes-client-0.9.2/runes_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-25 00:36:14.000000 runes-client-0.9.2/runes_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-25 00:36:14.000000 runes-client-0.9.2/runes_client.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-25 00:36:14.000000 runes-client-0.9.2/runes_client.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-25 00:36:14.000000 runes-client-0.9.2/runes_client.egg-info/top_level.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-25 00:36:14.563580 runes-client-0.9.2/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1565 2024-04-25 00:32:14.000000 runes-client-0.9.2/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-25 00:36:14.562496 runes-client-0.9.2/tests/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.9.2/tests/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.9.2/tests/test_audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.9.2/tests/test_core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.9.2/tests/test_registration.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.9.2/tests/test_results_handler.py
```

### Comparing `runes-client-0.9.1/LICENSE.md` & `runes-client-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/PKG-INFO` & `runes-client-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
-Home-page: https://dawnet.tools
+Home-page: https://signalsandsorcery.app
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: aiohttp
 Requires-Dist: websockets
@@ -44,15 +44,15 @@
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
 This is a simple example of a RUNES script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the SignalsAndSorceryAPI server.  The script then connects to the SignalsAndSorceryAPI server and waits for a plugin to interact with it. 
 
-For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
+For thorough documentation and tutorials visit: [https://signalsandsorcery.com/client/](https://signalsandsorcery.com/client/)
 
 ```python
 import runes_client.core as runes 
 from runes_client import RunesFilePath, ui_param
 
 # The token generated by the Crucible plugin.  
 # The token is used by the discovery server.  It associates the RUNE with the plugin.
```

### Comparing `runes-client-0.9.1/README.md` & `runes-client-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
 This is a simple example of a RUNES script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the SignalsAndSorceryAPI server.  The script then connects to the SignalsAndSorceryAPI server and waits for a plugin to interact with it. 
 
-For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
+For thorough documentation and tutorials visit: [https://signalsandsorcery.com/client/](https://signalsandsorcery.com/client/)
 
 ```python
 import runes_client.core as runes 
 from runes_client import RunesFilePath, ui_param
 
 # The token generated by the Crucible plugin.  
 # The token is used by the discovery server.  It associates the RUNE with the plugin.
```

### Comparing `runes-client-0.9.1/runes_client/__init__.py` & `runes-client-0.9.2/runes_client/__init__.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client/api_client.py` & `runes-client-0.9.2/runes_client/api_client.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client/config.py` & `runes-client-0.9.2/runes_client/config.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client/core.py` & `runes-client-0.9.2/runes_client/core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client/dn_tracer.py` & `runes-client-0.9.2/runes_client/dn_tracer.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client/file_uploader.py` & `runes-client-0.9.2/runes_client/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client/output/results_handler.py` & `runes-client-0.9.2/runes_client/output/results_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,18 @@
                         DNTag.DNMsg.value: str(e),
                     },
                 )
                 await self.add_error(str(e))
 
         elif input_type == "midi":
             converted_file_path = file_path
+        elif input_type == "image":
+            converted_file_path = file_path
+        else:
+            converted_file_path = file_path
 
         try:
             file_url = await self.file_uploader.upload(
                 converted_file_path, os.path.splitext(converted_file_path)[1][1:]
             )
 
             self.files.append(
```

### Comparing `runes-client-0.9.1/runes_client/utils/audio_utils.py` & `runes-client-0.9.2/runes_client/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/runes_client.egg-info/PKG-INFO` & `runes-client-0.9.2/runes_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
-Home-page: https://dawnet.tools
+Home-page: https://signalsandsorcery.app
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: aiohttp
 Requires-Dist: websockets
@@ -44,15 +44,15 @@
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
 This is a simple example of a RUNES script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the SignalsAndSorceryAPI server.  The script then connects to the SignalsAndSorceryAPI server and waits for a plugin to interact with it. 
 
-For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
+For thorough documentation and tutorials visit: [https://signalsandsorcery.com/client/](https://signalsandsorcery.com/client/)
 
 ```python
 import runes_client.core as runes 
 from runes_client import RunesFilePath, ui_param
 
 # The token generated by the Crucible plugin.  
 # The token is used by the discovery server.  It associates the RUNE with the plugin.
```

### Comparing `runes-client-0.9.1/runes_client.egg-info/SOURCES.txt` & `runes-client-0.9.2/runes_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/setup.py` & `runes-client-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 if not is_ffmpeg_installed():
     print(ffmpeg_warning_msg)
 
 setup(
     name="runes-client",
-    version="0.9.1",
+    version="0.9.2",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "websockets",
         "nest-asyncio",
         "sentry-sdk",
         "pydub",
@@ -49,9 +49,9 @@
     },
     # Additional metadata about your package
     author="Steve Hiehn",
     author_email="stevehiehn@gmail.com",
     description="Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://dawnet.tools",
+    url="https://signalsandsorcery.app",
 )
```

### Comparing `runes-client-0.9.1/tests/test_audio_utils.py` & `runes-client-0.9.2/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/tests/test_core.py` & `runes-client-0.9.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/tests/test_registration.py` & `runes-client-0.9.2/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.9.1/tests/test_results_handler.py` & `runes-client-0.9.2/tests/test_results_handler.py`

 * *Files identical despite different names*


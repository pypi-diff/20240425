# Comparing `tmp/pyutube-1.2.3.tar.gz` & `tmp/pyutube-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutube-1.2.3.tar", last modified: Thu Apr 25 10:05:13 2024, max compression
+gzip compressed data, was "pyutube-1.2.4.tar", last modified: Thu Apr 25 10:08:32 2024, max compression
```

## Comparing `pyutube-1.2.3.tar` & `pyutube-1.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.821809 pyutube-1.2.3/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.3/LICENSE.md
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 10:05:13.820541 pyutube-1.2.3/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-04-25 10:05:06.000000 pyutube-1.2.3/README.md
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.792628 pyutube-1.2.3/pyutube/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.3/pyutube/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.3/pyutube/__main__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-25 10:00:48.000000 pyutube-1.2.3/pyutube/cli.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14053 2024-04-25 09:45:49.000000 pyutube-1.2.3/pyutube/downloader.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.816728 pyutube-1.2.3/pyutube/tests/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.3/pyutube/tests/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.3/pyutube/tests/test_utils.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11318 2024-04-25 10:04:41.000000 pyutube-1.2.3/pyutube/utils.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.818966 pyutube-1.2.3/pyutube.egg-info/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/SOURCES.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/dependency_links.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/entry_points.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/requires.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/top_level.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-25 10:05:13.821973 pyutube-1.2.3/setup.cfg
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.3/setup.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:08:32.164840 pyutube-1.2.4/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.4/LICENSE.md
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 10:08:32.163629 pyutube-1.2.4/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-04-25 10:08:25.000000 pyutube-1.2.4/README.md
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:08:32.146509 pyutube-1.2.4/pyutube/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.4/pyutube/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.4/pyutube/__main__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-25 10:00:48.000000 pyutube-1.2.4/pyutube/cli.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14053 2024-04-25 09:45:49.000000 pyutube-1.2.4/pyutube/downloader.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:08:32.158718 pyutube-1.2.4/pyutube/tests/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.4/pyutube/tests/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.4/pyutube/tests/test_utils.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11218 2024-04-25 10:07:48.000000 pyutube-1.2.4/pyutube/utils.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:08:32.161847 pyutube-1.2.4/pyutube.egg-info/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 10:08:31.000000 pyutube-1.2.4/pyutube.egg-info/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-25 10:08:32.000000 pyutube-1.2.4/pyutube.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-25 10:08:31.000000 pyutube-1.2.4/pyutube.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-25 10:08:31.000000 pyutube-1.2.4/pyutube.egg-info/entry_points.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-25 10:08:31.000000 pyutube-1.2.4/pyutube.egg-info/requires.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-25 10:08:31.000000 pyutube-1.2.4/pyutube.egg-info/top_level.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-25 10:08:32.165001 pyutube-1.2.4/setup.cfg
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.4/setup.py
```

### Comparing `pyutube-1.2.3/LICENSE.md` & `pyutube-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.3/PKG-INFO` & `pyutube-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.3
+Version: 1.2.4
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
 Keywords: youtube,download,cli,pyutube,pytube
 Platform: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.3 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.4 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
 youtube,download,cli,pyutube,pytube Platform: Windows Platform: MacOS Platform:
 Linux Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `pyutube-1.2.3/README.md` & `pyutube-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.3/pyutube/cli.py` & `pyutube-1.2.4/pyutube/cli.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.3/pyutube/downloader.py` & `pyutube-1.2.4/pyutube/downloader.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.3/pyutube/tests/test_utils.py` & `pyutube-1.2.4/pyutube/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.3/pyutube/utils.py` & `pyutube-1.2.4/pyutube/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,26 @@
 import sys
 import re
 import os
 from datetime import timedelta
 
 import inquirer
 import requests
-import requests_cache
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from rich.console import Console
 from rich.theme import Theme
 from termcolor import colored
 
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __app__ = "pyutube"
 ABORTED_PREFIX = "aborted"
 CANCEL_PREFIX = "cancel"
 
-requests_cache.install_cache('update_cache', expire_after=timedelta(days=2))
-
 
 # Set up the console
 custom_theme = Theme({
     "info": "#64b0f2",
     "warning": "color(3)",
     "danger": "red",
     "success": "green",
```

### Comparing `pyutube-1.2.3/pyutube.egg-info/PKG-INFO` & `pyutube-1.2.4/pyutube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.3
+Version: 1.2.4
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
 Keywords: youtube,download,cli,pyutube,pytube
 Platform: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.3 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.4 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
 youtube,download,cli,pyutube,pytube Platform: Windows Platform: MacOS Platform:
 Linux Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `pyutube-1.2.3/setup.py` & `pyutube-1.2.4/setup.py`

 * *Files identical despite different names*


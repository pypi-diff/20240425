# Comparing `tmp/helios-client-0.3.20230805.post1.tar.gz` & `tmp/helios-client-0.4.20240424.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-client-0.3.20230805.post1.tar", last modified: Sun Aug  6 02:55:26 2023, max compression
+gzip compressed data, was "helios-client-0.4.20240424.post1.tar", last modified: Thu Apr 25 05:37:15 2024, max compression
```

## Comparing `helios-client-0.3.20230805.post1.tar` & `helios-client-0.4.20240424.post1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.361819 helios-client-0.3.20230805.post1/
--rw-rw-r--   0 kip       (1000) kip       (1000)     7652 2017-09-30 07:16:26.000000 helios-client-0.3.20230805.post1/Copying
--rw-rw-r--   0 kip       (1000) kip       (1000)       30 2019-05-23 01:39:54.000000 helios-client-0.3.20230805.post1/MANIFEST.in
--rw-rw-r--   0 kip       (1000) kip       (1000)     5676 2023-08-06 02:55:26.365819 helios-client-0.3.20230805.post1/PKG-INFO
--rw-rw-r--   0 kip       (1000) kip       (1000)     4165 2023-07-18 20:24:57.000000 helios-client-0.3.20230805.post1/README.md
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.361819 helios-client-0.3.20230805.post1/Source/
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.361819 helios-client-0.3.20230805.post1/Source/helios/
--rw-rw-r--   0 kip       (1000) kip       (1000)      228 2023-08-05 00:02:44.000000 helios-client-0.3.20230805.post1/Source/helios/__init__.py
--rw-rw-r--   0 kip       (1000) kip       (1000)      221 2023-08-06 01:58:51.000000 helios-client-0.3.20230805.post1/Source/helios/__version__.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     1457 2022-06-03 01:39:49.000000 helios-client-0.3.20230805.post1/Source/helios/chunked_upload.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)    42621 2023-08-06 02:44:26.000000 helios-client-0.3.20230805.post1/Source/helios/client.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3437 2022-06-03 01:39:58.000000 helios-client-0.3.20230805.post1/Source/helios/exceptions.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     4190 2023-07-31 01:31:52.000000 helios-client-0.3.20230805.post1/Source/helios/requests.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)    12909 2023-08-06 02:40:19.000000 helios-client-0.3.20230805.post1/Source/helios/responses.py
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.361819 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/
--rw-rw-r--   0 kip       (1000) kip       (1000)     5676 2023-08-06 02:55:26.000000 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/PKG-INFO
--rw-rw-r--   0 kip       (1000) kip       (1000)      727 2023-08-06 02:55:26.000000 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/SOURCES.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        1 2023-08-06 02:55:26.000000 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/dependency_links.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)       66 2023-08-06 02:55:26.000000 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/requires.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        7 2023-08-06 02:55:26.000000 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/top_level.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        1 2023-08-06 02:55:26.000000 helios-client-0.3.20230805.post1/Source/helios_client.egg-info/zip-safe
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.361819 helios-client-0.3.20230805.post1/debian/
--rw-rw-r--   0 kip       (1000) kip       (1000)      188 2023-08-06 01:59:20.000000 helios-client-0.3.20230805.post1/debian/changelog
--rw-rw-r--   0 kip       (1000) kip       (1000)     1129 2023-08-04 00:06:27.000000 helios-client-0.3.20230805.post1/debian/control
--rw-rw-r--   0 kip       (1000) kip       (1000)      391 2023-07-29 05:45:31.000000 helios-client-0.3.20230805.post1/debian/copyright
--rw-rw-r--   0 kip       (1000) kip       (1000)       11 2019-05-15 03:31:30.000000 helios-client-0.3.20230805.post1/debian/docs
--rwxr-xr-x   0 kip       (1000) kip       (1000)     3238 2022-06-03 01:41:05.000000 helios-client-0.3.20230805.post1/debian/rules
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.361819 helios-client-0.3.20230805.post1/debian/source/
--rw-rw-r--   0 kip       (1000) kip       (1000)       12 2015-01-02 04:54:06.000000 helios-client-0.3.20230805.post1/debian/source/format
--rw-rw-r--   0 kip       (1000) kip       (1000)       63 2019-09-16 23:53:59.000000 helios-client-0.3.20230805.post1/debian/source/options
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-08-06 02:55:26.365819 helios-client-0.3.20230805.post1/debian/tests/
--rw-------   0 kip       (1000) kip       (1000)      834 2023-07-31 02:21:26.000000 helios-client-0.3.20230805.post1/debian/tests/control
--rwx--x--x   0 kip       (1000) kip       (1000)      417 2023-07-31 01:48:32.000000 helios-client-0.3.20230805.post1/debian/tests/test-import-module.py
--rwx--x--x   0 kip       (1000) kip       (1000)     3388 2023-08-06 02:51:30.000000 helios-client-0.3.20230805.post1/debian/tests/test-module-usage.py
--rw-rw-r--   0 kip       (1000) kip       (1000)      213 2019-05-22 05:29:11.000000 helios-client-0.3.20230805.post1/debian/watch
--rw-rw-r--   0 kip       (1000) kip       (1000)       38 2023-08-06 02:55:26.365819 helios-client-0.3.20230805.post1/setup.cfg
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3310 2023-08-04 00:06:16.000000 helios-client-0.3.20230805.post1/setup.py
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/
+-rw-rw-r--   0 kip       (1000) kip       (1000)     7652 2017-09-30 07:16:26.000000 helios-client-0.4.20240424.post1/Copying
+-rw-rw-r--   0 kip       (1000) kip       (1000)       30 2019-05-23 01:39:54.000000 helios-client-0.4.20240424.post1/MANIFEST.in
+-rw-rw-r--   0 kip       (1000) kip       (1000)     5833 2024-04-25 05:37:15.127819 helios-client-0.4.20240424.post1/PKG-INFO
+-rw-rw-r--   0 kip       (1000) kip       (1000)     4342 2024-03-15 02:16:20.000000 helios-client-0.4.20240424.post1/README.md
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.119819 helios-client-0.4.20240424.post1/Source/
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/Source/helios/
+-rw-rw-r--   0 kip       (1000) kip       (1000)      228 2024-03-15 02:17:25.000000 helios-client-0.4.20240424.post1/Source/helios/__init__.py
+-rw-rw-r--   0 kip       (1000) kip       (1000)      221 2024-04-25 03:28:50.000000 helios-client-0.4.20240424.post1/Source/helios/__version__.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     1457 2024-03-15 02:17:14.000000 helios-client-0.4.20240424.post1/Source/helios/chunked_upload.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)    48195 2024-04-24 01:44:58.000000 helios-client-0.4.20240424.post1/Source/helios/client.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3437 2024-03-15 02:17:21.000000 helios-client-0.4.20240424.post1/Source/helios/exceptions.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     4937 2024-04-23 01:51:01.000000 helios-client-0.4.20240424.post1/Source/helios/requests.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)    12931 2024-04-17 01:46:47.000000 helios-client-0.4.20240424.post1/Source/helios/responses.py
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/
+-rw-rw-r--   0 kip       (1000) kip       (1000)     5833 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/PKG-INFO
+-rw-rw-r--   0 kip       (1000) kip       (1000)      752 2024-04-25 05:37:15.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        1 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)       92 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/requires.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        7 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/top_level.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        1 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/zip-safe
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/debian/
+-rw-rw-r--   0 kip       (1000) kip       (1000)      189 2024-04-25 04:43:34.000000 helios-client-0.4.20240424.post1/debian/changelog
+-rw-rw-r--   0 kip       (1000) kip       (1000)     1174 2024-04-25 05:28:12.000000 helios-client-0.4.20240424.post1/debian/control
+-rw-rw-r--   0 kip       (1000) kip       (1000)      377 2024-04-25 04:44:12.000000 helios-client-0.4.20240424.post1/debian/copyright
+-rw-rw-r--   0 kip       (1000) kip       (1000)       11 2019-05-15 03:31:30.000000 helios-client-0.4.20240424.post1/debian/docs
+-rw-rw-r--   0 kip       (1000) kip       (1000)      130 2024-04-25 05:27:55.000000 helios-client-0.4.20240424.post1/debian/lintian-overrides
+-rwxr-xr-x   0 kip       (1000) kip       (1000)     3238 2024-03-15 02:16:39.000000 helios-client-0.4.20240424.post1/debian/rules
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/debian/source/
+-rw-rw-r--   0 kip       (1000) kip       (1000)       12 2015-01-02 04:54:06.000000 helios-client-0.4.20240424.post1/debian/source/format
+-rw-rw-r--   0 kip       (1000) kip       (1000)       63 2019-09-16 23:53:59.000000 helios-client-0.4.20240424.post1/debian/source/options
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.127819 helios-client-0.4.20240424.post1/debian/tests/
+-rw-------   0 kip       (1000) kip       (1000)      834 2024-03-15 01:22:53.000000 helios-client-0.4.20240424.post1/debian/tests/control
+-rwx--x--x   0 kip       (1000) kip       (1000)      417 2024-03-15 01:09:49.000000 helios-client-0.4.20240424.post1/debian/tests/test-import-module.py
+-rwx--x--x   0 kip       (1000) kip       (1000)     3768 2024-04-23 02:00:12.000000 helios-client-0.4.20240424.post1/debian/tests/test-module-usage.py
+-rw-rw-r--   0 kip       (1000) kip       (1000)      214 2024-04-25 04:41:51.000000 helios-client-0.4.20240424.post1/debian/watch
+-rw-rw-r--   0 kip       (1000) kip       (1000)       38 2024-04-25 05:37:15.127819 helios-client-0.4.20240424.post1/setup.cfg
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3358 2024-04-07 02:31:28.000000 helios-client-0.4.20240424.post1/setup.py
```

### Comparing `helios-client-0.3.20230805.post1/Copying` & `helios-client-0.4.20240424.post1/Copying`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20230805.post1/PKG-INFO` & `helios-client-0.4.20240424.post1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: helios-client
-Version: 0.3.20230805.post1
+Version: 0.4.20240424.post1
 Summary: Pure python 3 module to communicate with a Helios server.
 Home-page: https://www.heliosmusic.io
 Author: Cartesian Theatre
 Author-email: kip@heliosmusic.io
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/cartesiantheatre/python-helios-client/issues
 Project-URL: Documentation, https://heliosmusic.io/api.html
 Project-URL: Source Code, https://github.com/cartesiantheatre/python-helios-client
 Keywords: music,similarity,match,catalogue,digital,signal,processing,machine,learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -59,27 +58,28 @@
 There are countless other examples, but let's talk about the first one. Nearly always, your client approaches you with samples already in hand. "Hey, do you have anything like this?" This could be an MP3 or a YouTube video URL. Because Helios allows you to search the catalogue using music itself as the search key, you could use the customer's samples directly to help them find what they're looking for.
 
 Traditionally, in the absence of such technology, the way this has been done for decades may surprise many. It is both costly and involves many hours or even days of manual human labour which delays the business process. The business must manually search, usually using [textual tags](https://heliosmusic.io/index.php/faq#tagging), and listen to a great deal of irrelevant music in the hopes of finding the one the client is actually willing to spend money on.
 
 ## Quick installation
 
 ### Ubuntu
-Packages already prepared for Ubuntu 22.04 (jammy) and later are available on our Personal Package Archive (PPA) [here](https://launchpad.net/%7Ekip/+archive/ubuntu/helios-public). To get the package installed and be up and running in seconds, just run the following two commands:
+Packages already prepared for Ubuntu 23.10 (mantic) and later are available on our Personal Package Archive (PPA) [here](https://launchpad.net/%7Ekip/+archive/ubuntu/helios-public). To get the package installed and be up and running in seconds, just run the following two commands:
 
 ```console
 $ sudo add-apt-repository ppa:kip/helios-public
 $ sudo apt install python3-helios-client
 ```
 
 ### PyPi
-If you are not using Ubuntu 22.04 or later and know what you are doing, you can use Python's ad hoc package manaement system. This is not recommended as a first choice because it is not as robust as a native package manager.
+If you are not using Ubuntu 23.10 or later and know what you are doing, you can use Python's ad hoc package management system. This is not recommended as a first choice because it is not as robust as a native package manager. But if you do choose to use `pip(1)` directly, you can always use it in a virtual environment.
 
 ```console
+$ python -m venv Environment
+$ source Environment/bin/activate
+$ cd Environment
 $ pip install helios-client
 ```
 
 ## Licensing
 
-This Python module is released under the terms of the [LGPL 3.0](https://www.gnu.org/licenses/lgpl-3.0.html) or greater. Copyright (C) 2015-2023 Cartesian Theatre. See [Copying](./Copying) for more information.
-
-
+This Python module is released under the terms of the [LGPL 3.0](https://www.gnu.org/licenses/lgpl-3.0.html) or greater. Copyright (C) 2015-2024 Cartesian Theatre. See [Copying](./Copying) for more information.
```

### Comparing `helios-client-0.3.20230805.post1/README.md` & `helios-client-0.4.20240424.post1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,25 +27,28 @@
 There are countless other examples, but let's talk about the first one. Nearly always, your client approaches you with samples already in hand. "Hey, do you have anything like this?" This could be an MP3 or a YouTube video URL. Because Helios allows you to search the catalogue using music itself as the search key, you could use the customer's samples directly to help them find what they're looking for.
 
 Traditionally, in the absence of such technology, the way this has been done for decades may surprise many. It is both costly and involves many hours or even days of manual human labour which delays the business process. The business must manually search, usually using [textual tags](https://heliosmusic.io/index.php/faq#tagging), and listen to a great deal of irrelevant music in the hopes of finding the one the client is actually willing to spend money on.
 
 ## Quick installation
 
 ### Ubuntu
-Packages already prepared for Ubuntu 22.04 (jammy) and later are available on our Personal Package Archive (PPA) [here](https://launchpad.net/%7Ekip/+archive/ubuntu/helios-public). To get the package installed and be up and running in seconds, just run the following two commands:
+Packages already prepared for Ubuntu 23.10 (mantic) and later are available on our Personal Package Archive (PPA) [here](https://launchpad.net/%7Ekip/+archive/ubuntu/helios-public). To get the package installed and be up and running in seconds, just run the following two commands:
 
 ```console
 $ sudo add-apt-repository ppa:kip/helios-public
 $ sudo apt install python3-helios-client
 ```
 
 ### PyPi
-If you are not using Ubuntu 22.04 or later and know what you are doing, you can use Python's ad hoc package manaement system. This is not recommended as a first choice because it is not as robust as a native package manager.
+If you are not using Ubuntu 23.10 or later and know what you are doing, you can use Python's ad hoc package management system. This is not recommended as a first choice because it is not as robust as a native package manager. But if you do choose to use `pip(1)` directly, you can always use it in a virtual environment.
 
 ```console
+$ python -m venv Environment
+$ source Environment/bin/activate
+$ cd Environment
 $ pip install helios-client
 ```
 
 ## Licensing
 
-This Python module is released under the terms of the [LGPL 3.0](https://www.gnu.org/licenses/lgpl-3.0.html) or greater. Copyright (C) 2015-2023 Cartesian Theatre. See [Copying](./Copying) for more information.
+This Python module is released under the terms of the [LGPL 3.0](https://www.gnu.org/licenses/lgpl-3.0.html) or greater. Copyright (C) 2015-2024 Cartesian Theatre. See [Copying](./Copying) for more information.
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios/chunked_upload.py` & `helios-client-0.4.20240424.post1/Source/helios/chunked_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2022 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # i18n...
 import gettext
 _ = gettext.gettext
 
 # Chunked upload class to allow file upload progress with Requests library...
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios/client.py` & `helios-client-0.4.20240424.post1/Source/helios/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #!/usr/bin/python3
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2023 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # Other imports...
 import json
 import marshmallow
 import os
 import simplejson
 from tqdm import tqdm
 import urllib3
 import re
 import requests
+from requests.adapters import HTTPAdapter, Retry
+from requests_toolbelt.utils import user_agent as ua
 import shutil
 import tempfile
 import helios
 from helios import __version__
 from helios.chunked_upload import chunked_upload
 import time
 
 # i18n...
 import gettext
 _ = gettext.gettext
 
 # Class to handle all client communication with a Helios server...
-class client:
+class Client:
 
     # Class attribute for JSON MIME type...
     _json_mime_type     = 'application/json'
 
     # Class attribute for compressed encoding...
     _accept_encoding    = 'br, gzip, deflate'
 
@@ -54,31 +56,45 @@
         self._tls               = tls
         self._tls_ca_file       = tls_ca_file
         self._tls_certificate   = tls_certificate
         self._tls_key           = tls_key
         self._verbose           = verbose
         self._version           = version
 
+        # Prepare a Retry object that will tell our HTTP adapter to retry a
+        #  total number of three times and wait one second in between...
+        retries = Retry(total=3, backoff_factor=1.0)
+
         # Construct an adaptor to automatically make three retry attempts on
         #  failed DNS lookups and connection timeouts...
-        self._adapter = requests.adapters.HTTPAdapter()   # Set constructor to max_retries=3 for three retries
+        self._adapter = HTTPAdapter(max_retries=retries)
         self._session.mount('http://', self._adapter)
         self._session.mount('https://', self._adapter)
 
         # Make sure host provided...
         if host is None:
             raise Exception(_('No host provided.'))
 
         # Make sure port provided...
         if port is None:
             raise Exception(_('No port provided.'))
 
+        # Configure a user agent builder...
+        user_agent = ua.UserAgentBuilder(
+            name='helios-python',
+            version=get_version())
+        user_agent.include_system()
+
+        # Build a user agent string from the builder...
+        user_agent_string = user_agent.build()
+
         # Initialize headers common to all queries...
-        self._common_headers                = {}
-        self._common_headers['User-Agent']  = F'helios-python {get_version()}'
+        self._common_headers                    = {}
+        self._common_headers['Accept-Encoding'] = 'identity'
+        self._common_headers['User-Agent']      = user_agent_string
 
         # If an API key was provided by user, add it to request headers...
         if api_key is not None:
             self._common_headers['X-API-Key']   = self._api_key
 
         # If verbosity is enabled, toggle in requests and http client libraries...
 #        if self._verbose:
@@ -90,16 +106,16 @@
 #            requests_log.propagate = True
 
     # Add the given learning example triplet...
     def add_learning_example(self, anchor_song_reference, positive_song_reference, negative_song_reference):
 
         # Initialize headers...
         headers                     = self._common_headers
-        headers['Accept']           = client._json_mime_type
-        headers['Content-Type']     = client._json_mime_type
+        headers['Accept']           = Client._json_mime_type
+        headers['Content-Type']     = Client._json_mime_type
 
         # Construct learning example object...
         learning_example = helios.requests.LearningExample(
             anchor_song_reference,
             positive_song_reference,
             negative_song_reference)
 
@@ -119,16 +135,17 @@
     # Add a new song to your music catalogue, optionally store it after
     #  analysis, and optionally invoke a progress callback of the from
     #  foo(bytes_read, new_bytes, total_bytes)...
     def add_song(self, new_song_dict, store=True, progress_callback=None):
 
         # Initialize headers...
         headers                     = self._common_headers
-        headers['Accept']           = client._json_mime_type
-        headers['Content-Type']     = client._json_mime_type
+        headers['Accept']           = Client._json_mime_type
+        headers['Accept-Encoding']  = Client._accept_encoding
+        headers['Content-Type']     = Client._json_mime_type
 
         # Prepare request...
         query_parameters            = {}
         query_parameters['store']   = str(store).lower()
 
         # Validate new_song_dict against schema...
         try:
@@ -228,16 +245,16 @@
     # Retrieve a list of all songs...
     def get_all_songs(self, page=None, page_size=None, progress=False, save_catalogue=None):
 
         # 3m32.299s with pagination for entire catalogue
 
         # Initialize headers...
         headers                             = self._common_headers
-        headers['Accept']                   = client._json_mime_type
-        headers['Accept-Encoding']          = client._accept_encoding
+        headers['Accept']                   = Client._json_mime_type
+        headers['Accept-Encoding']          = Client._accept_encoding
 
         # Endpoint to retrieve all songs...
         url = self._get_endpoint_url('/songs/all')
 
         # Storage for query parameters...
         query_parameters                    = {}
 
@@ -326,16 +343,27 @@
             all_songs_list = stored_song_schema.load(json_data)
 
             # If user requested to save response to disk, move the temp file
             #  to user's preference...
             if save_catalogue:
                 shutil.move(tempfile_name, save_catalogue)
 
+        # Check if songs to retrieve...
+        except requests.HTTPError as some_exception:
+
+            # No songs available. Return empty list...
+            if some_exception.response.status_code == 404:
+                return []
+
+            # Otherwise some other HTTP error...
+            else:
+                self._raise_http_exception(some_exception.response.json())
+
         # No more songs...
-        except helios.exceptions.NotFound:
+        except requests.exceptions.InvalidURL:
             return []
 
         # Deserialization error...
         except marshmallow.exceptions.MarshmallowError as some_exception:
             raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
 
         # Return list of stored songs...
@@ -364,16 +392,17 @@
         # Return constructed URL to caller...
         return url
 
     # Get system status about server...
     def get_system_status(self):
 
         # Initialize headers...
-        headers                 = self._common_headers
-        headers['Accept']       = client._json_mime_type
+        headers                     = self._common_headers
+        headers['Accept']           = Client._json_mime_type
+        headers['Accept-Encoding']  = Client._accept_encoding
 
         # Submit request...
         response = self._submit_request(
             endpoint='/status/system',
             method='GET',
             headers=headers)
 
@@ -391,15 +420,15 @@
         return system_status
 
     # Get information about available genres on the server...
     def get_genres_information(self):
 
         # Initialize headers...
         headers                 = self._common_headers
-        headers['Accept']       = client._json_mime_type
+        headers['Accept']       = Client._json_mime_type
 
         # Submit request, extract, construct each genre information and add to
         #  list...
         try:
 
             # Submit request...
             response = self._submit_request(
@@ -420,15 +449,15 @@
 
     # Get job status from server, returning the HTTP status code and the
     #  object the server sent us...
     def get_job_status(self, job_id, schema):
 
         # Initialize headers...
         headers                 = self._common_headers
-        headers['Accept']       = client._json_mime_type
+        headers['Accept']       = Client._json_mime_type
 
         # Format endpoint...
         endpoint = F'/status/jobs/{job_id}'
 
         # Submit request...
         response = self._submit_request(
             endpoint=endpoint,
@@ -474,16 +503,16 @@
             raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
 
     # Retrieve a list of all learning examples...
     def get_learning_examples(self):
 
         # Initialize headers...
         headers                         = self._common_headers
-        headers['Accept']               = client._json_mime_type
-        headers['Accept-Encoding']      = client._accept_encoding
+        headers['Accept']               = Client._json_mime_type
+        headers['Accept-Encoding']      = Client._accept_encoding
 
         # Submit request, extract, construct each learning example and add to
         #  list...
         try:
 
             # Submit request...
             response = self._submit_request(
@@ -498,21 +527,30 @@
         # Deserialization error...
         except marshmallow.exceptions.MarshmallowError as some_exception:
             raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
 
         # Return list of learning examples...
         return all_learning_examples
 
+    # Get a single random song...
+    def get_random_song(self):
+
+        # Retrieve the list of a single song...
+        random_songs_list = self.get_random_songs(size=1)
+
+        # Return it...
+        return random_songs_list[0]
+
     # Retrieve a list of random songs...
     def get_random_songs(self, size=1):
 
         # Initialize headers...
         headers                         = self._common_headers
-        headers['Accept']               = client._json_mime_type
-        headers['Accept-Encoding']      = client._accept_encoding
+        headers['Accept']               = Client._json_mime_type
+        headers['Accept-Encoding']      = Client._accept_encoding
 
         # Prepare request...
         query_parameters                = {}
         query_parameters['size']        = int(size)
 
         # Submit request, extract, construct each stored song and add to list...
         try:
@@ -540,17 +578,17 @@
         return random_songs_list
 
     # Perform a similarity search within the music catalogue...
     def get_similar_songs(self, similarity_search_dict, progress=False):
 
         # Initialize headers...
         headers                     = self._common_headers
-        headers['Accept']           = client._json_mime_type
-        headers['Content-Type']     = client._json_mime_type
-        headers['Accept-Encoding']  = client._accept_encoding
+        headers['Accept']           = Client._json_mime_type
+        headers['Content-Type']     = Client._json_mime_type
+        headers['Accept-Encoding']  = Client._accept_encoding
         headers['X-Helios-Expect']  = '202-accepted'
 
         # Validate similarity_search_dict against schema...
         try:
             similarity_search_schema = helios.requests.SimilaritySearchSchema()
             similarity_search_schema.load(similarity_search_dict)
         except marshmallow.ValidationError as some_exception:
@@ -680,15 +718,16 @@
         elif song_reference:
             endpoint = F'/songs/by_reference/{song_reference}'
         else:
             raise helios.exceptions.ExceptionBase(_('You must provide either a song_id or a song_reference.'))
 
         # Initialize headers...
         headers                         = self._common_headers
-        headers['Accept']               = client._json_mime_type
+        headers['Accept']               = Client._json_mime_type
+        headers['Accept-Encoding']      = Client._accept_encoding
 
         # Submit request...
         response = self._submit_request(
             endpoint=endpoint,
             method='GET',
             headers=headers)
 
@@ -705,22 +744,56 @@
         # Deserialization error...
         except marshmallow.exceptions.MarshmallowError as some_exception:
             raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
 
         # Return single stored song model...
         return songs_list[0]
 
+    # Retrieve the artwork for the given song as a tupel of a byte array and
+    #  MIME type...
+    def get_song_artwork(self, song_id=None, song_reference=None, maximum_height=None, maximum_width=None):
+
+        # Get the complete URL...
+        if song_id:
+            endpoint = F'/songs/download_artwork/by_id/{song_id}'
+        elif song_reference:
+            endpoint = F'/songs/download_artwork/by_reference/{song_reference}'
+        else:
+            raise helios.exceptions.ExceptionBase(_('You must provide either a song_id or a song_reference.'))
+
+        # Initialize headers...
+        headers = self._common_headers
+
+        # Prepare query parameters...
+        query_parameters                        = {}
+        if maximum_height:
+            query_parameters['maximum_height']  = int(maximum_height)
+        if maximum_width:
+            query_parameters['maximum_width']   = int(maximum_width)
+
+        # Submit request...
+        response = self._submit_request(
+            endpoint=endpoint,
+            method='GET',
+            headers=headers,
+            query_parameters=query_parameters)
+
+        # Return binary data array and MIME type...
+        return response.content, response.headers.get('Content-Type')
+
     # Download a song by ID or reference...
-    def get_song_download(self, song_id, song_reference, output, progress=False):
+    def get_song_download(self, output, song_id=None, song_reference=None, tui_progress=False, progress_callback=None):
 
         # Get the complete URL...
         if song_id:
             url = self._get_endpoint_url(F'/songs/download/by_id/{song_id}')
         elif song_reference:
             url = self._get_endpoint_url(F'/songs/download/by_reference/{song_reference}')
+        else:
+            raise Exception(_('You must provide either a song_id or a song_reference when calling get_song_download.'))
 
         # Initialize headers...
         headers             = self._common_headers
         headers['Accept']   = 'application/octet-stream'
 
         # Flag to requests on whether to verify server certificate. This can be
         #  either a boolean or a string according to documentation...
@@ -760,55 +833,69 @@
             # We reached the server. If we didn't get an expected response,
             #  raise an exception...
             response.raise_for_status()
 
             # Get total size of response body...
             total_size = int(response.headers.get('content-length'))
 
-            # Show progress if requested...
-            if progress:
-                progress_bar = tqdm(total=total_size, unit=_('B'), unit_scale=True)
+            # Total size of downloaded data...
+            current_size = 0
+
+            # Show TUI progress if requested...
+            if tui_progress:
+                tui_progress_bar = tqdm(total=total_size, unit=_('B'), unit_scale=True)
 
             # Write out the file...
             with open(output, 'wb') as file:
 
                 # As each chunk streams into memory, write it out...
                 for chunk in response.iter_content(chunk_size=8192):
 
                     # But skip keep-alive chunks...
                     if not chunk:
                         continue
 
                     # Append chunk to file...
                     file.write(chunk)
 
-                    # Advance progress, if requested...
-                    if progress:
-                        progress_bar.update(len(chunk))
+                    # Get current chunk size...
+                    chunk_size = len(chunk)
 
-            # Deallocate progress bar if we created one...
-            if progress:
-                progress_bar.close()
+                    # Add to total downloaded size...
+                    current_size += chunk_size
+
+                    # Advance TUI progress, if requested...
+                    if tui_progress:
+                        tui_progress_bar.update(chunk_size)
+
+                    # If user provided a progress callback, invoke it...
+                    if progress_callback:
+                        progress_callback(current_size=current_size, total_size=total_size)
+
+            # Deallocate TUI progress bar if we created one...
+            if tui_progress:
+                tui_progress_bar.close()
 
         # Connection problem...
         except requests.exceptions.ConnectionError as some_exception:
             raise helios.exceptions.Connection(
                 _(f'Unable to connect to {self._host}:{self._port}')) from some_exception
 
         # Server reported an error, raise appropriate exception...
         except requests.HTTPError as some_exception:
             self._raise_http_exception(some_exception.response.json())
 
     # Modify a song in the catalogue...
     def modify_song(self, patch_song_dict, store=None, song_id=None, song_reference=None):
 
         # Initialize headers...
-        headers                 = self._common_headers
-        headers['Accept']       = client._json_mime_type
-        headers['Content-Type'] = client._json_mime_type
+        headers                     = self._common_headers
+        headers['Accept']           = Client._json_mime_type
+        headers['Content-Type']     = Client._json_mime_type
+        headers['Accept-Encoding']  = Client._accept_encoding
 
         # Prepare endpoint...
         if song_id is not None:
             endpoint = F'/songs/by_id/{song_id}'
         elif song_reference is not None:
             endpoint = F'/songs/by_reference/{song_reference}'
         else:
@@ -843,20 +930,20 @@
         except marshmallow.exceptions.MarshmallowError as some_exception:
             raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
 
         # Parse response...
         return stored_song_response
 
     # Perform training on learning examples...
-    def perform_training(self, progress=False):
+    def perform_training(self, tui_progress=False):
 
         # Initialize headers...
         headers                     = self._common_headers
-        headers['Accept']           = client._json_mime_type
-        headers['Content-Type']     = client._json_mime_type
+        headers['Accept']           = Client._json_mime_type
+        headers['Content-Type']     = Client._json_mime_type
         headers['X-Helios-Expect']  = '202-accepted'
 
         # Construct perform training object...
         perform_training = helios.requests.PerformTraining()
 
         # Construct perform training schema to transform request into JSON...
         perform_training_schema = helios.requests.PerformTrainingSchema()
@@ -887,17 +974,17 @@
         # Extract job ID...
         job_id = matches.group(1)
 
         # Log job ID...
         if self._verbose:
             print(_(F'Server reported job started with job ID {job_id}...'))
 
-        # Optional progress bar, if requested by user and we have enough
+        # Optional TUI progress bar, if requested by user and we have enough
         #  information to manage one...
-        progress_bar = None
+        tui_progress_bar = None
 
         # Try to monitor progress until final update is available...
         try:
 
             # Status code received from server each time we poll it...
             status_code = 0
 
@@ -923,27 +1010,27 @@
 
                 # Status update available, but final result not ready yet...
                 if status_code == 202:
 
                     # Get the job's status...
                     job_status = response_object
 
-                    # If a progress bar was requested and does not exist yet,
-                    #  construct it...
-                    if progress and progress_bar is None and job_status.progress_total is not None:
-                        progress_bar = tqdm(total=job_status.progress_total)
+                    # If a TUI progress bar was requested and does not exist
+                    #  yet, construct it...
+                    if tui_progress and tui_progress_bar is None and job_status.progress_total is not None:
+                        tui_progress_bar = tqdm(total=job_status.progress_total)
 
-                    # If a progress bar exists, update it...
-                    if progress_bar is not None:
+                    # If a TUI progress bar exists, update it...
+                    if tui_progress_bar is not None:
 
                         # Update progress bar...
-                        progress_bar.update(job_status.progress_current)
+                        tui_progress_bar.update(job_status.progress_current)
 
                         # Set description...
-                        progress_bar.set_description(job_status.message)
+                        tui_progress_bar.set_description(job_status.message)
 
                 # For all other responses treat it as though it was unexpected...
                 else:
                     raise helios.exceptions.UnexpectedResponse(
                         _(F'Unexpected server response while polling job status: {response.status_code}'))
 
         # User trying to abort...
@@ -961,17 +1048,59 @@
         # Deserialization error...
         except marshmallow.exceptions.MarshmallowError as some_exception:
             raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
 
         # Cleanup tasks...
         finally:
 
-            # Deallocate progress bar if we created one...
-            if progress_bar is not None:
-                progress_bar.close()
+            # Deallocate TUI progress bar if we created one...
+            if tui_progress_bar is not None:
+                tui_progress_bar.close()
+
+    # Perform triplet mining from the system and user generated rankings for the
+    #  given search key and return list of triplets...
+    def perform_triplet_mining(self, search_reference, system_rankings, user_rankings):
+
+        # Initialize headers...
+        headers                     = self._common_headers
+        headers['Accept']           = Client._json_mime_type
+        headers['Content-Type']     = Client._json_mime_type
+        headers['Accept-Encoding']  = Client._accept_encoding
+
+        # Construct perform triplet mining request object...
+        perform_triplet_mining = helios.requests.PerformTripletMining(
+            search_reference,
+            system_rankings,
+            user_rankings)
+
+        # Construct perform triplet mining request schema to transform request
+        #  into JSON...
+        perform_triplet_mining_schema = helios.requests.PerformTripletMiningSchema()
+
+        # Try to submit request, extract, construct each received triplet and
+        #  add to list...
+        try:
+
+            # Submit request...
+            response = self._submit_request(
+                endpoint='/learning/examples/mine',
+                method='POST',
+                headers=headers,
+                data=perform_triplet_mining_schema.dumps(perform_triplet_mining))
+
+            # Validate response...
+            learning_examples_schema = helios.responses.LearningExampleSchema(many=True)
+            learning_examples_list = learning_examples_schema.load(response.json())
+
+        # Deserialization error...
+        except marshmallow.exceptions.MarshmallowError as some_exception:
+            raise helios.exceptions.UnexpectedResponse(some_exception) from some_exception
+
+        # Return the server generated list of learning examples...
+        return learning_examples_list
 
     # Take a server's error response that it emitted as JSON and raise an
     #  appropriate client exception...
     def _raise_http_exception(self, json_response):
 
         # Extract HTTP code from JSON response...
         code = 0
@@ -986,39 +1115,39 @@
         # Extract error summary from JSON response...
         summary = 'Server provided no summary.'
         if 'summary' in json_response:
             summary = json_response['summary']
 
         # Bad request exception. Suitable on a 400...
         if code == 400:
-            raise helios.exceptions.BadRequest(code, details, summary)
+            raise helios.exceptions.BadRequest(code, details, summary) from None
 
         # Unauthorized exception. Suitable on a 401...
         elif code == 401:
-            raise helios.exceptions.Unauthorized(code, details, summary)
+            raise helios.exceptions.Unauthorized(code, details, summary) from None
 
         # Not found exception. Suitable on a 404...
         elif code == 404:
-            raise helios.exceptions.NotFound(code, details, summary)
+            raise helios.exceptions.NotFound(code, details, summary) from None
 
         # Conflict exception. Suitable on a 409...
         elif code == 409:
-            raise helios.exceptions.Conflict(code, details, summary)
+            raise helios.exceptions.Conflict(code, details, summary) from None
 
         # Internal server error exception. Suitable on a 500...
         elif code == 500:
-            raise helios.exceptions.InternalServer(code, details, summary)
+            raise helios.exceptions.InternalServer(code, details, summary) from None
 
         # Insufficient storage exception. Suitable on a 507...
         elif code == 507:
-            raise helios.exceptions.InsufficientStorage(code, details, summary)
+            raise helios.exceptions.InsufficientStorage(code, details, summary) from None
 
         # Some other code...
         else:
-            raise helios.exceptions.ResponseExceptionBase(code, details, summary)
+            raise helios.exceptions.ResponseExceptionBase(code, details, summary) from None
 
     # Send a request to endpoint using method, headers, query parameters, and
     #  body...
     def _submit_request(
         self,
         endpoint,
         method,
@@ -1102,15 +1231,15 @@
                     data=data,
                     timeout=timeout,
                     verify=verify,
                     cert=public_private_key)
 
             # Unknown method...
             else:
-                raise Exception(F'Unknown method: {method}')
+                raise Exception(F'Unknown method: {method}') from None
 
             # We reached the server. If we didn't get an expected response,
             #  raise an exception...
             response.raise_for_status()
 
         # Can't establish connection problem...
         except requests.exceptions.ReadTimeout as some_exception:
@@ -1123,16 +1252,20 @@
                 _(F'Connection timeout while trying to connect to {self._host}:{self._port}')) from some_exception
 
         # Some other connection problem...
         except requests.exceptions.ConnectionError as some_exception:
             raise helios.exceptions.Connection(
                 _(F'Connection error while connecting to {self._host}:{self._port}')) from some_exception
 
+        # URL not found...
+        except requests.exceptions.InvalidURL as some_exception:
+            raise helios.exceptions.NotFound(_(F'URL not found at: {url}')) from some_exception
+
         # Server reported an error, raise appropriate exception...
-        except requests.HTTPError as some_exception:
+        except requests.exceptions.HTTPError as some_exception:
             try:
                 some_exception.response.json()
             except simplejson.errors.JSONDecodeError:
                 raise helios.exceptions.ResponseExceptionBase(
                     code=some_exception.response.status_code,
                     details=F'Server response had no JSON body, but code {some_exception.response.status_code}.',
                     summary=F'Server response had no JSON body, but code {some_exception.response.status_code}.') from some_exception
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios/exceptions.py` & `helios-client-0.4.20240424.post1/Source/helios/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2022 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # Base class for all Helios exceptions...
 class ExceptionBase(Exception):
 
     # Constructor...
     def __init__(self, message=None):
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios/requests.py` & `helios-client-0.4.20240424.post1/Source/helios/requests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2022 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # Imports...
 import attr
 from marshmallow import Schema, fields, post_load
 from helios.responses import LearningExample, LearningExampleSchema
 
@@ -92,14 +92,36 @@
 
     # Callback to receive dictionary of deserialized data...
     @post_load
     def make_perform_training(self, data, **kwargs):
         return PerformTraining(**data)
 
 
+# Perform triplet mining request...
+@attr.s
+class PerformTripletMining:
+    search_reference    = attr.ib(default=None)
+    system_rankings     = attr.ib(default=None)
+    user_rankings       = attr.ib(default=None)
+
+
+# Perform triplet mining schema request...
+class PerformTripletMiningSchema(Schema):
+
+    # Fields...
+    search_reference    = fields.String(allow_none=False, required=True)
+    system_rankings     = fields.List(fields.String(allow_none=False, required=True))
+    user_rankings       = fields.List(fields.String(allow_none=False, required=True))
+
+    # Callback to receive dictionary of deserialized data...
+    @post_load
+    def make_perform_triplet_mining(self, data, **kwargs):
+        return PerformTripletMining(**data)
+
+
 # Similarity search request...
 @attr.s
 class SimilaritySearch:
     similar_file            = attr.ib(default=None)
     similar_id              = attr.ib(default=None)
     similar_reference       = attr.ib(default=None)
     similar_url             = attr.ib(default=None)
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios/responses.py` & `helios-client-0.4.20240424.post1/Source/helios/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2023 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # System imports...
 import datetime
 
 # Other imports...
 import attr
@@ -253,15 +253,15 @@
     # Don't raise a ValidationError on load() when system's response contains
     #  new fields the client may not recognize yet...
     class Meta:
         unknown = EXCLUDE
 
     # Fields...
     examples                        = fields.Integer(required=True)
-    last_trained                    = fields.DateTime(required=True, format='rfc')
+    last_trained                    = fields.DateTime(required=True, format='iso') # ISO 8601
 
     # Callback to receive dictionary of deserialized data...
     @post_load
     def make_system_learning_status(self, data, **kwargs):
         return SystemLearningStatus(**data)
 
 
@@ -288,15 +288,15 @@
     # Don't raise a ValidationError on load() when system's response contains
     #  new fields the client may not recognize yet...
     class Meta:
         unknown = EXCLUDE
 
     # Fields...
     algorithm_age   = fields.Integer(required=True)
-    built           = fields.DateTime(required=True, format='rfc')
+    built           = fields.DateTime(required=True, format='iso') # ISO 8601
     configured      = fields.String(required=True)
     cpu             = fields.Nested(SystemCPUStatusSchema(), required=True)
     disk            = fields.Nested(SystemDiskStatusSchema(), required=True)
     encoding        = fields.String(required=True)
     learning        = fields.Nested(SystemLearningStatusSchema(), required=True)
     songs           = fields.Integer(required=True)
     system          = fields.String(required=True)
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios_client.egg-info/PKG-INFO` & `helios-client-0.4.20240424.post1/Source/helios_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: helios-client
-Version: 0.3.20230805.post1
+Version: 0.4.20240424.post1
 Summary: Pure python 3 module to communicate with a Helios server.
 Home-page: https://www.heliosmusic.io
 Author: Cartesian Theatre
 Author-email: kip@heliosmusic.io
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/cartesiantheatre/python-helios-client/issues
 Project-URL: Documentation, https://heliosmusic.io/api.html
 Project-URL: Source Code, https://github.com/cartesiantheatre/python-helios-client
 Keywords: music,similarity,match,catalogue,digital,signal,processing,machine,learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -59,27 +58,28 @@
 There are countless other examples, but let's talk about the first one. Nearly always, your client approaches you with samples already in hand. "Hey, do you have anything like this?" This could be an MP3 or a YouTube video URL. Because Helios allows you to search the catalogue using music itself as the search key, you could use the customer's samples directly to help them find what they're looking for.
 
 Traditionally, in the absence of such technology, the way this has been done for decades may surprise many. It is both costly and involves many hours or even days of manual human labour which delays the business process. The business must manually search, usually using [textual tags](https://heliosmusic.io/index.php/faq#tagging), and listen to a great deal of irrelevant music in the hopes of finding the one the client is actually willing to spend money on.
 
 ## Quick installation
 
 ### Ubuntu
-Packages already prepared for Ubuntu 22.04 (jammy) and later are available on our Personal Package Archive (PPA) [here](https://launchpad.net/%7Ekip/+archive/ubuntu/helios-public). To get the package installed and be up and running in seconds, just run the following two commands:
+Packages already prepared for Ubuntu 23.10 (mantic) and later are available on our Personal Package Archive (PPA) [here](https://launchpad.net/%7Ekip/+archive/ubuntu/helios-public). To get the package installed and be up and running in seconds, just run the following two commands:
 
 ```console
 $ sudo add-apt-repository ppa:kip/helios-public
 $ sudo apt install python3-helios-client
 ```
 
 ### PyPi
-If you are not using Ubuntu 22.04 or later and know what you are doing, you can use Python's ad hoc package manaement system. This is not recommended as a first choice because it is not as robust as a native package manager.
+If you are not using Ubuntu 23.10 or later and know what you are doing, you can use Python's ad hoc package management system. This is not recommended as a first choice because it is not as robust as a native package manager. But if you do choose to use `pip(1)` directly, you can always use it in a virtual environment.
 
 ```console
+$ python -m venv Environment
+$ source Environment/bin/activate
+$ cd Environment
 $ pip install helios-client
 ```
 
 ## Licensing
 
-This Python module is released under the terms of the [LGPL 3.0](https://www.gnu.org/licenses/lgpl-3.0.html) or greater. Copyright (C) 2015-2023 Cartesian Theatre. See [Copying](./Copying) for more information.
-
-
+This Python module is released under the terms of the [LGPL 3.0](https://www.gnu.org/licenses/lgpl-3.0.html) or greater. Copyright (C) 2015-2024 Cartesian Theatre. See [Copying](./Copying) for more information.
```

### Comparing `helios-client-0.3.20230805.post1/Source/helios_client.egg-info/SOURCES.txt` & `helios-client-0.4.20240424.post1/Source/helios_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 Source/helios_client.egg-info/requires.txt
 Source/helios_client.egg-info/top_level.txt
 Source/helios_client.egg-info/zip-safe
 debian/changelog
 debian/control
 debian/copyright
 debian/docs
+debian/lintian-overrides
 debian/rules
 debian/watch
 debian/source/format
 debian/source/options
 debian/tests/control
 debian/tests/test-import-module.py
 debian/tests/test-module-usage.py
```

### Comparing `helios-client-0.3.20230805.post1/debian/control` & `helios-client-0.4.20240424.post1/debian/control`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Source: python-helios-client
 Section: python
 Priority: optional
-Maintainer: Cartesian Theatre Packaging <packaging@cartesiantheatre.com>
-Standards-Version: 4.6.0.1
+Maintainer: Cartesian Theatre Packages <packages@cartesiantheatre.com>
+Standards-Version: 4.6.2.0
 Build-Depends:
-    debhelper-compat (= 11),
+    debhelper-compat (= 13),
     dh-exec,
     dh-python,
     lintian,
     python3-all,
     python3-attr (>= 18.2.0),
     python3-marshmallow (>= 3.16.0),
     python3-brotli,
     python3-requests,
+    python3-requests-toolbelt,
     python3-setuptools,
     python3-simplejson,
-    python3-tqdm
+    python3-tqdm,
+    python3-urllib3
 Homepage: https://www.heliosmusic.io
 Vcs-Git: https://www.github.com/cartesiantheatre/python-helios-client.git
 Vcs-Browser: https://github.com/cartesiantheatre/python-helios-client
 Rules-Requires-Root: no
 
 Package: python3-helios-client
 Architecture: all
 Multi-Arch: foreign
 Depends:
     ${misc:Depends},
     ${python3:Depends},
     python3-all,
     python3-setuptools
-Description: pure python module to access a remote Helios server (Python 3)
- Helios is an intelligent music recommendation platform.
+Description: pure Python module to access a remote Helios server (Python 3)
+ Helios is an intelligent music discovery platform.
  .
  This is an easy to use public pure Python 3 module that provides an API to
  communicate with a remote Helios server. The helios-client-utilities package
  is an example that uses it.
```

### Comparing `helios-client-0.3.20230805.post1/debian/rules` & `helios-client-0.4.20240424.post1/debian/rules`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/make -f
 #
 #   Helios.
-#   Copyright (C) 2015-2022 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # Output every command that modifies files on the build system...
 DH_VERBOSE = 1
 export DH_OPTIONS=-v
 
 # Tell pybuild the name of our module...
```

### Comparing `helios-client-0.3.20230805.post1/debian/tests/control` & `helios-client-0.4.20240424.post1/debian/tests/control`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 #   Helios.
-#   Copyright (C) 2015-2023 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # Functional test to verify module imports without issue...
 Tests: test-import-module.py
 Depends: python3-helios-client
 Restrictions: isolation-container
```

### Comparing `helios-client-0.3.20230805.post1/debian/tests/test-module-usage.py` & `helios-client-0.4.20240424.post1/debian/tests/test-module-usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env -S python3 -Werror -Wignore::ResourceWarning
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2023 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # System imports...
 import base64
 import glob
 import sys
 from pprint import pprint
@@ -38,15 +38,15 @@
     finally:
         temporary_socket.close()
 
     # Alert user of what we're doing...
     print(F'Local IP address is... {local_ip_address}')
 
     # Create a client...
-    client = helios.client(host=local_ip_address)
+    client = helios.Client(host=local_ip_address)
 
     # Query status...
     print('Querying Helios system status...')
     system_status = client.get_system_status()
 
     # Show status...
     pprint(attr.asdict(system_status))
@@ -110,10 +110,27 @@
         print('Deleting the following record...')
         pprint(stored_song_schema.dump(song))
 
         # Delete the record...
         client.delete_song(song_id=song.id)
         print('')
 
+    # Generate some example triplets...
+    learning_examples_list = client.perform_triplet_mining(
+        'SEARCH_REFERENCE',
+        [
+            'SONG_1',
+            'SONG_2',
+            'SONG_3',
+            'SONG_4',
+            'SONG_5'
+        ],
+        [
+            'SONG_2',
+            'SONG_1',
+            'SONG_4'
+        ])
+    pprint(learning_examples_list)
+
     # Done...
     print('Done...')
     sys.exit(0)
```

### Comparing `helios-client-0.3.20230805.post1/setup.py` & `helios-client-0.4.20240424.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 #
 #   Helios, intelligent music.
-#   Copyright (C) 2015-2023 Cartesian Theatre. All rights reserved.
+#   Copyright (C) 2015-2024 Cartesian Theatre. All rights reserved.
 #
 
 # Import modules...
 from __future__ import with_statement
 from setuptools import setup, find_packages
 import importlib.util
 import os
@@ -87,16 +87,18 @@
     # Options...
     include_package_data=True,
     install_requires=[
         'attrs >= 18.2.0',
         'brotli',
         'marshmallow >= 3.16.0',
         'requests',
+        'requests-toolbelt',
         'simplejson',
-        'tqdm'
+        'tqdm',
+        'urllib3'
     ],
     package_dir={'': 'Source'},
     packages=find_packages(where='Source'),
     python_requires='>= 3.7',
     zip_safe=True
 )
```


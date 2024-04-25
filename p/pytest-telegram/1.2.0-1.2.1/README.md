# Comparing `tmp/pytest-telegram-1.2.0.tar.gz` & `tmp/pytest_telegram-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-telegram-1.2.0.tar", last modified: Thu Dec 10 20:18:50 2020, max compression
+gzip compressed data, was "pytest_telegram-1.2.1.tar", last modified: Thu Apr 25 08:17:30 2024, max compression
```

## Comparing `pytest-telegram-1.2.0.tar` & `pytest_telegram-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 20:18:50.433066 pytest-telegram-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     4222 2020-12-10 20:18:50.433066 pytest-telegram-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2373 2020-12-10 20:18:40.000000 pytest-telegram-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 20:18:50.433066 pytest-telegram-1.2.0/pytest_telegram/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-10 20:18:40.000000 pytest-telegram-1.2.0/pytest_telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4688 2020-12-10 20:18:40.000000 pytest-telegram-1.2.0/pytest_telegram/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 20:18:50.433066 pytest-telegram-1.2.0/pytest_telegram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4222 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      357 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       53 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-12-10 20:18:50.000000 pytest-telegram-1.2.0/pytest_telegram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      394 2020-12-10 20:18:50.437065 pytest-telegram-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1534 2020-12-10 20:18:40.000000 pytest-telegram-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:17:30.759897 pytest_telegram-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 08:17:21.000000 pytest_telegram-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-25 08:17:30.759897 pytest_telegram-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-25 08:17:21.000000 pytest_telegram-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:17:30.759897 pytest_telegram-1.2.1/pytest_telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:17:21.000000 pytest_telegram-1.2.1/pytest_telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-25 08:17:21.000000 pytest_telegram-1.2.1/pytest_telegram/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:17:30.759897 pytest_telegram-1.2.1/pytest_telegram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 08:17:30.000000 pytest_telegram-1.2.1/pytest_telegram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-25 08:17:30.759897 pytest_telegram-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-25 08:17:21.000000 pytest_telegram-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:17:30.759897 pytest_telegram-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-25 08:17:21.000000 pytest_telegram-1.2.1/tests/test_plugin.py
```

### Comparing `pytest-telegram-1.2.0/README.rst` & `pytest_telegram-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-telegram-1.2.0/pytest_telegram/plugin.py` & `pytest_telegram-1.2.1/pytest_telegram/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 import time
-
+import logging
 import pytest
 import requests
 
+from requests import exceptions
+
+
+LOG = logging.getLogger(__name__)
+
 
 def pytest_addoption(parser):
     group = parser.getgroup('telegram')
     group.addoption(
         '--telegram_id',
         action='store',
         dest='telegram_id',
@@ -116,15 +121,20 @@
     session_time = time.time() - terminalreporter._sessionstarttime
     time_taken = f'\nTime taken: {str(time.strftime("%H:%M:%S", time.gmtime(session_time)))}'
 
     if failed == 0 and error == 0:
         sticker_payload = {'chat_id': chat_id, 'sticker': success_sticker_id}
     else:
         sticker_payload = {'chat_id': chat_id, 'sticker': fail_sticker_id}
-
-    message_id = None
-    if not disable_stickers:
-        message_id = requests.post(f'{telegram_uri}/sendSticker', json=sticker_payload).json()['result']['message_id']
-    message_payload = {'chat_id': chat_id,
-                       'text': f'{final_results}{time_taken}{custom_text}{report_url}\n{failed_tests}{error_tests}',
-                       'reply_to_message_id': message_id}
-    requests.post(f'{telegram_uri}/sendMessage', json=message_payload).json()
+    try:
+        message_id = None
+        if not disable_stickers:
+            message_id = requests.post(f'{telegram_uri}/sendSticker', json=sticker_payload).json()['result']['message_id']
+        message_payload = {
+            'chat_id': chat_id,
+            'text': f'{final_results}{time_taken}{custom_text}{report_url}\n{failed_tests}{error_tests}',
+            'reply_to_message_id': message_id
+        }
+        requests.post(f'{telegram_uri}/sendMessage', json=message_payload).json()
+    except exceptions.RequestException as e:
+        LOG.error("TELEGRAM Sending Message Error!!!")
+        LOG.exception(e)
```

### Comparing `pytest-telegram-1.2.0/setup.py` & `pytest_telegram-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ],
     name='pytest-telegram',
     packages=find_packages(include=['pytest_telegram']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rad96/pytest-telegram',
-    version='1.2.0',
+    version='1.2.1',
     zip_safe=False,
     entry_points={
         'pytest11': [
             'pytest-telegram = pytest_telegram.plugin',
         ]
     }
 )
```


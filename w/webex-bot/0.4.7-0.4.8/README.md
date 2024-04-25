# Comparing `tmp/webex_bot-0.4.7.tar.gz` & `tmp/webex_bot-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webex_bot-0.4.7.tar", last modified: Wed Apr 24 11:12:10 2024, max compression
+gzip compressed data, was "webex_bot-0.4.8.tar", last modified: Thu Apr 25 14:47:26 2024, max compression
```

## Comparing `webex_bot-0.4.7.tar` & `webex_bot-0.4.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-24 11:11:23.000000 webex_bot-0.4.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 11:11:23.000000 webex_bot-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 11:11:23.000000 webex_bot-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-24 11:12:10.569086 webex_bot-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-04-24 11:11:23.000000 webex_bot-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4800 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 11:11:23.000000 webex_bot-0.4.7/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 11:12:10.573086 webex_bot-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-24 11:11:23.000000 webex_bot-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 11:11:23.000000 webex_bot-0.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 11:11:23.000000 webex_bot-0.4.7/tests/test_webex_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/webex_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/webex_bot/cards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/cards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/webex_bot/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/commands/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/webex_bot/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/models/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/models/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/webex_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/webex_bot/websockets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-24 11:11:23.000000 webex_bot-0.4.7/webex_bot/websockets/webex_websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:12:10.569086 webex_bot-0.4.7/webex_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-24 11:12:10.000000 webex_bot-0.4.7/webex_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-24 11:12:10.000000 webex_bot-0.4.7/webex_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:12:10.000000 webex_bot-0.4.7/webex_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:12:02.000000 webex_bot-0.4.7/webex_bot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 11:12:10.000000 webex_bot-0.4.7/webex_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 11:12:10.000000 webex_bot-0.4.7/webex_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.738644 webex_bot-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-25 14:46:55.000000 webex_bot-0.4.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 14:46:55.000000 webex_bot-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-25 14:46:55.000000 webex_bot-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-25 14:47:26.738644 webex_bot-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-25 14:46:55.000000 webex_bot-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.734644 webex_bot-0.4.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4800 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 14:46:55.000000 webex_bot-0.4.8/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 14:47:26.738644 webex_bot-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-25 14:46:55.000000 webex_bot-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.734644 webex_bot-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 14:46:55.000000 webex_bot-0.4.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-25 14:46:55.000000 webex_bot-0.4.8/tests/test_webex_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.734644 webex_bot-0.4.8/webex_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.734644 webex_bot-0.4.8/webex_bot/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/cards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.738644 webex_bot-0.4.8/webex_bot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/commands/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.738644 webex_bot-0.4.8/webex_bot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/webex_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.738644 webex_bot-0.4.8/webex_bot/websockets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-25 14:46:55.000000 webex_bot-0.4.8/webex_bot/websockets/webex_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:47:26.734644 webex_bot-0.4.8/webex_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-25 14:47:26.000000 webex_bot-0.4.8/webex_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-25 14:47:26.000000 webex_bot-0.4.8/webex_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:47:26.000000 webex_bot-0.4.8/webex_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:47:20.000000 webex_bot-0.4.8/webex_bot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 14:47:26.000000 webex_bot-0.4.8/webex_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 14:47:26.000000 webex_bot-0.4.8/webex_bot.egg-info/top_level.txt
```

### Comparing `webex_bot-0.4.7/CONTRIBUTING.rst` & `webex_bot-0.4.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/LICENSE` & `webex_bot-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/PKG-INFO` & `webex_bot-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webex_bot
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python package for a Webex Bot based on websockets.
 Home-page: https://github.com/fbradyirl/webex_bot
 Author: Finbarr Brady
 Author-email: finbarr@somemail.com
 License: MIT license
 Keywords: webex_bot
 Platform: UNKNOWN
@@ -355,14 +355,18 @@
 * feat(20231212): add help image size parameter (#46)
 * update websockets to 11.0.3 (#43)
 
 ### 0.4.7 (2024-Apr-24)
 
 * Fix for help_command syntax issue
 
+### 0.4.8 (2024-Apr-25)
+
+* Fix for help_command missing commands.
+
 [1]: https://github.com/aaugustin/websockets
 
 [2]: https://github.com/CiscoDevNet/webexteamssdk
 
 [3]: https://developer.webex.com/docs/bots
 
 [4]: https://github.com/fbradyirl/webex_bot/blob/main/example.py
```

### Comparing `webex_bot-0.4.7/README.md` & `webex_bot-0.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,18 @@
 * feat(20231212): add help image size parameter (#46)
 * update websockets to 11.0.3 (#43)
 
 ### 0.4.7 (2024-Apr-24)
 
 * Fix for help_command syntax issue
 
+### 0.4.8 (2024-Apr-25)
+
+* Fix for help_command missing commands.
+
 [1]: https://github.com/aaugustin/websockets
 
 [2]: https://github.com/CiscoDevNet/webexteamssdk
 
 [3]: https://developer.webex.com/docs/bots
 
 [4]: https://github.com/fbradyirl/webex_bot/blob/main/example.py
```

### Comparing `webex_bot-0.4.7/docs/Makefile` & `webex_bot-0.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/docs/conf.py` & `webex_bot-0.4.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/docs/installation.rst` & `webex_bot-0.4.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/docs/make.bat` & `webex_bot-0.4.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/setup.py` & `webex_bot-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,10 +34,10 @@
     keywords='webex_bot',
     name='webex_bot',
     packages=find_packages(include=['webex_bot', 'webex_bot.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/fbradyirl/webex_bot',
-    version='0.4.7',
+    version='0.4.8',
     zip_safe=False,
 )
```

### Comparing `webex_bot-0.4.7/tests/test_webex_bot.py` & `webex_bot-0.4.8/tests/test_webex_bot.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot/commands/echo.py` & `webex_bot-0.4.8/webex_bot/commands/echo.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot/commands/help.py` & `webex_bot-0.4.8/webex_bot/commands/help.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot/exceptions.py` & `webex_bot-0.4.8/webex_bot/exceptions.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot/models/command.py` & `webex_bot-0.4.8/webex_bot/models/command.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot/models/response.py` & `webex_bot-0.4.8/webex_bot/models/response.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot/webex_bot.py` & `webex_bot-0.4.8/webex_bot/webex_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         self.commands = {
             self.help_command
         }
 
         if include_demo_commands:
             self.add_command(EchoCommand())
 
+        self.help_command.commands = self.commands
+
         self.card_callback_commands = {}
         self.approved_users = approved_users
         self.approved_domains = approved_domains
         self.approved_rooms = approved_rooms
         self.approval_parameters_check()
         self.bot_display_name = ""
         self.get_me_info()
```

### Comparing `webex_bot-0.4.7/webex_bot/websockets/webex_websocket_client.py` & `webex_bot-0.4.8/webex_bot/websockets/webex_websocket_client.py`

 * *Files identical despite different names*

### Comparing `webex_bot-0.4.7/webex_bot.egg-info/PKG-INFO` & `webex_bot-0.4.8/webex_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webex-bot
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python package for a Webex Bot based on websockets.
 Home-page: https://github.com/fbradyirl/webex_bot
 Author: Finbarr Brady
 Author-email: finbarr@somemail.com
 License: MIT license
 Keywords: webex_bot
 Platform: UNKNOWN
@@ -355,14 +355,18 @@
 * feat(20231212): add help image size parameter (#46)
 * update websockets to 11.0.3 (#43)
 
 ### 0.4.7 (2024-Apr-24)
 
 * Fix for help_command syntax issue
 
+### 0.4.8 (2024-Apr-25)
+
+* Fix for help_command missing commands.
+
 [1]: https://github.com/aaugustin/websockets
 
 [2]: https://github.com/CiscoDevNet/webexteamssdk
 
 [3]: https://developer.webex.com/docs/bots
 
 [4]: https://github.com/fbradyirl/webex_bot/blob/main/example.py
```

### Comparing `webex_bot-0.4.7/webex_bot.egg-info/SOURCES.txt` & `webex_bot-0.4.8/webex_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/pytgpt_bot-0.0.3.tar.gz` & `tmp/pytgpt_bot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.3.tar", last modified: Thu Apr 25 08:24:42 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.4.tar", last modified: Thu Apr 25 08:36:52 2024, max compression
```

## Comparing `pytgpt_bot-0.0.3.tar` & `pytgpt_bot-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/pytgpt_bot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:24:42.259015 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 08:24:42.000000 pytgpt_bot-0.0.3/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:24:42.263015 pytgpt_bot-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-25 08:24:26.000000 pytgpt_bot-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:52.643882 pytgpt_bot-0.0.4/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/setup.py
```

### Comparing `pytgpt_bot-0.0.3/LICENSE` & `pytgpt_bot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.3/PKG-INFO` & `pytgpt_bot-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.3 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.4 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.0.3/README.md` & `pytgpt_bot-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.3/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.4/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.3/pytgpt_bot/config.py` & `pytgpt_bot-0.0.4/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.3/pytgpt_bot/db.py` & `pytgpt_bot-0.0.4/pytgpt_bot/db.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.3/pytgpt_bot/main.py` & `pytgpt_bot-0.0.4/pytgpt_bot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
     return decorator
 
 
 @bot.message_handler(commands=["help", "start"])
 @handler_formatter
 def home(message: telebot.types.Message):
     """
-    Welcome to [pytgpt](https://github.com/Simatwa/python-tgpt).
+    Welcome to [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot).
     /help : Show this help info.
     /chat : Chat with AI.
     /imager : Generate image from text. (default)
     /prodia : Generate image from text. (Prodia)
     /audio : Generate audio from text.
     /intro : Check current chat intro.
     /history : Check chat history.
-    /sintro : Set new value for chat intro
+    /sintro : Set new value for chat intro.
     /reset : Start new chat thread.
     /myid : Echo your Telegram ID.
     /default : Chat with AI.
     """
 
     return bot.send_message(
         message.chat.id,
```

### Comparing `pytgpt_bot-0.0.3/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.4/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.3 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.4 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
```

### Comparing `pytgpt_bot-0.0.3/setup.py` & `pytgpt_bot-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.3",
+    version="0.0.4",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
```


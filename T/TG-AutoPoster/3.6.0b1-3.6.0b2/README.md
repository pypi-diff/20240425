# Comparing `tmp/tg_autoposter-3.6.0b1.tar.gz` & `tmp/tg_autoposter-3.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_autoposter-3.6.0b1.tar", max compression
+gzip compressed data, was "tg_autoposter-3.6.0b2.tar", last modified: Thu Apr 25 19:22:40 2024, max compression
```

## Comparing `tg_autoposter-3.6.0b1.tar` & `tg_autoposter-3.6.0b2.tar`

### file list

```diff
@@ -1,37 +1,60 @@
--rw-r--r--   0        0        0    17022 2023-07-22 07:43:00.777076 tg_autoposter-3.6.0b1/README.md
--rw-r--r--   0        0        0     7035 2023-10-21 08:04:43.614481 tg_autoposter-3.6.0b1/TG_AutoPoster/TG_AutoPoster.py
--rw-r--r--   0        0        0      219 2023-12-28 19:02:46.712350 tg_autoposter-3.6.0b1/TG_AutoPoster/__init__.py
--rw-r--r--   0        0        0     3780 2023-10-21 07:00:23.463618 tg_autoposter-3.6.0b1/TG_AutoPoster/__main__.py
--rw-r--r--   0        0        0      526 2023-07-10 18:14:52.019191 tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/__init__.py
--rw-r--r--   0        0        0     6331 2023-01-17 15:09:03.103010 tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/callback.py
--rw-r--r--   0        0        0     9397 2023-07-10 18:21:16.690403 tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/commands.py
--rw-r--r--   0        0        0     2324 2023-01-27 07:29:15.534083 tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/handlers.py
--rw-r--r--   0        0        0      944 2022-08-27 13:46:12.000000 tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/inline.py
--rw-r--r--   0        0        0       57 2023-01-16 17:25:14.420668 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-01-17 15:19:59.091458 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tg/__init__.py
--rw-r--r--   0        0        0     7402 2023-07-10 18:22:10.901435 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tg/messages.py
--rw-r--r--   0        0        0     6330 2023-01-17 15:23:08.799668 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tg/tools.py
--rw-r--r--   0        0        0     2100 2022-08-27 13:46:12.000000 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tools.py
--rw-r--r--   0        0        0      129 2022-05-24 17:16:32.000000 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/__init__.py
--rw-r--r--   0        0        0     8387 2023-04-10 10:03:22.251705 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/group.py
--rw-r--r--   0        0        0     1513 2023-06-11 15:19:44.359821 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/handlers.py
--rw-r--r--   0        0        0    19853 2023-12-28 17:30:26.575170 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/parser.py
--rw-r--r--   0        0        0     6055 2022-09-14 07:20:50.000000 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/sender.py
--rw-r--r--   0        0        0     3932 2023-07-10 15:42:48.136874 tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/tools.py
--rw-r--r--   0        0        0      661 2023-12-28 19:55:21.423723 tg_autoposter-3.6.0b1/pyproject.toml
--rw-r--r--   0        0        0      434 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/__init__.py
--rw-r--r--   0        0        0    23350 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/audio.py
--rw-r--r--   0        0        0     2596 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/audio_url_decoder.py
--rw-r--r--   0        0        0     7267 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/bot_longpoll.py
--rw-r--r--   0        0        0     2693 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/enums.py
--rw-r--r--   0        0        0     4052 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/exceptions.py
--rw-r--r--   0        0        0     2792 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/execute.py
--rw-r--r--   0        0        0    10316 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/keyboard.py
--rw-r--r--   0        0        0    20677 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/longpoll.py
--rw-r--r--   0        0        0     7442 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/requests_pool.py
--rw-r--r--   0        0        0     3702 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/streaming.py
--rw-r--r--   0        0        0     8182 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/tools.py
--rw-r--r--   0        0        0    23910 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/upload.py
--rw-r--r--   0        0        0     4019 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/utils.py
--rw-r--r--   0        0        0    26826 2023-12-28 19:48:00.174646 tg_autoposter-3.6.0b1/vk_api/vk_api/vk_api.py
--rw-r--r--   0        0        0    18069 1970-01-01 00:00:00.000000 tg_autoposter-3.6.0b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.433843 tg_autoposter-3.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-25 19:22:40.433843 tg_autoposter-3.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.425843 tg_autoposter-3.6.0b2/TG_AutoPoster/
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/TG_AutoPoster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.425843 tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/inline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.429843 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.429843 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tg/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tg/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tg/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.429843 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20558 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.433843 tg_autoposter-3.6.0b2/TG_AutoPoster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-25 19:22:40.000000 tg_autoposter-3.6.0b2/TG_AutoPoster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 19:22:40.000000 tg_autoposter-3.6.0b2/TG_AutoPoster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:22:40.000000 tg_autoposter-3.6.0b2/TG_AutoPoster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-25 19:22:40.000000 tg_autoposter-3.6.0b2/TG_AutoPoster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 19:22:40.000000 tg_autoposter-3.6.0b2/TG_AutoPoster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:22:40.433843 tg_autoposter-3.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-25 19:22:35.000000 tg_autoposter-3.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.425843 tg_autoposter-3.6.0b2/vk_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.429843 tg_autoposter-3.6.0b2/vk_api/jconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/jconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/jconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/jconfig/jconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/jconfig/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:40.433843 tg_autoposter-3.6.0b2/vk_api/vk_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/audio_url_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/bot_longpoll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/longpoll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/requests_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23910 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26826 2024-04-25 19:22:36.000000 tg_autoposter-3.6.0b2/vk_api/vk_api/vk_api.py
```

### Comparing `tg_autoposter-3.6.0b1/README.md` & `tg_autoposter-3.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/TG_AutoPoster.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/TG_AutoPoster.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/__main__.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/__main__.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/__init__.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/callback.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/callback.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/commands.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/commands.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/handlers.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import pyrogram.filters
 from pyrogram.types import Message
 
 from .. import AutoPoster
 from ..utils.tg import messages, tools
 
-@AutoPoster.on_message(tools.status_filter("set"))
+
+@AutoPoster.on_message(pyrogram.filters.private & tools.status_filter("set"))
 def update_header_footer(bot: AutoPoster, message: Message):
     _, domain, key = bot.conversations[message.from_user.id]
     bot.reload_config()
     if domain == "global":
         if message.text.markdown == "DELETE" and key in bot.config["settings"]:
             bot.config["settings"].pop(key)
         else:
@@ -21,17 +22,21 @@
             bot.config["domains"][domain].pop(key)
         else:
             bot.config["domains"][domain][key] = str(message.text.markdown)
     bot.save_config()
     message.reply(messages.CHANGE_SUCCESS.format(key.capitalize()))
     bot.conversations.pop(message.from_user.id)
 
+
 @AutoPoster.on_message(
-    tools.status_filter("stop_list")
-    | tools.status_filter("blacklist"))
+    pyrogram.filters.private & (
+            tools.status_filter("stop_list")
+            | tools.status_filter("blacklist")
+    )
+)
 def stoplist_update(bot: AutoPoster, message: Message):
     filetype, domain = bot.conversations[message.from_user.id]
 
     bot.reload_config()
     if domain == "global":
         global_stoplist = Path(bot.config.get("settings", {}).get(
             filetype,
@@ -52,10 +57,12 @@
     bot.save_config()
 
 
 @AutoPoster.on_message(pyrogram.filters.forwarded & pyrogram.filters.private)
 def get_forward_id(_, message: Message):
     if message.forward_from:
         id_ = message.forward_from.id
-    else:
+    elif message.forward_from_chat:
         id_ = message.forward_from_chat.id
-    message.reply("Channel (user) ID is `{}`".format(id_))
+    else:
+        id_ = "hidden"
+    message.reply("Channel (user) ID is `{}`".format(id_))
```

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/plugins/inline.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/plugins/inline.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tg/messages.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tg/messages.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tg/tools.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tg/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 def option_filter(option):
     def func(_, __, callback_query: CallbackQuery):
         return callback_query.data.split()[0] == option
 
     return filters.create(func)
 
+
 def status_filter(status):
     def func(_, bot, message: Message):
         if message.from_user.id in bot.conversations.keys():
             return bot.conversations[message.from_user.id][0] == status
 
     return filters.create(func)
```

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/tools.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/tools.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/group.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/group.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/handlers.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/handlers.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/parser.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import urllib.error
 from re import IGNORECASE, MULTILINE, sub
 
 import requests
-from bs4 import BeautifulSoup
 from loguru import logger
 from pyrogram.types import (InlineKeyboardButton, InlineKeyboardMarkup,
                             InputMediaAudio, InputMediaDocument,
                             InputMediaPhoto, InputMediaVideo)
 from vk_api import VkApi, exceptions
 from vk_api.audio import VkAudio
 from wget import download, detect_filename
 
 from ..tools import build_menu, split
-from .tools import (Attachments, add_audio_tags, download_video, gif_to_video,
-                    m3u8_to_mp3)
+from .tools import Attachments, add_audio_tags, gif_to_video, m3u8_to_mp3
 
 MAX_FILENAME_LENGTH = 255
 DOMAIN_REGEX = r"https://(m\.)?vk\.com/"
 USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; rv:91.0) Gecko/20100101 Firefox/91.0"
 
 
 class Post:
@@ -175,14 +173,21 @@
         photo = download(photo, bar=None)
         if photo:
             self.attachments.media.append(InputMediaPhoto(photo))
 
     def parse_doc(self, attachment):
         logger.info("[VK] Извлечение документа {}", attachment["title"])
         logger.debug(attachment)
+        if not self.check_file_size(attachment["url"]):
+            logger.warning(
+                '[VK] Размер документа превышает допустимый. '
+                'Добавляем ссылку на документ в текст.'
+            )
+            self.text += '\n📃 <a href="{url}">{title}</a>'.format(**attachment)
+            return
         try:
             attachment["title"] = sub(
                 r"[/\\:*?\"><|]", "", attachment["title"]
             )
             if attachment["title"].endswith(attachment["ext"]):
                 doc = download(
                     attachment["url"], out="{title}".format(**attachment)
@@ -204,18 +209,24 @@
             )
             self.text += '\n📃 <a href="{url}">{title}</a>'.format(**attachment)
 
     def parse_video(self, attachment):
         logger.info("[VK] Извлечение видео")
         logger.debug(attachment)
 
+        lnk = "https://m.vk.com/video{owner_id}_{id}".format(**attachment)
+        vid_key = "{owner_id}_{id}".format(**attachment)
+        if attachment.get("access_key"):
+            lnk += "?list={access_key}"
+            vid_key += "_{access_key}"
+
         video_text = (
-            '\n🎥 <a href="https://m.vk.com/video{owner_id}_{id}?list={access_key}">{title}</a>'
+            '\n🎥 <a href="{}">{title}</a>'
             '\n👁 {views} раз(а) ⏳ {duration} сек'
-        ).format(**attachment)
+        ).format(lnk, **attachment)
 
         if self.video_token is None:
             logger.warning(
                 "[VK] Токен для получения видеозаписей не доступен. "
                 "Добавляем ссылку на видео в текст."
             )
             self.text += video_text
@@ -224,15 +235,15 @@
         video = self.session.http.get(
             "https://api.vk.com/method/video.get",
             params=dict(
                 v="5.223",
                 client_id=7879029,
                 access_token=self.video_token,
                 owner_id=attachment["owner_id"],
-                videos="{owner_id}_{id}_{access_key}".format(**attachment),
+                videos=vid_key,
             )
         )
         if video.ok:
             video = video.json()["response"]["items"][0]
         else:
             logger.warning(
                 "[VK] Не удалось получить прямую ссылку на видео. "
@@ -245,27 +256,28 @@
         for k, v in video["files"].items():
             if k in ("mp4_240", "mp4_360", "mp4_480", "mp4_720"):
                 video_link = v
 
         if video_link is not None:
             video_file = self.session.http.get(video_link, stream=True)
             if video_file.ok:
-                if int(video_file.headers['Content-Length']) >= 2 * 10**9:
+                if not self.check_file_size(video_link):
                     logger.info(
-                        "[VK] Видео весит более 2 ГБ. "
+                        "[VK] Размер видео превышает допустимый. "
                         "Добавляем ссылку на видео в текст."
                     )
                     self.text += video_text
                 else:
                     video_name = detect_filename(
                         headers=video_file.headers, default="video.mp4",
                     )
                     with open(video_name, "wb") as f:
-                        for chunk in video_file:
-                            f.write(chunk)
+                        for chunk in video_file.iter_content(chunk_size=1024):
+                            if chunk:
+                                f.write(chunk)
                     self.attachments.media.append(InputMediaVideo(video_name))
         else:
             self.text += video_text
 
     def parse_music(self, attachment):
         logger.info(
             "[VK] Извлечение аудио {} - {}",
@@ -460,14 +472,18 @@
             self.session,
             self.sign_posts,
             self.what_to_parse,
         )
         self.repost.parse_post()
         self.repost.text = split(repost_source + " ".join(self.repost.text))
 
+    def check_file_size(self, url, max_size=2e9):
+        r = self.session.http.head(url)
+        return int(r.headers["Content-Length"]) < max_size
+
     def __bool__(self):
         return (
             bool("".join(self.text))
             or bool(self.attachments)
             or bool(self.poll)
         )
```

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/sender.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/sender.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/TG_AutoPoster/utils/vk/tools.py` & `tg_autoposter-3.6.0b2/TG_AutoPoster/utils/vk/tools.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/audio.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/audio.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/audio_url_decoder.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/audio_url_decoder.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/bot_longpoll.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/bot_longpoll.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/enums.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/enums.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/exceptions.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/execute.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/execute.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/keyboard.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/keyboard.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/longpoll.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/longpoll.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/requests_pool.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/requests_pool.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/streaming.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/streaming.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/tools.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/tools.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/upload.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/upload.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/utils.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/utils.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/vk_api/vk_api/vk_api.py` & `tg_autoposter-3.6.0b2/vk_api/vk_api/vk_api.py`

 * *Files identical despite different names*

### Comparing `tg_autoposter-3.6.0b1/PKG-INFO` & `tg_autoposter-3.6.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: TG_AutoPoster
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: Telegram Bot for reposting from VK
-License: MIT
-Author: Adrian Polyakov
+Home-page: https://github.com/qwertyadrian/TG_AutoPoster
+Download-URL: https://github.com/qwertyadrian/TG_AutoPoster/releases/latest
+Author: qwertyadrian
 Author-email: me@qwertyadrian.ru
-Requires-Python: >=3.8,<4.0
+License: MIT License
+Platform: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: Pyrogram (>=2.0.106,<3.0.0)
-Requires-Dist: TgCrypto (>=1.2.5,<2.0.0)
-Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: m3u8 (>=4.0.0,<5.0.0)
-Requires-Dist: moviepy (>=1.0.3,<2.0.0)
-Requires-Dist: mutagen (>=1.47.0,<2.0.0)
-Requires-Dist: pycryptodome (>=3.19.1,<4.0.0)
-Requires-Dist: wget (>=3.2,<4.0)
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENCE.md
+Requires-Dist: pyrogram==2.0.106
+Requires-Dist: tgcrypto
+Requires-Dist: loguru==0.7.2
+Requires-Dist: wget==3.2
+Requires-Dist: mutagen==1.47.0
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: apscheduler==3.10.4
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: m3u8==4.0.0
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: moviepy==1.0.3
 
 TG_AutoPoster 
 =============
 Бот, пересылающий записи из групп ВК в канал/чат/ЛС в Telegram.
 
 [![License MIT](https://img.shields.io/github/license/qwertyadrian/TG_AutoPoster.svg)](/LICENCE.md) 
 ![Python Version](https://img.shields.io/pypi/pyversions/tg_autoposter) 
@@ -119,8 +129,7 @@
 1. [GitHub Issues](https://github.com/qwertyadrian/TG_AutoPoster/issues/new/choose)
 2. Telegram: [@QwertyAdrian](https://t.me/QwertyAdrian)
 
 Для пожертвований на развитие проекта:
 1. [Qiwi](https://qiwi.com/n/QWERTYADRIAN)
 2. Bitcoin: `1H1UVnXgvcLo3RWmxuYmi7b16ADo6XBWw5`
 3. TON: `EQD42Z5d8d1gT1uSpKTAaLYHlQ95vdMXrlNlYMpSFpQawwuY`
-
```


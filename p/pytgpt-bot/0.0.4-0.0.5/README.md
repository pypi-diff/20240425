# Comparing `tmp/pytgpt_bot-0.0.4.tar.gz` & `tmp/pytgpt_bot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.0.4.tar", last modified: Thu Apr 25 08:36:52 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.0.5.tar", last modified: Thu Apr 25 13:11:00 2024, max compression
```

## Comparing `pytgpt_bot-0.0.4.tar` & `pytgpt_bot-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:52.643882 pytgpt_bot-0.0.4/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/pytgpt_bot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 08:36:52.000000 pytgpt_bot-0.0.4/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:36:52.647882 pytgpt_bot-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-25 08:36:33.000000 pytgpt_bot-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:11:00.713943 pytgpt_bot-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-04-25 13:11:00.709943 pytgpt_bot-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:11:00.709943 pytgpt_bot-0.0.5/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/pytgpt_bot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:11:00.709943 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 13:11:00.000000 pytgpt_bot-0.0.5/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:11:00.713943 pytgpt_bot-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-25 13:10:39.000000 pytgpt_bot-0.0.5/setup.py
```

### Comparing `pytgpt_bot-0.0.4/LICENSE` & `pytgpt_bot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.4/PKG-INFO` & `pytgpt_bot-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -93,15 +93,15 @@
 ### 1. Chat with AI
 
 - **Command**: `/chat`
 - **Description**: Engage in a conversation with AI. This feature allows you to interact with the bot in a natural, conversational manner.
 
 ### 2. Generate Images from Text
 
-- **Command**: `/imager`
+- **Command**: `/image`
 - **Description**: Generate images from text descriptions. This feature uses AI to create visual representations of your text inputs, making it a fun and creative way to explore the capabilities of AI.
 
 - **Variant**: `/prodia`
 - **Description**: Generate images from text descriptions using the Prodia AI model. This variant offers a different style of image generation, providing a unique twist to your creative endeavors.
 
 ### 3. Generate Audio from Text
 
@@ -131,18 +131,33 @@
 ### 8. Echo Your Telegram ID
 
 - **Command**: `/myid`
 - **Description**: Echo your Telegram ID. This feature provides you with your unique Telegram ID, useful for personalized interactions or for troubleshooting purposes and configuring admin.
 
 ### 9. Clear chat data
 
-- **Command**: `/clear_database`
+- **Command**: `/clear_chats`
 - **Description**: This is an administrative command for deleting all entries of chat database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
 
-### 10. Default Chat with AI
+### 10. Check total Chat
+
+- **Command**: `/total_chats`
+- **Description**: This is an administrative command for checking total chat records. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 11. Drop entire chat
+
+- **Command**: `/drop_chats`
+- **Description**: This is an administrative command that **drops** entire chat table and create new one. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 12. Run sql statements
+
+- **Command**: `/sql`
+- **Description**: This is an administrative command for running **SQL STATEMENTS** against the database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 12. Default Chat with AI
 
 - **Command**: `<Any other text>`
 - **Description**: Engage in a default chat with AI. This command is a shortcut to the `/chat` command, offering a quick and straightforward way to start a conversation with the bot.
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.4 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.5 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -39,15 +39,15 @@
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
 Features ### 1. Chat with AI - **Command**: `/chat` - **Description**: Engage
 in a conversation with AI. This feature allows you to interact with the bot in
 a natural, conversational manner. ### 2. Generate Images from Text -
-**Command**: `/imager` - **Description**: Generate images from text
+**Command**: `/image` - **Description**: Generate images from text
 descriptions. This feature uses AI to create visual representations of your
 text inputs, making it a fun and creative way to explore the capabilities of
 AI. - **Variant**: `/prodia` - **Description**: Generate images from text
 descriptions using the Prodia AI model. This variant offers a different style
 of image generation, providing a unique twist to your creative endeavors. ###
 3. Generate Audio from Text - **Command**: `/audio` - **Description**: Generate
 audio from text. This feature allows you to convert your text inputs into
@@ -64,20 +64,33 @@
 the current chat, allowing you to tailor the conversation to your preferences.
 ### 7. Start New Chat Thread - **Command**: `/reset` - **Description**: Start a
 new chat thread. This feature allows you to begin a fresh conversation with the
 bot, resetting the chat history and allowing for a new start. ### 8. Echo Your
 Telegram ID - **Command**: `/myid` - **Description**: Echo your Telegram ID.
 This feature provides you with your unique Telegram ID, useful for personalized
 interactions or for troubleshooting purposes and configuring admin. ### 9.
-Clear chat data - **Command**: `/clear_database` - **Description**: This is an
+Clear chat data - **Command**: `/clear_chats` - **Description**: This is an
 administrative command for deleting all entries of chat database. The user's
 Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
 pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 10. Default Chat with AI - **Command**: `` - **Description**: Engage in a
-default chat with AI. This command is a shortcut to the `/chat` command,
-offering a quick and straightforward way to start a conversation with the bot.
-## Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+### 10. Check total Chat - **Command**: `/total_chats` - **Description**: This
+is an administrative command for checking total chat records. The user's
+Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
+pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+### 11. Drop entire chat - **Command**: `/drop_chats` - **Description**: This
+is an administrative command that **drops** entire chat table and create new
+one. The user's Telegram ID must match the one set at the [.env](https://
+github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/
+env#L2) config file. ### 12. Run sql statements - **Command**: `/sql` -
+**Description**: This is an administrative command for running **SQL
+STATEMENTS** against the database. The user's Telegram ID must match the one
+set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/
+7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file. ### 12. Default
+Chat with AI - **Command**: `` - **Description**: Engage in a default chat with
+AI. This command is a shortcut to the `/chat` command, offering a quick and
+straightforward way to start a conversation with the bot. ## Support and
+Feedback If you have any questions, feedback, or suggestions for `pytgpt`,
+please feel free to reach out. Your input is valuable in helping us improve and
+expand the bot's capabilities. ## License `pytgpt-bot` is open-source and
+available under the [MIT License](LICENSE). Feel free to use, modify, and
+distribute the code as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy
+your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.4/README.md` & `pytgpt_bot-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ### 1. Chat with AI
 
 - **Command**: `/chat`
 - **Description**: Engage in a conversation with AI. This feature allows you to interact with the bot in a natural, conversational manner.
 
 ### 2. Generate Images from Text
 
-- **Command**: `/imager`
+- **Command**: `/image`
 - **Description**: Generate images from text descriptions. This feature uses AI to create visual representations of your text inputs, making it a fun and creative way to explore the capabilities of AI.
 
 - **Variant**: `/prodia`
 - **Description**: Generate images from text descriptions using the Prodia AI model. This variant offers a different style of image generation, providing a unique twist to your creative endeavors.
 
 ### 3. Generate Audio from Text
 
@@ -92,18 +92,33 @@
 ### 8. Echo Your Telegram ID
 
 - **Command**: `/myid`
 - **Description**: Echo your Telegram ID. This feature provides you with your unique Telegram ID, useful for personalized interactions or for troubleshooting purposes and configuring admin.
 
 ### 9. Clear chat data
 
-- **Command**: `/clear_database`
+- **Command**: `/clear_chats`
 - **Description**: This is an administrative command for deleting all entries of chat database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
 
-### 10. Default Chat with AI
+### 10. Check total Chat
+
+- **Command**: `/total_chats`
+- **Description**: This is an administrative command for checking total chat records. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 11. Drop entire chat
+
+- **Command**: `/drop_chats`
+- **Description**: This is an administrative command that **drops** entire chat table and create new one. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 12. Run sql statements
+
+- **Command**: `/sql`
+- **Description**: This is an administrative command for running **SQL STATEMENTS** against the database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 12. Default Chat with AI
 
 - **Command**: `<Any other text>`
 - **Description**: Engage in a default chat with AI. This command is a shortcut to the `/chat` command, offering a quick and straightforward way to start a conversation with the bot.
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
 Features ### 1. Chat with AI - **Command**: `/chat` - **Description**: Engage
 in a conversation with AI. This feature allows you to interact with the bot in
 a natural, conversational manner. ### 2. Generate Images from Text -
-**Command**: `/imager` - **Description**: Generate images from text
+**Command**: `/image` - **Description**: Generate images from text
 descriptions. This feature uses AI to create visual representations of your
 text inputs, making it a fun and creative way to explore the capabilities of
 AI. - **Variant**: `/prodia` - **Description**: Generate images from text
 descriptions using the Prodia AI model. This variant offers a different style
 of image generation, providing a unique twist to your creative endeavors. ###
 3. Generate Audio from Text - **Command**: `/audio` - **Description**: Generate
 audio from text. This feature allows you to convert your text inputs into
@@ -40,20 +40,33 @@
 the current chat, allowing you to tailor the conversation to your preferences.
 ### 7. Start New Chat Thread - **Command**: `/reset` - **Description**: Start a
 new chat thread. This feature allows you to begin a fresh conversation with the
 bot, resetting the chat history and allowing for a new start. ### 8. Echo Your
 Telegram ID - **Command**: `/myid` - **Description**: Echo your Telegram ID.
 This feature provides you with your unique Telegram ID, useful for personalized
 interactions or for troubleshooting purposes and configuring admin. ### 9.
-Clear chat data - **Command**: `/clear_database` - **Description**: This is an
+Clear chat data - **Command**: `/clear_chats` - **Description**: This is an
 administrative command for deleting all entries of chat database. The user's
 Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
 pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 10. Default Chat with AI - **Command**: `` - **Description**: Engage in a
-default chat with AI. This command is a shortcut to the `/chat` command,
-offering a quick and straightforward way to start a conversation with the bot.
-## Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+### 10. Check total Chat - **Command**: `/total_chats` - **Description**: This
+is an administrative command for checking total chat records. The user's
+Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
+pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+### 11. Drop entire chat - **Command**: `/drop_chats` - **Description**: This
+is an administrative command that **drops** entire chat table and create new
+one. The user's Telegram ID must match the one set at the [.env](https://
+github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/
+env#L2) config file. ### 12. Run sql statements - **Command**: `/sql` -
+**Description**: This is an administrative command for running **SQL
+STATEMENTS** against the database. The user's Telegram ID must match the one
+set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/
+7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file. ### 12. Default
+Chat with AI - **Command**: `` - **Description**: Engage in a default chat with
+AI. This command is a shortcut to the `/chat` command, offering a quick and
+straightforward way to start a conversation with the bot. ## Support and
+Feedback If you have any questions, feedback, or suggestions for `pytgpt`,
+please feel free to reach out. Your input is valuable in helping us improve and
+expand the bot's capabilities. ## License `pytgpt-bot` is open-source and
+available under the [MIT License](LICENSE). Feel free to use, modify, and
+distribute the code as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy
+your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.4/pytgpt_bot/cli.py` & `pytgpt_bot-0.0.5/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.4/pytgpt_bot/config.py` & `pytgpt_bot-0.0.5/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.0.4/pytgpt_bot/db.py` & `pytgpt_bot-0.0.5/pytgpt_bot/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     def query(sql: str) -> typing.Union[tuple[tuple], typing.NoReturn]:
         """Run sql commands and return entries"""
         conn = sqlite3.connect(path_to_db)
         csr = conn.cursor()
         csr.execute(sql)
         entries = csr.fetchall()
         csr.close()
+        conn.commit()
         conn.close()
         return entries
 
 
 class User(Chat):
     """User chat model"""
```

### Comparing `pytgpt_bot-0.0.4/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.0.5/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Telegram bot for text generation, text-to-image and text-to-audio conversions.
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
@@ -93,15 +93,15 @@
 ### 1. Chat with AI
 
 - **Command**: `/chat`
 - **Description**: Engage in a conversation with AI. This feature allows you to interact with the bot in a natural, conversational manner.
 
 ### 2. Generate Images from Text
 
-- **Command**: `/imager`
+- **Command**: `/image`
 - **Description**: Generate images from text descriptions. This feature uses AI to create visual representations of your text inputs, making it a fun and creative way to explore the capabilities of AI.
 
 - **Variant**: `/prodia`
 - **Description**: Generate images from text descriptions using the Prodia AI model. This variant offers a different style of image generation, providing a unique twist to your creative endeavors.
 
 ### 3. Generate Audio from Text
 
@@ -131,18 +131,33 @@
 ### 8. Echo Your Telegram ID
 
 - **Command**: `/myid`
 - **Description**: Echo your Telegram ID. This feature provides you with your unique Telegram ID, useful for personalized interactions or for troubleshooting purposes and configuring admin.
 
 ### 9. Clear chat data
 
-- **Command**: `/clear_database`
+- **Command**: `/clear_chats`
 - **Description**: This is an administrative command for deleting all entries of chat database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
 
-### 10. Default Chat with AI
+### 10. Check total Chat
+
+- **Command**: `/total_chats`
+- **Description**: This is an administrative command for checking total chat records. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 11. Drop entire chat
+
+- **Command**: `/drop_chats`
+- **Description**: This is an administrative command that **drops** entire chat table and create new one. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 12. Run sql statements
+
+- **Command**: `/sql`
+- **Description**: This is an administrative command for running **SQL STATEMENTS** against the database. The user's Telegram ID must match the one set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+
+### 12. Default Chat with AI
 
 - **Command**: `<Any other text>`
 - **Description**: Engage in a default chat with AI. This command is a shortcut to the `/chat` command, offering a quick and straightforward way to start a conversation with the bot.
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.4 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.0.5 Summary: Telegram bot for
 text generation, text-to-image and text-to-audio conversions. Home-page: https:
 //github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
@@ -39,15 +39,15 @@
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the server
 `python3 run.py`. Alternatively, using CLI interface:: `$ pytgpt-bot run ` ##
 Features ### 1. Chat with AI - **Command**: `/chat` - **Description**: Engage
 in a conversation with AI. This feature allows you to interact with the bot in
 a natural, conversational manner. ### 2. Generate Images from Text -
-**Command**: `/imager` - **Description**: Generate images from text
+**Command**: `/image` - **Description**: Generate images from text
 descriptions. This feature uses AI to create visual representations of your
 text inputs, making it a fun and creative way to explore the capabilities of
 AI. - **Variant**: `/prodia` - **Description**: Generate images from text
 descriptions using the Prodia AI model. This variant offers a different style
 of image generation, providing a unique twist to your creative endeavors. ###
 3. Generate Audio from Text - **Command**: `/audio` - **Description**: Generate
 audio from text. This feature allows you to convert your text inputs into
@@ -64,20 +64,33 @@
 the current chat, allowing you to tailor the conversation to your preferences.
 ### 7. Start New Chat Thread - **Command**: `/reset` - **Description**: Start a
 new chat thread. This feature allows you to begin a fresh conversation with the
 bot, resetting the chat history and allowing for a new start. ### 8. Echo Your
 Telegram ID - **Command**: `/myid` - **Description**: Echo your Telegram ID.
 This feature provides you with your unique Telegram ID, useful for personalized
 interactions or for troubleshooting purposes and configuring admin. ### 9.
-Clear chat data - **Command**: `/clear_database` - **Description**: This is an
+Clear chat data - **Command**: `/clear_chats` - **Description**: This is an
 administrative command for deleting all entries of chat database. The user's
 Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
 pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
-### 10. Default Chat with AI - **Command**: `` - **Description**: Engage in a
-default chat with AI. This command is a shortcut to the `/chat` command,
-offering a quick and straightforward way to start a conversation with the bot.
-## Support and Feedback If you have any questions, feedback, or suggestions for
-`pytgpt`, please feel free to reach out. Your input is valuable in helping us
-improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
-source and available under the [MIT License](LICENSE). Feel free to use,
-modify, and distribute the code as you see fit. --- Thank you for using
-`pytgpt-bot`. Enjoy your AI-powered interactions!
+### 10. Check total Chat - **Command**: `/total_chats` - **Description**: This
+is an administrative command for checking total chat records. The user's
+Telegram ID must match the one set at the [.env](https://github.com/Simatwa/
+pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file.
+### 11. Drop entire chat - **Command**: `/drop_chats` - **Description**: This
+is an administrative command that **drops** entire chat table and create new
+one. The user's Telegram ID must match the one set at the [.env](https://
+github.com/Simatwa/pytgpt-bot/blob/7b1bfed971674be938de2b2163711f6602d54995/
+env#L2) config file. ### 12. Run sql statements - **Command**: `/sql` -
+**Description**: This is an administrative command for running **SQL
+STATEMENTS** against the database. The user's Telegram ID must match the one
+set at the [.env](https://github.com/Simatwa/pytgpt-bot/blob/
+7b1bfed971674be938de2b2163711f6602d54995/env#L2) config file. ### 12. Default
+Chat with AI - **Command**: `` - **Description**: Engage in a default chat with
+AI. This command is a shortcut to the `/chat` command, offering a quick and
+straightforward way to start a conversation with the bot. ## Support and
+Feedback If you have any questions, feedback, or suggestions for `pytgpt`,
+please feel free to reach out. Your input is valuable in helping us improve and
+expand the bot's capabilities. ## License `pytgpt-bot` is open-source and
+available under the [MIT License](LICENSE). Feel free to use, modify, and
+distribute the code as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy
+your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.0.4/setup.py` & `pytgpt_bot-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for text generation, text-to-image and text-to-audio conversions.",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
@@ -35,15 +35,15 @@
     },
     install_requires=[
         "pytelegrambotapi==4.17.0",
         "python-tgpt==0.6.6",
         "python-dotenv==1.0.0",
         "appdirs==1.4.4",
         "click==8.1.3",
-        ],
+    ],
     python_requires=">=3.10",
     keywords=[
         "ai",
         "tgpt",
         "pytgpt",
         "chatbot",
         "telegrambot",
```


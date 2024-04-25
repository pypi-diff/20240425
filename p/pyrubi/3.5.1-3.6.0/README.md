# Comparing `tmp/pyrubi-3.5.1.tar.gz` & `tmp/pyrubi-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-3.5.1.tar", last modified: Sun Feb 11 19:29:29 2024, max compression
+gzip compressed data, was "pyrubi-3.6.0.tar", last modified: Thu Apr 25 16:25:43 2024, max compression
```

## Comparing `pyrubi-3.5.1.tar` & `pyrubi-3.6.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.924883 pyrubi-3.5.1/
--rw-rw-rw-   0        0        0     3103 2024-02-11 19:29:29.916985 pyrubi-3.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1780 2024-02-11 19:28:09.000000 pyrubi-3.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.856787 pyrubi-3.5.1/pyrubi/
--rw-rw-rw-   0        0        0       83 2024-02-11 19:27:49.000000 pyrubi-3.5.1/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.873430 pyrubi-3.5.1/pyrubi/client/
--rw-rw-rw-   0        0        0       26 2023-07-17 19:26:44.000000 pyrubi-3.5.1/pyrubi/client/__init__.py
--rw-rw-rw-   0        0        0    29641 2024-02-11 14:53:55.000000 pyrubi-3.5.1/pyrubi/client/client.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.873430 pyrubi-3.5.1/pyrubi/crypto/
--rw-rw-rw-   0        0        0       28 2023-09-02 10:19:39.000000 pyrubi-3.5.1/pyrubi/crypto/__init__.py
--rw-rw-rw-   0        0        0     2937 2024-02-01 18:58:55.000000 pyrubi-3.5.1/pyrubi/crypto/crypto.py
--rw-rw-rw-   0        0        0     1201 2024-02-04 15:18:44.000000 pyrubi-3.5.1/pyrubi/enums.py
--rw-rw-rw-   0        0        0      696 2024-02-10 07:57:01.000000 pyrubi-3.5.1/pyrubi/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.873430 pyrubi-3.5.1/pyrubi/methods/
--rw-rw-rw-   0        0        0       28 2023-07-18 12:41:47.000000 pyrubi-3.5.1/pyrubi/methods/__init__.py
--rw-rw-rw-   0        0        0    56558 2024-02-11 15:03:58.000000 pyrubi-3.5.1/pyrubi/methods/methods.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.883848 pyrubi-3.5.1/pyrubi/network/
--rw-rw-rw-   0        0        0       84 2024-02-05 14:41:32.000000 pyrubi-3.5.1/pyrubi/network/__init__.py
--rw-rw-rw-   0        0        0      601 2024-02-10 07:29:25.000000 pyrubi-3.5.1/pyrubi/network/helper.py
--rw-rw-rw-   0        0        0     8016 2024-02-11 15:33:22.000000 pyrubi-3.5.1/pyrubi/network/network.py
--rw-rw-rw-   0        0        0     3744 2024-02-11 08:16:34.000000 pyrubi-3.5.1/pyrubi/network/socket.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.886146 pyrubi-3.5.1/pyrubi/sessions/
--rw-rw-rw-   0        0        0       30 2024-02-10 19:01:41.000000 pyrubi-3.5.1/pyrubi/sessions/__init__.py
--rw-rw-rw-   0        0        0     2876 2024-02-05 13:42:29.000000 pyrubi-3.5.1/pyrubi/sessions/sessions.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.886146 pyrubi-3.5.1/pyrubi/types/
--rw-rw-rw-   0        0        0       27 2024-02-11 19:26:40.000000 pyrubi-3.5.1/pyrubi/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.916985 pyrubi-3.5.1/pyrubi/types/socket/
--rw-rw-rw-   0        0        0       28 2024-02-11 19:24:38.000000 pyrubi-3.5.1/pyrubi/types/socket/__init__.py
--rw-rw-rw-   0        0        0     6341 2024-02-10 16:24:28.000000 pyrubi-3.5.1/pyrubi/types/socket/message.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.916985 pyrubi-3.5.1/pyrubi/utils/
--rw-rw-rw-   0        0        0       54 2024-02-10 16:41:57.000000 pyrubi-3.5.1/pyrubi/utils/__init__.py
--rw-rw-rw-   0        0        0     2222 2024-02-11 14:39:45.000000 pyrubi-3.5.1/pyrubi/utils/configs.py
--rw-rw-rw-   0        0        0     8779 2024-02-11 14:44:40.000000 pyrubi-3.5.1/pyrubi/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-11 19:29:29.916985 pyrubi-3.5.1/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     3103 2024-02-11 19:29:29.000000 pyrubi-3.5.1/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      694 2024-02-11 19:29:29.000000 pyrubi-3.5.1/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-11 19:29:29.000000 pyrubi-3.5.1/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-02-11 19:29:29.000000 pyrubi-3.5.1/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-11 19:29:29.000000 pyrubi-3.5.1/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-11 19:29:29.924883 pyrubi-3.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1392 2024-02-11 19:27:59.000000 pyrubi-3.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.820064 pyrubi-3.6.0/
+-rw-rw-rw-   0        0        0     3110 2024-04-25 16:25:43.820064 pyrubi-3.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2024-04-25 16:24:17.000000 pyrubi-3.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.660167 pyrubi-3.6.0/pyrubi/
+-rw-rw-rw-   0        0        0       83 2024-04-25 15:41:51.000000 pyrubi-3.6.0/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.683461 pyrubi-3.6.0/pyrubi/client/
+-rw-rw-rw-   0        0        0       26 2023-07-17 19:26:44.000000 pyrubi-3.6.0/pyrubi/client/__init__.py
+-rw-rw-rw-   0        0        0    30006 2024-04-25 15:40:41.000000 pyrubi-3.6.0/pyrubi/client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.699147 pyrubi-3.6.0/pyrubi/crypto/
+-rw-rw-rw-   0        0        0       28 2023-09-02 10:19:39.000000 pyrubi-3.6.0/pyrubi/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2937 2024-02-01 18:58:55.000000 pyrubi-3.6.0/pyrubi/crypto/crypto.py
+-rw-rw-rw-   0        0        0     1053 2024-04-25 14:54:31.000000 pyrubi-3.6.0/pyrubi/enums.py
+-rw-rw-rw-   0        0        0      696 2024-02-10 07:57:01.000000 pyrubi-3.6.0/pyrubi/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.710230 pyrubi-3.6.0/pyrubi/methods/
+-rw-rw-rw-   0        0        0       28 2023-07-18 12:41:47.000000 pyrubi-3.6.0/pyrubi/methods/__init__.py
+-rw-rw-rw-   0        0        0    59114 2024-04-25 15:04:52.000000 pyrubi-3.6.0/pyrubi/methods/methods.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.731752 pyrubi-3.6.0/pyrubi/network/
+-rw-rw-rw-   0        0        0       84 2024-02-05 14:41:32.000000 pyrubi-3.6.0/pyrubi/network/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-02-10 07:29:25.000000 pyrubi-3.6.0/pyrubi/network/helper.py
+-rw-rw-rw-   0        0        0     8016 2024-02-11 15:33:22.000000 pyrubi-3.6.0/pyrubi/network/network.py
+-rw-rw-rw-   0        0        0     3744 2024-02-11 08:16:34.000000 pyrubi-3.6.0/pyrubi/network/socket.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.750018 pyrubi-3.6.0/pyrubi/sessions/
+-rw-rw-rw-   0        0        0       30 2024-02-10 19:01:41.000000 pyrubi-3.6.0/pyrubi/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2876 2024-02-05 13:42:29.000000 pyrubi-3.6.0/pyrubi/sessions/sessions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.750018 pyrubi-3.6.0/pyrubi/types/
+-rw-rw-rw-   0        0        0       27 2024-02-11 19:26:40.000000 pyrubi-3.6.0/pyrubi/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.771729 pyrubi-3.6.0/pyrubi/types/socket/
+-rw-rw-rw-   0        0        0       28 2024-02-11 19:24:38.000000 pyrubi-3.6.0/pyrubi/types/socket/__init__.py
+-rw-rw-rw-   0        0        0     6866 2024-03-18 13:01:50.000000 pyrubi-3.6.0/pyrubi/types/socket/message.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.810237 pyrubi-3.6.0/pyrubi/utils/
+-rw-rw-rw-   0        0        0       54 2024-02-10 16:41:57.000000 pyrubi-3.6.0/pyrubi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2222 2024-02-11 14:39:45.000000 pyrubi-3.6.0/pyrubi/utils/configs.py
+-rw-rw-rw-   0        0        0     8816 2024-03-18 21:09:50.000000 pyrubi-3.6.0/pyrubi/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:25:43.810237 pyrubi-3.6.0/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     3110 2024-04-25 16:25:43.000000 pyrubi-3.6.0/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2024-04-25 16:25:43.000000 pyrubi-3.6.0/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:25:43.000000 pyrubi-3.6.0/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-25 16:25:43.000000 pyrubi-3.6.0/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 16:25:43.000000 pyrubi-3.6.0/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:25:43.820064 pyrubi-3.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2024-04-25 16:25:03.000000 pyrubi-3.6.0/setup.py
```

### Comparing `pyrubi-3.5.1/PKG-INFO` & `pyrubi-3.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 3.5.1
+Version: 3.6.0
 Summary: This is a powerful and easy library for building self bot in the Rubika.
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
 Keywords: rubika,rubino,pyrubi,pyrubika,bot,chat
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,31 +24,29 @@
 Requires-Dist: urllib3
 Requires-Dist: tqdm
 Requires-Dist: websocket-client
 Requires-Dist: pycryptodome
 Requires-Dist: mutagen
 Requires-Dist: filetype
 
-<p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='pyrubi image' width='270' height=120 class="image">
+<div align='center'>
+    <img style='border-radius: 10px' src='https://iili.io/HIjPRS9.jpg' alt='pyrubi image' width='320' height='140'>
+    <br>
+    <br>
+    <b>Fast & powerfull Rubika API library</b>
     <br>
-    <b>Fast and powerfull Rubika API library</b>
-</p>
-
-<p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubi_documents'>Documents</a>
-</p>
+</div>
 
 
-## Pyrubi 3.5.1
-> Fast and powerfull Rubika API library for building self bots.
-
+# Pyrubi 3.6.0
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/project/pyrubi)
+> Fast and powerfull Rubika API library for building self bots.
 
 
 <hr>
 
 ### Install or Update:
 
 ``` bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 3.5.1 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 3.6.0 Summary: This is a powerful
 and easy library for building self bot in the Rubika. Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
 ali.ganji.za@gmail.com Keywords: rubika,rubino,pyrubi,pyrubika,bot,chat
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -12,19 +12,20 @@
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown Requires-Dist: urllib3 Requires-Dist: tqdm Requires-Dist: websocket-
 client Requires-Dist: pycryptodome Requires-Dist: mutagen Requires-Dist:
 filetype
                                 [pyrubi image]
-                     FFaasstt aanndd ppoowweerrffuullll RRuubbiikkaa AAPPII lliibbrraarryy
+
+                     FFaasstt && ppoowweerrffuullll RRuubbiikkaa AAPPII lliibbrraarryy
                              _G_i_t_H_u_b â¢ _D_o_c_u_m_e_n_t_s
-## Pyrubi 3.5.1 > Fast and powerfull Rubika API library for building self bots.
-[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
-project/pyrubi)
+# Pyrubi 3.6.0 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://
+pepy.tech/project/pyrubi) > Fast and powerfull Rubika API library for building
+self bots.
 ===============================================================================
 ### Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
 ### Quick start: ``` python from pyrubi import Client from pyrubi.types import
 Message client = Client("mySelf") @client.on_message(regexp="hello") def
 send_hello(message: Message): message.reply("**hello** __from__ ##pyrubi##")
 client.run() ``` also you can enter your session data manually: ```python from
```

### Comparing `pyrubi-3.5.1/README.md` & `pyrubi-3.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-<p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='pyrubi image' width='270' height=120 class="image">
+<div align='center'>
+    <img style='border-radius: 10px' src='https://iili.io/HIjPRS9.jpg' alt='pyrubi image' width='320' height='140'>
+    <br>
+    <br>
+    <b>Fast & powerfull Rubika API library</b>
     <br>
-    <b>Fast and powerfull Rubika API library</b>
-</p>
-
-<p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubi_documents'>Documents</a>
-</p>
+</div>
 
 
-## Pyrubi 3.5.1
-> Fast and powerfull Rubika API library for building self bots.
-
+# Pyrubi 3.6.0
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/project/pyrubi)
+> Fast and powerfull Rubika API library for building self bots.
 
 
 <hr>
 
 ### Install or Update:
 
 ``` bash
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                                 [pyrubi image]
-                     FFaasstt aanndd ppoowweerrffuullll RRuubbiikkaa AAPPII lliibbrraarryy
+
+                     FFaasstt && ppoowweerrffuullll RRuubbiikkaa AAPPII lliibbrraarryy
                              _G_i_t_H_u_b â¢ _D_o_c_u_m_e_n_t_s
-## Pyrubi 3.5.1 > Fast and powerfull Rubika API library for building self bots.
-[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
-project/pyrubi)
+# Pyrubi 3.6.0 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://
+pepy.tech/project/pyrubi) > Fast and powerfull Rubika API library for building
+self bots.
 ===============================================================================
 ### Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
 ### Quick start: ``` python from pyrubi import Client from pyrubi.types import
 Message client = Client("mySelf") @client.on_message(regexp="hello") def
 send_hello(message: Message): message.reply("**hello** __from__ ##pyrubi##")
 client.run() ``` also you can enter your session data manually: ```python from
```

### Comparing `pyrubi-3.5.1/pyrubi/client/client.py` & `pyrubi-3.6.0/pyrubi/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,19 +272,19 @@
     
     def send_image(self, object_guid:str, file:str, message_id:str=None, text:str=None, is_spoil:bool=False, thumbnail:str=None, file_name:str=None) -> dict:
         return self.methods.sendImage(objectGuid=object_guid, file=file, text=text, messageId=message_id, isSpoil=is_spoil, thumbInline=thumbnail, fileName=file_name)
     
     def send_video(self, object_guid:str, file:str, message_id:str=None, text:str=None, is_spoil:bool=False, thumbnail:str=None, file_name:str=None) -> dict:
         return self.methods.sendVideo(objectGuid=object_guid, file=file, text=text, messageId=message_id, isSpoil=is_spoil, thumbInline=thumbnail, fileName=file_name)
     
-    def send_video_message(self, object_guid:str, file:str, message_id:str=None, text:str=None, file_name:str=None) -> dict:
-        return self.methods.sendVideoMessage(objectGuid=object_guid, file=file, text=text, messageId=message_id, fileName=file_name)
+    def send_video_message(self, object_guid:str, file:str, message_id:str=None, text:str=None, thumbnail:str=None, file_name:str=None) -> dict:
+        return self.methods.sendVideoMessage(objectGuid=object_guid, file=file, text=text, messageId=message_id, thumbInline=thumbnail, fileName=file_name)
     
-    def send_gif(self, object_guid:str, file:str, message_id:str=None, text:str=None, file_name:str=None) -> dict:
-        return self.methods.sendGif(objectGuid=object_guid, file=file, text=text, messageId=message_id, fileName=file_name)
+    def send_gif(self, object_guid:str, file:str, message_id:str=None, text:str=None, thumbnail:str=None, file_name:str=None) -> dict:
+        return self.methods.sendGif(objectGuid=object_guid, file=file, text=text, messageId=message_id, thumbInline=thumbnail, fileName=file_name)
     
     def send_music(self, object_guid:str, file:str, message_id:str=None, text:str=None, file_name:str=None, performer:str=None) -> dict:
         return self.methods.sendMusic(objectGuid=object_guid, file=file, text=text, messageId=message_id, fileName=file_name, performer=performer)
     
     def send_voice(self, object_guid:str, file:str, message_id:str=None, text:str=None, file_name:str=None, time:int=0) -> dict:
         return self.methods.sendVoice(objectGuid=object_guid, file=file, text=text, messageId=message_id, fileName=file_name, time=time)
     
@@ -320,15 +320,15 @@
     
     def seen_messages(self, object_guid:str, min_id:str, max_id:str) -> dict:
         return self.methods.seenChatMessages(objectGuid=object_guid, minId=min_id, maxId=max_id)
     
     def get_messages_interval(self, object_guid:str, middle_message_id:str) -> dict:
         return self.methods.getMessagesInterval(objectGuid=object_guid, middleMessageId=middle_message_id)
     
-    def get_messages(self, object_guid:str, max_message_id:str, filter_type:str=None, limit:int=50) -> dict:
+    def get_messages(self, object_guid:str, max_message_id:str=None, filter_type:str=None, limit:int=50) -> dict:
         return self.methods.getMessages(objectGuid=object_guid, maxId=max_message_id, filterType=filter_type, limit=limit)
     
     def get_last_message(self, object_guid:str) -> dict:
         return self.methods.getChatInfo(objectGuid=object_guid)["chat"].get("last_message")
     
     def get_last_message_id(self, object_guid:str) -> str:
         return self.methods.getChatInfo(objectGuid=object_guid)["chat"].get("last_message_id")
@@ -493,16 +493,16 @@
     
     def get_two_passcode_status(self) -> dict:
         return self.methods.getTwoPasscodeStatus()
     
     def get_privacy_setting(self) -> dict:
         return self.methods.getPrivacySetting()
     
-    def get_blocked_users(self) -> dict:
-        return self.methods.getBlockedUsers()
+    def get_blocked_users(self, start_id:str=None) -> dict:
+        return self.methods.getBlockedUsers(startId=start_id)
     
     # Other methods
 
     def get_me(self) -> dict:
         return self.methods.getMe()
     
     def transcribe_voice(self, object_guid:str, message_id:str) -> dict:
@@ -534,14 +534,22 @@
     
     def get_download_link(self, object_guid:str=None, message_id:str=None, file_inline:dict=None) -> dict:
         return self.methods.getDownloadLink(objectGuid=object_guid, messageId=message_id, fileInline=file_inline)
     
     def download(self, object_guid:str=None, message_id:str=None, save:bool=False, save_as:str=None, file_inline:dict=None) -> dict:
         return self.methods.download(objectGuid=object_guid, messageId=message_id, save=save, saveAs=save_as, fileInline=file_inline)
     
+    def play_voice(self, object_guid: str, file:str) -> None:
+        from asyncio import run
+        
+        async def main():
+            await self.methods.playVoice(objectGuid=object_guid, file=file)
+
+        run(main())
+    
     def on_message(self, filters:list=[], regexp:str=None):
         def handler(func):
             self.methods.add_handler(
                 func=func,
                 filters=filters,
                 regexp=regexp
             )
```

### Comparing `pyrubi-3.5.1/pyrubi/crypto/crypto.py` & `pyrubi-3.6.0/pyrubi/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/enums.py` & `pyrubi-3.6.0/pyrubi/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-class Enums:
+class SetAdminAccessList:
+    set_admin:str = "SetAdmin"
+    ban_member:str = "BanMember"
+    change_info:str = "ChangeInfo"
+    pin_messages:str = "PinMessages"
+    delete_messages:str = "DeleteGlobalAllMessages"
+    edit_messages:str = "EditMessages"
+    set_join_link:str = "SetJoinLink"
+    set_member_access:str = "SetMemberAccess"
+    delete_global_all_messages:str = "DeleteGlobalAllMessages"
 
-    class SetAdminAccessList:
-        set_admin:str = "SetAdmin"
-        ban_member:str = "BanMember"
-        change_info:str = "ChangeInfo"
-        pin_messages:str = "PinMessages"
-        delete_messages:str = "DeleteGlobalAllMessages"
-        edit_messages:str = "EditMessages"
-        set_join_link:str = "SetJoinLink"
-        set_member_access:str = "SetMemberAccess"
-        delete_global_all_messages:str = "DeleteGlobalAllMessages"
+class SetGroupDefaultAccessList:
+    send_messages:str = "SendMessages"
+    add_member:str = "AddMember"
+    view_admins:str = "ViewAdmins"
+    view_members:str = "ViewMembers"
 
-    class SetGroupDefaultAccessList:
-        send_messages:str = "SendMessages"
-        add_member:str = "AddMember"
-        view_admins:str = "ViewAdmins"
-        view_members:str = "ViewMembers"
+class ChatActivities:
+    typing:str = "Typing"
+    recording:str = "Recording"
+    uploading:str = "Uploading"
 
-    class ChatActivities:
-        typing:str = "Typing"
-        recording:str = "Recording"
-        uploading:str = "Uploading"
-
-    class Filters:
-        user:str = "User"
-        group:str = "Group"
-        channel:str = "Channel"
-        bot:str = "Bot"
-        service:str = "Service"
-        media:str = "Media"
-        file:str = "File"
-        image:str = "Image"
-        video:str = "Video"
-        gif:str = "Gif"
-        music:str = "Music"
-        voice:str = "Voice"
-        sticker:str = "Sticker"
+class Filters:
+    user:str = "User"
+    group:str = "Group"
+    channel:str = "Channel"
+    bot:str = "Bot"
+    service:str = "Service"
+    media:str = "Media"
+    file:str = "File"
+    image:str = "Image"
+    video:str = "Video"
+    gif:str = "Gif"
+    music:str = "Music"
+    voice:str = "Voice"
+    sticker:str = "Sticker"
```

### Comparing `pyrubi-3.5.1/pyrubi/exceptions.py` & `pyrubi-3.6.0/pyrubi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/methods/methods.py` & `pyrubi-3.6.0/pyrubi/methods/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from random import randint
 from ..network import Network, Socket
 from ..crypto import Cryption
 from ..utils import Utils
 from random import choice
 from time import sleep
+from pyrubi.exceptions import InvalidAuth, InvalidInput
+import asyncio
 
 class Methods:
 
     def __init__(self, sessionData:dict, platform:str, apiVersion:int, proxy:str, timeOut:int, showProgressBar:bool) -> None:
         self.platform = platform.lower()
         if not self.platform in ["android", "web", "rubx", "rubikax", "rubino"]:
             print("The \"{}\" is not a valid platform. Choose these one -> (web, android, rubx)".format(platform))
@@ -260,22 +262,22 @@
         chatType:str = Utils.getChatTypeByGuid(objectGuid=objectGuid)
 
         return self.network.request(
             method=f"create{chatType}VoiceChat",
             input={f"{chatType.lower()}_guid": objectGuid}
         )
     
-    def joinVoiceChat(self, objectGuid:str, myGuid:str, voiceChatId:str) -> dict:
+    def joinVoiceChat(self, objectGuid:str, myGuid:str, voiceChatId:str, sdp_offer_data:str) -> dict:
         return self.network.request(
             method=f"join{Utils.getChatTypeByGuid(objectGuid=objectGuid)}VoiceChat",
             input={
                 "chat_guid": objectGuid,
-                "sdp_offer_data": "v=0\no=- -6112403547879777339 2 IN IP4 127.0.0.1\ns=-\nt=0 0\na=group:BUNDLE 0\na=msid-semantic: WMS audio0\nm=audio 9 UDP\\/TLS\\/RTP\\/SAVPF 111\nc=IN IP4 0.0.0.0\na=rtcp:9 IN IP4 0.0.0.0\na=ice-ufrag:IqUf\na=ice-pwd:mwo47t9uImp1xuV9T1HBKcPD\na=ice-options:trickle\na=fingerprint:sha-256 44:84:68:B4:AE:68:1A:2A:D6:35:CB:CF:3F:EA:F6:59:BD:25:1F:E0:B2:35:49:FF:7A:72:80:6F:F4:4D:FC:0D\na=setup:passive\na=mid:0\na=sendrecv\na=msid:audio0 audio0\na=rtcp-mux\na=rtpmap:111 opus\\/48000\\/2\na=rtcp-fb:111 transport-cc\na=fmtp:111 minptime=10;useinbandfec=1\na=rtpmap:110 telephone-event\\/48000\na=ssrc:1343160491\na=ssrc:1343160491 msid:audio0 audio0\na=ssrc:1343160491 mslabel:audio0\na=ssrc:1343160491 label:audio0",
-                "self_object_guid": myGuid,
-                "voice_chat_id": voiceChatId
+                "voice_chat_id": voiceChatId,
+                "sdp_offer_data": sdp_offer_data,
+                "self_object_guid": myGuid
             }
         )
 
     def setChatVoiceChatSetting(self, objectGuid:str, voideChatId:str, title:str, joinMuted:bool) -> dict:
         chatType:str = Utils.getChatTypeByGuid(objectGuid=objectGuid)
 
         input:dict = {
@@ -316,35 +318,36 @@
             method=f"get{chatType}VoiceChatParticipants",
             input={
                 f"{chatType.lower()}_guid": objectGuid,
                 "voice_chat_id": voideChatId,
             }
         )
     
-    def setChatVoiceChatState(self, objectGuid:str, voideChatId:str, activity:str) -> dict:
+    def setChatVoiceChatState(self, objectGuid:str, voideChatId:str, activity:str, participantObjectGuid:str) -> dict:
         chatType:str = Utils.getChatTypeByGuid(objectGuid=objectGuid)
 
         return self.network.request(
-            method=f"get{chatType}VoiceChatState",
+            method=f"set{chatType}VoiceChatState",
             input={
-                f"{chatType.lower()}_guid": objectGuid,
+                "chat_guid": objectGuid,
                 "voice_chat_id": voideChatId,
-                "activity": activity
+                "action": activity,
+                "participant_object_guid": participantObjectGuid
             }
         )
     
     def sendChatVoiceChatActivity(self, objectGuid:str, voideChatId:str, activity:str, participantObjectGuid:str) -> dict:
         chatType:str = Utils.getChatTypeByGuid(objectGuid=objectGuid)
 
         return self.network.request(
-            method=f"get{chatType}VoiceChatActivity",
+            method=f"send{chatType}VoiceChatActivity",
             input={
-                f"{chatType.lower()}_guid": objectGuid,
+                "chat_guid": objectGuid,
                 "voice_chat_id": voideChatId,
-                "action": activity,
+                "activity": activity,
                 "participant_object_guid": participantObjectGuid
             }
         )
     
     def leaveChatVoiceChat(self, objectGuid:str, voideChatId:str) -> dict:
         chatType:str = Utils.getChatTypeByGuid(objectGuid=objectGuid)
 
@@ -822,32 +825,34 @@
             messageId=messageId,
             fileName=fileName,
             type="Video",
             isSpoil=isSpoil,
             customThumbInline=thumbInline
         )
     
-    def sendVideoMessage(self, objectGuid:str, file:str, messageId:str, text:str, fileName:str) -> dict:
+    def sendVideoMessage(self, objectGuid:str, file:str, messageId:str, text:str, thumbInline:str, fileName:str) -> dict:
         return self.baseSendFileInline(
             objectGuid=objectGuid,
             file=file,
             text=text,
             messageId=messageId,
             fileName=fileName,
-            type="VideoMessage"
+            type="VideoMessage",
+            customThumbInline=thumbInline
         )
     
-    def sendGif(self, objectGuid:str, file:str, messageId:str, text:str, fileName:str) -> dict:
+    def sendGif(self, objectGuid:str, file:str, messageId:str, text:str, thumbInline:str, fileName:str) -> dict:
         return self.baseSendFileInline(
             objectGuid=objectGuid,
             file=file,
             text=text,
             messageId=messageId,
             fileName=fileName,
-            type="Gif"
+            type="Gif",
+            customThumbInline=thumbInline
         )
     
     def sendMusic(self, objectGuid:str, file:str, messageId:str, text:str, fileName:str, performer:str) -> dict:
         return self.baseSendFileInline(
             objectGuid=objectGuid,
             file=file,
             text=text,
@@ -904,15 +909,15 @@
             data["metadata"] = {"meta_data_parts": metadata[0]}
         return self.network.request("editMessage", data)
     
     def actionOnMessageReaction(self, objectGuid:str, messageId:str, reactionId:int, action:str) -> dict:
         return self.network.request(
             method="actionOnMessageReaction",
             input={
-                "action": action, #Add #Remove
+                "action": action, #Add OR Remove
                 "object_guid": objectGuid,
                 "message_id": messageId,
                 "reaction_id": reactionId
             }
         )
     
     def setPinMessage(self, objectGuid:str, messageId:str, action:str) -> dict:
@@ -1289,15 +1294,15 @@
     
     def discardCall(self, callId:str, duration:int, reason:str) -> dict:
         return self.network.request(
             method="discardCall",
             input={
                 "call_id": callId,
                 "duration": duration,
-                "reason": reason #Missed #Disconnect
+                "reason": reason #Missed OR Disconnect
             }
         )
     
     # Setting methods
 
     def setSetting(
             self,
@@ -1447,16 +1452,16 @@
     
     def getTwoPasscodeStatus(self) -> dict:
         return self.network.request(method="getTwoPasscodeStatus")
     
     def getPrivacySetting(self) -> dict:
         return self.network.request(method="getPrivacySetting")
     
-    def getBlockedUsers(self) -> dict:
-        return self.network.request(method="getBlockedUsers")
+    def getBlockedUsers(self, startId:str) -> dict:
+        return self.network.request(method="getBlockedUsers", input={"start_id": startId})
     
     # Other methods
 
     def getMe(self) -> dict:
         data:dict = self.network.request(method="getUserInfo")
         data.update(self.sessionData)
         return data
@@ -1542,14 +1547,86 @@
             with open(saveAs or fileInline["file_name"], "wb") as file:
                 file.write(downloadedData)
 
         fileInline["file"] = downloadedData
 
         return fileInline
     
+    async def playVoice(self, objectGuid:str, file: str) -> None:
+        try:
+            from aiortc import RTCPeerConnection, RTCSessionDescription
+            from aiortc.contrib.media import MediaPlayer
+                
+            voiceChatId: str = self.getChatInfo(objectGuid)["chat"].get("group_voice_chat_id")
+
+            if not voiceChatId:
+                voiceChatId:str = self.createChatVoiceChat(objectGuid=objectGuid)["group_voice_chat_update"]["voice_chat_id"]
+
+            rtcConnection = RTCPeerConnection()
+            player: MediaPlayer = MediaPlayer(file)
+            rtcConnection.addTrack(player.audio)
+            spdOffer = await rtcConnection.createOffer()
+            await rtcConnection.setLocalDescription(spdOffer)
+
+            answerSdp = self.joinVoiceChat(
+                objectGuid=objectGuid,
+                myGuid=self.sessionData["user"]["user_guid"],
+                voiceChatId=voiceChatId,
+                sdp_offer_data=spdOffer.sdp
+            )["sdp_answer_data"]
+            
+            self.setChatVoiceChatState(
+                objectGuid=objectGuid,
+                voideChatId=voiceChatId,
+                activity="Unmute",
+                participantObjectGuid=self.sessionData["user"]["user_guid"]
+            )
+
+            remoteDescription = RTCSessionDescription(answerSdp, "answer")
+            await rtcConnection.setRemoteDescription(remoteDescription)
+
+            def onEnded():
+                asyncio.ensure_future(rtcConnection.close())
+
+            player.audio.on("ended", onEnded)
+
+            def keepAlive():
+                while rtcConnection.connectionState != "closed":
+                    try:
+                        if self.sendChatVoiceChatActivity(
+                            objectGuid=objectGuid,
+                            voideChatId=voiceChatId,
+                            activity="Speaking",
+                            participantObjectGuid=self.sessionData["user"]["user_guid"]
+                        )["status"] != "OK":
+                            break
+                        
+                        if self.getChatVoiceChatUpdates(
+                            objectGuid=objectGuid,
+                            voideChatId=voiceChatId
+                        )["status"] != "OK":
+                            break
+
+                        sleep(8)
+                    except (InvalidInput, InvalidAuth):
+                        break
+                    except:
+                        continue
+                
+            from threading import Thread
+            Thread(target=keepAlive, daemon=False).start()
+
+            while rtcConnection.connectionState != "closed":
+                await asyncio.sleep(1)
+
+            asyncio.ensure_future(rtcConnection.close())
+
+        except ImportError:
+            print("The aiortc library is not installed!")
+
     def add_handler(self, func, filters:list, regexp:str) -> None:
         self.socket.addHandler(
             func=func,
             filters=filters,
             regexp=regexp
         )
         return func
```

### Comparing `pyrubi-3.5.1/pyrubi/network/helper.py` & `pyrubi-3.6.0/pyrubi/network/helper.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/network/network.py` & `pyrubi-3.6.0/pyrubi/network/network.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/network/socket.py` & `pyrubi-3.6.0/pyrubi/network/socket.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/sessions/sessions.py` & `pyrubi-3.6.0/pyrubi/sessions/sessions.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/types/socket/message.py` & `pyrubi-3.6.0/pyrubi/types/socket/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+class ReplyInfo:
+    def __init__(self, text, author_guid) -> None:
+        self.text = text
+        self.author_guid = author_guid
+        pass
+
+    @classmethod
+    def from_json(cls, json: dict):
+        return cls(json["text"], json["author_object_guid"])
+
 class Message:
     def __init__(self, data:dict, methods:object) -> None:
         self.data = data
         self.methods = methods
 
     @property
     def object_guid(self) -> str:
@@ -138,14 +148,21 @@
     @property
     def has_link(self) -> bool:
         for link in ["http:/", "https:/", "www.", ".ir", ".com", ".net" "@"]:
             if link in self.text.lower():
                 return True
         return False
     
+    @property
+    def reply_info(self) -> ReplyInfo:
+        if not self.reply_message_id:
+            return
+        
+        return ReplyInfo.from_json(self.methods.getMessagesById(self.object_guid, [self.reply_message_id])["messages"][0])
+    
     def reply(self, text:str) -> dict:
         return self.methods.sendText(objectGuid=self.object_guid, text=text, messageId=self.message_id)
     
     def seen(self) -> dict:
         return self.methods.seenChats(seenList={self.object_guid: self.message_id})
     
     def reaction(self, reaction:int) -> dict:
```

### Comparing `pyrubi-3.5.1/pyrubi/utils/configs.py` & `pyrubi-3.6.0/pyrubi/utils/configs.py`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/pyrubi/utils/utils.py` & `pyrubi-3.6.0/pyrubi/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,16 @@
         return result, real_text
     
     def checkLink(url:str) -> dict:
         for i in ["http:/", "https://"]:
             if url.startswith(i): return True
 
     def getMimeFromByte(bytes:bytes) -> str:
-        return (guess(bytes).extension or "pyrubi")
+        mime = guess(bytes)
+        return "pyrubi" if mime is None else mime.extension
     
     def generateFileName(mime:str) -> str:
         return "Pyrubi Library {}.{}".format(randint(1, 1000), mime)
     
     def getImageSize(bytes:bytes) -> str:
         try:
             from PIL import Image
```

### Comparing `pyrubi-3.5.1/pyrubi.egg-info/PKG-INFO` & `pyrubi-3.6.0/pyrubi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 3.5.1
+Version: 3.6.0
 Summary: This is a powerful and easy library for building self bot in the Rubika.
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
 Keywords: rubika,rubino,pyrubi,pyrubika,bot,chat
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,31 +24,29 @@
 Requires-Dist: urllib3
 Requires-Dist: tqdm
 Requires-Dist: websocket-client
 Requires-Dist: pycryptodome
 Requires-Dist: mutagen
 Requires-Dist: filetype
 
-<p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='pyrubi image' width='270' height=120 class="image">
+<div align='center'>
+    <img style='border-radius: 10px' src='https://iili.io/HIjPRS9.jpg' alt='pyrubi image' width='320' height='140'>
+    <br>
+    <br>
+    <b>Fast & powerfull Rubika API library</b>
     <br>
-    <b>Fast and powerfull Rubika API library</b>
-</p>
-
-<p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubi_documents'>Documents</a>
-</p>
+</div>
 
 
-## Pyrubi 3.5.1
-> Fast and powerfull Rubika API library for building self bots.
-
+# Pyrubi 3.6.0
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/project/pyrubi)
+> Fast and powerfull Rubika API library for building self bots.
 
 
 <hr>
 
 ### Install or Update:
 
 ``` bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 3.5.1 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 3.6.0 Summary: This is a powerful
 and easy library for building self bot in the Rubika. Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
 ali.ganji.za@gmail.com Keywords: rubika,rubino,pyrubi,pyrubika,bot,chat
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -12,19 +12,20 @@
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown Requires-Dist: urllib3 Requires-Dist: tqdm Requires-Dist: websocket-
 client Requires-Dist: pycryptodome Requires-Dist: mutagen Requires-Dist:
 filetype
                                 [pyrubi image]
-                     FFaasstt aanndd ppoowweerrffuullll RRuubbiikkaa AAPPII lliibbrraarryy
+
+                     FFaasstt && ppoowweerrffuullll RRuubbiikkaa AAPPII lliibbrraarryy
                              _G_i_t_H_u_b â¢ _D_o_c_u_m_e_n_t_s
-## Pyrubi 3.5.1 > Fast and powerfull Rubika API library for building self bots.
-[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
-project/pyrubi)
+# Pyrubi 3.6.0 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://
+pepy.tech/project/pyrubi) > Fast and powerfull Rubika API library for building
+self bots.
 ===============================================================================
 ### Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
 ### Quick start: ``` python from pyrubi import Client from pyrubi.types import
 Message client = Client("mySelf") @client.on_message(regexp="hello") def
 send_hello(message: Message): message.reply("**hello** __from__ ##pyrubi##")
 client.run() ``` also you can enter your session data manually: ```python from
```

### Comparing `pyrubi-3.5.1/pyrubi.egg-info/SOURCES.txt` & `pyrubi-3.6.0/pyrubi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrubi-3.5.1/setup.py` & `pyrubi-3.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "pyrubi",
-    version = "3.5.1",
+    version = "3.6.0",
     author="Ali Ganji zadeh",
     author_email = "ali.ganji.za@gmail.com",
     description = "This is a powerful and easy library for building self bot in the Rubika.",
     keywords = ["rubika", "rubino", "pyrubi", "pyrubika", "bot", "chat"],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.7",
     long_description_content_type = "text/markdown",
```


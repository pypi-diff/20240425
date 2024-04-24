# Comparing `tmp/reflex_chat-0.0.1a8.tar.gz` & `tmp/reflex_chat-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_chat-0.0.1a8.tar", last modified: Sat Apr 20 21:08:31 2024, max compression
+gzip compressed data, was "reflex_chat-0.0.2a1.tar", last modified: Wed Apr 24 23:35:20 2024, max compression
```

## Comparing `reflex_chat-0.0.1a8.tar` & `reflex_chat-0.0.2a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:08:31.558884 reflex_chat-0.0.1a8/
--rw-r--r--   0 nikhil     (501) staff       (20)     3797 2024-04-20 21:08:31.558713 reflex_chat-0.0.1a8/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)     3315 2024-04-19 00:01:12.000000 reflex_chat-0.0.1a8/README.md
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:08:31.556542 reflex_chat-0.0.1a8/custom_components/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:08:31.557661 reflex_chat-0.0.1a8/custom_components/reflex_chat/
--rw-r--r--   0 nikhil     (501) staff       (20)       20 2024-04-18 23:20:53.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)     1199 2024-04-20 21:06:33.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat/api.py
--rw-r--r--   0 nikhil     (501) staff       (20)     5077 2024-04-20 20:59:25.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat/chat.py
--rw-r--r--   0 nikhil     (501) staff       (20)     1809 2024-04-18 23:20:53.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat/components.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:08:31.558443 reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/
--rw-r--r--   0 nikhil     (501) staff       (20)     3797 2024-04-20 21:08:31.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)      449 2024-04-20 21:08:31.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/SOURCES.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-20 21:08:31.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/dependency_links.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-20 21:08:31.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/requires.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-20 21:08:31.000000 reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/top_level.txt
--rw-r--r--   0 nikhil     (501) staff       (20)      646 2024-04-20 21:07:36.000000 reflex_chat-0.0.1a8/pyproject.toml
--rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-20 21:08:31.558917 reflex_chat-0.0.1a8/setup.cfg
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-24 23:35:20.108488 reflex_chat-0.0.2a1/
+-rw-r--r--   0 nikhil     (501) staff       (20)     3994 2024-04-24 23:35:20.108264 reflex_chat-0.0.2a1/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)     3438 2024-04-22 21:02:37.000000 reflex_chat-0.0.2a1/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-24 23:35:20.105735 reflex_chat-0.0.2a1/custom_components/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-24 23:35:20.107104 reflex_chat-0.0.2a1/custom_components/reflex_chat/
+-rw-r--r--   0 nikhil     (501) staff       (20)       20 2024-04-18 23:20:53.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     1032 2024-04-22 20:48:37.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat/api.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     5082 2024-04-22 20:51:28.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat/chat.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     1745 2024-04-24 23:32:59.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat/components.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-24 23:35:20.107958 reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)     3994 2024-04-24 23:35:20.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      449 2024-04-24 23:35:20.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-24 23:35:20.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-24 23:35:20.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-24 23:35:20.000000 reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      708 2024-04-24 23:33:23.000000 reflex_chat-0.0.2a1/pyproject.toml
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-24 23:35:20.108525 reflex_chat-0.0.2a1/setup.cfg
```

### Comparing `reflex_chat-0.0.1a8/PKG-INFO` & `reflex_chat-0.0.2a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: reflex-chat
-Version: 0.0.1a8
+Version: 0.0.2a1
 Summary: Reflex custom component chat
-Author-email: nikhil@reflex.dev
+Author-email: Nikhil Rao <nikhil@reflex.dev>
 License: Apache-2.0
-Project-URL: Homepage, https://github.com/picklelo/reflex-chat
+Project-URL: homepage, https://github.com/picklelo/reflex-chat
+Project-URL: source, https://github.com/picklelo/reflex-chat
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: reflex>=0.4.7
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -91,14 +92,16 @@
 chat1 = chat()
 
 @rx.page()
 def index() -> rx.Component:
     return rx.container(
         # Get the messages through chat1.State.messages.
         rx.text("Total Messages: ", chat1.State.messages.length()),
+        # Get the last user message through chat1.State.last_user_message.
+        rx.text(chat1.State.last_user_message),
         rx.hstack(
             chat1,
             height="100vh",
         ),
         # Get the processing state through chat1.State.processing.
         background_color=rx.cond(chat1.State.processing, "gray", "white"),
         size="4",
```

### Comparing `reflex_chat-0.0.1a8/README.md` & `reflex_chat-0.0.2a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 chat1 = chat()
 
 @rx.page()
 def index() -> rx.Component:
     return rx.container(
         # Get the messages through chat1.State.messages.
         rx.text("Total Messages: ", chat1.State.messages.length()),
+        # Get the last user message through chat1.State.last_user_message.
+        rx.text(chat1.State.last_user_message),
         rx.hstack(
             chat1,
             height="100vh",
         ),
         # Get the processing state through chat1.State.processing.
         background_color=rx.cond(chat1.State.processing, "gray", "white"),
         size="4",
```

### Comparing `reflex_chat-0.0.1a8/custom_components/reflex_chat/api.py` & `reflex_chat-0.0.2a1/custom_components/reflex_chat/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 """Define common AI API functions."""
 
 import os
 
-try:
-    from openai import OpenAI
-
-    client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
-except ImportError:
-    print("OpenAI is not installed. Please install it with `pip install openai`.")
-
 
 async def default_process(chat):
     """Process the chat messages.
 
     Args:
         chat: The chat object.
     """
@@ -27,14 +20,15 @@
     model=os.getenv("OPENAI_MODEL", "gpt-3.5-turbo"),
 ):
     """Get the response from the API.
 
     Args:
         form_data: A dict with the current question.
     """
+    from openai import OpenAI
     client = client or OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
 
     async def process(chat):
         # Start a new session to answer the question.
         session = client.chat.completions.create(
             model=model,
             messages=chat.get_messages(),
```

### Comparing `reflex_chat-0.0.1a8/custom_components/reflex_chat/chat.py` & `reflex_chat-0.0.2a1/custom_components/reflex_chat/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,8 +153,8 @@
             answer: The answer to add to the chat history.
         """
         self.messages[-1]["content"] += answer or ""
 
 
 chat = Chat.create
 
-chat()
+c1 = chat()
```

### Comparing `reflex_chat-0.0.1a8/custom_components/reflex_chat/components.py` & `reflex_chat-0.0.2a1/custom_components/reflex_chat/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,17 @@
     )
 
 
 def action_bar(ChatState) -> rx.Component:
     """The action bar to send a new message."""
     return rx.form(
         rx.hstack(
-            rx.input.root(
-                rx.input.input(
-                    placeholder="Type something...",
-                    id=ChatState.__name__,
-                ),
+            rx.input(
+                placeholder="Type something...",
+                id=ChatState.__name__,
                 width="100%",
             ),
             rx.spacer(),
             rx.button(
                 "Send",
                 type="submit",
             ),
```

### Comparing `reflex_chat-0.0.1a8/custom_components/reflex_chat.egg-info/PKG-INFO` & `reflex_chat-0.0.2a1/custom_components/reflex_chat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: reflex-chat
-Version: 0.0.1a8
+Version: 0.0.2a1
 Summary: Reflex custom component chat
-Author-email: nikhil@reflex.dev
+Author-email: Nikhil Rao <nikhil@reflex.dev>
 License: Apache-2.0
-Project-URL: Homepage, https://github.com/picklelo/reflex-chat
+Project-URL: homepage, https://github.com/picklelo/reflex-chat
+Project-URL: source, https://github.com/picklelo/reflex-chat
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: reflex>=0.4.7
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -91,14 +92,16 @@
 chat1 = chat()
 
 @rx.page()
 def index() -> rx.Component:
     return rx.container(
         # Get the messages through chat1.State.messages.
         rx.text("Total Messages: ", chat1.State.messages.length()),
+        # Get the last user message through chat1.State.last_user_message.
+        rx.text(chat1.State.last_user_message),
         rx.hstack(
             chat1,
             height="100vh",
         ),
         # Get the processing state through chat1.State.processing.
         background_color=rx.cond(chat1.State.processing, "gray", "white"),
         size="4",
```

### Comparing `reflex_chat-0.0.1a8/pyproject.toml` & `reflex_chat-0.0.2a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-chat"
-version = "0.0.1a8"
+version = "0.0.2a1"
 description = "Reflex custom component chat"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
-authors = [{ name = "", email = "nikhil@reflex.dev" }]
+authors = [{ name = "Nikhil Rao", email = "nikhil@reflex.dev" }]
 keywords = ["reflex","reflex-custom-components"]
 
 dependencies = ["reflex>=0.4.7"]
 
 classifiers = ["Development Status :: 4 - Beta"]
 
 [project.urls]
-Homepage = "https://github.com/picklelo/reflex-chat"
+homepage = "https://github.com/picklelo/reflex-chat"
+source = "https://github.com/picklelo/reflex-chat"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
+
 [tool.setuptools.packages.find]
 where = ["custom_components"]
```


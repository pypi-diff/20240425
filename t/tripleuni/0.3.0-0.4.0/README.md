# Comparing `tmp/tripleuni-0.3.0.tar.gz` & `tmp/tripleuni-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripleuni-0.3.0.tar", last modified: Sat Mar 30 15:15:41 2024, max compression
+gzip compressed data, was "tripleuni-0.4.0.tar", last modified: Thu Apr 25 07:29:48 2024, max compression
```

## Comparing `tripleuni-0.3.0.tar` & `tripleuni-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 15:15:41.655452 tripleuni-0.3.0/
--rw-rw-rw-   0        0        0     1100 2024-02-05 11:55:03.000000 tripleuni-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4336 2024-03-30 15:15:41.654059 tripleuni-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2037 2024-03-28 10:27:06.000000 tripleuni-0.3.0/README.md
--rw-rw-rw-   0        0        0     6078 2024-03-28 09:30:40.000000 tripleuni-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 15:15:41.655452 tripleuni-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 15:15:41.603262 tripleuni-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 15:15:41.624129 tripleuni-0.3.0/src/tripleuni/
--rw-rw-rw-   0        0        0       74 2024-03-28 09:56:32.000000 tripleuni-0.3.0/src/tripleuni/ChatBot.py
--rw-rw-rw-   0        0        0     9125 2024-03-30 15:15:12.000000 tripleuni-0.3.0/src/tripleuni/TripleClient.py
--rw-rw-rw-   0        0        0       47 2024-03-25 11:26:31.000000 tripleuni-0.3.0/src/tripleuni/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 15:15:41.652048 tripleuni-0.3.0/src/tripleuni.egg-info/
--rw-rw-rw-   0        0        0     4336 2024-03-30 15:15:41.000000 tripleuni-0.3.0/src/tripleuni.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-03-30 15:15:41.000000 tripleuni-0.3.0/src/tripleuni.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 15:15:41.000000 tripleuni-0.3.0/src/tripleuni.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-30 15:15:41.000000 tripleuni-0.3.0/src/tripleuni.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-30 15:15:41.000000 tripleuni-0.3.0/src/tripleuni.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-30 15:15:41.650050 tripleuni-0.3.0/tests/
--rw-rw-rw-   0        0        0      353 2024-03-25 14:05:21.000000 tripleuni-0.3.0/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:48.597846 tripleuni-0.4.0/
+-rw-rw-rw-   0        0        0     1100 2024-02-05 11:55:03.000000 tripleuni-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4336 2024-04-25 07:29:48.595849 tripleuni-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2037 2024-03-28 10:27:06.000000 tripleuni-0.4.0/README.md
+-rw-rw-rw-   0        0        0     6078 2024-04-25 07:25:52.000000 tripleuni-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:29:48.597846 tripleuni-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:48.555261 tripleuni-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:48.565681 tripleuni-0.4.0/src/tripleuni/
+-rw-rw-rw-   0        0        0       74 2024-03-28 09:56:32.000000 tripleuni-0.4.0/src/tripleuni/ChatBot.py
+-rw-rw-rw-   0        0        0     9943 2024-04-25 07:28:19.000000 tripleuni-0.4.0/src/tripleuni/TripleClient.py
+-rw-rw-rw-   0        0        0       47 2024-03-25 11:26:31.000000 tripleuni-0.4.0/src/tripleuni/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:48.594846 tripleuni-0.4.0/src/tripleuni.egg-info/
+-rw-rw-rw-   0        0        0     4336 2024-04-25 07:29:48.000000 tripleuni-0.4.0/src/tripleuni.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-04-25 07:29:48.000000 tripleuni-0.4.0/src/tripleuni.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:29:48.000000 tripleuni-0.4.0/src/tripleuni.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-25 07:29:48.000000 tripleuni-0.4.0/src/tripleuni.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 07:29:48.000000 tripleuni-0.4.0/src/tripleuni.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:48.592839 tripleuni-0.4.0/tests/
+-rw-rw-rw-   0        0        0      353 2024-03-25 14:05:21.000000 tripleuni-0.4.0/tests/test_simple.py
```

### Comparing `tripleuni-0.3.0/LICENSE.txt` & `tripleuni-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tripleuni-0.3.0/PKG-INFO` & `tripleuni-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tripleuni
-Version: 0.3.0
+Version: 0.4.0
 Summary: python library for tripleuni
 Author-email: Zilong ZHOU <zzl0712@outlook.com>
 Maintainer-email: Zilong ZHOU <zzl0712@outlook.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `tripleuni-0.3.0/README.md` & `tripleuni-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tripleuni-0.3.0/pyproject.toml` & `tripleuni-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "tripleuni"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.3.0"  # Required
+version = "0.4.0"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "python library for tripleuni"  # Required
 
 # This is an optional longer description of your project that represents
```

### Comparing `tripleuni-0.3.0/src/tripleuni/TripleClient.py` & `tripleuni-0.4.0/src/tripleuni/TripleClient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,49 @@
 import requests
+import os
 
 
 class TripleClient:
-    def __init__(self, token: str = None):
+    def __init__(self, token: str = None, domain: str = "uuunnniii", version: str = "v4"):
         self.session: requests.Session = requests.Session()
         self.if_login: bool = False if token is None else True
         self.stored_data: dict = {}
         self.token: str = token
+        self.domain: str = domain
+        self.version: str = version
+
+    def checkToken(self) -> bool:
+        """
+        Check if the token is valid
+        :return: bool
+        """
+        post_data = {
+            "token": self.token,
+            "language": "zh-CN"
+        }
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/post/list/all.php", data=post_data)
+
+        if post_response.status_code == 200:
+            post_response_data = post_response.json()
+            if post_response_data['code'] == 200:
+                return True
+
+        return False
 
     def sendVerification(self, email: str) -> dict:
         """
         Send a verification code to the email
         :param email:
         :return: bool
         """
         email_data = {
             "user_email": email,
             "language": "zh-CN"
         }
-        email_response = self.session.post("https://api.tripleuni.com/v4/user/register/web/email.php", data=email_data)
+        email_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/user/register/web/email.php", data=email_data)
 
         if email_response.status_code == 200:
             email_response_data = email_response.json()
             if email_response_data['code'] == 200:
                 self.stored_data = email_response_data
 
             return email_response_data
@@ -40,15 +61,15 @@
             "vcode_vcode": vcode,
             "vcode_key": stored_data['vcode_key'],
             "user_itsc": stored_data['user_itsc'],
             "user_email_suffix": stored_data['user_email_suffix'],
             "user_school_label": stored_data['user_school_label'],
             "language": "zh-CN"
         }
-        varify_response = self.session.post("https://api.tripleuni.com/v4/user/register/web/verify.php",
+        varify_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/user/register/web/verify.php",
                                             data=verify_data)
 
         if varify_response.status_code == 200:
             varify_response_data = varify_response.json()
             if varify_response_data['code'] == 200:
                 self.token = varify_response_data['token']
 
@@ -63,15 +84,15 @@
         :return: response data in dict or {}
         """
         post_data = {
             "token": self.token,
             "page": page,
             "language": "zh-CN"
         }
-        post_response = self.session.post("https://api.tripleuni.com/v4/post/list/all.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/post/list/all.php", data=post_data)
 
         if post_response.status_code == 200:
             post_response_data = post_response.json()
             if post_response_data['code'] == 200:
                 return post_response_data
 
         return {}
@@ -88,15 +109,15 @@
             "token": self.token,
             "uni_post_id": uniPostId,
             "comment_msg": msg,
             "language": "zh-CN",
             "user_is_real_name": real_name
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/comment/post.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/comment/post.php", data=post_data)
 
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def createChatSession(self, uni_post_id: int, real_name: str = 'false') -> dict:
@@ -111,15 +132,15 @@
             "uni_post_id": uni_post_id,
             "language": "zh-CN",
             "to_type": "post",
             "sender_is_real_name": real_name,
             "comment_order": "null"
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/pm/chat/create.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/pm/chat/create.php", data=post_data)
 
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def sendChatMsg(self, chat_id: int, msg: str) -> dict:
@@ -132,15 +153,15 @@
         post_data = {
             "token": self.token,
             "chat_id": chat_id,
             "pm_msg": msg,
             "language": "zh-CN"
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/pm/message/send.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/pm/message/send.php", data=post_data)
 
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def sendChatMsgToPost(self, uni_post_id: int, msg: str, real_name: str = 'false') -> dict:
@@ -168,15 +189,15 @@
             "uni_post_id": uni_post_id,
             "comment_msg": msg,
             "language": "zh-CN",
             "user_is_real_name": real_name,
             "comment_father_id": comment_father_id
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/comment/post.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/comment/post.php", data=post_data)
 
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def followPost(self, uni_post_id: int) -> dict:
@@ -189,15 +210,15 @@
         """
         post_data = {
             "token": self.token,
             "uni_post_id": uni_post_id,
             "language": "zh-CN"
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/post/single/follow.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/post/single/follow.php", data=post_data)
 
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def reportPost(self, uni_post_id: int, comment_order: int, comment_msg: str, report_msg: str) -> dict:
@@ -214,15 +235,15 @@
             "uni_post_id": uni_post_id,
             "comment_order": comment_order,
             "comment_msg": comment_msg,
             "report_msg": report_msg,
             "language": "zh-CN"
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/post/single/report.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/post/single/report.php", data=post_data)
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def getDetail(self, uni_post_id: int) -> dict:
         """
@@ -232,15 +253,15 @@
         """
         post_data = {
             "token": self.token,
             "uni_post_id": uni_post_id,
             "language": "zh-CN"
         }
 
-        post_response = self.session.post("https://api.tripleuni.com/v4/post/single/get.php", data=post_data)
+        post_response = self.session.post(f"https://api.{self.domain}.com/{self.version}/post/single/get.php", data=post_data)
         if post_response.status_code == 200:
             return post_response.json()
 
         return {}
 
     def streamWithChatbot(self, msg: str, history: str = "[]"):
         """
@@ -254,15 +275,15 @@
 
         params = {
             "token": self.token,
             "question": msg,
             "history": history,
         }
 
-        response = self.session.get("https://chat.tripleuni.com", params=params, stream=True)
+        response = self.session.get(f"https://chat.{self.domain}.com", params=params, stream=True)
         for line in response.iter_lines():
             line = line.decode("utf-8")
 
             if line.startswith("event: close"):
                 break
 
             if line.startswith("data:"):
@@ -280,10 +301,9 @@
 
 if __name__ == "__main__":
     import os
 
     token = os.getenv("TRIPLE_TOKEN")
     client = TripleClient(token)
 
-    code = client.chatWithChatbot("一加一等于多少")
-    print(code)
+    print(client.checkToken())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tripleuni-0.3.0/src/tripleuni.egg-info/PKG-INFO` & `tripleuni-0.4.0/src/tripleuni.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tripleuni
-Version: 0.3.0
+Version: 0.4.0
 Summary: python library for tripleuni
 Author-email: Zilong ZHOU <zzl0712@outlook.com>
 Maintainer-email: Zilong ZHOU <zzl0712@outlook.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```


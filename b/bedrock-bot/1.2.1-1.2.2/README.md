# Comparing `tmp/bedrock_bot-1.2.1.tar.gz` & `tmp/bedrock_bot-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.2.1.tar", max compression
+gzip compressed data, was "bedrock_bot-1.2.2.tar", max compression
```

## Comparing `bedrock_bot-1.2.1.tar` & `bedrock_bot-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/README.md
--rw-r--r--   0        0        0      120 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     3991 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/cli.py
--rw-r--r--   0        0        0      143 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/models/__init__.py
--rw-r--r--   0        0        0     2142 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/models/base_model.py
--rw-r--r--   0        0        0     1476 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/models/claude.py
--rw-r--r--   0        0        0     1149 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/models/mistral.py
--rw-r--r--   0        0        0      175 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-23 12:26:02.132701 bedrock_bot-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/README.md
+-rw-r--r--   0        0        0      120 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     4018 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/cli.py
+-rw-r--r--   0        0        0      143 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/__init__.py
+-rw-r--r--   0        0        0     2146 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/base_model.py
+-rw-r--r--   0        0        0     1476 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/claude.py
+-rw-r--r--   0        0        0     1149 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/mistral.py
+-rw-r--r--   0        0        0      175 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/util.py
+-rw-r--r--   0        0        0      470 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.2.2/PKG-INFO
```

### Comparing `bedrock_bot-1.2.1/LICENSE` & `bedrock_bot-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.1/README.md` & `bedrock_bot-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.1/bedrock_bot/cli.py` & `bedrock_bot-1.2.2/bedrock_bot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     return user_input
 
 
 def handle_input_files(input_file) -> list:
     output = []
     if input_file:
         for file in input_file:
-            output.append(file.read())
+            output.append(f"File '{file.name}':\n" + file.read())
     return output
 
 
 @click.command()
 @click.argument("args", nargs=-1)
 @click.option(
     "-r",
```

### Comparing `bedrock_bot-1.2.1/bedrock_bot/models/base_model.py` & `bedrock_bot-1.2.2/bedrock_bot/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 
     def append_message(self, role: ConversationRole, message: str):
         self.messages.append({"role": role.value, "content": message})
 
     def invoke(self, message: str):
         self.append_message(ConversationRole.USER, message)
 
-        logger.info(f"Sending current messages to AI: {self.messages}")
         response = self._invoke()
         self.append_message(ConversationRole.ASSISTANT, response)
         return response
 
     def _create_invoke_body(self) -> dict:
         raise NotImplementedError
 
     def _handle_response(self, body) -> str:
         raise NotImplementedError
 
     def _invoke(self):
         body = self._create_invoke_body() | self.model_params
 
         with console.status("[bold green]Waiting for response..."):
+            logger.info(f"Sending current messages to AI: {self.messages}")
             response = self._bedrock.invoke_model(
                 modelId=self._model_id, body=json.dumps(body)
             )
             body = json.loads(response["body"].read())
 
             output = self._handle_response(body)
```

### Comparing `bedrock_bot-1.2.1/bedrock_bot/models/claude.py` & `bedrock_bot-1.2.2/bedrock_bot/models/claude.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.1/bedrock_bot/models/mistral.py` & `bedrock_bot-1.2.2/bedrock_bot/models/mistral.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.1/PKG-INFO` & `bedrock_bot-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


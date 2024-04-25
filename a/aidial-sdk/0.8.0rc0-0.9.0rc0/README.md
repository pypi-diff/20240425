# Comparing `tmp/aidial_sdk-0.8.0rc0.tar.gz` & `tmp/aidial_sdk-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aidial_sdk-0.8.0rc0.tar", max compression
+gzip compressed data, was "aidial_sdk-0.9.0rc0.tar", max compression
```

## Comparing `aidial_sdk-0.8.0rc0.tar` & `aidial_sdk-0.9.0rc0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0    11348 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/LICENSE
--rw-r--r--   0        0        0     3849 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/README.md
--rw-r--r--   0        0        0      135 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/__init__.py
--rw-r--r--   0        0        0     7893 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/application.py
--rw-r--r--   0        0        0      802 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/__init__.py
--rw-r--r--   0        0        0     1032 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/base.py
--rw-r--r--   0        0        0     5997 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/choice.py
--rw-r--r--   0        0        0      524 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/choice_base.py
--rw-r--r--   0        0        0    13174 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/chunks.py
--rw-r--r--   0        0        0      266 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/enums.py
--rw-r--r--   0        0        0     1450 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/function_call.py
--rw-r--r--   0        0        0     1479 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/function_tool_call.py
--rw-r--r--   0        0        0     3389 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/request.py
--rw-r--r--   0        0        0    12242 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/response.py
--rw-r--r--   0        0        0     3914 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/stage.py
--rw-r--r--   0        0        0        0 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/deployment/__init__.py
--rw-r--r--   0        0        0     2288 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/deployment/from_request_mixin.py
--rw-r--r--   0        0        0      255 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/deployment/rate.py
--rw-r--r--   0        0        0      912 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/deployment/tokenize.py
--rw-r--r--   0        0        0      705 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/deployment/truncate_prompt.py
--rw-r--r--   0        0        0      914 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/exceptions.py
--rw-r--r--   0        0        0     3068 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/header_propagator.py
--rw-r--r--   0        0        0      114 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/pydantic_v1/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/telemetry/__init__.py
--rw-r--r--   0        0        0     2565 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/telemetry/init.py
--rw-r--r--   0        0        0      382 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/telemetry/types.py
--rw-r--r--   0        0        0        0 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/__init__.py
--rw-r--r--   0        0        0      834 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/errors.py
--rw-r--r--   0        0        0       92 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/json.py
--rw-r--r--   0        0        0      835 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/log_config.py
--rw-r--r--   0        0        0      823 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/logging.py
--rw-r--r--   0        0        0     4912 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/merge_chunks.py
--rw-r--r--   0        0        0      125 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/pydantic.py
--rw-r--r--   0        0        0      720 2024-03-08 11:42:26.247050 aidial_sdk-0.8.0rc0/aidial_sdk/utils/streaming.py
--rw-r--r--   0        0        0     3052 2024-03-08 11:42:34.102975 aidial_sdk-0.8.0rc0/pyproject.toml
--rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 aidial_sdk-0.8.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/LICENSE
+-rw-r--r--   0        0        0     3849 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/README.md
+-rw-r--r--   0        0        0      135 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/__init__.py
+-rw-r--r--   0        0        0     7893 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/application.py
+-rw-r--r--   0        0        0      802 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/__init__.py
+-rw-r--r--   0        0        0     1032 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/base.py
+-rw-r--r--   0        0        0     5997 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/choice.py
+-rw-r--r--   0        0        0      524 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/choice_base.py
+-rw-r--r--   0        0        0    13174 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/chunks.py
+-rw-r--r--   0        0        0      266 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/enums.py
+-rw-r--r--   0        0        0     1450 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/function_call.py
+-rw-r--r--   0        0        0     1479 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/function_tool_call.py
+-rw-r--r--   0        0        0     3391 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/request.py
+-rw-r--r--   0        0        0    12242 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/response.py
+-rw-r--r--   0        0        0     3914 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/stage.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/deployment/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/deployment/from_request_mixin.py
+-rw-r--r--   0        0        0      255 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/deployment/rate.py
+-rw-r--r--   0        0        0      912 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/deployment/tokenize.py
+-rw-r--r--   0        0        0      705 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/deployment/truncate_prompt.py
+-rw-r--r--   0        0        0      914 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/exceptions.py
+-rw-r--r--   0        0        0     3068 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/header_propagator.py
+-rw-r--r--   0        0        0      114 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/telemetry/__init__.py
+-rw-r--r--   0        0        0     3799 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/telemetry/init.py
+-rw-r--r--   0        0        0     1557 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/telemetry/types.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/env.py
+-rw-r--r--   0        0        0      834 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/errors.py
+-rw-r--r--   0        0        0       92 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/json.py
+-rw-r--r--   0        0        0      835 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/log_config.py
+-rw-r--r--   0        0        0      823 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/logging.py
+-rw-r--r--   0        0        0     4912 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/merge_chunks.py
+-rw-r--r--   0        0        0      125 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/pydantic.py
+-rw-r--r--   0        0        0      720 2024-04-25 15:10:15.819030 aidial_sdk-0.9.0rc0/aidial_sdk/utils/streaming.py
+-rw-r--r--   0        0        0     3057 2024-04-25 15:10:25.243073 aidial_sdk-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 aidial_sdk-0.9.0rc0/PKG-INFO
```

### Comparing `aidial_sdk-0.8.0rc0/LICENSE` & `aidial_sdk-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/README.md` & `aidial_sdk-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/application.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/application.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/__init__.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/__init__.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/base.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/base.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/choice.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/choice.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/choice_base.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/choice_base.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/chunks.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/chunks.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/function_call.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/function_call.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/function_tool_call.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/function_tool_call.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/request.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,17 +107,17 @@
     function: FunctionChoice
 
 
 class AzureChatCompletionRequest(ExtraForbidModel):
     model: Optional[StrictStr] = None
     messages: List[Message]
     functions: Optional[List[Function]] = None
-    function_call: Optional[
-        Union[Literal["auto", "none"], FunctionChoice]
-    ] = None
+    function_call: Optional[Union[Literal["auto", "none"], FunctionChoice]] = (
+        None
+    )
     tools: Optional[List[Tool]] = None
     tool_choice: Optional[Union[Literal["auto", "none"], ToolChoice]] = None
     addons: Optional[List[Addon]] = None
     stream: bool = False
     temperature: Optional[Temperature] = None
     top_p: Optional[TopP] = None
     n: Optional[N] = None
```

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/response.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/response.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/chat_completion/stage.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/chat_completion/stage.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/deployment/from_request_mixin.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/deployment/from_request_mixin.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/deployment/tokenize.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/deployment/tokenize.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/deployment/truncate_prompt.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/deployment/truncate_prompt.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/exceptions.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/header_propagator.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/header_propagator.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/utils/errors.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/utils/errors.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/utils/log_config.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/utils/logging.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/utils/logging.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/utils/merge_chunks.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/utils/merge_chunks.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/aidial_sdk/utils/streaming.py` & `aidial_sdk-0.9.0rc0/aidial_sdk/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `aidial_sdk-0.8.0rc0/pyproject.toml` & `aidial_sdk-0.9.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aidial-sdk"
-version = "0.8.0rc"
+version = "0.9.0rc"
 description = "Framework to create applications and model adapters for AI DIAL"
 authors = ["EPAM RAIL <SpecialEPM-DIALDevTeam@epam.com>"]
 homepage = "https://epam-rail.com"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/epam/ai-dial-sdk"
 
@@ -54,15 +54,15 @@
 httpx = "^0.25.0"
 nox = "^2023.4.22"
 pillow = "^10.2.0"
 aiohttp = "^3.9.0"
 
 [tool.poetry.group.lint.dependencies]
 flake8 = "^6.0.0"
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 isort = "^5.12.0"
 pyright = "^1.1.324"
 autoflake = "^2.2.0"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests"
```

### Comparing `aidial_sdk-0.8.0rc0/PKG-INFO` & `aidial_sdk-0.9.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aidial-sdk
-Version: 0.8.0rc0
+Version: 0.9.0rc0
 Summary: Framework to create applications and model adapters for AI DIAL
 Home-page: https://epam-rail.com
 License: Apache-2.0
 Author: EPAM RAIL
 Author-email: SpecialEPM-DIALDevTeam@epam.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


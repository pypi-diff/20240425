# Comparing `tmp/langchain_upstage-0.1.1.tar.gz` & `tmp/langchain_upstage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.1.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.2.tar", max compression
```

## Comparing `langchain_upstage-0.1.1.tar` & `langchain_upstage-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/LICENSE
--rw-r--r--   0        0        0      979 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/README.md
--rw-r--r--   0        0        0      496 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9097 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0     6430 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/layout_analysis.py
--rw-r--r--   0        0        0    12390 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/layout_analysis_parsers.py
--rw-r--r--   0        0        0        0 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/py.typed
--rw-r--r--   0        0        0     3328 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/tools/groundedness_check.py
--rw-r--r--   0        0        0     2727 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/LICENSE
+-rw-r--r--   0        0        0      979 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/README.md
+-rw-r--r--   0        0        0      496 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9097 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0     6430 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/layout_analysis.py
+-rw-r--r--   0        0        0    12390 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/layout_analysis_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     3574 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/langchain_upstage/tools/groundedness_check.py
+-rw-r--r--   0        0        0     2727 2024-04-25 17:41:56.353300 langchain_upstage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.2/PKG-INFO
```

### Comparing `langchain_upstage-0.1.1/LICENSE` & `langchain_upstage-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.1/README.md` & `langchain_upstage-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.1/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.2/langchain_upstage/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.1/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.2/langchain_upstage/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.1/langchain_upstage/layout_analysis.py` & `langchain_upstage-0.1.2/langchain_upstage/layout_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.1/langchain_upstage/layout_analysis_parsers.py` & `langchain_upstage-0.1.2/langchain_upstage/layout_analysis_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.1/langchain_upstage/tools/groundedness_check.py` & `langchain_upstage-0.1.2/langchain_upstage/tools/groundedness_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
-from typing import Literal, Optional, Type, Union
+from typing import Any, Literal, Optional, Type, Union
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForToolRun,
     CallbackManagerForToolRun,
 )
 from langchain_core.messages import AIMessage, HumanMessage
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr
 from langchain_core.tools import BaseTool
+from langchain_core.utils import convert_to_secret_str
 
 from langchain_upstage import ChatUpstage
 
 
 class GroundednessCheckInput(BaseModel):
     """Input for the Groundedness Check tool."""
 
@@ -47,19 +48,22 @@
         "the assistant's message is grounded in the provided context."
     )
     upstage_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     api_wrapper: ChatUpstage
 
     args_schema: Type[BaseModel] = GroundednessCheckInput
 
-    def __init__(self, upstage_api_key: Optional[SecretStr] = None):
+    def __init__(self, **kwargs: Any) -> None:
+        upstage_api_key = kwargs.get("upstage_api_key", None)
+        if not upstage_api_key:
+            upstage_api_key = kwargs.get("api_key", None)
         if not upstage_api_key:
             upstage_api_key = SecretStr(os.getenv("UPSTAGE_API_KEY", ""))
-        else:
-            upstage_api_key = upstage_api_key
+        upstage_api_key = convert_to_secret_str(upstage_api_key)
+
         if (
             not upstage_api_key
             or not upstage_api_key.get_secret_value()
             or upstage_api_key.get_secret_value() == ""
         ):
             raise ValueError("UPSTAGE_API_KEY must be set or passed")
 
@@ -72,20 +76,22 @@
     def _run(
         self,
         context: str,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> Union[str, Literal["grounded", "notGrounded", "notSure"]]:
         """Use the tool."""
-        response = self.api_wrapper.invoke([HumanMessage(context), AIMessage(query)])
+        response = self.api_wrapper.invoke(
+            [HumanMessage(context), AIMessage(query)], stream=False
+        )
         return str(response.content)
 
     async def _arun(
         self,
         context: str,
         query: str,
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> Union[str, Literal["grounded", "notGrounded", "notSure"]]:
         response = await self.api_wrapper.ainvoke(
-            [HumanMessage(context), AIMessage(query)]
+            [HumanMessage(context), AIMessage(query)], stream=False
         )
         return str(response.content)
```

### Comparing `langchain_upstage-0.1.1/pyproject.toml` & `langchain_upstage-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-upstage"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting Upstage and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_upstage-0.1.1/PKG-INFO` & `langchain_upstage-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.1
+Version: 0.1.2
 Summary: An integration package connecting Upstage and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/openai_responses-0.1.1.tar.gz` & `tmp/openai_responses-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.1.1.tar", max compression
+gzip compressed data, was "openai_responses-0.2.0.tar", max compression
```

## Comparing `openai_responses-0.1.1.tar` & `openai_responses-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.1.1/LICENSE
--rw-r--r--   0        0        0    16997 2024-03-23 01:51:09.678668 openai_responses-0.1.1/README.md
--rw-r--r--   0        0        0     1141 2024-04-08 18:30:59.409316 openai_responses-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      914 2024-03-21 19:31:44.143224 openai_responses-0.1.1/src/openai_responses/__init__.py
--rw-r--r--   0        0        0       22 2024-03-18 14:06:25.547593 openai_responses-0.1.1/src/openai_responses/__version__.py
--rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.1.1/src/openai_responses/decorators.py
--rw-r--r--   0        0        0     3897 2024-04-08 18:29:00.096382 openai_responses-0.1.1/src/openai_responses/endpoints/_base.py
--rw-r--r--   0        0        0     3499 2024-03-22 21:16:42.162524 openai_responses-0.1.1/src/openai_responses/endpoints/_partial_schemas.py
--rw-r--r--   0        0        0     7231 2024-03-21 18:17:51.512106 openai_responses-0.1.1/src/openai_responses/endpoints/assistants.py
--rw-r--r--   0        0        0     4726 2024-03-21 18:18:02.635761 openai_responses-0.1.1/src/openai_responses/endpoints/chat.py
--rw-r--r--   0        0        0     1877 2024-03-21 18:18:07.877059 openai_responses-0.1.1/src/openai_responses/endpoints/embeddings.py
--rw-r--r--   0        0        0     4393 2024-03-21 18:18:14.915452 openai_responses-0.1.1/src/openai_responses/endpoints/files.py
--rw-r--r--   0        0        0    30123 2024-03-22 21:54:34.912310 openai_responses-0.1.1/src/openai_responses/endpoints/threads.py
--rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.1.1/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.1.1/src/openai_responses/py.typed
--rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.1.1/src/openai_responses/state.py
--rw-r--r--   0        0        0      629 2024-03-21 17:34:29.686060 openai_responses-0.1.1/src/openai_responses/utils.py
--rw-r--r--   0        0        0    17857 1970-01-01 00:00:00.000000 openai_responses-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-25 00:49:10.288971 openai_responses-0.2.0/README.md
+-rw-r--r--   0        0        0     1204 2024-04-24 20:15:43.213841 openai_responses-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      914 2024-03-21 19:31:44.143224 openai_responses-0.2.0/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0     1304 2024-03-21 18:06:20.705461 openai_responses-0.2.0/src/openai_responses/decorators.py
+-rw-r--r--   0        0        0     3897 2024-04-08 18:59:21.709797 openai_responses-0.2.0/src/openai_responses/endpoints/_base.py
+-rw-r--r--   0        0        0     3645 2024-04-24 19:35:49.112709 openai_responses-0.2.0/src/openai_responses/endpoints/_partial_schemas.py
+-rw-r--r--   0        0        0     8027 2024-04-24 19:35:49.113131 openai_responses-0.2.0/src/openai_responses/endpoints/assistants.py
+-rw-r--r--   0        0        0     5513 2024-04-24 20:15:43.214166 openai_responses-0.2.0/src/openai_responses/endpoints/chat.py
+-rw-r--r--   0        0        0     1877 2024-03-21 18:18:07.877059 openai_responses-0.2.0/src/openai_responses/endpoints/embeddings.py
+-rw-r--r--   0        0        0     4393 2024-03-21 18:18:14.915452 openai_responses-0.2.0/src/openai_responses/endpoints/files.py
+-rw-r--r--   0        0        0    33237 2024-04-24 20:11:09.681468 openai_responses-0.2.0/src/openai_responses/endpoints/threads.py
+-rw-r--r--   0        0        0     1785 2024-03-22 20:38:26.409131 openai_responses-0.2.0/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.2.0/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     5155 2024-03-21 19:42:49.038879 openai_responses-0.2.0/src/openai_responses/state.py
+-rw-r--r--   0        0        0      154 2024-04-24 20:15:43.214354 openai_responses-0.2.0/src/openai_responses/tokens.py
+-rw-r--r--   0        0        0      740 2024-04-24 14:35:49.271898 openai_responses-0.2.0/src/openai_responses/utils.py
+-rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 openai_responses-0.2.0/PKG-INFO
```

### Comparing `openai_responses-0.1.1/LICENSE` & `openai_responses-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/pyproject.toml` & `openai_responses-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.1.1"
+version = "0.2.0"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://github.com/mharrisb1/openai-responses-python"
 packages = [{ include = "openai_responses", from = "src" }]
 
 [tool.poetry.plugins.pytest11]
 openai_responses = "openai_responses.plugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-openai = ">=1.14"
+openai = "^1.23"
 respx = "^0.20.2"
 decorator = "^5.1.1"
 faker-openai-api-provider = "^0.1.0"
+tiktoken = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 types-decorator = "^5.1.8.20240310"
+mkdocs-material = "^9.5.18"
+tox = "^4.14.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 typeCheckingMode = "strict"
```

### Comparing `openai_responses-0.1.1/src/openai_responses/__init__.py` & `openai_responses-0.2.0/src/openai_responses/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/decorators.py` & `openai_responses-0.2.0/src/openai_responses/decorators.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/_base.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/_base.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/_partial_schemas.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/_partial_schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from openai._utils._transform import PropertyInfo
 from openai.types.beta.assistant_tool_param import AssistantToolParam
 from openai.types.beta.threads.run_status import RunStatus
 
 __all__ = ["PartialRun", "PartialRunStep"]
 
 
+class PartialIncompleteDetails(TypedDict):
+    reason: Optional[Literal["max_completion_tokens", "max_prompt_tokens"]]
+
+
 class PartialFunctionNoOutput(TypedDict):
     name: str
     arguments: str
 
 
 class PartialRequiredActionFunctionToolCall(TypedDict):
     id: str
@@ -30,26 +34,26 @@
 
 class PartialLastError(TypedDict, total=False):
     code: Literal["server_error", "rate_limit_exceeded", "invalid_prompt"]
     message: str
 
 
 class PartialRun(TypedDict, total=False):
-    status: RunStatus
-    required_action: PartialRequiredAction
-    last_error: PartialLastError
-    expires_at: int
-    started_at: int
     cancelled_at: int
-    failed_at: int
     completed_at: int
-    model: str
+    expires_at: int
+    failed_at: int
+    incomplete_details: PartialIncompleteDetails
     instructions: str
+    last_error: PartialLastError
+    model: str
+    required_action: PartialRequiredAction
+    started_at: int
+    status: RunStatus
     tools: List[AssistantToolParam]
-    file_ids: List[str]
 
 
 class PartialCodeInterpreterOutputLogs(TypedDict):
     logs: str
     type: Literal["logs"]
```

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/assistants.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/assistants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import json
 from functools import partial
 from typing import Any, Iterable, List, Optional
 
 import httpx
 import respx
 
-from openai.types import FunctionDefinition
 from openai.pagination import SyncCursorPage
-from openai.types.beta.assistant import Assistant
+from openai.types.beta.assistant import Assistant, ToolResources
 from openai.types.beta.function_tool import FunctionTool
-from openai.types.beta.retrieval_tool import RetrievalTool
+from openai.types.beta.file_search_tool import FileSearchTool
 from openai.types.beta.assistant_tool import AssistantTool
 from openai.types.beta.assistant_deleted import AssistantDeleted
 from openai.types.beta.code_interpreter_tool import CodeInterpreterTool
 from openai.types.beta.assistant_tool_param import AssistantToolParam
 from openai.types.beta.assistant_create_params import AssistantCreateParams
 from openai.types.beta.assistant_update_params import AssistantUpdateParams
+from openai.types.beta.assistant_response_format import AssistantResponseFormat
+from openai.types.beta.assistant_response_format_option import (
+    AssistantResponseFormatOption,
+)
+from openai.types.beta.assistant_response_format_option_param import (
+    AssistantResponseFormatOptionParam,
+)
 
 from ._base import StatefulMock, CallContainer
 from ..decorators import side_effect
 from ..state import StateStore
-from ..utils import model_dict, utcnow_unix_timestamp_s
+from ..utils import model_dict, model_parse, utcnow_unix_timestamp_s, remove_none
 
 
 class AssistantsMock(StatefulMock):
     def __init__(self) -> None:
         super().__init__()
         self.url = self.BASE_URL + "/assistants"
         self.create = CallContainer()
@@ -82,21 +88,29 @@
 
         content_tools = content.get("tools", [])
 
         asst = Assistant(
             id=self._faker.beta.assistant.id(),
             created_at=utcnow_unix_timestamp_s(),
             description=content.get("description"),
-            file_ids=content.get("file_ids", []),
             instructions=content.get("instructions"),
             metadata=content.get("metadata"),
             model=content["model"],
             name=content.get("name"),
             object="assistant",
-            tools=self._parse_tool_params(content_tools),
+            tools=self._parse_tool_params(content_tools) or [],
+            response_format=self._parse_response_format_params(
+                content.get("response_format")
+            ),
+            temperature=content.get("temperature"),
+            tool_resources=model_parse(
+                ToolResources,
+                content.get("tool_resources"),
+            ),
+            top_p=content.get("top_p"),
         )
         state_store.beta.assistants.put(asst)
 
         return httpx.Response(status_code=201, json=model_dict(asst))
 
     @side_effect
     def _list(
@@ -155,23 +169,29 @@
 
         asst = state_store.beta.assistants.get(id)
 
         if not asst:
             return httpx.Response(status_code=404)
 
         asst.description = content.get("description", asst.description)
-        asst.file_ids = content.get("file_ids", asst.file_ids)
         asst.instructions = content.get("instructions", asst.instructions)
         asst.metadata = content.get("metadata", asst.metadata)
         asst.model = content.get("model", asst.model)
         asst.name = content.get("name", asst.name)
-
-        update_tools = content.get("tools")
-        if update_tools:
-            asst.tools = self._parse_tool_params(update_tools)
+        asst.response_format = (
+            self._parse_response_format_params(content.get("response_format"))
+            or asst.response_format
+        )
+        asst.temperature = content.get("temperature", asst.temperature)
+        asst.tool_resources = (
+            model_parse(ToolResources, content.get("tool_resources"))
+            or asst.tool_resources
+        )
+        asst.tools = self._parse_tool_params(content.get("tools")) or asst.tools
+        asst.top_p = content.get("top_p", asst.top_p)
 
         state_store.beta.assistants.put(asst)
 
         return httpx.Response(status_code=200, json=model_dict(asst))
 
     @side_effect
     def _delete(
@@ -192,29 +212,29 @@
             json=model_dict(
                 AssistantDeleted(id=id, deleted=deleted, object="assistant.deleted")
             ),
         )
 
     @staticmethod
     def _parse_tool_params(
-        tool_params: Iterable[AssistantToolParam],
-    ) -> List[AssistantTool]:
-        tools: List[AssistantTool] = []
-
-        for tool in tool_params:
-            if tool["type"] == "code_interpreter":
-                tools.append(CodeInterpreterTool(type=tool["type"]))
-            elif tool["type"] == "retrieval":
-                tools.append(RetrievalTool(type=tool["type"]))
-            else:
-                tools.append(
-                    FunctionTool(
-                        type=tool["type"],
-                        function=FunctionDefinition(
-                            name=tool["function"]["name"],
-                            description=tool["function"].get("description"),
-                            parameters=tool["function"].get("parameters"),
-                        ),
-                    )
-                )
+        params: Optional[Iterable[AssistantToolParam]],
+    ) -> Optional[List[AssistantTool]]:
+        m = {
+            "code_interpreter": CodeInterpreterTool,
+            "file_search": FileSearchTool,
+            "function": FunctionTool,
+        }
+        return (
+            remove_none([model_parse(m[tool["type"]], tool) for tool in params])  # type: ignore
+            if params
+            else None
+        )
 
-        return tools
+    @staticmethod
+    def _parse_response_format_params(
+        params: Optional[AssistantResponseFormatOptionParam],
+    ) -> Optional[AssistantResponseFormatOption]:
+        return (
+            model_parse(AssistantResponseFormat, params)
+            if isinstance(params, dict)
+            else params
+        )
```

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/chat.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Function,
 )
 from openai.types.chat.completion_create_params import CompletionCreateParams
 
 from ._base import StatelessMock, CallContainer
 from ..decorators import side_effect
 from ..utils import model_dict, utcnow_unix_timestamp_s
+from ..tokens import count_tokens
 
 
 class ChatMock:
     def __init__(self) -> None:
         self.completions = ChatCompletionMock()
 
 
@@ -97,15 +98,36 @@
             choices=[
                 self._choice_partial_to_model(i, p) for i, p in enumerate(choices)
             ],
             model=content["model"],
             created=utcnow_unix_timestamp_s(),
             system_fingerprint="",
             object="chat.completion",
-            usage=CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0),
+        )
+
+        generated = ""
+        for choice in completion.choices:
+            if choice.message.content:
+                generated += choice.message.content
+            elif choice.message.tool_calls:
+                for tool_call in choice.message.tool_calls:
+                    generated += tool_call.function.arguments
+
+        prompt = ""
+        for message in content["messages"]:
+            prompt += str(message.get("content"))
+
+        completion_tokens = count_tokens(completion.model, generated)
+        prompt_tokens = count_tokens(completion.model, prompt)
+        total_tokens = completion_tokens + prompt_tokens
+
+        completion.usage = CompletionUsage(
+            completion_tokens=completion_tokens,
+            prompt_tokens=prompt_tokens,
+            total_tokens=total_tokens,
         )
 
         return httpx.Response(status_code=201, json=model_dict(completion))
 
     def _choice_partial_to_model(self, i: int, p: PartialChoice) -> Choice:
 
         def fn_call_partial_to_model(p: Optional[PartialFunctionCall]):
@@ -130,14 +152,15 @@
                             function=Function(
                                 arguments=call_function.get("arguments", ""),
                                 name=call_function.get("name", ""),
                             ),
                             type="function",
                         )
                     )
+                return calls
 
         message = ChatCompletionMessage(
             content=p.get("message", {}).get("content"),
             role="assistant",
             function_call=fn_call_partial_to_model(
                 p.get("message", {}).get("function_call")
             ),
```

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/embeddings.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/files.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/endpoints/threads.py` & `openai_responses-0.2.0/src/openai_responses/endpoints/threads.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 import json
 from functools import partial
-from typing import Any, List, Literal, Optional, Sequence, TypedDict, Union
+from typing import Any, Iterable, List, Literal, Optional, Sequence, TypedDict, Union
 
 import httpx
+
+from openai.types.beta.assistant_tool_choice import AssistantToolChoice
+from openai.types.beta.assistant_tool_choice_option import AssistantToolChoiceOption
+from openai.types.beta.assistant_tool_choice_option_param import (
+    AssistantToolChoiceOptionParam,
+)
+from openai.types.beta.code_interpreter_tool import CodeInterpreterTool
+from openai.types.beta.file_search_tool import FileSearchTool
 import respx
 
 from openai.pagination import SyncCursorPage
 from openai.types.beta.assistant import Assistant
 
-from openai.types.beta.thread import Thread
+from openai.types.beta.thread import Thread, ToolResources
 from openai.types.beta.thread_deleted import ThreadDeleted
 from openai.types.beta.thread_update_params import ThreadUpdateParams
 from openai.types.beta.thread_create_params import (
     ThreadCreateParams,
     Message as ThreadMessageCreateParams,
+    MessageAttachment as ThreadMessageCreateAttachmentParams,
 )
 
 from openai.types.beta.threads.text import Text
 from openai.types.beta.threads.text_content_block import TextContentBlock
 
-from openai.types.beta.threads.message import Message
-from openai.types.beta.threads.message_create_params import MessageCreateParams
+from openai.types.beta.threads.message import Message, Attachment as MessageAttachment
+from openai.types.beta.threads.message_create_params import (
+    MessageCreateParams,
+    Attachment as MessageCreateAttachmentParams,
+)
 from openai.types.beta.threads.message_update_params import MessageUpdateParams
 
-from openai.types.beta.threads.run import Run, LastError, RequiredAction, Usage
+from openai.types.beta.threads.run import (
+    IncompleteDetails,
+    Run,
+    LastError,
+    RequiredAction,
+    TruncationStrategy,
+    Usage,
+)
 from openai.types.beta.threads.run_create_params import RunCreateParams
 from openai.types.beta.threads.run_update_params import RunUpdateParams
 
 from openai.types.beta.threads.runs.run_step import (
     RunStep,
     LastError as RunStepLastError,
 )
@@ -37,15 +56,15 @@
 )
 
 from ._base import StatefulMock, CallContainer
 from ._partial_schemas import PartialRun, PartialRunStep
 from .assistants import AssistantsMock
 from ..decorators import side_effect
 from ..state import StateStore
-from ..utils import model_dict, model_parse, utcnow_unix_timestamp_s
+from ..utils import model_dict, model_parse, remove_none, utcnow_unix_timestamp_s
 
 __all__ = ["ThreadsMock", "MessagesMock", "RunsMock"]
 
 
 class ThreadsMock(StatefulMock):
     def __init__(self) -> None:
         super().__init__()
@@ -99,14 +118,15 @@
         self.create.route = route
 
         content: ThreadCreateParams = json.loads(request.content)
 
         thread = Thread(
             id=self._faker.beta.thread.id(),
             created_at=utcnow_unix_timestamp_s(),
+            tool_resources=model_parse(ToolResources, content.get("tool_resources")),
             metadata=content.get("metadata"),
             object="thread",
         )
         messages = [
             self.messages._parse_message_create_params(thread.id, m)
             for m in content.get("messages", [])
         ]
@@ -152,14 +172,18 @@
         content: ThreadUpdateParams = json.loads(request.content)
 
         thread = state_store.beta.threads.get(id)
 
         if not thread:
             return httpx.Response(status_code=404)
 
+        thread.tool_resources = (
+            model_parse(ToolResources, content.get("tool_resources"))
+            or thread.tool_resources
+        )
         thread.metadata = content.get("metadata", thread.metadata)
 
         state_store.beta.threads.put(thread)
 
         return httpx.Response(status_code=200, json=model_dict(thread))
 
     @side_effect
@@ -347,32 +371,63 @@
         state_store.beta.threads.messages.put(message)
 
         return httpx.Response(status_code=200, json=model_dict(message))
 
     def _parse_message_create_params(
         self,
         thread_id: str,
-        create_message: Union[ThreadMessageCreateParams, MessageCreateParams],
+        params: Union[ThreadMessageCreateParams, MessageCreateParams],
     ) -> Message:
         return Message(
             id=self._faker.beta.thread.message.id(),
+            attachments=self._parse_attachments_params(params.get("attachments")),
             content=[
                 TextContentBlock(
-                    text=Text(annotations=[], value=create_message["content"]),
+                    text=Text(annotations=[], value=params["content"]),
                     type="text",
                 )
             ],
             created_at=utcnow_unix_timestamp_s(),
-            file_ids=create_message.get("file_ids", []),
+            metadata=params.get("metadata"),
             object="thread.message",
-            role=create_message["role"],
+            role=params["role"],
             status="completed",
             thread_id=thread_id,
         )
 
+    @staticmethod
+    def _parse_attachments_params(
+        params: Optional[
+            Union[
+                Iterable[MessageCreateAttachmentParams],
+                Iterable[ThreadMessageCreateAttachmentParams],
+            ]
+        ],
+    ) -> Optional[List[MessageAttachment]]:
+        m = {"code_interpreter": CodeInterpreterTool, "file_search": FileSearchTool}
+        return (
+            remove_none(
+                [
+                    model_parse(
+                        MessageAttachment,
+                        {
+                            "file_id": attachment.get("file_id"),
+                            "tools": [
+                                model_parse(m[t["type"]], t)  # type: ignore
+                                for t in attachment.get("tools", [])
+                            ],
+                        },
+                    )
+                    for attachment in params
+                ]
+            )
+            if params
+            else None
+        )
+
 
 class MultiMethodSequence(TypedDict, total=False):
     create: Sequence[PartialRun]
     retrieve: Sequence[PartialRun]
 
 
 class RunsMock(StatefulMock):
@@ -460,44 +515,65 @@
             asst = state_store.beta.assistants.get(content["assistant_id"])
 
             if not asst:
                 return httpx.Response(status_code=404)
 
             partial_run = self._merge_partial_run_with_assistant(partial_run, asst)
 
+        # TODO: create additional messages
+
         run = Run(
             id=self._faker.beta.thread.run.id(),
-            object="thread.run",
-            created_at=utcnow_unix_timestamp_s(),
-            thread_id=thread_id,
             assistant_id=content["assistant_id"],
-            status=partial_run.get("status", "queued"),
-            required_action=model_parse(
-                RequiredAction,
-                partial_run.get("required_action"),
+            cancelled_at=partial_run.get("cancelled_at"),
+            completed_at=partial_run.get("completed_at"),
+            created_at=utcnow_unix_timestamp_s(),
+            expires_at=partial_run.get("expires_at"),
+            failed_at=partial_run.get("failed_at"),
+            incomplete_details=model_parse(
+                IncompleteDetails,
+                partial_run.get("incomplete_details"),
+            ),
+            instructions="\n".join(
+                [
+                    partial_run.get("instructions", ""),
+                    content.get("additional_instructions", "") or "",
+                ]
             ),
             last_error=model_parse(
                 LastError,
                 partial_run.get("last_error"),
             ),
-            expires_at=partial_run.get("expires_at"),
-            started_at=partial_run.get("started_at"),
-            cancelled_at=partial_run.get("cancelled_at"),
-            failed_at=partial_run.get("failed_at"),
-            completed_at=partial_run.get("completed_at"),
-            model=partial_run.get("model", "gpt-3.5-turbo"),
-            instructions=partial_run.get("instructions", ""),
-            tools=AssistantsMock._parse_tool_params(partial_run.get("tools", [])),
-            file_ids=partial_run.get("file_ids", []),
+            max_completion_tokens=content.get("max_completion_tokens"),
+            max_prompt_tokens=content.get("max_prompt_tokens"),
             metadata=content.get("metadata"),
+            model=partial_run.get("model", "gpt-3.5-turbo"),
+            object="thread.run",
+            required_action=model_parse(
+                RequiredAction,
+                partial_run.get("required_action"),
+            ),
+            response_format=AssistantsMock._parse_response_format_params(
+                content.get("response_format")
+            ),
+            started_at=partial_run.get("started_at"),
+            status=partial_run.get("status", "queued"),
+            thread_id=thread_id,
+            tool_choice=self._parse_tool_choice_params(content.get("tool_choice")),
+            tools=AssistantsMock._parse_tool_params(partial_run.get("tools")) or [],
+            truncation_strategy=model_parse(
+                TruncationStrategy, content.get("truncation_strategy")
+            ),
             usage=Usage(
                 completion_tokens=0,
                 prompt_tokens=0,
                 total_tokens=0,
             ),
+            temperature=content.get("temperature"),
+            top_p=content.get("top_p"),
         )
 
         state_store.beta.threads.runs.put(run)
 
         return httpx.Response(status_code=201, json=model_dict(run))
 
     def _retrieve(
@@ -533,34 +609,39 @@
         )
 
         if validate_assistant_exists:
             asst = state_store.beta.assistants.get(run.assistant_id)
             if asst:
                 partial_run = self._merge_partial_run_with_assistant(partial_run, asst)
 
-        run.status = partial_run.get("status", run.status)
-        run.expires_at = partial_run.get("expires_at", run.expires_at)
-        run.started_at = partial_run.get("started_at", run.started_at)
         run.cancelled_at = partial_run.get("cancelled_at", run.cancelled_at)
-        run.failed_at = partial_run.get("failed_at", run.failed_at)
         run.completed_at = partial_run.get("completed_at", run.completed_at)
-        run.model = partial_run.get("model", run.model)
-        run.instructions = partial_run.get("instructions", run.instructions)
-        run.file_ids = partial_run.get("file_ids", run.file_ids)
-
-        if partial_run.get("required_action"):
-            run.required_action = model_parse(
-                RequiredAction, partial_run.get("required_action")
+        run.expires_at = partial_run.get("expires_at", run.expires_at)
+        run.failed_at = partial_run.get("failed_at", run.failed_at)
+        run.incomplete_details = (
+            model_parse(
+                IncompleteDetails,
+                partial_run.get("incomplete_details"),
             )
-
-        if partial_run.get("last_error"):
-            run.last_error = model_parse(LastError, partial_run.get("last_error"))
-
-        if partial_run.get("tools"):
-            run.tools = AssistantsMock._parse_tool_params(partial_run.get("tools", []))
+            or run.incomplete_details
+        )
+        run.instructions = partial_run.get("instructions", run.instructions)
+        run.last_error = (
+            model_parse(LastError, partial_run.get("last_error")) or run.last_error
+        )
+        run.model = partial_run.get("model", run.model)
+        run.required_action = (
+            model_parse(RequiredAction, partial_run.get("required_action"))
+            or run.required_action
+        )
+        run.started_at = partial_run.get("started_at", run.started_at)
+        run.status = partial_run.get("status", run.status)
+        run.tools = (
+            AssistantsMock._parse_tool_params(partial_run.get("tools")) or run.tools
+        )
 
         state_store.beta.threads.runs.put(run)
 
         return httpx.Response(status_code=200, json=model_dict(run))
 
     def _list(
         self,
@@ -737,27 +818,35 @@
     @staticmethod
     def _merge_partial_run_with_assistant(
         run: Optional[PartialRun],
         asst: Assistant,
     ) -> PartialRun:
         if not run:
             return {
-                "file_ids": asst.file_ids,
                 "instructions": asst.instructions or "",
                 "model": asst.model,
                 "tools": [model_dict(tool) for tool in asst.tools],  # type: ignore
             }
         else:
             return run | {
-                "file_ids": run.get("file_ids", asst.file_ids),
                 "instructions": run.get("instructions", asst.instructions or ""),
                 "model": run.get("model", asst.model),
                 "tools": run.get("tools", [model_dict(tool) for tool in asst.tools]),  # type: ignore
             }
 
+    @staticmethod
+    def _parse_tool_choice_params(
+        params: Optional[AssistantToolChoiceOptionParam],
+    ) -> Optional[AssistantToolChoiceOption]:
+        return (
+            model_parse(AssistantToolChoice, params)
+            if isinstance(params, dict)
+            else params
+        )
+
 
 class RunStepsMock(StatefulMock):
     def __init__(self) -> None:
         super().__init__()
         self.url = (
             self.BASE_URL + r"/threads/(?P<thread_id>\w+)/runs/(?P<run_id>\w+)/steps"
         )
```

### Comparing `openai_responses-0.1.1/src/openai_responses/plugin.py` & `openai_responses-0.2.0/src/openai_responses/plugin.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/state.py` & `openai_responses-0.2.0/src/openai_responses/state.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.1.1/src/openai_responses/utils.py` & `openai_responses-0.2.0/src/openai_responses/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime as dt
-from typing import Any, Optional, Type, TypeVar
+from typing import Any, List, Optional, Type, TypeVar
 
 from openai import BaseModel
 
+T = TypeVar("T")
 M = TypeVar("M", bound=BaseModel)
 
 
 def utcnow_unix_timestamp_s() -> int:
     return int(dt.datetime.now().timestamp())
 
 
@@ -20,7 +21,11 @@
 def model_parse(m: Type[M], d: Optional[object]) -> Optional[M]:
     if not d:
         return None
     if hasattr(m, "model_validate"):
         return getattr(m, "model_validate")(d)
     else:
         return getattr(m, "parse_obj")(d)
+
+
+def remove_none(ls: List[Optional[T]]) -> List[T]:
+    return [el for el in ls if el]
```


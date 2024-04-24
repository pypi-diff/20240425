# Comparing `tmp/log10_io-0.8.1.tar.gz` & `tmp/log10_io-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.8.1.tar", max compression
+gzip compressed data, was "log10_io-0.8.2.tar", max compression
```

## Comparing `log10_io-0.8.1.tar` & `log10_io-0.8.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1083 2024-04-19 15:31:23.572588 log10_io-0.8.1/LICENSE
--rw-r--r--   0        0        0     8934 2024-04-19 15:31:23.572588 log10_io-0.8.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 15:31:23.572588 log10_io-0.8.1/log10/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-19 15:31:23.572588 log10_io-0.8.1/log10/__main__.py
--rw-r--r--   0        0        0    10275 2024-04-19 15:31:23.572588 log10_io-0.8.1/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/bigquery.py
--rw-r--r--   0        0        0    22333 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/evals.py
--rw-r--r--   0        0        0     5459 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4487 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8357 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/feedback/feedback.py
--rw-r--r--   0        0        0     4880 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/langchain.py
--rw-r--r--   0        0        0     4432 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/litellm.py
--rw-r--r--   0        0        0     7967 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/llm.py
--rw-r--r--   0        0        0    35998 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/load.py
--rw-r--r--   0        0        0     2886 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/openai.py
--rw-r--r--   0        0        0     6915 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/together.py
--rw-r--r--   0        0        0     2101 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/tools.py
--rw-r--r--   0        0        0     1931 2024-04-19 15:31:23.576588 log10_io-0.8.1/log10/utils.py
--rw-r--r--   0        0        0     2242 2024-04-19 15:31:23.576588 log10_io-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    10430 1970-01-01 00:00:00.000000 log10_io-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-24 22:32:57.779244 log10_io-0.8.2/LICENSE
+-rw-r--r--   0        0        0     9613 2024-04-24 22:32:57.779244 log10_io-0.8.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/__main__.py
+-rw-r--r--   0        0        0    11700 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6079 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/bigquery.py
+-rw-r--r--   0        0        0      719 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/cli_utils.py
+-rw-r--r--   0        0        0    22337 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/evals.py
+-rw-r--r--   0        0        0     5459 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4487 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     4880 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/langchain.py
+-rw-r--r--   0        0        0     4432 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/llm.py
+-rw-r--r--   0        0        0    39884 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/openai.py
+-rw-r--r--   0        0        0     6915 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/tools.py
+-rw-r--r--   0        0        0     1211 2024-04-24 22:32:57.783244 log10_io-0.8.2/log10/utils.py
+-rw-r--r--   0        0        0     2242 2024-04-24 22:32:57.787244 log10_io-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 log10_io-0.8.2/PKG-INFO
```

### Comparing `log10_io-0.8.1/LICENSE` & `log10_io-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/README.md` & `log10_io-0.8.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,28 +41,29 @@
 
 Log10 offers various integration methods, including a python LLM library wrapper, the Log10 LLM abstraction, and callbacks, to facilitate its use in both existing production environments and new projects.
 Pick the one that works best for you.
 
 #### OpenAI
 | log10 ver| openai v0 | openai v1 |
 |----------|----------|----------|
-| 0.4 | `load(openai)` ✅ | ❌ |
-| 0.5 | `load(openai)` ✅ | `from log10.load import OpenAI` ✅ |
+| 0.4 | `log10(openai)` ✅ | ❌ |
+| 0.5+ | `log10(openai)` ✅ | `from log10.load import OpenAI` ✅ |
 
 **OpenAI v0** - Use library wrapper `log10(openai)`. Check out `examples/logging` in log10 version `0.4.6`.
 ```python
 import openai
 from log10.load import log10
 
 log10(openai)
 # openai calls are now logged - including 3rd party libs using openai such as magentic or langchain
 ```
 
 **OpenAI v1**
-> NOTE: We added OpenAI v1 API support in log10 `0.5.0` release. `load.log10(openai)` still works for openai v1.
+> NOTE: We added OpenAI v1 API support in log10 `0.5.0` release. `load.log10(openai)` still works for openai v1. This also enables logging LLM completions from providers which support OpenAI API, such as [Ollama](https://github.com/ollama/ollama/blob/main/docs/openai.md).
+
 ```python
 from log10.load import OpenAI
 # from openai import OpenAI
 
 client = OpenAI()
 completion = client.completions.create(model="gpt-3.5-turbo-instruct", prompt="Once upon a time")
 # All completions.create and chat.completions.create calls will be logged
@@ -154,14 +155,19 @@
 * Summary feedback: Use [TLDR summary feedback](/log10/feedback/_summary_feedback_utils.py) rubics to rate summarization. E.g. `log10 feedback predict --task_id $FEEDBACK_TASK_ID --content '{"prompt": "this is article", "response": "summary of the article."}'`.
   * You can pass a file containing the context with `--file` or pass a completion from your Log10 logs with `--completion_id`.
 * Custom Feedback Rubrics: Integrate your own feedback criteria for personalized assessments.
 * Getting Started: To explore all options and usage details, use CLI `log10 feedback predict --help`.
 
 Feel free to integrate AutoFeedback into your workflow to enhance the feedback and evaluation process.
 
+### ⚖️📊 Model Comparison
+Easily benchmark your logged completions using LLM models from OpenAI, Anthropic, Mistral, Meta, etc., by using the `log10 completions benchmark_models` command in the log10 CLI.
+Generate detailed reports and gain insights to enhance your model's performance and cost.
+Please refer to the [cli doc](cli_docs.md#log10-completions-benchmark_models) or the [demo video](https://www.loom.com/share/6d088f9f079f4e65962741f58344d77e?sid=1d2c51e6-8978-4422-af5b-d39ebe561b83) for details.
+
 ### 🔍🐞 Prompt chain debugging
 
 Prompt chains such as those in [Langchain](https://github.com/hwchase17/langchain) can be difficult to debug. Log10 provides prompt provenance, session tracking and call stack functionality to help debug chains.
 
 ### 🧠🔁 Readiness for RLHF & self hosting
 
 Use your data and feedback from users to fine-tune custom models with RLHF with the option of building and deploying more reliable, accurate and efficient self-hosted models.
```

### Comparing `log10_io-0.8.1/log10/__main__.py` & `log10_io-0.8.2/log10/__main__.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/_httpx_utils.py` & `log10_io-0.8.2/log10/_httpx_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,86 +151,100 @@
         full_response = ""
         finished = False
         async for chunk in super().aiter_bytes(*args, **kwargs):
             full_response += chunk.decode(errors="ignore")
 
             if "data: [DONE]" in full_response:
                 finished = True
-            yield chunk
 
-        completion_id = self.request.headers.get("x-log10-completion-id", "")
-        if finished and completion_id:
-            current_stack_frame = traceback.extract_stack()
-            stacktrace = [
-                {
-                    "file": frame.filename,
-                    "line": frame.line,
-                    "lineno": frame.lineno,
-                    "name": frame.name,
-                }
-                for frame in current_stack_frame
-            ]
-            full_content = ""
-            function_name = ""
-            full_argument = ""
-            responses = full_response.split("\n\n")
-            for r in responses:
-                if "data: [DONE]" in r:
-                    break
-
-                r_json = json.loads(r[6:])
-
-                delta = r_json["choices"][0]["delta"]
-
-                # Delta may have content
-                if "content" in delta:
-                    content = delta["content"]
-                    if content:
-                        full_content += content
-
-                # May be a function call, and have to reconstruct the arguments
-                if "function_call" in delta:
-                    # May be function name
-                    if "name" in delta["function_call"]:
-                        function_name = delta["function_call"]["name"]
-                    # May be function arguments
-                    if "arguments" in delta["function_call"]:
-                        full_argument += delta["function_call"]["arguments"]
-
-            response_json = r_json.copy()
-            response_json["object"] = "completion"
-
-            # If finish_reason is function_call - don't log the response
-            if not (
-                "choices" in response_json
-                and response_json["choices"]
-                and response_json["choices"][0]["finish_reason"] == "function_call"
-            ):
-                response_json["choices"][0]["message"] = {
-                    "role": "assistant",
-                    "content": full_content,
-                }
-            else:
-                response_json["choices"][0]["function_call"] = {
-                    "name": function_name,
-                    "arguments": full_argument,
-                }
-
-            log_row = {
-                "response": json.dumps(response_json),
-                "status": "finished",
-                "duration": int(time.time() - self.request.started) * 1000,
-                "stacktrace": json.dumps(stacktrace),
-                "kind": "chat",
-                "request": self.request.content.decode("utf-8"),
-                "session_id": sessionID,
-            }
-            if get_log10_session_tags():
-                log_row["tags"] = get_log10_session_tags()
-            await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
+                completion_id = self.request.headers.get("x-log10-completion-id", "")
+                if finished and completion_id:
+                    current_stack_frame = traceback.extract_stack()
+                    stacktrace = [
+                        {
+                            "file": frame.filename,
+                            "line": frame.line,
+                            "lineno": frame.lineno,
+                            "name": frame.name,
+                        }
+                        for frame in current_stack_frame
+                    ]
+                    full_content = ""
+                    function_name = ""
+                    full_argument = ""
+                    tool_calls = []
+                    responses = full_response.split("\n\n")
+                    for r in responses:
+                        if "data: [DONE]" in r:
+                            break
+
+                        r_json = json.loads(r[6:])
+
+                        delta = r_json["choices"][0]["delta"]
+
+                        # Delta may have content
+                        if "content" in delta:
+                            content = delta["content"]
+                            if content:
+                                full_content += content
+
+                        # May be a function call, and have to reconstruct the arguments
+                        if "function_call" in delta:
+                            # May be function name
+                            if "name" in delta["function_call"]:
+                                function_name = delta["function_call"]["name"]
+                            # May be function arguments
+                            if "arguments" in delta["function_call"]:
+                                full_argument += delta["function_call"]["arguments"]
+
+                        if tc := delta.get("tool_calls", []):
+                            if tc[0].get("id", ""):
+                                tool_calls.append(tc[0])
+                            elif tc[0].get("function", {}).get("arguments", ""):
+                                idx = tc[0].get("index")
+                                tool_calls[idx]["function"]["arguments"] += tc[0]["function"]["arguments"]
+
+                    response_json = r_json.copy()
+                    response_json["object"] = "completion"
+                    # r_json is the last response before "data: [DONE]"
+                    # it contains the finish_reason
+                    finish_reason = response_json["choices"][0]["finish_reason"]
+
+                    # If finish_reason is function_call - don't log the response
+                    if not (
+                        "choices" in response_json
+                        and response_json["choices"]
+                        and response_json["choices"][0]["finish_reason"] in ["function_call", "tool_calls"]
+                    ):
+                        response_json["choices"][0]["message"] = {"role": "assistant", "content": full_content}
+                    elif finish_reason == "function_call":
+                        response_json["choices"][0]["function_call"] = {
+                            "name": function_name,
+                            "arguments": full_argument,
+                        }
+                    elif finish_reason == "tool_calls":
+                        response_json["choices"][0]["message"] = {
+                            "content": None,
+                            "role": "assistant",
+                            "tool_calls": tool_calls,
+                        }
+
+                    log_row = {
+                        "response": json.dumps(response_json),
+                        "status": "finished",
+                        "duration": int(time.time() - self.request.started) * 1000,
+                        "stacktrace": json.dumps(stacktrace),
+                        "kind": "chat",
+                        "request": self.request.content.decode("utf-8"),
+                        "session_id": sessionID,
+                    }
+                    if get_log10_session_tags():
+                        log_row["tags"] = get_log10_session_tags()
+                    await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
+            yield chunk
 
 
 class _LogTransport(httpx.AsyncBaseTransport):
     def __init__(self, transport: httpx.AsyncBaseTransport):
         self.transport = transport
 
     async def handle_async_request(self, request: httpx.Request) -> httpx.Response:
```

### Comparing `log10_io-0.8.1/log10/agents/camel.py` & `log10_io-0.8.2/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/agents/scrape_summarizer.py` & `log10_io-0.8.2/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/anthropic.py` & `log10_io-0.8.2/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/bigquery.py` & `log10_io-0.8.2/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/completions/completions.py` & `log10_io-0.8.2/log10/completions/completions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import pandas as pd
 import rich
 import tqdm
 from rich.console import Console
 from rich.table import Table
 
 from log10._httpx_utils import _get_time_diff, _try_get
+from log10.cli_utils import generate_markdown_report, generate_results_table
 from log10.llm import Log10Config
 from log10.prompt_analyzer import PromptAnalyzer, convert_suggestion_to_markdown, display_prompt_analyzer_suggestions
-from log10.utils import generate_markdown_report, generate_results_table
 
 
 _log10_config = Log10Config()
 
 
 def _get_completion(id: str) -> httpx.Response:
     url = f"{_log10_config.url}/api/completions/{id}?organization_id={_log10_config.org_id}"
```

### Comparing `log10_io-0.8.1/log10/evals.py` & `log10_io-0.8.2/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.8.2/log10/feedback/_summary_feedback_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/feedback/autofeedback.py` & `log10_io-0.8.2/log10/feedback/autofeedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/feedback/feedback.py` & `log10_io-0.8.2/log10/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/feedback/feedback_task.py` & `log10_io-0.8.2/log10/feedback/feedback_task.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/langchain.py` & `log10_io-0.8.2/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/litellm.py` & `log10_io-0.8.2/log10/litellm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/llm.py` & `log10_io-0.8.2/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/load.py` & `log10_io-0.8.2/log10/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,14 +254,15 @@
         self.function_name = ""
         self.function_arguments = ""
         self.start_time = time.perf_counter()
         self.gpt_id = None
         self.model = None
         self.finish_reason = None
         self.usage = None
+        self.tool_calls = []
 
     def __iter__(self):
         return self
 
     def __next__(self):
         try:
             chunk = next(self.response)
@@ -282,17 +283,27 @@
                 if getattr(chunk, "usage", None):
                     self.usage = chunk.usage
             elif chunk.choices[0].delta.function_call:
                 arguments = chunk.choices[0].delta.function_call.arguments
                 self.function_arguments += arguments
                 if not self.function_name and chunk.choices[0].delta.function_call.name:
                     self.function_name = chunk.choices[0].delta.function_call.name
-            else:
+            elif tc := chunk.choices[0].delta.tool_calls:
+                # self.tool_calls is a list
+                if tc[0].id:
+                    self.tool_calls.append(tc[0].dict())
+                elif tc[0].function.arguments:
+                    self.tool_calls[tc[0].index]["function"]["arguments"] += tc[0].function.arguments
+            elif chunk.choices[0].finish_reason:
                 self.finish_reason = chunk.choices[0].finish_reason
 
+                # in Magentic stream, this is reached instead of StopIteration
+                if self.finish_reason == "stop":
+                    raise StopIteration
+
             return chunk
         except StopIteration as se:
             # Log the final result
             # Create fake response for openai format.
             if self.final_result:
                 response = {
                     "id": self.gpt_id,
@@ -321,14 +332,31 @@
                             "function_call": {
                                 "name": self.function_name,
                                 "arguments": self.function_arguments,
                             },
                         }
                     ],
                 }
+            elif self.tool_calls:
+                response = {
+                    "id": self.gpt_id,
+                    "object": "completion",
+                    "model": self.model,
+                    "choices": [
+                        {
+                            "index": 0,
+                            "finish_reason": self.finish_reason,
+                            "message": {
+                                "content": "",
+                                "role": "assistant",
+                                "tool_calls": self.tool_calls,
+                            },
+                        }
+                    ],
+                }
             if self.usage:
                 response["usage"] = self.usage.dict()
             self.partial_log_row["response"] = json.dumps(response)
             self.partial_log_row["duration"] = int((time.perf_counter() - self.start_time) * 1000)
 
             try:
                 res = post_request(self.completion_url + "/" + self.completionID, self.partial_log_row)
@@ -503,14 +531,39 @@
             {"model": args[1]["model_name"], "messages": [{"role": "user", "content": args[1]["prompt"]}]}
         )
     elif "mistralai" in func.__module__:
         log_row["kind"] = "chat"
     elif "openai" in func.__module__:
         kind = "chat" if "chat" in func.__module__ else "completion"
         log_row["kind"] = kind
+    elif "google.generativeai" in func.__module__:
+        if func.__name__ == "send_message":
+            log_row["kind"] = "chat"
+            history_messages = []
+            if system_instruction := args[0].model._system_instruction:
+                history_messages.append({"role": "system", "content": system_instruction.parts[0].text})
+            if history := args[0].history:
+                for m in history:
+                    role = "assistant" if m.role == "model" else "user"
+                    content = m.parts[0].text
+                    history_messages.append({"role": role, "content": content})
+
+            history_messages.append({"role": "user", "content": args[1]})
+            kwargs_copy.update({"model": args[0].model.model_name.split("/")[-1], "messages": history_messages})
+            if kwargs_copy.get("generation_config") and hasattr(kwargs_copy["generation_config"], "__dict__"):
+                for key, value in kwargs_copy["generation_config"].__dict__.items():
+                    if not value:
+                        continue
+                    if key == "max_output_tokens":
+                        kwargs_copy["max_tokens"] = value
+                    elif key == "stop_sequences":
+                        kwargs_copy["stop"] = value
+                    elif key in ["temperature", "top_p", "top_k"]:
+                        kwargs_copy[key] = value
+                kwargs_copy.pop("generation_config")
 
     log_row["request"] = json.dumps(kwargs_copy)
 
     return log_row
 
 
 def intercepting_decorator(func):
@@ -613,14 +666,32 @@
                     tokens_usage = {
                         "prompt_tokens": response_dict["usage_metadata"]["prompt_token_count"],
                         "completion_tokens": response_dict["usage_metadata"]["candidates_token_count"],
                         "total_tokens": response_dict["usage_metadata"]["total_token_count"],
                     }
                     ret_response["usage"] = tokens_usage
                     response = ret_response
+                elif "google.generativeai" in func.__module__:
+                    ret_response = {
+                        "id": str(uuid.uuid4()),
+                        "object": "chat.completion",
+                        "choices": [
+                            {
+                                "index": 0,
+                                "finish_reason": str(output.candidates[0].finish_reason.name).lower(),
+                                "message": {"role": "assistant", "content": output.text},
+                            }
+                        ],
+                        "usage": {
+                            "prompt_tokens": 0,
+                            "completion_tokens": 0,
+                            "total_tokens": 0,
+                        },
+                    }
+                    response = ret_response
                 elif "openai" in func.__module__:
                     if type(output).__name__ == "Stream":
                         log_row["response"] = response
                         log_row["status"] = "finished"
                         return StreamingResponseWrapper(
                             completion_url=completion_url,
                             completionID=completionID,
@@ -875,18 +946,25 @@
             method = getattr(attr, "create")
             setattr(attr, "create", intercepting_decorator(method))
 
             attr = module.api_resources.chat_completion.ChatCompletion
             mothod = getattr(attr, "create")
             setattr(attr, "create", intercepting_decorator(mothod))
     elif module.__name__ == "vertexai":
-        # patch chat send_message function
+        # patch chat _send_message function
         attr = module.generative_models._generative_models.ChatSession
         method = getattr(attr, "_send_message")
         setattr(attr, "_send_message", intercepting_decorator(method))
+    elif module.__name__ == "google.generativeai":
+        # patch ChatSession send_message function
+        attr = module.ChatSession
+        method = getattr(attr, "send_message")
+        setattr(attr, "send_message", intercepting_decorator(method))
+    else:
+        logger.warning(f"Unsupported module: {module.__name__}. Please contact us for support at support@log10.io.")
 
         # For future reference:
         # if callable(attr) and isinstance(attr, types.FunctionType):
         #     print(f"attr:{attr}")
         #     setattr(module, name, intercepting_decorator(attr))
         # elif inspect.isclass(attr):  # Check if attribute is a class
         #     intercept_class_methods(attr)
```

### Comparing `log10_io-0.8.1/log10/mosaicml.py` & `log10_io-0.8.2/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/openai.py` & `log10_io-0.8.2/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/prompt_analyzer.py` & `log10_io-0.8.2/log10/prompt_analyzer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/schemas/bigquery.json` & `log10_io-0.8.2/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/together.py` & `log10_io-0.8.2/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/log10/tools.py` & `log10_io-0.8.2/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.1/pyproject.toml` & `log10_io-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.8.1"
+version = "0.8.2"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `log10_io-0.8.1/PKG-INFO` & `log10_io-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.8.1
+Version: 0.8.2
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -79,28 +79,29 @@
 
 Log10 offers various integration methods, including a python LLM library wrapper, the Log10 LLM abstraction, and callbacks, to facilitate its use in both existing production environments and new projects.
 Pick the one that works best for you.
 
 #### OpenAI
 | log10 ver| openai v0 | openai v1 |
 |----------|----------|----------|
-| 0.4 | `load(openai)` ✅ | ❌ |
-| 0.5 | `load(openai)` ✅ | `from log10.load import OpenAI` ✅ |
+| 0.4 | `log10(openai)` ✅ | ❌ |
+| 0.5+ | `log10(openai)` ✅ | `from log10.load import OpenAI` ✅ |
 
 **OpenAI v0** - Use library wrapper `log10(openai)`. Check out `examples/logging` in log10 version `0.4.6`.
 ```python
 import openai
 from log10.load import log10
 
 log10(openai)
 # openai calls are now logged - including 3rd party libs using openai such as magentic or langchain
 ```
 
 **OpenAI v1**
-> NOTE: We added OpenAI v1 API support in log10 `0.5.0` release. `load.log10(openai)` still works for openai v1.
+> NOTE: We added OpenAI v1 API support in log10 `0.5.0` release. `load.log10(openai)` still works for openai v1. This also enables logging LLM completions from providers which support OpenAI API, such as [Ollama](https://github.com/ollama/ollama/blob/main/docs/openai.md).
+
 ```python
 from log10.load import OpenAI
 # from openai import OpenAI
 
 client = OpenAI()
 completion = client.completions.create(model="gpt-3.5-turbo-instruct", prompt="Once upon a time")
 # All completions.create and chat.completions.create calls will be logged
@@ -192,14 +193,19 @@
 * Summary feedback: Use [TLDR summary feedback](/log10/feedback/_summary_feedback_utils.py) rubics to rate summarization. E.g. `log10 feedback predict --task_id $FEEDBACK_TASK_ID --content '{"prompt": "this is article", "response": "summary of the article."}'`.
   * You can pass a file containing the context with `--file` or pass a completion from your Log10 logs with `--completion_id`.
 * Custom Feedback Rubrics: Integrate your own feedback criteria for personalized assessments.
 * Getting Started: To explore all options and usage details, use CLI `log10 feedback predict --help`.
 
 Feel free to integrate AutoFeedback into your workflow to enhance the feedback and evaluation process.
 
+### ⚖️📊 Model Comparison
+Easily benchmark your logged completions using LLM models from OpenAI, Anthropic, Mistral, Meta, etc., by using the `log10 completions benchmark_models` command in the log10 CLI.
+Generate detailed reports and gain insights to enhance your model's performance and cost.
+Please refer to the [cli doc](cli_docs.md#log10-completions-benchmark_models) or the [demo video](https://www.loom.com/share/6d088f9f079f4e65962741f58344d77e?sid=1d2c51e6-8978-4422-af5b-d39ebe561b83) for details.
+
 ### 🔍🐞 Prompt chain debugging
 
 Prompt chains such as those in [Langchain](https://github.com/hwchase17/langchain) can be difficult to debug. Log10 provides prompt provenance, session tracking and call stack functionality to help debug chains.
 
 ### 🧠🔁 Readiness for RLHF & self hosting
 
 Use your data and feedback from users to fine-tune custom models with RLHF with the option of building and deploying more reliable, accurate and efficient self-hosted models.
```


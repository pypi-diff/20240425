# Comparing `tmp/openllmtelemetry-0.0.1b3.tar.gz` & `tmp/openllmtelemetry-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openllmtelemetry-0.0.1b3.tar", max compression
+gzip compressed data, was "openllmtelemetry-0.0.1b4.tar", max compression
```

## Comparing `openllmtelemetry-0.0.1b3.tar` & `openllmtelemetry-0.0.1b4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-11-22 23:28:04.346648 openllmtelemetry-0.0.1b3/LICENSE
--rw-r--r--   0        0        0     4317 2024-04-16 22:03:19.873936 openllmtelemetry-0.0.1b3/README.md
--rw-r--r--   0        0        0       75 2024-03-28 15:52:01.437323 openllmtelemetry-0.0.1b3/openllmtelemetry/__init__.py
--rw-r--r--   0        0        0     4102 2024-04-16 22:26:41.453939 openllmtelemetry-0.0.1b3/openllmtelemetry/instrument.py
--rw-r--r--   0        0        0    11339 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/LICENSE
--rw-r--r--   0        0        0        0 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0     9709 2024-04-16 23:10:56.443936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0     1673 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
--rw-r--r--   0        0        0     1050 2024-04-16 22:42:47.913936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     4007 2024-04-16 15:25:23.173936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0     7720 2024-04-16 21:09:01.783937 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     4749 2024-04-16 21:00:54.453936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0     2838 2024-04-16 18:36:02.693936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0      560 2024-04-16 20:59:41.313936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     1732 2024-04-16 20:59:44.483936 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     2239 2024-04-16 15:25:33.883935 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0       28 2024-03-22 16:01:52.610949 openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     1415 2024-04-16 22:26:46.593938 openllmtelemetry-0.0.1b3/openllmtelemetry/intrument_openai.py
--rw-r--r--   0        0        0     3118 2024-04-16 16:58:47.443939 openllmtelemetry-0.0.1b3/openllmtelemetry/secure.py
--rw-r--r--   0        0        0     1786 2024-03-28 20:14:24.636459 openllmtelemetry-0.0.1b3/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
--rw-r--r--   0        0        0      477 2024-04-16 14:55:43.883938 openllmtelemetry-0.0.1b3/openllmtelemetry/version.py
--rw-r--r--   0        0        0     1653 2024-04-17 13:24:53.999372 openllmtelemetry-0.0.1b3/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0     4317 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/README.md
+-rw-r--r--   0        0        0       75 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/__init__.py
+-rw-r--r--   0        0        0     8339 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/openllmtelemetry/config.py
+-rw-r--r--   0        0        0     1933 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrument.py
+-rw-r--r--   0        0        0    11339 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    11395 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     1673 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0     1044 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4007 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0     7703 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     4740 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     2838 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0      560 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     1726 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2233 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     1403 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/intrument_openai.py
+-rw-r--r--   0        0        0     3150 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/secure.py
+-rw-r--r--   0        0        0     1786 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b4/openllmtelemetry/span_exporter.py
+-rw-r--r--   0        0        0      477 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b4/openllmtelemetry/version.py
+-rw-r--r--   0        0        0     1653 2024-04-25 19:18:19.665151 openllmtelemetry-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b4/PKG-INFO
```

### Comparing `openllmtelemetry-0.0.1b3/LICENSE` & `openllmtelemetry-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/README.md` & `openllmtelemetry-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/LICENSE` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/bedrock/__init__.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     _SUPPRESS_INSTRUMENTATION_KEY,
     unwrap,
 )
 from opentelemetry.trace import SpanKind, get_tracer
 from wrapt import wrap_function_wrapper
 
 from openllmtelemetry.instrumentation.bedrock.reusable_streaming_body import ReusableStreamingBody
-from openllmtelemetry.secure import WhyLabsSecureApi  # noqa: E402
+from openllmtelemetry.secure import GuardrailsApi  # noqa: E402
 from openllmtelemetry.semantic_conventions.gen_ai import LLMRequestTypeValues, SpanAttributes
 from openllmtelemetry.version import __version__
 
 LOGGER = logging.getLogger(__name__)
 
 _instruments = ("boto3 >= 1.28.57",)
 
@@ -36,39 +36,76 @@
             span.set_attribute(name, value)
     return
 
 
 def _with_tracer_wrapper(func):
     """Helper for providing tracer for wrapper functions."""
 
-    def _with_tracer(tracer, secure_api: WhyLabsSecureApi, to_wrap):
+    def _with_tracer(tracer, secure_api: GuardrailsApi, to_wrap):
         def wrapper(wrapped, instance, args, kwargs):
             return func(tracer, secure_api, to_wrap, wrapped, instance, args, kwargs)
 
         return wrapper
 
     return _with_tracer
 
+def _handle_request(secure_api: Optional[GuardrailsApi], prompt: str, span):
+    prompt_metrics = None
+    if prompt is not None:
+        prompt_metrics = secure_api.eval_prompt(prompt) if secure_api is not None else None
+    if prompt_metrics and span is not None:
+            LOGGER.debug(prompt_metrics)
+            metrics = prompt_metrics.metrics[0]
+            for k in metrics.additional_keys:
+                if metrics.additional_properties[k] is not None:
+                    metric_value = metrics.additional_properties[k]
+                    span.set_attribute(f"langkit.metrics.{k}", metric_value)
+    return prompt
+
+
+def _handle_response(secure_api: Optional[GuardrailsApi], prompt, response, span):
+    response_text: Optional[str] = None
+    response_metrics = None
+    results = response.get("results")
+    if results:
+        response_message = results[0]
+        if response_message:
+            response_text = response_message.get("outputText")
+    if response_text is not None:
+        response_metrics = secure_api.eval_response(prompt=prompt, response=response_text) if secure_api is not None else None
+    if response_metrics:
+        LOGGER.debug(response_metrics)
+        metrics = response_metrics.metrics[0]
+
+        for k in metrics.additional_keys:
+            if metrics.additional_properties[k] is not None:
+                metric_value = metrics.additional_properties[k]
+                span.set_attribute(f"langkit.metrics.{k}", metric_value)
+    else:
+        LOGGER.debug("response metrics is none, skipping")
+
+    return response
+
 
 @_with_tracer_wrapper
-def _wrap(tracer, secure_api: WhyLabsSecureApi, to_wrap, wrapped, instance, args, kwargs):
+def _wrap(tracer, secure_api: GuardrailsApi, to_wrap, wrapped, instance, args, kwargs):
     """Instruments and calls every function defined in TO_WRAP."""
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     if kwargs.get("service_name") == "bedrock-runtime":
         client = wrapped(*args, **kwargs)
         client.invoke_model = _instrumented_model_invoke(client.invoke_model, tracer, secure_api)
 
         return client
+    response = wrapped(*args, **kwargs)
+    return response
 
-    return wrapped(*args, **kwargs)
 
-
-def _instrumented_model_invoke(fn, tracer, secure_api: WhyLabsSecureApi):
+def _instrumented_model_invoke(fn, tracer, secure_api: GuardrailsApi):
     @wraps(fn)
     def with_instrumentation(*args, **kwargs):
         with tracer.start_as_current_span("bedrock.completion", kind=SpanKind.CLIENT) as span:
             request_body = json.loads(kwargs.get("body"))
             (vendor, model) = kwargs.get("modelId").split(".")
             is_titan_text = model.startswith("titan-text-")
 
@@ -84,32 +121,34 @@
             elif vendor == "amazon":
                 if is_titan_text:
                     prompt = request_body["inputText"]
                 else:
                     LOGGER.debug("LLM not suppported yet")
             LOGGER.debug(f"extracted prompt: {prompt}")
             # TODO: check for input text first
+            prompt = _handle_request(secure_api, prompt, span)
             response = fn(*args, **kwargs)
-            # noinspection PyProtectedMember
+
             response["body"] = ReusableStreamingBody(response["body"]._raw_stream, response["body"]._content_length)
             response_body = json.loads(response.get("body").read())
+            response_body = _handle_response(secure_api, prompt, response_body, span)
+            # noinspection PyProtectedMember
 
             _set_span_attribute(span, SpanAttributes.LLM_VENDOR, vendor)
             _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MODEL, model)
 
             if vendor == "cohere":
                 _set_cohere_span_attributes(span, request_body, response_body)
             elif vendor == "anthropic":
                 _set_anthropic_span_attributes(span, request_body, response_body)
             elif vendor == "ai21":
                 _set_ai21_span_attributes(span, request_body, response_body)
             elif vendor == "meta":
                 _set_llama_span_attributes(span, request_body, response_body)
             elif vendor == "amazon":
-                print("Bedrock vendor")
                 _set_amazon_titan_span_attributes(span, request_body, response_body)
 
             return response
 
     return with_instrumentation
 
 
@@ -124,20 +163,19 @@
             _set_span_attribute(span, SpanAttributes.LLM_USAGE_TOTAL_TOKENS, total_tokens)
 
         _set_span_attribute(span, SpanAttributes.LLM_USAGE_PROMPT_TOKENS, input_token_count)
 
         if should_send_prompts():
             _set_span_attribute(span, f"{SpanAttributes.LLM_PROMPTS}.0.user", request_body.get("inputText"))
             contents = response_body.get("results")
-            _set_span_attribute(span, f"{SpanAttributes.LLM_COMPLETIONS}.0.content", contents[0].get('outputText') if contents else "")
+            _set_span_attribute(span, f"{SpanAttributes.LLM_COMPLETIONS}.0.content", contents[0].get("outputText") if contents else "")
     except Exception as ex:  # pylint: disable=broad-except
         LOGGER.warning(f"Failed to set input attributes for openai span, error:{str(ex)}")
 
 
-
 def _set_cohere_span_attributes(span, request_body, response_body):
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_TYPE, LLMRequestTypeValues.COMPLETION.value)
     _set_span_attribute(span, SpanAttributes.LLM_TOP_P, request_body.get("p"))
     _set_span_attribute(span, SpanAttributes.LLM_TEMPERATURE, request_body.get("temperature"))
     _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MAX_TOKENS, request_body.get("max_tokens"))
 
     if should_send_prompts():
@@ -183,15 +221,15 @@
         for i, generation in enumerate(response_body.get("generations")):
             _set_span_attribute(span, f"{SpanAttributes.LLM_COMPLETIONS}.{i}.content", response_body)
 
 
 class BedrockInstrumentor(BaseInstrumentor):
     """An instrumentor for Bedrock's client library."""
 
-    def __init__(self, secure_api: Optional[WhyLabsSecureApi]):
+    def __init__(self, secure_api: Optional[GuardrailsApi]):
         self._secure_api = secure_api
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/__init__.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 from typing import Collection, Optional
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 
-from openllmtelemetry.secure import WhyLabsSecureApi
+from openllmtelemetry.secure import GuardrailsApi
 
 from .utils import is_openai_v1
 from .v0 import OpenAIV0Instrumentor
 from .v1 import OpenAIV1Instrumentor
 
 _instruments = ("openai>=0.27.0",)
 
 LOGGER = logging.getLogger(__name__)
 
 
 class OpenAIInstrumentor(BaseInstrumentor):
     """An instrumentor for OpenAI's client library."""
 
-    def __init__(self, secure_api: Optional[WhyLabsSecureApi]):
+    def __init__(self, secure_api: Optional[GuardrailsApi]):
         LOGGER.info("Instrumenting OpenAI")
 
         self._guard = secure_api
         if is_openai_v1():
             self._instrumentor = OpenAIV1Instrumentor(self._guard)
         else:
             self._instrumentor = OpenAIV0Instrumentor(self._guard)
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/__init__.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,25 @@
     _set_response_attributes,
     _set_span_attribute,
     is_streaming_response,
     model_as_dict,
     should_send_prompts,
 )
 from openllmtelemetry.instrumentation.openai.utils import _with_tracer_wrapper, is_openai_v1
-from openllmtelemetry.secure import WhyLabsSecureApi  # noqa: E402
+from openllmtelemetry.secure import GuardrailsApi  # noqa: E402
 from openllmtelemetry.semantic_conventions.gen_ai import LLMRequestTypeValues, SpanAttributes
 
 SPAN_NAME = "openai.chat"
 LLM_REQUEST_TYPE = LLMRequestTypeValues.CHAT
 
 LOGGER = logging.getLogger(__name__)
 
 
 @_with_tracer_wrapper
-def chat_wrapper(tracer, secure_api: WhyLabsSecureApi, wrapped, instance, args, kwargs):
+def chat_wrapper(tracer, secure_api: GuardrailsApi, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     # span needs to be opened and closed manually because the response is a generator
     span = tracer.start_span(
         SPAN_NAME,
         kind=SpanKind.CLIENT,
@@ -57,39 +57,39 @@
     _handle_response(secure_api, prompt, response, span)
     span.end()
 
     return response
 
 
 @_with_tracer_wrapper
-async def achat_wrapper(tracer, guard: WhyLabsSecureApi, wrapped, instance, args, kwargs):
+async def achat_wrapper(tracer, guard: GuardrailsApi, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     span = tracer.start_span(
         SPAN_NAME,
         kind=SpanKind.CLIENT,
         attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value, "span.type": "completion"},
     )
-    (prompt, prompt_metrics) = _handle_request(guard, span, kwargs)
+    prompt, prompt_metrics = _handle_request(guard, span, kwargs)
     LOGGER.debug("Prompt metrics: ", prompt_metrics)
     response = await wrapped(*args, **kwargs)
     LOGGER.debug(f"Async type response: {type(response)}")
 
     if is_streaming_response(response):
         # span will be closed after the generator is done
         return _abuild_from_streaming_response(span, response)
 
     _handle_response(guard, prompt, response, span)
     span.end()
 
     return response
 
 
-def _handle_request(secure_api: WhyLabsSecureApi, span, kwargs):
+def _handle_request(secure_api: GuardrailsApi, span, kwargs):
     _set_request_attributes(span, kwargs)
     stream = kwargs.get("stream")
     LOGGER.debug("Stream: %s. ", stream)
     LOGGER.debug(f"Stream: {stream}")
     messages = kwargs.get("messages")
     user_messages = [m["content"] for m in messages if m["role"] == "user"]
     prompt = user_messages[-1]
@@ -98,15 +98,15 @@
     if should_send_prompts():
         _set_prompts(span, messages)
         _set_functions_attributes(span, kwargs.get("functions"))
 
     return prompt, prompt_metrics
 
 
-def _handle_response(secure_api: WhyLabsSecureApi, prompt, response, span):
+def _handle_response(secure_api: GuardrailsApi, prompt, response, span):
     if is_openai_v1():
         response_dict = model_as_dict(response)
     else:
         response_dict = response
     response = response_dict["choices"][0]["message"]["content"]
     response_metrics = secure_api.eval_response(prompt=prompt, response=response) if secure_api is not None else None
     if response_metrics:
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     should_send_prompts,
 )
 from openllmtelemetry.instrumentation.openai.utils import (
     _with_tracer_wrapper,
     is_openai_v1,
     start_as_current_span_async,
 )
-from openllmtelemetry.secure import WhyLabsSecureApi
+from openllmtelemetry.secure import GuardrailsApi
 from openllmtelemetry.semantic_conventions.gen_ai import LLMRequestTypeValues, SpanAttributes
 
 SPAN_NAME = "openai.completion"
 LLM_REQUEST_TYPE = LLMRequestTypeValues.COMPLETION
 
 logger = logging.getLogger(__name__)
 
 
 @_with_tracer_wrapper
-def completion_wrapper(tracer, secure_api: Optional[WhyLabsSecureApi], wrapped, instance, args, kwargs):
+def completion_wrapper(tracer, secure_api: Optional[GuardrailsApi], wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     # span needs to be opened and closed manually because the response is a generator
     span = tracer.start_span(
         SPAN_NAME,
         kind=SpanKind.CLIENT,
@@ -51,15 +51,15 @@
         _handle_response(response, span)
 
     span.end()
     return response
 
 
 @_with_tracer_wrapper
-async def acompletion_wrapper(tracer, guard: Optional[WhyLabsSecureApi], wrapped, instance, args, kwargs):
+async def acompletion_wrapper(tracer, guard: Optional[GuardrailsApi], wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     async with start_as_current_span_async(
         tracer=tracer,
         name=SPAN_NAME,
         kind=SpanKind.CLIENT,
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/utils.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/v0/__init__.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/v0/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     completion_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.shared.embeddings_wrappers import (
     aembeddings_wrapper,
     embeddings_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.version import __version__
-from openllmtelemetry.secure import WhyLabsSecureApi
+from openllmtelemetry.secure import GuardrailsApi
 
 _instruments = ("openai >= 0.27.0", "openai < 1.0.0")
 
 
 class OpenAIV0Instrumentor(BaseInstrumentor):
-    def __init__(self, guard: Optional[WhyLabsSecureApi]):
+    def __init__(self, guard: Optional[GuardrailsApi]):
         self._guard = guard
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/instrumentation/openai/v1/__init__.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/instrumentation/openai/v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     completion_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.shared.embeddings_wrappers import (
     aembeddings_wrapper,
     embeddings_wrapper,
 )
 from openllmtelemetry.instrumentation.openai.version import __version__
-from openllmtelemetry.secure import WhyLabsSecureApi
+from openllmtelemetry.secure import GuardrailsApi
 
 _instruments = ("openai >= 1.0.0",)
 
 
 class OpenAIV1Instrumentor(BaseInstrumentor):
-    def __init__(self, guard: WhyLabsSecureApi):
+    def __init__(self, guard: GuardrailsApi):
         self._secure_api = guard
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/intrument_openai.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/intrument_openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import importlib
 import logging
 from typing import Optional
 
 from opentelemetry.trace import Tracer
 
-from openllmtelemetry.secure import WhyLabsSecureApi
+from openllmtelemetry.secure import GuardrailsApi
 
 LOGGER = logging.getLogger(__name__)
 
 
-def init_instrumentors(trace_provider: Tracer, secure_api: Optional[WhyLabsSecureApi]):
+def init_instrumentors(trace_provider: Tracer, secure_api: Optional[GuardrailsApi]):
     for instrumentor in [init_openai_instrumentor, init_bedrock_instrumentor]:
         instrumentor(trace_provider=trace_provider, secure_api=secure_api)
 
 
-def init_openai_instrumentor(trace_provider: Tracer, secure_api: Optional[WhyLabsSecureApi]):
+def init_openai_instrumentor(trace_provider: Tracer, secure_api: Optional[GuardrailsApi]):
     if importlib.util.find_spec("openai") is not None:  # type: ignore
         from openllmtelemetry.instrumentation.openai import OpenAIInstrumentor
 
         instrumentor = OpenAIInstrumentor(secure_api=secure_api)
         instrumentor.instrument(trace_provider=trace_provider, guard=secure_api)  # type: ignore
     else:
         LOGGER.warning("OpenAPI not found, skipping instrumentation")
 
 
-def init_bedrock_instrumentor(trace_provider: Tracer, secure_api: Optional[WhyLabsSecureApi]):
+def init_bedrock_instrumentor(trace_provider: Tracer, secure_api: Optional[GuardrailsApi]):
     if importlib.util.find_spec("boto3") is not None:  # type: ignore
         from openllmtelemetry.instrumentation.bedrock import BedrockInstrumentor
 
         instrumentor = BedrockInstrumentor(secure_api=secure_api)
         instrumentor.instrument(trace_provider=trace_provider, guard=secure_api)  # type: ignore
     else:
         LOGGER.warning("Boto3 not found, skipping instrumentation")
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/secure.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/secure.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 from httpx import Timeout
 from whylogs_container_client import AuthenticatedClient
 from whylogs_container_client.models import EvaluationResult, HTTPValidationError, LLMValidateRequest
 
 LOGGER = logging.getLogger(__name__)
 
 
-class WhyLabsSecureApi(object):
+class GuardrailsApi(object):
     def __init__(
         self,
-        guard_endpoint: str,
-        guard_api_key: str,
+        guardrails_endpoint: str,
+        guardrails_api_key: str,
         dataset_id: str,
         timeout: Optional[float] = 1.0,
         auth_header_name: str = "X-API-Key",
     ):
         """
         Construct a new WhyLabs Guard client
 
-        :param guard_endpoint: the endpoint for the guard client
-        :param guard_api_key: the API key to authorize with the endpoint
+        :param guardrails_endpoint: the endpoint for the guard client
+        :param guardrails_api_key: the API key to authorize with the endpoint
         :param dataset_id: the default dataset ID
         :param timeout: timeout in second
         :param auth_header_name: the name of the auth header. Shouldn't be set normally
         """
-        self._api_key = guard_api_key
+        self._api_key = guardrails_api_key
         self._dataset_id = dataset_id
         self._client = AuthenticatedClient(
-            base_url=guard_endpoint,  # type: ignore
-            token=guard_api_key,  #
+            base_url=guardrails_endpoint,  # type: ignore
+            token=guardrails_api_key,  #
             prefix="",  #
             auth_header_name=auth_header_name,  # type: ignore
             timeout=Timeout(timeout, read=timeout),  # type: ignore
         )  # type: ignore
 
     def eval_prompt(self, prompt: str) -> Optional[EvaluationResult]:
         profiling_request = LLMValidateRequest(prompt=prompt, dataset_id=self._dataset_id)
```

### Comparing `openllmtelemetry-0.0.1b3/openllmtelemetry/semantic_conventions/gen_ai/__init__.py` & `openllmtelemetry-0.0.1b4/openllmtelemetry/semantic_conventions/gen_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b3/pyproject.toml` & `openllmtelemetry-0.0.1b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenLLMTelemetry"
-version = "0.0.1.b3"
+version = "0.0.1.b4"
 description = "End-to-end observability with built-in security guardrails."
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `openllmtelemetry-0.0.1b3/PKG-INFO` & `openllmtelemetry-0.0.1b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenLLMTelemetry
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: End-to-end observability with built-in security guardrails.
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


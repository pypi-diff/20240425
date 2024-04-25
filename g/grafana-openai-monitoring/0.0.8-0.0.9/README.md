# Comparing `tmp/grafana_openai_monitoring-0.0.8.tar.gz` & `tmp/grafana_openai_monitoring-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana_openai_monitoring-0.0.8.tar", max compression
+gzip compressed data, was "grafana_openai_monitoring-0.0.9.tar", max compression
```

## Comparing `grafana_openai_monitoring-0.0.8.tar` & `grafana_openai_monitoring-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     5230 2024-01-10 08:41:48.716840 grafana_openai_monitoring-0.0.8/README.md
--rw-r--r--   0        0        0      598 2024-01-10 08:42:00.180949 grafana_openai_monitoring-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4904 2024-01-10 08:41:48.716840 grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/__handlers.py
--rw-r--r--   0        0        0        0 2024-01-10 08:41:48.716840 grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/__init__.py
--rw-r--r--   0        0        0     5319 2024-01-10 08:41:48.716840 grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/chat_v1.py
--rw-r--r--   0        0        0     9496 2024-01-10 08:41:48.716840 grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/chat_v2.py
--rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 grafana_openai_monitoring-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     5230 2024-04-25 07:21:48.039536 grafana_openai_monitoring-0.0.9/README.md
+-rw-r--r--   0        0        0      598 2024-04-25 07:21:55.787561 grafana_openai_monitoring-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4891 2024-04-25 07:21:48.039536 grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/__handlers.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:21:48.039536 grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/__init__.py
+-rw-r--r--   0        0        0     5618 2024-04-25 07:21:48.039536 grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/chat_v1.py
+-rw-r--r--   0        0        0    10030 2024-04-25 07:21:48.039536 grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/chat_v2.py
+-rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 grafana_openai_monitoring-0.0.9/PKG-INFO
```

### Comparing `grafana_openai_monitoring-0.0.8/README.md` & `grafana_openai_monitoring-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `grafana_openai_monitoring-0.0.8/pyproject.toml` & `grafana_openai_monitoring-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grafana-openai-monitoring"
-version = "0.0.8"
+version = "0.0.9"
 description = "Library to monitor your OpenAI usage and send metrics and logs to Grafana Cloud"
 authors = ["Ishan Jain <ishan.jain@grafana.com>"]
 repository = "https://github.com/grafana/grafana-openai-monitoring"
 readme = "README.md"
 homepage = "https://github.com/grafana/grafana-openai-monitoring"
 keywords = ["observability", "monitoring", "openai", "grafana", "gpt"]
```

### Comparing `grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/__handlers.py` & `grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/__handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 
     __send_metrics(metrics_url, metrics_username, access_token, metrics):
         Send metrics to the specified Prometheus URL.
     
     __send_logs(logs_url, metrics_username, access_token, metrics):
         Send logs to the specified Loki URL.
 """
-
+import logging
 import requests
 
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.ERROR)
+
 # Function to check if all required arguments are provided and modify metrics and logs URLs
 def __check(metrics_url, logs_url, metrics_username, logs_username, access_token):
     # Check if all required parameters are provided
     if not all([metrics_url, logs_url, metrics_username, logs_username, access_token]):
         raise ValueError("All parameters (metrics_url, logs_url, metrics_username, "
                          "logs_username, access_token) must be provided")
 
@@ -88,25 +91,23 @@
         response = requests.post(logs_url,
                                  auth=(logs_username, access_token),
                                  json=logs,
                                  headers={"Content-Type": "application/json"},
                                  timeout=60
                                 )
         response.raise_for_status()  # Raise an exception for non-2xx status codes
-        return response
     except requests.exceptions.RequestException as err:
-        raise requests.exceptions.RequestException(f"Error sending Logs: {err}")
+        logger.error("Error sending Logs: %s", err)
 
 # Function to send metrics to the specified metrics URL
 def __send_metrics(metrics_url, metrics_username, access_token, metrics):
     try:
         body = '\n'.join(metrics)
         response = requests.post(metrics_url,
                                  headers={'Content-Type': 'text/plain'},
                                  data=str(body),
                                  auth=(metrics_username, access_token),
                                  timeout=60
                             )
         response.raise_for_status()  # Raise an exception for non-2xx status codes
-        return response
     except requests.exceptions.RequestException as err:
-        raise requests.exceptions.RequestException(f"Error sending Metrics: {err}")
+        logger.error("Error sending Metrics: %s", err)
```

### Comparing `grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/chat_v1.py` & `grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/chat_v1.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 API usage and responses.
 """
 
 import time
 from .__handlers import __send_metrics, __send_logs, __calculate_cost, __check
 
 # Decorator function to monitor chat completion
-def monitor(func, metrics_url, logs_url, metrics_username, logs_username, access_token): # pylint: disable=too-many-arguments
+# pylint: disable=too-many-arguments
+def monitor(func, metrics_url, logs_url, metrics_username, logs_username, access_token,
+            disable_content=False, environment="default"):
     """
     A decorator function to monitor chat completions using the OpenAI API.
 
     This decorator wraps an OpenAI API function and enhances it with monitoring
     capabilities by sending metrics and logs to specified endpoints.
 
     Args:
@@ -68,15 +70,16 @@
 
         # Prepare logs to be sent
         logs = {
             "streams": [
             {
                     "stream": {
                         "job": "integrations/openai", 
-                        "prompt": prompt, 
+                        "prompt": prompt,
+                        "environment": environment,
                         "model": response.model, 
                         "finish_reason": response.choices[0].finish_reason,
                         "prompt_tokens": str(response.usage.prompt_tokens), 
                         "completion_tokens": str(response.usage.completion_tokens), 
                         "total_tokens": str(response.usage.total_tokens)
                     },
                     "values": [
@@ -86,46 +89,47 @@
                         ]
                     ]
 
                 }
             ]
         }
 
-        # Send logs to the specified logs URL
-        __send_logs(logs_url=logs_url,
-                    logs_username=logs_username,
-                    access_token=access_token,
-                    logs=logs
-        )
+        if disable_content is True:
+            # Send logs to the specified logs URL
+            __send_logs(logs_url=logs_url,
+                        logs_username=logs_username,
+                        access_token=access_token,
+                        logs=logs
+            )
 
         # Prepare metrics to be sent
         metrics = [
             # Metric to track the number of completion tokens used in the response
             f'openai,job=integrations/openai,'
-            f'source=python_chatv1,model={response.model} '
+            f'source=python_chatv1,model={response.model},environment={environment} '
             f'completionTokens={response.usage.completion_tokens}',
 
             # Metric to track the number of prompt tokens used in the response
             f'openai,job=integrations/openai,'
-            f'source=python_chatv1,model={response.model} '
+            f'source=python_chatv1,model={response.model},environment={environment} '
             f'promptTokens={response.usage.prompt_tokens}',
 
             # Metric to track the total number of tokens used in the response
             f'openai,job=integrations/openai,'
-            f'source=python_chatv1,model={response.model} '
+            f'source=python_chatv1,model={response.model},environment={environment} '
             f'totalTokens={response.usage.total_tokens}',
 
             # Metric to track the duration of the API request and response cycle
             f'openai,job=integrations/openai,'
-            f'source=python_chatv1,model={response.model} '
+            f'source=python_chatv1,model={response.model},environment={environment} '
             f'requestDuration={duration}',
 
             # Metric to track the usage cost based on the model and token usage
             f'openai,job=integrations/openai,'
-            f'source=python_chatv1,model={response.model} '
+            f'source=python_chatv1,model={response.model},environment={environment} '
             f'usageCost={cost}',
         ]
 
 
         # Send metrics to the specified metrics URL
         __send_metrics(metrics_url=metrics_url,
                        metrics_username=metrics_username,
```

### Comparing `grafana_openai_monitoring-0.0.8/src/grafana_openai_monitoring/chat_v2.py` & `grafana_openai_monitoring-0.0.9/src/grafana_openai_monitoring/chat_v2.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 API usage and responses.
 """
 
 import time
 from .__handlers import __send_metrics, __send_logs, __calculate_cost, __check
 
 # Decorator function to monitor chat completion
-def monitor(func, metrics_url, logs_url, metrics_username, logs_username, access_token, use_async=False): # pylint: disable=too-many-arguments, line-too-long
+def monitor(func, metrics_url, logs_url, metrics_username, logs_username, access_token, use_async=False, disable_content=False, environment="default"): # pylint: disable=too-many-arguments, line-too-long
     """
     A decorator function to monitor chat completions using the OpenAI API.
 
     This decorator wraps an OpenAI API function and enhances it with monitoring
     capabilities by sending metrics and logs to specified endpoints.
 
     Args:
@@ -68,15 +68,16 @@
 
         # Prepare logs to be sent
         logs = {
             "streams": [
             {
                     "stream": {
                         "job": "integrations/openai", 
-                        "prompt": prompt, 
+                        "prompt": prompt,
+                        "environment": environment,
                         "model": response.model, 
                         "role": response.choices[0].message.role,
                         "finish_reason": response.choices[0].finish_reason,
                         "prompt_tokens": str(response.usage.prompt_tokens), 
                         "completion_tokens": str(response.usage.completion_tokens), 
                         "total_tokens": str(response.usage.total_tokens)
                     },
@@ -86,47 +87,47 @@
                             response.choices[0].message.content
                         ]
                     ]
 
                 }
             ]
         }
-
-        # Send logs to the specified logs URL
-        __send_logs(logs_url=logs_url,
-                    logs_username=logs_username,
-                    access_token=access_token,
-                    logs=logs
-        )
+        if disable_content is True:
+            # Send logs to the specified logs URL
+            __send_logs(logs_url=logs_url,
+                        logs_username=logs_username,
+                        access_token=access_token,
+                        logs=logs
+            )
 
         # Prepare metrics to be sent
         metrics = [
             # Metric to track the number of completion tokens used in the response
             f'openai,job=integrations/openai,'
-            f'source=python_chatv2,model={response.model} '
+            f'source=python_chatv2,model={response.model},environment={environment} '
             f'completionTokens={response.usage.completion_tokens}',
 
             # Metric to track the number of prompt tokens used in the response
             f'openai,job=integrations/openai,'
-            f'source=python_chatv2,model={response.model} '
+            f'source=python_chatv2,model={response.model},environment={environment} '
             f'promptTokens={response.usage.prompt_tokens}',
 
             # Metric to track the total number of tokens used in the response
             f'openai,job=integrations/openai,'
-            f'source=python_chatv2,model={response.model} '
+            f'source=python_chatv2,model={response.model},environment={environment} '
             f'totalTokens={response.usage.total_tokens}',
 
             # Metric to track the usage cost based on the model and token usage
             f'openai,job=integrations/openai,'
-            f'source=python_chatv2,model={response.model} '
+            f'source=python_chatv2,model={response.model},environment={environment} '
             f'usageCost={cost}',
 
             # Metric to track the duration of the API request and response cycle
             f'openai,job=integrations/openai,'
-            f'source=python_chatv2,model={response.model} '
+            f'source=python_chatv2,model={response.model},environment={environment} '
             f'requestDuration={duration}',
         ]
 
         # Send metrics to the specified metrics URL
         __send_metrics(metrics_url=metrics_url,
                        metrics_username=metrics_username,
                        access_token=access_token,
@@ -164,15 +165,16 @@
 
             # Prepare logs to be sent
             logs = {
                 "streams": [
                 {
                         "stream": {
                             "job": "integrations/openai", 
-                            "prompt": prompt, 
+                            "prompt": prompt,
+                            "environment": environment,
                             "model": response.model, 
                             "role": response.choices[0].message.role,
                             "finish_reason": response.choices[0].finish_reason,
                             "prompt_tokens": str(response.usage.prompt_tokens), 
                             "completion_tokens": str(response.usage.completion_tokens), 
                             "total_tokens": str(response.usage.total_tokens)
                         },
@@ -182,47 +184,47 @@
                                 response.choices[0].message.content
                             ]
                         ]
 
                     }
                 ]
             }
-
-            # Send logs to the specified logs URL
-            __send_logs(logs_url=logs_url,
-                        logs_username=logs_username,
-                        access_token=access_token,
-                        logs=logs
-            )
+            if disable_content is True:
+                # Send logs to the specified logs URL
+                __send_logs(logs_url=logs_url,
+                            logs_username=logs_username,
+                            access_token=access_token,
+                            logs=logs
+                )
 
             # Prepare metrics to be sent
             metrics = [
                 # Metric to track the number of completion tokens used in the response
                 f'openai,job=integrations/openai,'
-                f'source=python_chatv2,model={response.model} '
+                f'source=python_chatv2,model={response.model},environment={environment} '
                 f'completionTokens={response.usage.completion_tokens}',
 
                 # Metric to track the number of prompt tokens used in the response
                 f'openai,job=integrations/openai,'
-                f'source=python_chatv2,model={response.model} '
+                f'source=python_chatv2,model={response.model},environment={environment} '
                 f'promptTokens={response.usage.prompt_tokens}',
 
                 # Metric to track the total number of tokens used in the response
                 f'openai,job=integrations/openai,'
-                f'source=python_chatv2,model={response.model} '
+                f'source=python_chatv2,model={response.model},environment={environment} '
                 f'totalTokens={response.usage.total_tokens}',
 
                 # Metric to track the usage cost based on the model and token usage
                 f'openai,job=integrations/openai,'
-                f'source=python_chatv2,model={response.model} '
+                f'source=python_chatv2,model={response.model},environment={environment} '
                 f'usageCost={cost}',
 
                 # Metric to track the duration of the API request and response cycle
                 f'openai,job=integrations/openai,'
-                f'source=python_chatv2,model={response.model} '
+                f'source=python_chatv2,model={response.model},environment={environment} '
                 f'requestDuration={duration}',
             ]
 
             # Send metrics to the specified metrics URL
             __send_metrics(metrics_url=metrics_url,
                            metrics_username=metrics_username,
                            access_token=access_token,
```

### Comparing `grafana_openai_monitoring-0.0.8/PKG-INFO` & `grafana_openai_monitoring-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-openai-monitoring
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to monitor your OpenAI usage and send metrics and logs to Grafana Cloud
 Home-page: https://github.com/grafana/grafana-openai-monitoring
 Keywords: observability,monitoring,openai,grafana,gpt
 Author: Ishan Jain
 Author-email: ishan.jain@grafana.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
```


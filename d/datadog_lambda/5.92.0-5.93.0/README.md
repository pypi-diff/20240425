# Comparing `tmp/datadog_lambda-5.92.0.tar.gz` & `tmp/datadog_lambda-5.93.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-5.92.0.tar", max compression
+gzip compressed data, was "datadog_lambda-5.93.0.tar", max compression
```

## Comparing `datadog_lambda-5.92.0.tar` & `datadog_lambda-5.93.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11379 2024-03-28 15:07:13.036733 datadog_lambda-5.92.0/LICENSE
--rw-r--r--   0        0        0      290 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      141 2024-03-28 15:07:13.036733 datadog_lambda-5.92.0/NOTICE
--rw-r--r--   0        0        0     5943 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/README.md
--rw-r--r--   0        0        0      723 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     8107 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0      662 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2024-03-28 15:07:13.036733 datadog_lambda-5.92.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0      766 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/logger.py
--rw-r--r--   0        0        0     4707 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2024-03-28 15:07:13.620736 datadog_lambda-5.92.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     2112 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    48234 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    15223 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3448 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1366 2024-03-28 15:07:13.624736 datadog_lambda-5.92.0/pyproject.toml
--rw-r--r--   0        0        0     7326 1970-01-01 00:00:00.000000 datadog_lambda-5.92.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2024-04-25 17:56:08.424389 datadog_lambda-5.93.0/LICENSE
+-rw-r--r--   0        0        0     1381 2024-04-25 17:56:08.876391 datadog_lambda-5.93.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      141 2024-04-25 17:56:08.424389 datadog_lambda-5.93.0/NOTICE
+-rw-r--r--   0        0        0     5943 2024-04-25 17:56:08.876391 datadog_lambda-5.93.0/README.md
+-rw-r--r--   0        0        0      637 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     8171 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0      621 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      992 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0      766 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/logger.py
+-rw-r--r--   0        0        0     4595 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4710 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     2091 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     2487 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    47962 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12177 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0       23 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/version.py
+-rw-r--r--   0        0        0    15272 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3749 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1435 2024-04-25 17:56:08.880391 datadog_lambda-5.93.0/pyproject.toml
+-rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 datadog_lambda-5.93.0/PKG-INFO
```

### Comparing `datadog_lambda-5.92.0/LICENSE` & `datadog_lambda-5.93.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/README.md` & `datadog_lambda-5.93.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/datadog_lambda/__init__.py` & `datadog_lambda-5.93.0/datadog_lambda/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from datadog_lambda.cold_start import initialize_cold_start_tracing
-from datadog_lambda.logger import initialize_logging
 import os
 
 
 if os.environ.get("DD_INSTRUMENTATION_TELEMETRY_ENABLED") is None:
     os.environ["DD_INSTRUMENTATION_TELEMETRY_ENABLED"] = "false"
 
 if os.environ.get("DD_API_SECURITY_ENABLED") is None:
     os.environ["DD_API_SECURITY_ENABLED"] = "False"
 
 initialize_cold_start_tracing()
 
 # The minor version corresponds to the Lambda layer version.
 # E.g.,, version 0.5.0 gets packaged into layer version 5.
-try:
-    import importlib.metadata as importlib_metadata
-except ModuleNotFoundError:
-    import importlib_metadata
+from datadog_lambda.version import __version__  # noqa: E402 F401
+from datadog_lambda.logger import initialize_logging  # noqa: E402
 
-__version__ = importlib_metadata.version(__name__)
 
 initialize_logging(__name__)
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/api.py` & `datadog_lambda-5.93.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/datadog_lambda/cold_start.py` & `datadog_lambda-5.93.0/datadog_lambda/cold_start.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,24 @@
 
 def is_new_sandbox():
     return is_cold_start() or is_proactive_init()
 
 
 def get_cold_start_tag():
     """Returns the cold start tag to be used in metrics"""
-    return "cold_start:{}".format(str(is_cold_start()).lower())
+    return "cold_start:true" if _cold_start else "cold_start:false"
 
 
 def get_proactive_init_tag():
     """Returns the proactive init tag to be used in metrics"""
-    return "proactive_initialization:{}".format(str(is_proactive_init()).lower())
+    return (
+        "proactive_initialization:true"
+        if _proactive_initialization
+        else "proactive_initialization:false"
+    )
 
 
 class ImportNode(object):
     def __init__(self, module_name, full_file_path, start_time_ns, end_time_ns=None):
         self.module_name = module_name
         self.full_file_path = full_file_path
         self.start_time_ns = start_time_ns
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/constants.py` & `datadog_lambda-5.93.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-5.93.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/datadog_lambda/extension.py` & `datadog_lambda-5.93.0/datadog_lambda/extension.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import logging
-from os import path
+import os
 
 AGENT_URL = "http://127.0.0.1:8124"
 FLUSH_PATH = "/lambda/flush"
 EXTENSION_PATH = "/opt/extensions/datadog-agent"
 
 logger = logging.getLogger(__name__)
 
 
 def is_extension_present():
-    if path.exists(EXTENSION_PATH):
-        return True
-    return False
+    return os.path.exists(EXTENSION_PATH)
 
 
 def flush_extension():
     try:
         import urllib.request
 
         req = urllib.request.Request(AGENT_URL + FLUSH_PATH, "".encode("ascii"))
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/handler.py` & `datadog_lambda-5.93.0/datadog_lambda/handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 path = os.environ.get("DD_LAMBDA_HANDLER", None)
 if path is None:
     raise HandlerError(
         "DD_LAMBDA_HANDLER is not defined. Can't use prebuilt datadog handler"
     )
 parts = path.rsplit(".", 1)
 if len(parts) != 2:
-    raise HandlerError("Value %s for DD_LAMBDA_HANDLER has invalid format." % path)
+    raise HandlerError(f"Value {path} for DD_LAMBDA_HANDLER has invalid format.")
 
 
 (mod_name, handler_name) = parts
 modified_mod_name = modify_module_name(mod_name)
 handler_module = import_module(modified_mod_name)
 handler = datadog_lambda_wrapper(getattr(handler_module, handler_name))
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/logger.py` & `datadog_lambda-5.93.0/datadog_lambda/logger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/datadog_lambda/metric.py` & `datadog_lambda-5.93.0/datadog_lambda/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Unless explicitly stated otherwise all files in this repository are licensed
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
 
 import os
-import json
 import time
 import logging
+import ujson as json
 
 from datadog_lambda.extension import should_use_extension
-from datadog_lambda.tags import get_enhanced_metrics_tags, tag_dd_lambda_layer
+from datadog_lambda.tags import get_enhanced_metrics_tags, dd_lambda_layer_tag
 from datadog_lambda.api import init_api
 
 logger = logging.getLogger(__name__)
 
 lambda_stats = None
 
 init_api()
@@ -28,14 +28,18 @@
     # end of invocation. To make metrics submitted from a long-running Lambda
     # function available sooner, consider using the Datadog Lambda extension.
     from datadog_lambda.thread_stats_writer import ThreadStatsWriter
 
     flush_in_thread = os.environ.get("DD_FLUSH_IN_THREAD", "").lower() == "true"
     lambda_stats = ThreadStatsWriter(flush_in_thread)
 
+enhanced_metrics_enabled = (
+    os.environ.get("DD_ENHANCED_METRICS", "true").lower() == "true"
+)
+
 
 def lambda_metric(metric_name, value, timestamp=None, tags=None, force_async=False):
     """
     Submit a data point to Datadog distribution metrics.
     https://docs.datadoghq.com/graphing/metrics/distributions/
 
     When DD_FLUSH_TO_LOG is True, write metric to log, and
@@ -46,15 +50,16 @@
     periodically and at the end of the function execution in a
     background thread.
 
     Note that if the extension is present, it will override the DD_FLUSH_TO_LOG value
     and always use the layer to send metrics to the extension
     """
     flush_to_logs = os.environ.get("DD_FLUSH_TO_LOG", "").lower() == "true"
-    tags = tag_dd_lambda_layer(tags)
+    tags = [] if tags is None else list(tags)
+    tags.append(dd_lambda_layer_tag)
 
     if should_use_extension:
         logger.debug(
             "Sending metric %s value %s to Datadog via extension", metric_name, value
         )
         lambda_stats.distribution(metric_name, value, tags=tags, timestamp=timestamp)
     else:
@@ -76,41 +81,32 @@
     print(
         json.dumps(
             {
                 "m": metric_name,
                 "v": value,
                 "e": timestamp or int(time.time()),
                 "t": tags,
-            }
+            },
+            escape_forward_slashes=False,
         )
     )
 
 
 def flush_stats():
     lambda_stats.flush()
 
 
-def are_enhanced_metrics_enabled():
-    """Check env var to find if enhanced metrics should be submitted
-
-    Returns:
-        boolean for whether enhanced metrics are enabled
-    """
-    # DD_ENHANCED_METRICS defaults to true
-    return os.environ.get("DD_ENHANCED_METRICS", "true").lower() == "true"
-
-
 def submit_enhanced_metric(metric_name, lambda_context):
     """Submits the enhanced metric with the given name
 
     Args:
         metric_name (str): metric name w/o enhanced prefix i.e. "invocations" or "errors"
         lambda_context (dict): Lambda context dict passed to the function by AWS
     """
-    if not are_enhanced_metrics_enabled():
+    if not enhanced_metrics_enabled:
         logger.debug(
             "Not submitting enhanced metric %s because enhanced metrics are disabled",
             metric_name,
         )
         return
     tags = get_enhanced_metrics_tags(lambda_context)
     metric_name = "aws.lambda.enhanced." + metric_name
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/patch.py` & `datadog_lambda-5.93.0/datadog_lambda/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Unless explicitly stated otherwise all files in this repository are licensed
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
 
-import json
 import os
 import sys
 import logging
 import zlib
+import ujson as json
 
 from wrapt import wrap_function_wrapper as wrap
 from wrapt.importer import when_imported
 from ddtrace import patch_all as patch_all_dd
 
 from datadog_lambda.tracing import (
     get_dd_trace_context,
@@ -140,20 +140,20 @@
     # Sort the datapoints POSTed by their name so that snapshots always align
     data = request.body or "{}"
     # If payload is compressed, decompress it so we can parse it
     if request.headers.get("Content-Encoding") == "deflate":
         data = zlib.decompress(data)
     data_dict = json.loads(data)
     data_dict.get("series", []).sort(key=lambda series: series.get("metric"))
-    sorted_data = json.dumps(data_dict)
+    sorted_data = json.dumps(data_dict, escape_forward_slashes=False)
 
     # Sort headers to prevent any differences in ordering
     headers = request.headers or {}
     sorted_headers = sorted(
         "{}:{}".format(key, value) for key, value in headers.items()
     )
-    sorted_header_str = json.dumps(sorted_headers)
+    sorted_header_str = json.dumps(sorted_headers, escape_forward_slashes=False)
     print(
         "HTTP {} {} Headers: {} Data: {}".format(
             method, url, sorted_header_str, sorted_data
         )
     )
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/tag_object.py` & `datadog_lambda-5.93.0/datadog_lambda/tag_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Unless explicitly stated otherwise all files in this repository are licensed
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2021 Datadog, Inc.
 
 from decimal import Decimal
-import json
 import logging
+import ujson as json
 
 redactable_keys = ["authorization", "x-authorization", "password", "token"]
 max_depth = 10
 logger = logging.getLogger(__name__)
 
 
 def tag_object(span, key, obj, depth=0):
@@ -26,25 +26,25 @@
         except ValueError:
             redacted = _redact_val(key, obj[0:5000])
             return span.set_tag(key, redacted)
     if isinstance(obj, int) or isinstance(obj, float) or isinstance(obj, Decimal):
         return span.set_tag(key, str(obj))
     if isinstance(obj, list):
         for k, v in enumerate(obj):
-            formatted_key = "{}.{}".format(key, k)
+            formatted_key = f"{key}.{k}"
             tag_object(span, formatted_key, v, depth)
         return
     if hasattr(obj, "items"):
         for k, v in obj.items():
-            formatted_key = "{}.{}".format(key, k)
+            formatted_key = f"{key}.{k}"
             tag_object(span, formatted_key, v, depth)
         return
     if hasattr(obj, "to_dict"):
         for k, v in obj.to_dict().items():
-            formatted_key = "{}.{}".format(key, k)
+            formatted_key = f"{key}.{k}"
             tag_object(span, formatted_key, v, depth)
         return
     try:
         value_as_str = str(obj)
     except Exception:
         value_as_str = "UNKNOWN"
     return span.set_tag(key, value_as_str)
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/tags.py` & `datadog_lambda-5.93.0/datadog_lambda/tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,70 @@
 import sys
 
-from platform import python_version_tuple
-
 from datadog_lambda import __version__
 from datadog_lambda.cold_start import get_cold_start_tag
 
 
-def _format_dd_lambda_layer_tag():
-    """
-    Formats the dd_lambda_layer tag, e.g., 'dd_lambda_layer:datadog-python39_1'
-    """
-    runtime = "python{}{}".format(sys.version_info[0], sys.version_info[1])
-    return "dd_lambda_layer:datadog-{}_{}".format(runtime, __version__)
-
-
-def tag_dd_lambda_layer(tags):
-    """
-    Used by lambda_metric to insert the dd_lambda_layer tag
-    """
-    dd_lambda_layer_tag = _format_dd_lambda_layer_tag()
-    if tags:
-        return tags + [dd_lambda_layer_tag]
-    else:
-        return [dd_lambda_layer_tag]
+_major, _minor = sys.version_info[0], sys.version_info[1]
+dd_lambda_layer_tag = f"dd_lambda_layer:datadog-python{_major}{_minor}_{__version__}"
+runtime_tag = f"runtime:python{_major}.{_minor}"
+library_version_tag = f"datadog_lambda:v{__version__}"
 
 
 def parse_lambda_tags_from_arn(lambda_context):
     """Generate the list of lambda tags based on the data in the arn
     Args:
         lambda_context: Aws lambda context object
             ex: lambda_context.arn = arn:aws:lambda:us-east-1:123597598159:function:my-lambda:1
     """
     # Set up flag for extra testing to distinguish between a version or alias
-    hasAlias = False
+    has_alias = False
     # Cap the number of times to spli
     split_arn = lambda_context.invoked_function_arn.split(":")
 
     if len(split_arn) > 7:
-        hasAlias = True
+        has_alias = True
         _, _, _, region, account_id, _, function_name, alias = split_arn
     else:
         _, _, _, region, account_id, _, function_name = split_arn
 
     # Add the standard tags to a list
     tags = [
-        "region:{}".format(region),
-        "account_id:{}".format(account_id),
-        "functionname:{}".format(function_name),
+        f"region:{region}",
+        f"account_id:{account_id}",
+        f"functionname:{function_name}",
     ]
 
     # Check if we have a version or alias
-    if hasAlias:
+    if has_alias:
         # If $Latest, drop the $ for datadog tag convention. A lambda alias can't start with $
         if alias.startswith("$"):
             alias = alias[1:]
         # Versions are numeric. Aliases need the executed version tag
         elif not check_if_number(alias):
-            tags.append("executedversion:{}".format(lambda_context.function_version))
+            tags.append(f"executedversion:{lambda_context.function_version}")
         # create resource tag with function name and alias/version
-        resource = "resource:{}:{}".format(function_name, alias)
+        resource = f"resource:{function_name}:{alias}"
     else:
         # Resource is only the function name otherwise
-        resource = "resource:{}".format(function_name)
+        resource = f"resource:{function_name}"
 
     tags.append(resource)
 
     return tags
 
 
-def get_runtime_tag():
-    """Get the runtime tag from the current Python version"""
-    major_version, minor_version, _ = python_version_tuple()
-
-    return "runtime:python{major}.{minor}".format(
-        major=major_version, minor=minor_version
-    )
-
-
-def get_library_version_tag():
-    """Get datadog lambda library tag"""
-    return "datadog_lambda:v{}".format(__version__)
-
-
 def get_enhanced_metrics_tags(lambda_context):
     """Get the list of tags to apply to enhanced metrics"""
-    return parse_lambda_tags_from_arn(lambda_context) + [
-        get_cold_start_tag(),
-        "memorysize:{}".format(lambda_context.memory_limit_in_mb),
-        get_runtime_tag(),
-        get_library_version_tag(),
-    ]
+    tags = parse_lambda_tags_from_arn(lambda_context)
+    tags.append(get_cold_start_tag())
+    tags.append(f"memorysize:{lambda_context.memory_limit_in_mb}")
+    tags.append(runtime_tag)
+    tags.append(library_version_tag)
+    return tags
 
 
 def check_if_number(alias):
     """
     Check if the alias is a version or number.
     Python 2 has no easy way to test this like Python 3
     """
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-5.93.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-5.92.0/datadog_lambda/tracing.py` & `datadog_lambda-5.93.0/datadog_lambda/tracing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Unless explicitly stated otherwise all files in this repository are licensed
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
 import hashlib
 import logging
 import os
-import json
 import base64
+import ujson as json
 from datetime import datetime, timezone
 from typing import Optional, Dict
 
 from datadog_lambda.metric import submit_errors_metric
 
 try:
     from typing import Literal
@@ -62,14 +62,16 @@
         os.environ.get("DD_INSTRUMENTATION_TELEMETRY_ENABLED", "false").lower()
         == "true"
     ):
         from ddtrace.internal.telemetry import telemetry_writer
 
         telemetry_writer.enable()
 
+is_lambda_context = os.environ.get(XrayDaemon.FUNCTION_NAME_HEADER_NAME) != ""
+
 propagator = HTTPPropagator()
 
 DD_TRACE_JAVA_TRACE_ID_PADDING = "00000000"
 
 
 def _convert_xray_trace_id(xray_trace_id):
     """
@@ -89,15 +91,15 @@
     """
     Convert X-Ray sampled (True/False) to its Datadog counterpart.
     """
     return SamplingPriority.USER_KEEP if xray_sampled else SamplingPriority.USER_REJECT
 
 
 def _get_xray_trace_context():
-    if not is_lambda_context():
+    if not is_lambda_context:
         return None
 
     xray_trace_entity = parse_xray_header(
         os.environ.get(XrayDaemon.XRAY_TRACE_ID_HEADER_NAME, "")
     )
     if xray_trace_entity is None:
         return None
@@ -105,30 +107,28 @@
         trace_id=_convert_xray_trace_id(xray_trace_entity.get("trace_id")),
         span_id=_convert_xray_entity_id(xray_trace_entity.get("parent_id")),
         sampling_priority=_convert_xray_sampling(xray_trace_entity.get("sampled")),
     )
     logger.debug(
         "Converted trace context %s from X-Ray segment %s",
         trace_context,
-        (
-            xray_trace_entity["trace_id"],
-            xray_trace_entity["parent_id"],
-            xray_trace_entity["sampled"],
-        ),
+        xray_trace_entity,
     )
     return trace_context
 
 
 def _get_dd_trace_py_context():
     span = tracer.current_span()
     if not span:
         return None
 
     logger.debug(
-        "found dd trace context: %s", (span.context.trace_id, span.context.span_id)
+        "found dd trace context: trace_id=%s span_id=%s",
+        span.context.trace_id,
+        span.context.span_id,
     )
     return span.context
 
 
 def _is_context_complete(context):
     return (
         context
@@ -231,74 +231,70 @@
         logger.debug("Failed extracting context as EventBridge to SQS.")
 
     try:
         first_record = event.get("Records")[0]
 
         # logic to deal with SNS => SQS event
         if "body" in first_record:
-            body_str = first_record.get("body", {})
+            body_str = first_record.get("body")
             try:
                 body = json.loads(body_str)
                 if body.get("Type", "") == "Notification" and "TopicArn" in body:
                     logger.debug("Found SNS message inside SQS event")
                     first_record = get_first_record(create_sns_event(body))
             except Exception:
-                first_record = event.get("Records")[0]
                 pass
 
-        msg_attributes = first_record.get(
-            "messageAttributes",
-            first_record.get("Sns", {}).get("MessageAttributes", {}),
-        )
-        dd_payload = msg_attributes.get("_datadog", {})
+        msg_attributes = first_record.get("messageAttributes")
+        if msg_attributes is None:
+            sns_record = first_record.get("Sns") or {}
+            msg_attributes = sns_record.get("MessageAttributes") or {}
+        dd_payload = msg_attributes.get("_datadog")
         if dd_payload:
             # SQS uses dataType and binaryValue/stringValue
             # SNS uses Type and Value
             dd_json_data = None
-            dd_json_data_type = dd_payload.get("Type", dd_payload.get("dataType", ""))
+            dd_json_data_type = dd_payload.get("Type") or dd_payload.get("dataType")
             if dd_json_data_type == "Binary":
-                dd_json_data = dd_payload.get(
-                    "binaryValue",
-                    dd_payload.get("Value", r"{}"),
-                )
-                dd_json_data = base64.b64decode(dd_json_data)
+                dd_json_data = dd_payload.get("binaryValue") or dd_payload.get("Value")
+                if dd_json_data:
+                    dd_json_data = base64.b64decode(dd_json_data)
             elif dd_json_data_type == "String":
-                dd_json_data = dd_payload.get(
-                    "stringValue",
-                    dd_payload.get("Value", r"{}"),
-                )
+                dd_json_data = dd_payload.get("stringValue") or dd_payload.get("Value")
             else:
                 logger.debug(
                     "Datadog Lambda Python only supports extracting trace"
                     "context from String or Binary SQS/SNS message attributes"
                 )
 
             if dd_json_data:
                 dd_data = json.loads(dd_json_data)
                 return propagator.extract(dd_data)
         else:
             # Handle case where trace context is injected into attributes.AWSTraceHeader
             # example: Root=1-654321ab-000000001234567890abcdef;Parent=0123456789abcdef;Sampled=1
-            x_ray_header = first_record.get("attributes", {}).get("AWSTraceHeader")
-            if x_ray_header:
-                x_ray_context = parse_xray_header(x_ray_header)
-                trace_id_parts = x_ray_context.get("trace_id", "").split("-")
-                if len(trace_id_parts) > 2 and trace_id_parts[2].startswith(
-                    DD_TRACE_JAVA_TRACE_ID_PADDING
-                ):
-                    # If it starts with eight 0's padding,
-                    # then this AWSTraceHeader contains Datadog injected trace context
-                    logger.debug(
-                        "Found dd-trace injected trace context from AWSTraceHeader"
-                    )
-                    return Context(
-                        trace_id=int(trace_id_parts[2][8:], 16),
-                        span_id=int(int(x_ray_context["parent_id"], 16)),
-                        sampling_priority=float(x_ray_context["sampled"]),
-                    )
+            attrs = first_record.get("attributes")
+            if attrs:
+                x_ray_header = attrs.get("AWSTraceHeader")
+                if x_ray_header:
+                    x_ray_context = parse_xray_header(x_ray_header)
+                    trace_id_parts = x_ray_context.get("trace_id", "").split("-")
+                    if len(trace_id_parts) > 2 and trace_id_parts[2].startswith(
+                        DD_TRACE_JAVA_TRACE_ID_PADDING
+                    ):
+                        # If it starts with eight 0's padding,
+                        # then this AWSTraceHeader contains Datadog injected trace context
+                        logger.debug(
+                            "Found dd-trace injected trace context from AWSTraceHeader"
+                        )
+                        return Context(
+                            trace_id=int(trace_id_parts[2][8:], 16),
+                            span_id=int(x_ray_context["parent_id"], 16),
+                            sampling_priority=float(x_ray_context["sampled"]),
+                        )
         return extract_context_from_lambda_context(lambda_context)
     except Exception as e:
         logger.debug("The trace extractor returned with error %s", e)
         return extract_context_from_lambda_context(lambda_context)
 
 
 def _extract_context_from_eventbridge_sqs_event(event):
@@ -335,29 +331,30 @@
 
 def extract_context_from_kinesis_event(event, lambda_context):
     """
     Extract datadog trace context from a Kinesis Stream's base64 encoded data string
     """
     try:
         record = get_first_record(event)
-        data = record.get("kinesis", {}).get("data", None)
+        kinesis = record.get("kinesis")
+        if not kinesis:
+            return extract_context_from_lambda_context(lambda_context)
+        data = kinesis.get("data")
         if data:
             b64_bytes = data.encode("ascii")
             str_bytes = base64.b64decode(b64_bytes)
             data_str = str_bytes.decode("ascii")
             data_obj = json.loads(data_str)
             dd_ctx = data_obj.get("_datadog")
-
-        if not dd_ctx:
-            return extract_context_from_lambda_context(lambda_context)
-
-        return propagator.extract(dd_ctx)
+            if dd_ctx:
+                return propagator.extract(dd_ctx)
     except Exception as e:
         logger.debug("The trace extractor returned with error %s", e)
-        return extract_context_from_lambda_context(lambda_context)
+
+    return extract_context_from_lambda_context(lambda_context)
 
 
 def _deterministic_md5_hash(s: str) -> int:
     """MD5 here is to generate trace_id, not for any encryption."""
     hex_number = hashlib.md5(s.encode("ascii")).hexdigest()
     binary = bin(int(hex_number, 16))
     binary_str = str(binary)
@@ -376,15 +373,15 @@
     """
     try:
         execution_id = event.get("Execution").get("Id")
         state_name = event.get("State").get("Name")
         state_entered_time = event.get("State").get("EnteredTime")
         trace_id = _deterministic_md5_hash(execution_id)
         parent_id = _deterministic_md5_hash(
-            execution_id + "#" + state_name + "#" + state_entered_time
+            f"{execution_id}#{state_name}#{state_entered_time}"
         )
         sampling_priority = SamplingPriority.AUTO_KEEP
         return Context(
             trace_id=trace_id, span_id=parent_id, sampling_priority=sampling_priority
         )
     except Exception as e:
         logger.debug("The Step Functions trace extractor returned with error %s", e)
@@ -392,19 +389,15 @@
 
 
 def extract_context_custom_extractor(extractor, event, lambda_context):
     """
     Extract Datadog trace context using a custom trace extractor function
     """
     try:
-        (
-            trace_id,
-            parent_id,
-            sampling_priority,
-        ) = extractor(event, lambda_context)
+        trace_id, parent_id, sampling_priority = extractor(event, lambda_context)
         return Context(
             trace_id=int(trace_id),
             span_id=int(parent_id),
             sampling_priority=int(sampling_priority),
         )
     except Exception as e:
         logger.debug("The trace extractor returned with error %s", e)
@@ -422,46 +415,54 @@
     except Exception as e:
         logger.debug("unknown error while checking is_authorizer_response %s", e)
     return False
 
 
 def get_injected_authorizer_data(event, is_http_api) -> dict:
     try:
-        authorizer_headers = event.get("requestContext", {}).get("authorizer")
+        req_ctx = event.get("requestContext")
+        if not req_ctx:
+            return None
+        authorizer_headers = req_ctx.get("authorizer")
         if not authorizer_headers:
             return None
 
-        dd_data_raw = (
-            authorizer_headers.get("lambda", {}).get("_datadog")
-            if is_http_api
-            else authorizer_headers.get("_datadog")
-        )
+        if is_http_api:
+            lambda_hdr = authorizer_headers.get("lambda")
+            if not lambda_hdr:
+                return None
+            dd_data_raw = lambda_hdr.get("_datadog")
+        else:
+            dd_data_raw = authorizer_headers.get("_datadog")
 
         if not dd_data_raw:
             return None
 
         injected_data = json.loads(base64.b64decode(dd_data_raw))
 
         # Lambda authorizer's results can be cached. But the payload will still have the injected
         # data in cached requests. How to distinguish cached case and ignore the injected data ?
         # APIGateway automatically injects a integrationLatency data in some cases. If it's >0 we
         # know that it's not cached. But integrationLatency is not available for Http API case. In
         # that case, we use the injected Authorizing_Request_Id to tell if it's cached. But token
         # authorizers don't pass on the requestId. The Authorizing_Request_Id can't work for all
         # cases neither. As a result, we combine both methods as shown below.
-        if authorizer_headers.get("integrationLatency", 0) > 0 or event.get(
-            "requestContext", {}
-        ).get("requestId") == injected_data.get(Headers.Authorizing_Request_Id):
+        if authorizer_headers.get("integrationLatency", 0) > 0:
             return injected_data
-        else:
+        req_ctx = event.get("requestContext")
+        if not req_ctx:
             return None
+        if req_ctx.get("requestId") == injected_data.get(
+            Headers.Authorizing_Request_Id
+        ):
+            return injected_data
+        return None
 
     except Exception as e:
         logger.debug("Failed to check if invocated by an authorizer. error %s", e)
-        return None
 
 
 def extract_dd_trace_context(
     event, lambda_context, extractor=None, decode_authorizer_context: bool = True
 ):
     """
     Extract Datadog trace context from the Lambda `event` object.
@@ -525,16 +526,16 @@
 
     global dd_trace_context
 
     try:
         xray_context = _get_xray_trace_context()  # xray (sub)segment
     except Exception as e:
         logger.debug(
-            "get_dd_trace_context couldn't read from segment from x-ray, with error %s"
-            % e
+            "get_dd_trace_context couldn't read from segment from x-ray, with error %s",
+            e,
         )
     if not xray_context:
         return None
 
     if not _is_context_complete(dd_trace_context):
         return xray_context
 
@@ -565,15 +566,15 @@
     """
     Create a dummy span, and overrides its trace_id and span_id, to make
     ddtrace.helpers.get_log_correlation_context() return a dict containing the correct ids for both
     auto and manual log correlations.
 
     TODO: Remove me when Datadog tracer is natively supported in Lambda.
     """
-    if not is_lambda_context():
+    if not is_lambda_context:
         logger.debug("set_correlation_ids is only supported in LambdaContext")
         return
     if dd_tracing_enabled:
         logger.debug("using ddtrace implementation for spans")
         return
 
     context = get_dd_trace_context_obj()
@@ -609,38 +610,31 @@
 
     # Patch `logging.Logger.makeRecord` to actually inject correlation ids
     patch(logging=True)
 
     logger.debug("logs injection configured")
 
 
-def is_lambda_context():
-    """
-    Return True if the X-Ray context is `LambdaContext`, rather than the
-    regular `Context` (e.g., when testing lambda functions locally).
-    """
-    return os.environ.get(XrayDaemon.FUNCTION_NAME_HEADER_NAME, "") != ""
-
-
 def set_dd_trace_py_root(trace_context_source, merge_xray_traces):
     if trace_context_source == TraceContextSource.EVENT or merge_xray_traces:
         context = Context(
             trace_id=dd_trace_context.trace_id,
             span_id=dd_trace_context.span_id,
             sampling_priority=dd_trace_context.sampling_priority,
         )
         if merge_xray_traces:
             xray_context = _get_xray_trace_context()
             if xray_context and xray_context.span_id:
                 context.span_id = xray_context.span_id
 
         tracer.context_provider.activate(context)
         logger.debug(
-            "Set dd trace root context to: %s",
-            (context.trace_id, context.span_id),
+            "Set dd trace root context to: trace_id=%s span_id=%s",
+            context.trace_id,
+            context.span_id,
         )
 
 
 def create_inferred_span(
     event,
     context,
     event_source: _EventSource = None,
@@ -693,17 +687,15 @@
             return create_inferred_span_from_eventbridge_event(event, context)
     except Exception as e:
         logger.debug(
             "Unable to infer span. Detected type: %s. Reason: %s",
             event_source.to_string(),
             e,
         )
-        return None
     logger.debug("Unable to infer a span: unknown event type")
-    return None
 
 
 def create_service_mapping(val):
     new_service_mapping = {}
     for entry in val.split(","):
         parts = entry.split(":")
         if len(parts) == 2:
@@ -717,56 +709,56 @@
 def determine_service_name(service_mapping, specific_key, generic_key, default_value):
     service_name = service_mapping.get(specific_key)
     if service_name is None:
         service_name = service_mapping.get(generic_key, default_value)
     return service_name
 
 
-service_mapping = {}
 # Initialization code
 service_mapping_str = os.getenv("DD_SERVICE_MAPPING", "")
 service_mapping = create_service_mapping(service_mapping_str)
 
+_dd_origin = {"_dd.origin": "lambda"}
+
 
 def create_inferred_span_from_lambda_function_url_event(event, context):
     request_context = event.get("requestContext")
     api_id = request_context.get("apiId")
     domain = request_context.get("domainName")
     service_name = determine_service_name(service_mapping, api_id, "lambda_url", domain)
-    method = request_context.get("http", {}).get("method")
-    path = request_context.get("http", {}).get("path")
-    resource = "{0} {1}".format(method, path)
+    http = request_context.get("http")
+    method = http.get("method") if http else None
+    path = http.get("path") if http else None
+    resource = f"{method} {path}"
     tags = {
         "operation_name": "aws.lambda.url",
         "http.url": domain + path,
         "endpoint": path,
         "http.method": method,
         "resource_names": domain + path,
         "request_id": context.aws_request_id,
     }
     request_time_epoch = request_context.get("timeEpoch")
-    args = {
-        "service": service_name,
-        "resource": resource,
-        "span_type": "http",
-    }
-    tracer.set_tags(
-        {"_dd.origin": "lambda"}
-    )  # function urls don't count as lambda_inferred,
+    tracer.set_tags(_dd_origin)  # function urls don't count as lambda_inferred,
     # because they're in the same service as the inferring lambda function
-    span = tracer.trace("aws.lambda.url", **args)
+    span = tracer.trace(
+        "aws.lambda.url", service=service_name, resource=resource, span_type="http"
+    )
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
     if span:
         span.set_tags(tags)
-    span.start = request_time_epoch / 1000
+        span.start_ns = int(request_time_epoch) * 1e6
     return span
 
 
 def is_api_gateway_invocation_async(event):
-    return event.get("headers", {}).get("X-Amz-Invocation-Type") == "Event"
+    hdrs = event.get("headers")
+    if not hdrs:
+        return False
+    return hdrs.get("X-Amz-Invocation-Type") == "Event"
 
 
 def insert_upstream_authorizer_span(
     kwargs_to_start_span, other_tags_for_span, start_time_ns, finish_time_ns
 ):
     """Insert the authorizer span.
         Without this:        parent span --child-> inferred span
@@ -858,15 +850,15 @@
     else:
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
     args = {
         "service": service_name,
         "resource": endpoint,
         "span_type": "web",
     }
-    tracer.set_tags({"_dd.origin": "lambda"})
+    tracer.set_tags(_dd_origin)
     upstream_authorizer_span = None
     finish_time_ns = None
     if decode_authorizer_context:
         upstream_authorizer_span, finish_time_ns = process_injected_data(
             event, request_time_epoch_ms, args, tags
         )
     span = tracer.trace("aws.apigateway.websocket", **args)
@@ -889,15 +881,16 @@
     domain = request_context.get("domainName", "")
     api_id = request_context.get("apiId")
     service_name = determine_service_name(
         service_mapping, api_id, "lambda_api_gateway", domain
     )
     method = event.get("httpMethod")
     path = event.get("path")
-    resource = "{0} {1}".format(method, path)
+    resource_path = _get_resource_path(event, request_context)
+    resource = f"{method} {resource_path}"
     tags = {
         "operation_name": "aws.apigateway.rest",
         "http.url": domain + path,
         "endpoint": path,
         "http.method": method,
         "resource_names": resource,
         "apiid": api_id,
@@ -911,15 +904,15 @@
     else:
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
     args = {
         "service": service_name,
         "resource": resource,
         "span_type": "http",
     }
-    tracer.set_tags({"_dd.origin": "lambda"})
+    tracer.set_tags(_dd_origin)
     upstream_authorizer_span = None
     finish_time_ns = None
     if decode_authorizer_context:
         upstream_authorizer_span, finish_time_ns = process_injected_data(
             event, request_time_epoch_ms, args, tags
         )
     span = tracer.trace("aws.apigateway", **args)
@@ -932,59 +925,68 @@
             else request_time_epoch_ms * 1e6
         )
         if upstream_authorizer_span:
             span.parent_id = upstream_authorizer_span.span_id
     return span
 
 
+def _get_resource_path(event, request_context):
+    route_key = request_context.get("routeKey") or ""
+    if "{" in route_key:
+        try:
+            return route_key.split(" ")[1]
+        except Exception as e:
+            logger.debug("Error parsing routeKey: %s", e)
+    return event.get("rawPath") or request_context.get("resourcePath") or route_key
+
+
 def create_inferred_span_from_http_api_event(
     event, context, decode_authorizer_context: bool = True
 ):
     request_context = event.get("requestContext")
     domain = request_context.get("domainName")
     api_id = request_context.get("apiId")
     service_name = determine_service_name(
         service_mapping, api_id, "lambda_api_gateway", domain
     )
-    method = request_context.get("http", {}).get("method")
+    http = request_context.get("http") or {}
+    method = http.get("method")
     path = event.get("rawPath")
-    resource = "{0} {1}".format(method, path)
+    resource_path = _get_resource_path(event, request_context)
+    resource = f"{method} {resource_path}"
     tags = {
         "operation_name": "aws.httpapi",
         "endpoint": path,
         "http.url": domain + path,
-        "http.method": request_context.get("http", {}).get("method"),
-        "http.protocol": request_context.get("http", {}).get("protocol"),
-        "http.source_ip": request_context.get("http", {}).get("sourceIp"),
-        "http.user_agent": request_context.get("http", {}).get("userAgent"),
+        "http.method": http.get("method"),
+        "http.protocol": http.get("protocol"),
+        "http.source_ip": http.get("sourceIp"),
+        "http.user_agent": http.get("userAgent"),
         "resource_names": resource,
         "request_id": context.aws_request_id,
         "apiid": api_id,
         "apiname": api_id,
         "stage": request_context.get("stage"),
     }
     request_time_epoch_ms = int(request_context.get("timeEpoch"))
     if is_api_gateway_invocation_async(event):
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     else:
         InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="sync")
-    args = {
-        "service": service_name,
-        "resource": resource,
-        "span_type": "http",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
+    tracer.set_tags(_dd_origin)
     inferred_span_start_ns = request_time_epoch_ms * 1e6
     if decode_authorizer_context:
         injected_authorizer_data = get_injected_authorizer_data(event, True)
         if injected_authorizer_data:
             inferred_span_start_ns = injected_authorizer_data.get(
                 Headers.Parent_Span_Finish_Time
             )
-    span = tracer.trace("aws.httpapi", **args)
+    span = tracer.trace(
+        "aws.httpapi", service=service_name, resource=resource, span_type="http"
+    )
     if span:
         span.set_tags(tags)
         span.start_ns = int(inferred_span_start_ns)
     return span
 
 
 def create_inferred_span_from_sqs_event(event, context):
@@ -992,29 +994,25 @@
 
     event_record = get_first_record(event)
     event_source_arn = event_record.get("eventSourceARN")
     queue_name = event_source_arn.split(":")[-1]
     service_name = determine_service_name(
         service_mapping, queue_name, "lambda_sqs", "sqs"
     )
+    attrs = event_record.get("attributes") or {}
     tags = {
         "operation_name": "aws.sqs",
         "resource_names": queue_name,
         "queuename": queue_name,
         "event_source_arn": event_source_arn,
         "receipt_handle": event_record.get("receiptHandle"),
-        "sender_id": event_record.get("attributes", {}).get("SenderId"),
+        "sender_id": attrs.get("SenderId"),
     }
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
-    request_time_epoch = event_record.get("attributes", {}).get("SentTimestamp")
-    args = {
-        "service": service_name,
-        "resource": queue_name,
-        "span_type": "web",
-    }
+    request_time_epoch = attrs.get("SentTimestamp")
     start_time = int(request_time_epoch) / 1000
 
     upstream_span = None
     if "body" in event_record:
         body_str = event_record.get("body", {})
         try:
             body = json.loads(body_str)
@@ -1035,65 +1033,65 @@
                     upstream_span = create_inferred_span_from_eventbridge_event(
                         body, context
                     )
                     upstream_span.finish(finish_time=start_time)
 
         except Exception as e:
             logger.debug(
-                "Unable to create upstream span from SQS message, with error %s" % e
+                "Unable to create upstream span from SQS message, with error %s", e
             )
             pass
 
     # trace context needs to be set again as it is reset
     # when sns_span.finish executes
     tracer.context_provider.activate(trace_ctx)
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.sqs", **args)
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.sqs", service=service_name, resource=queue_name, span_type="web"
+    )
     if span:
         span.set_tags(tags)
     span.start = start_time
     if upstream_span:
         span.parent_id = upstream_span.span_id
 
     return span
 
 
 def create_inferred_span_from_sns_event(event, context):
     event_record = get_first_record(event)
-    sns_message = event_record.get("Sns")
-    topic_arn = event_record.get("Sns", {}).get("TopicArn")
+    sns_message = event_record.get("Sns") or {}
+    topic_arn = sns_message.get("TopicArn")
     topic_name = topic_arn.split(":")[-1]
     service_name = determine_service_name(
         service_mapping, topic_name, "lambda_sns", "sns"
     )
     tags = {
         "operation_name": "aws.sns",
         "resource_names": topic_name,
         "topicname": topic_name,
         "topic_arn": topic_arn,
         "message_id": sns_message.get("MessageId"),
         "type": sns_message.get("Type"),
     }
 
     # Subject not available in SNS => SQS scenario
-    if "Subject" in sns_message and sns_message["Subject"]:
-        tags["subject"] = sns_message.get("Subject")
+    subject = sns_message.get("Subject")
+    if subject:
+        tags["subject"] = subject
 
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
     sns_dt_format = "%Y-%m-%dT%H:%M:%S.%fZ"
-    timestamp = event_record.get("Sns", {}).get("Timestamp")
+    timestamp = sns_message.get("Timestamp")
     dt = datetime.strptime(timestamp, sns_dt_format)
 
-    args = {
-        "service": service_name,
-        "resource": topic_name,
-        "span_type": "web",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.sns", **args)
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.sns", service=service_name, resource=topic_name, span_type="web"
+    )
     if span:
         span.set_tags(tags)
     span.start = dt.replace(tzinfo=timezone.utc).timestamp()
     return span
 
 
 def create_inferred_span_from_kinesis_event(event, context):
@@ -1101,108 +1099,99 @@
     event_source_arn = event_record.get("eventSourceARN")
     event_id = event_record.get("eventID")
     stream_name = event_source_arn.split(":")[-1]
     shard_id = event_id.split(":")[0]
     service_name = determine_service_name(
         service_mapping, stream_name, "lambda_kinesis", "kinesis"
     )
+    kinesis = event_record.get("kinesis") or {}
     tags = {
         "operation_name": "aws.kinesis",
         "resource_names": stream_name,
         "streamname": stream_name,
         "shardid": shard_id,
         "event_source_arn": event_source_arn,
         "event_id": event_id,
         "event_name": event_record.get("eventName"),
         "event_version": event_record.get("eventVersion"),
-        "partition_key": event_record.get("kinesis", {}).get("partitionKey"),
+        "partition_key": kinesis.get("partitionKey"),
     }
     InferredSpanInfo.set_tags(tags, tag_source="self", synchronicity="async")
-    request_time_epoch = event_record.get("kinesis", {}).get(
-        "approximateArrivalTimestamp"
-    )
+    request_time_epoch = kinesis.get("approximateArrivalTimestamp")
 
-    args = {
-        "service": service_name,
-        "resource": stream_name,
-        "span_type": "web",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.kinesis", **args)
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.kinesis", service=service_name, resource=stream_name, span_type="web"
+    )
     if span:
         span.set_tags(tags)
     span.start = request_time_epoch
     return span
 
 
 def create_inferred_span_from_dynamodb_event(event, context):
     event_record = get_first_record(event)
     event_source_arn = event_record.get("eventSourceARN")
     table_name = event_source_arn.split("/")[1]
     service_name = determine_service_name(
         service_mapping, table_name, "lambda_dynamodb", "dynamodb"
     )
-    dynamodb_message = event_record.get("dynamodb")
+    dynamodb_message = event_record.get("dynamodb") or {}
     tags = {
         "operation_name": "aws.dynamodb",
         "resource_names": table_name,
         "tablename": table_name,
         "event_source_arn": event_source_arn,
         "event_id": event_record.get("eventID"),
         "event_name": event_record.get("eventName"),
         "event_version": event_record.get("eventVersion"),
         "stream_view_type": dynamodb_message.get("StreamViewType"),
         "size_bytes": str(dynamodb_message.get("SizeBytes")),
     }
     InferredSpanInfo.set_tags(tags, synchronicity="async", tag_source="self")
-    request_time_epoch = event_record.get("dynamodb", {}).get(
-        "ApproximateCreationDateTime"
+    request_time_epoch = dynamodb_message.get("ApproximateCreationDateTime")
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.dynamodb", service=service_name, resource=table_name, span_type="web"
     )
-    args = {
-        "service": service_name,
-        "resource": table_name,
-        "span_type": "web",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.dynamodb", **args)
     if span:
         span.set_tags(tags)
 
     span.start = int(request_time_epoch)
     return span
 
 
 def create_inferred_span_from_s3_event(event, context):
     event_record = get_first_record(event)
-    bucket_name = event_record.get("s3", {}).get("bucket", {}).get("name")
+    s3 = event_record.get("s3") or {}
+    bucket = s3.get("bucket") or {}
+    obj = s3.get("object") or {}
+    bucket_name = bucket.get("name")
     service_name = determine_service_name(
         service_mapping, bucket_name, "lambda_s3", "s3"
     )
     tags = {
         "operation_name": "aws.s3",
         "resource_names": bucket_name,
         "event_name": event_record.get("eventName"),
         "bucketname": bucket_name,
-        "bucket_arn": event_record.get("s3", {}).get("bucket", {}).get("arn"),
-        "object_key": event_record.get("s3", {}).get("object", {}).get("key"),
-        "object_size": str(event_record.get("s3", {}).get("object", {}).get("size")),
-        "object_etag": event_record.get("s3", {}).get("object", {}).get("eTag"),
+        "bucket_arn": bucket.get("arn"),
+        "object_key": obj.get("key"),
+        "object_size": str(obj.get("size")),
+        "object_etag": obj.get("eTag"),
     }
     InferredSpanInfo.set_tags(tags, synchronicity="async", tag_source="self")
     dt_format = "%Y-%m-%dT%H:%M:%S.%fZ"
     timestamp = event_record.get("eventTime")
     dt = datetime.strptime(timestamp, dt_format)
 
-    args = {
-        "service": service_name,
-        "resource": bucket_name,
-        "span_type": "web",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.s3", **args)
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.s3", service=service_name, resource=bucket_name, span_type="web"
+    )
     if span:
         span.set_tags(tags)
     span.start = dt.replace(tzinfo=timezone.utc).timestamp()
     return span
 
 
 def create_inferred_span_from_eventbridge_event(event, context):
@@ -1220,21 +1209,18 @@
         synchronicity="async",
         tag_source="self",
     )
     dt_format = "%Y-%m-%dT%H:%M:%SZ"
     timestamp = event.get("time")
     dt = datetime.strptime(timestamp, dt_format)
 
-    args = {
-        "service": service_name,
-        "resource": source,
-        "span_type": "web",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.eventbridge", **args)
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.eventbridge", service=service_name, resource=source, span_type="web"
+    )
     if span:
         span.set_tags(tags)
     span.start = dt.replace(tzinfo=timezone.utc).timestamp()
     return span
 
 
 def create_function_execution_span(
@@ -1243,15 +1229,15 @@
     is_cold_start,
     is_proactive_init,
     trace_context_source,
     merge_xray_traces,
     trigger_tags,
     parent_span=None,
 ):
-    tags = {}
+    tags = None
     if context:
         function_arn = (context.invoked_function_arn or "").lower()
         tk = function_arn.split(":")
         function_arn = ":".join(tk[0:7]) if len(tk) > 7 else function_arn
         function_version = tk[7] if len(tk) > 7 else "$LATEST"
         tags = {
             "cold_start": str(is_cold_start).lower(),
@@ -1262,26 +1248,27 @@
             "functionname": context.function_name.lower()
             if context.function_name
             else None,
             "datadog_lambda": datadog_lambda_version,
             "dd_trace": ddtrace_version,
             "span.name": "aws.lambda",
         }
+    tags = tags or {}
     if is_proactive_init:
         tags["proactive_initialization"] = str(is_proactive_init).lower()
     if trace_context_source == TraceContextSource.XRAY and merge_xray_traces:
         tags["_dd.parent_source"] = trace_context_source
     tags.update(trigger_tags)
-    args = {
-        "service": "aws.lambda",
-        "resource": function_name,
-        "span_type": "serverless",
-    }
-    tracer.set_tags({"_dd.origin": "lambda"})
-    span = tracer.trace("aws.lambda", **args)
+    tracer.set_tags(_dd_origin)
+    span = tracer.trace(
+        "aws.lambda",
+        service="aws.lambda",
+        resource=function_name,
+        span_type="serverless",
+    )
     if span:
         span.set_tags(tags)
     if parent_span:
         span.parent_id = parent_span.span_id
     return span
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/trigger.py` & `datadog_lambda-5.93.0/datadog_lambda/trigger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Unless explicitly stated otherwise all files in this repository are licensed
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
 
 import base64
 import gzip
-import json
+import ujson as json
 from io import BytesIO, BufferedReader
 from enum import Enum
 from typing import Any
 
 
 class _stringTypedEnum(Enum):
     """
@@ -106,31 +106,31 @@
     records = event.get("Records")
     if records and len(records) > 0:
         return records[0]
 
 
 def parse_event_source(event: dict) -> _EventSource:
     """Determines the source of the trigger event"""
-    if type(event) is not dict:
+    if not isinstance(event, dict):
         return _EventSource(EventTypes.UNKNOWN)
 
-    event_source = _EventSource(EventTypes.UNKNOWN)
+    event_source = None
 
     request_context = event.get("requestContext")
     if request_context and request_context.get("stage"):
         if "domainName" in request_context and detect_lambda_function_url_domain(
             request_context.get("domainName")
         ):
             return _EventSource(EventTypes.LAMBDA_FUNCTION_URL)
         event_source = _EventSource(EventTypes.API_GATEWAY)
         if "httpMethod" in event:
             event_source.subtype = EventSubtypes.API_GATEWAY
         if "routeKey" in event:
             event_source.subtype = EventSubtypes.HTTP_API
-        if event.get("requestContext", {}).get("messageDirection"):
+        if request_context.get("messageDirection"):
             event_source.subtype = EventSubtypes.WEBSOCKET
 
     if request_context and request_context.get("elb"):
         event_source = _EventSource(EventTypes.ALB)
 
     if event.get("awslogs"):
         event_source = _EventSource(EventTypes.CLOUDWATCH_LOGS)
@@ -147,33 +147,31 @@
         event_source = _EventSource(EventTypes.CLOUDWATCH_EVENTS)
 
     if "Execution" in event and "StateMachine" in event and "State" in event:
         event_source = _EventSource(EventTypes.STEPFUNCTIONS)
 
     event_record = get_first_record(event)
     if event_record:
-        aws_event_source = event_record.get(
-            "eventSource", event_record.get("EventSource")
+        aws_event_source = event_record.get("eventSource") or event_record.get(
+            "EventSource"
         )
-
         if aws_event_source == "aws:dynamodb":
             event_source = _EventSource(EventTypes.DYNAMODB)
         if aws_event_source == "aws:kinesis":
             event_source = _EventSource(EventTypes.KINESIS)
         if aws_event_source == "aws:s3":
             event_source = _EventSource(EventTypes.S3)
         if aws_event_source == "aws:sns":
             event_source = _EventSource(EventTypes.SNS)
         if aws_event_source == "aws:sqs":
             event_source = _EventSource(EventTypes.SQS)
-
         if event_record.get("cf"):
             event_source = _EventSource(EventTypes.CLOUDFRONT)
 
-    return event_source
+    return event_source or _EventSource(EventTypes.UNKNOWN)
 
 
 def detect_lambda_function_url_domain(domain: str) -> bool:
     #  e.g. "etsn5fibjr.lambda-url.eu-south-1.amazonaws.com"
     domain_parts = domain.split(".")
     if len(domain_parts) < 2:
         return False
@@ -189,28 +187,34 @@
     region = split_function_arn[3]
     account_id = split_function_arn[4]
     aws_arn = get_aws_partition_by_region(region)
 
     event_record = get_first_record(event)
     # e.g. arn:aws:s3:::lambda-xyz123-abc890
     if source.to_string() == "s3":
-        return event_record.get("s3", {}).get("bucket", {}).get("arn")
+        s3 = event_record.get("s3")
+        if s3:
+            bucket = s3.get("bucket")
+            if bucket:
+                return bucket.get("arn")
+        return None
 
     # e.g. arn:aws:sns:us-east-1:123456789012:sns-lambda
     if source.to_string() == "sns":
-        return event_record.get("Sns", {}).get("TopicArn")
+        sns = event_record.get("Sns")
+        if sns:
+            return sns.get("TopicArn")
+        return None
 
     # e.g. arn:aws:cloudfront::123456789012:distribution/ABC123XYZ
     if source.event_type == EventTypes.CLOUDFRONT:
         distribution_id = (
             event_record.get("cf", {}).get("config", {}).get("distributionId")
         )
-        return "arn:{}:cloudfront::{}:distribution/{}".format(
-            aws_arn, account_id, distribution_id
-        )
+        return f"arn:{aws_arn}:cloudfront::{account_id}:distribution/{distribution_id}"
 
     # e.g. arn:aws:lambda:<region>:<account_id>:url:<function-name>:<function-qualifier>
     if source.equals(EventTypes.LAMBDA_FUNCTION_URL):
         function_name = ""
         if len(split_function_arn) >= 7:
             function_name = split_function_arn[6]
         function_arn = f"arn:aws:lambda:{region}:{account_id}:url:{function_name}"
@@ -219,34 +223,36 @@
             function_qualifier = split_function_arn[7]
             function_arn = function_arn + f":{function_qualifier}"
         return function_arn
 
     # e.g. arn:aws:apigateway:us-east-1::/restapis/xyz123/stages/default
     if source.event_type == EventTypes.API_GATEWAY:
         request_context = event.get("requestContext")
-        return "arn:{}:apigateway:{}::/restapis/{}/stages/{}".format(
-            aws_arn, region, request_context.get("apiId"), request_context.get("stage")
-        )
+        api_id = request_context.get("apiId")
+        stage = request_context.get("stage")
+        return f"arn:{aws_arn}:apigateway:{region}::/restapis/{api_id}/stages/{stage}"
 
     # e.g. arn:aws:elasticloadbalancing:us-east-1:123456789012:targetgroup/lambda-xyz/123
     if source.event_type == EventTypes.ALB:
         request_context = event.get("requestContext")
-        return request_context.get("elb", {}).get("targetGroupArn")
+        if request_context:
+            elb = request_context.get("elb")
+            if elb:
+                return elb.get("targetGroupArn")
+        return None
 
     # e.g. arn:aws:logs:us-west-1:123456789012:log-group:/my-log-group-xyz
     if source.event_type == EventTypes.CLOUDWATCH_LOGS:
         with gzip.GzipFile(
             fileobj=BytesIO(base64.b64decode(event.get("awslogs", {}).get("data")))
         ) as decompress_stream:
             data = b"".join(BufferedReader(decompress_stream))
         logs = json.loads(data)
         log_group = logs.get("logGroup", "cloudwatch")
-        return "arn:{}:logs:{}:{}:log-group:{}".format(
-            aws_arn, region, account_id, log_group
-        )
+        return f"arn:{aws_arn}:logs:{region}:{account_id}:log-group:{log_group}"
 
     # e.g. arn:aws:events:us-east-1:123456789012:rule/my-schedule
     if source.event_type == EventTypes.CLOUDWATCH_EVENTS and event.get("resources"):
         return event.get("resources")[0]
 
 
 def get_event_source_arn(source: _EventSource, event: dict, context: Any) -> str:
@@ -292,56 +298,54 @@
     headers = event.get("headers")
     if headers and headers.get("Referer"):
         http_tags["http.referer"] = headers.get("Referer")
 
     return http_tags
 
 
+_http_event_types = (
+    EventTypes.API_GATEWAY,
+    EventTypes.ALB,
+    EventTypes.LAMBDA_FUNCTION_URL,
+)
+
+
 def extract_trigger_tags(event: dict, context: Any) -> dict:
     """
     Parses the trigger event object to get tags to be added to the span metadata
     """
     trigger_tags = {}
     event_source = parse_event_source(event)
     if event_source.to_string() is not None and event_source.to_string() != "unknown":
         trigger_tags["function_trigger.event_source"] = event_source.to_string()
 
         event_source_arn = get_event_source_arn(event_source, event, context)
         if event_source_arn:
             trigger_tags["function_trigger.event_source_arn"] = event_source_arn
 
-    if event_source.event_type in [
-        EventTypes.API_GATEWAY,
-        EventTypes.ALB,
-        EventTypes.LAMBDA_FUNCTION_URL,
-    ]:
+    if event_source.event_type in _http_event_types:
         trigger_tags.update(extract_http_tags(event))
 
     return trigger_tags
 
 
+_str_http_triggers = [et.value for et in _http_event_types]
+
+
 def extract_http_status_code_tag(trigger_tags, response):
     """
     If the Lambda was triggered by API Gateway, Lambda Function URL, or ALB,
     add the returned status code as a tag to the function execution span.
     """
     if trigger_tags is None:
         return
     str_event_source = trigger_tags.get("function_trigger.event_source")
     # it would be cleaner if each event type was a constant object that
     # knew some properties about itself like this.
-    str_http_triggers = [
-        et.value
-        for et in [
-            EventTypes.API_GATEWAY,
-            EventTypes.LAMBDA_FUNCTION_URL,
-            EventTypes.ALB,
-        ]
-    ]
-    if str_event_source not in str_http_triggers:
+    if str_event_source not in _str_http_triggers:
         return
 
     status_code = "200"
     if response is None:
         # Return a 502 status if no response is found
         status_code = "502"
     elif hasattr(response, "get"):
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/wrapper.py` & `datadog_lambda-5.93.0/datadog_lambda/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
 import base64
 import os
 import logging
 import traceback
+import ujson as json
 from importlib import import_module
-import json
 from time import time_ns
 
 from datadog_lambda.extension import should_use_extension, flush_extension
 from datadog_lambda.cold_start import (
     set_cold_start,
     is_cold_start,
     is_proactive_init,
@@ -254,15 +254,17 @@
         injected_headers = {}
         source_span = self.inferred_span if self.inferred_span else self.span
         span_context = source_span.context
         propagator.inject(span_context, injected_headers)
         injected_headers[Headers.Parent_Span_Finish_Time] = finish_time_ns
         if request_id is not None:
             injected_headers[Headers.Authorizing_Request_Id] = request_id
-        datadog_data = base64.b64encode(json.dumps(injected_headers).encode()).decode()
+        datadog_data = base64.b64encode(
+            json.dumps(injected_headers, escape_forward_slashes=False).encode()
+        ).decode()
         self.response.setdefault("context", {})
         self.response["context"]["_datadog"] = datadog_data
 
     def _before(self, event, context):
         try:
             self.response = None
             set_cold_start(init_timestamp_ns)
@@ -377,13 +379,12 @@
                 )
             logger.debug("datadog_lambda_wrapper _after() done")
         except Exception as e:
             logger.error(format_err_with_traceback(e))
 
 
 def format_err_with_traceback(e):
-    return "Error {}. Traceback: {}".format(
-        e, traceback.format_exc().replace("\n", "\r")
-    )
+    tb = traceback.format_exc().replace("\n", "\r")
+    return f"Error {e}. Traceback: {tb}"
 
 
 datadog_lambda_wrapper = _LambdaDecorator
```

### Comparing `datadog_lambda-5.92.0/datadog_lambda/xray.py` & `datadog_lambda-5.93.0/datadog_lambda/xray.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 import os
 import logging
-import json
 import binascii
 import time
 import socket
+import ujson as json
 
 from datadog_lambda.constants import XrayDaemon, XraySubsegment, TraceContextSource
 
 logger = logging.getLogger(__name__)
 
 
-def get_xray_host_port(address):
-    if address == "":
-        logger.debug("X-Ray daemon env var not set, not sending sub-segment")
-        return None
-    parts = address.split(":")
-    if len(parts) <= 1:
-        logger.debug("X-Ray daemon env var not set, not sending sub-segment")
-        return None
-    port = int(parts[1])
-    host = parts[0]
-    return (host, port)
-
-
-def send(host_port_tuple, payload):
-    sock = None
-    try:
-        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        sock.setblocking(0)
-        sock.connect(host_port_tuple)
-        sock.send(payload.encode("utf-8"))
-    except Exception as e_send:
-        logger.error("Error occurred submitting to xray daemon: %s", str(e_send))
-    try:
-        sock.close()
-    except Exception as e_close:
-        logger.error("Error while closing the socket: %s", str(e_close))
+class Socket(object):
+    def __init__(self):
+        self.sock = None
+
+    @property
+    def host_port_tuple(self):
+        if not hasattr(self, "_host_port_tuple"):
+            self._host_port_tuple = self._get_xray_host_port(
+                os.environ.get(XrayDaemon.XRAY_DAEMON_ADDRESS, "")
+            )
+        return self._host_port_tuple
+
+    def send(self, payload):
+        if not self.sock:
+            self._connect()
+        try:
+            self.sock.send(payload.encode("utf-8"))
+        except Exception as e_send:
+            logger.error("Error occurred submitting to xray daemon: %s", e_send)
+
+    def _connect(self):
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.sock.setblocking(0)
+        self.sock.connect(self.host_port_tuple)
+
+    def _get_xray_host_port(self, address):
+        if address == "":
+            logger.debug("X-Ray daemon env var not set, not sending sub-segment")
+            return None
+        parts = address.split(":")
+        if len(parts) <= 1:
+            logger.debug("X-Ray daemon env var not set, not sending sub-segment")
+            return None
+        port = int(parts[1])
+        host = parts[0]
+        return (host, port)
+
+
+sock = Socket()
 
 
 def build_segment_payload(payload):
     if payload is None:
         return None
-    return '{"format": "json", "version": 1}' + "\n" + payload
+    return '{"format": "json", "version": 1}\n' + payload
 
 
 def parse_xray_header(raw_trace_id):
     # Example:
     # Root=1-5e272390-8c398be037738dc042009320;Parent=94ae789b969f1cc5;Sampled=1;Lineage=c6c5b1b9:0
     logger.debug("Reading trace context from env var %s", raw_trace_id)
     if len(raw_trace_id) == 0:
@@ -85,24 +98,22 @@
             "end_time": time.time(),
             "type": "subsegment",
             "metadata": {
                 XraySubsegment.NAMESPACE: {
                     key: metadata,
                 }
             },
-        }
+        },
+        escape_forward_slashes=False,
     )
     return segment
 
 
 def send_segment(key, metadata):
-    host_port_tuple = get_xray_host_port(
-        os.environ.get(XrayDaemon.XRAY_DAEMON_ADDRESS, "")
-    )
-    if host_port_tuple is None:
+    if sock.host_port_tuple is None:
         return None
     context = parse_xray_header(
         os.environ.get(XrayDaemon.XRAY_TRACE_ID_HEADER_NAME, "")
     )
     if context is None:
         logger.debug(
             "Failed to create segment since it was not possible to get trace context from header"
@@ -111,8 +122,8 @@
 
     # Skip adding segment, if the xray trace is going to be sampled away.
     if context["sampled"] == "0":
         logger.debug("Skipping sending metadata, x-ray trace was sampled out")
         return None
     segment = build_segment(context, key, metadata)
     segment_payload = build_segment_payload(segment)
-    send(host_port_tuple, segment_payload)
+    sock.send(segment_payload)
```

### Comparing `datadog_lambda-5.92.0/pyproject.toml` & `datadog_lambda-5.93.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "5.92.0"
+version = "5.93.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
@@ -24,30 +24,34 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4"
 datadog = ">=0.41.0,<1.0.0"
 wrapt = "^1.11.2"
 ddtrace = ">=2.7.2"
+ujson = ">=5.9.0"
 urllib3 = [
     {version = "<2.0.0", python = "<3.11", optional = true},
     {version = "<2.1.0", python = ">=3.11", optional = true},
 ]
-importlib_metadata = {version = "*", python = "<3.8"}
 boto3 = { version = "^1.28.0", optional = true }
-typing_extensions = {version = "^4.0", python = "<3.8"}
 requests = { version ="^2.22.0", optional = true }
 pytest = { version= "^8.0.0", optional = true }
+pytest-benchmark = { version = "^4.0", optional = true }
 flake8 = { version = "^5.0.4", optional = true }
 
 
 [tool.poetry.extras]
 dev = [
     "boto3",
     "flake8",
     "pytest",
+    "pytest-benchmark",
     "requests",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+addopts = "--benchmark-disable --benchmark-autosave"
```

### Comparing `datadog_lambda-5.92.0/PKG-INFO` & `datadog_lambda-5.93.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog_lambda
-Version: 5.92.0
+Version: 5.93.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.8.0,<4
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Requires-Dist: boto3 (>=1.28.0,<2.0.0) ; extra == "dev"
 Requires-Dist: datadog (>=0.41.0,<1.0.0)
 Requires-Dist: ddtrace (>=2.7.2)
 Requires-Dist: flake8 (>=5.0.4,<6.0.0) ; extra == "dev"
-Requires-Dist: importlib_metadata ; python_version < "3.8"
 Requires-Dist: pytest (>=8.0.0,<9.0.0) ; extra == "dev"
+Requires-Dist: pytest-benchmark (>=4.0,<5.0) ; extra == "dev"
 Requires-Dist: requests (>=2.22.0,<3.0.0) ; extra == "dev"
-Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version < "3.8"
+Requires-Dist: ujson (>=5.9.0)
 Requires-Dist: urllib3 (<2.0.0) ; python_version < "3.11"
 Requires-Dist: urllib3 (<2.1.0) ; python_version >= "3.11"
 Requires-Dist: wrapt (>=1.11.2,<2.0.0)
 Project-URL: Repository, https://github.com/DataDog/datadog-lambda-python
 Description-Content-Type: text/markdown
 
 # datadog-lambda-python
```


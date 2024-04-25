# Comparing `tmp/great_expectations_cloud-20240424.0.tar.gz` & `tmp/great_expectations_cloud-20240425.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240424.0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240425.0.tar", max compression
```

## Comparing `great_expectations_cloud-20240424.0.tar` & `great_expectations_cloud-20240425.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-24 18:01:13.866627 great_expectations_cloud-20240424.0/LICENSE
--rw-r--r--   0        0        0     9269 2024-04-24 18:01:13.866627 great_expectations_cloud-20240424.0/README.md
--rw-r--r--   0        0        0      150 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    16465 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5395 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9457 2024-04-24 18:01:13.902627 great_expectations_cloud-20240424.0/pyproject.toml
--rw-r--r--   0        0        0    10598 1970-01-01 00:00:00.000000 great_expectations_cloud-20240424.0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-25 18:18:38.263824 great_expectations_cloud-20240425.0/LICENSE
+-rw-r--r--   0        0        0     9269 2024-04-25 18:18:38.263824 great_expectations_cloud-20240425.0/README.md
+-rw-r--r--   0        0        0      150 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-25 18:18:38.295824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    16116 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5395 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9457 2024-04-25 18:18:38.299824 great_expectations_cloud-20240425.0/pyproject.toml
+-rw-r--r--   0        0        0    10598 1970-01-01 00:00:00.000000 great_expectations_cloud-20240425.0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240424.0/LICENSE` & `great_expectations_cloud-20240425.0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/README.md` & `great_expectations_cloud-20240425.0/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
     """
 
     _PYPI_GX_AGENT_PACKAGE_NAME = "great_expectations_cloud"
     _PYPI_GREAT_EXPECTATIONS_PACKAGE_NAME = "great_expectations"
 
     def __init__(self: Self):
         agent_version: str = self.get_current_gx_agent_version()
-        great_expectations_version: str = self._get_current_great_expectations_version()
         print(f"GX Agent version: {agent_version}")
-        print(f"Great Expectations version: {great_expectations_version}")
         print("Initializing the GX Agent.")
         self._set_http_session_headers()
         self._config = self._get_config()
         print("Loading a DataContext - this might take a moment.")
 
         with warnings.catch_warnings():
             # suppress warnings about GX version
@@ -154,19 +152,14 @@
                 subscriber.close()
 
     @classmethod
     def get_current_gx_agent_version(cls) -> str:
         version: str = metadata_version(cls._PYPI_GX_AGENT_PACKAGE_NAME)
         return version
 
-    @classmethod
-    def _get_current_great_expectations_version(cls) -> str:
-        version: str = metadata_version(cls._PYPI_GREAT_EXPECTATIONS_PACKAGE_NAME)
-        return version
-
     def _handle_event_as_thread_enter(self, event_context: EventContext) -> None:
         """Schedule _handle_event to run in a thread.
 
         Callback passed to Subscriber.consume which forwards events to
         the EventHandler for processing.
 
         Args:
```

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240425.0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240425.0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240424.0/pyproject.toml` & `great_expectations_cloud-20240425.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240424.0"
+version = "20240425.0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240424.0/PKG-INFO` & `great_expectations_cloud-20240425.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240424.0
+Version: 20240425.0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
```


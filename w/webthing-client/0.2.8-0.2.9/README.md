# Comparing `tmp/webthing_client-0.2.8.tar.gz` & `tmp/webthing_client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webthing_client-0.2.8.tar", max compression
+gzip compressed data, was "webthing_client-0.2.9.tar", max compression
```

## Comparing `webthing_client-0.2.8.tar` & `webthing_client-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1649 2023-02-06 09:57:29.936975 webthing_client-0.2.8/LICENSE
--rw-r--r--   0        0        0      629 2024-04-16 07:02:16.402645 webthing_client-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      325 2023-09-01 06:19:20.858836 webthing_client-0.2.8/README.md
--rw-r--r--   0        0        0        0 2023-09-01 06:19:20.859837 webthing_client-0.2.8/webthing_client/__init__.py
--rw-r--r--   0        0        0    32194 2024-04-16 06:52:52.447000 webthing_client-0.2.8/webthing_client/client.py
--rw-r--r--   0        0        0     1110 2024-02-25 09:18:17.801821 webthing_client-0.2.8/webthing_client/input/action/event_input.py
--rw-r--r--   0        0        0      559 2024-02-25 09:18:25.339336 webthing_client-0.2.8/webthing_client/input/action/event_type_input.py
--rw-r--r--   0        0        0      552 2024-02-28 12:31:21.667211 webthing_client-0.2.8/webthing_client/input/action/from_to_user_input.py
--rw-r--r--   0        0        0      335 2024-02-25 09:18:47.773047 webthing_client-0.2.8/webthing_client/input/action/iri_user_input.py
--rw-r--r--   0        0        0      958 2024-02-25 09:50:00.172735 webthing_client-0.2.8/webthing_client/input/action/resolution_input.py
--rw-r--r--   0        0        0      501 2024-02-28 12:31:21.674209 webthing_client-0.2.8/webthing_client/input/from_to_input.py
--rw-r--r--   0        0        0      284 2024-02-25 09:17:40.428692 webthing_client-0.2.8/webthing_client/input/iri_input.py
--rw-r--r--   0        0        0      573 2024-02-29 08:15:42.300381 webthing_client-0.2.8/webthing_client/input/property_observations_input.py
--rw-r--r--   0        0        0     1262 2024-04-11 11:55:16.307929 webthing_client-0.2.8/webthing_client/input/replay/replay_input.py
--rw-r--r--   0        0        0     1497 2024-03-07 08:08:34.615412 webthing_client-0.2.8/webthing_client/model/action/action.py
--rw-r--r--   0        0        0      483 2024-02-25 08:39:10.164817 webthing_client-0.2.8/webthing_client/model/action/base.py
--rw-r--r--   0        0        0     5769 2024-03-07 08:10:40.389847 webthing_client-0.2.8/webthing_client/model/action/operation/operation.py
--rw-r--r--   0        0        0     1354 2024-03-07 08:09:59.699008 webthing_client-0.2.8/webthing_client/model/action/request.py
--rw-r--r--   0        0        0     2303 2024-04-02 09:37:23.149678 webthing_client-0.2.8/webthing_client/model/action/resolution.py
--rw-r--r--   0        0        0     2576 2024-03-08 10:35:26.561490 webthing_client-0.2.8/webthing_client/model/event/event.py
--rw-r--r--   0        0        0     2167 2024-03-07 08:11:29.041992 webthing_client-0.2.8/webthing_client/model/event/event_type.py
--rw-r--r--   0        0        0     1078 2024-02-25 09:10:43.844340 webthing_client-0.2.8/webthing_client/model/event/feedback.py
--rw-r--r--   0        0        0     2792 2024-03-07 14:05:26.244036 webthing_client-0.2.8/webthing_client/model/event/feedback_schema.py
--rw-r--r--   0        0        0      845 2024-02-28 12:31:21.667211 webthing_client-0.2.8/webthing_client/model/event/observation.py
--rw-r--r--   0        0        0     1276 2024-02-23 16:53:39.147090 webthing_client-0.2.8/webthing_client/model/event/stimulus.py
--rw-r--r--   0        0        0      125 2024-03-07 08:09:17.428059 webthing_client-0.2.8/webthing_client/model/ontology.py
--rw-r--r--   0        0        0      591 2024-02-29 09:01:40.135207 webthing_client-0.2.8/webthing_client/model/property/observable_property.py
--rw-r--r--   0        0        0     3781 2024-04-16 06:59:05.967785 webthing_client-0.2.8/webthing_client/model/replay/replay.py
--rw-r--r--   0        0        0      871 2024-02-25 08:42:01.491567 webthing_client-0.2.8/webthing_client/model/system/sensor.py
--rw-r--r--   0        0        0      890 2024-02-25 08:41:34.495865 webthing_client-0.2.8/webthing_client/model/system/system.py
--rw-r--r--   0        0        0     1635 2024-03-07 08:12:27.305511 webthing_client-0.2.8/webthing_client/model/user/user.py
--rw-r--r--   0        0        0      900 2024-02-28 12:31:21.670210 webthing_client-0.2.8/webthing_client/model/webthing_observation.py
--rw-r--r--   0        0        0        0 2021-11-19 14:10:06.477733 webthing_client-0.2.8/webthing_client/standard_api/__init__.py
--rw-r--r--   0        0        0     9996 2023-06-07 11:34:51.827080 webthing_client-0.2.8/webthing_client/standard_api/api_handler.py
--rw-r--r--   0        0        0     1651 2021-11-29 12:35:22.731824 webthing_client-0.2.8/webthing_client/standard_api/api_marshalling.py
--rw-r--r--   0        0        0     6354 2024-03-20 12:02:38.241459 webthing_client-0.2.8/webthing_client/stomp.py
--rw-r--r--   0        0        0     1897 2024-04-11 10:57:32.328600 webthing_client-0.2.8/webthing_client/utils.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 webthing_client-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1649 2023-02-06 09:57:29.936975 webthing_client-0.2.9/LICENSE
+-rw-r--r--   0        0        0      629 2024-04-19 07:03:30.820037 webthing_client-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-09-01 06:19:20.858836 webthing_client-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-09-01 06:19:20.859837 webthing_client-0.2.9/webthing_client/__init__.py
+-rw-r--r--   0        0        0    32194 2024-04-16 06:52:52.447000 webthing_client-0.2.9/webthing_client/client.py
+-rw-r--r--   0        0        0     1110 2024-02-25 09:18:17.801821 webthing_client-0.2.9/webthing_client/input/action/event_input.py
+-rw-r--r--   0        0        0      559 2024-02-25 09:18:25.339336 webthing_client-0.2.9/webthing_client/input/action/event_type_input.py
+-rw-r--r--   0        0        0      552 2024-02-28 12:31:21.667211 webthing_client-0.2.9/webthing_client/input/action/from_to_user_input.py
+-rw-r--r--   0        0        0      335 2024-02-25 09:18:47.773047 webthing_client-0.2.9/webthing_client/input/action/iri_user_input.py
+-rw-r--r--   0        0        0      958 2024-02-25 09:50:00.172735 webthing_client-0.2.9/webthing_client/input/action/resolution_input.py
+-rw-r--r--   0        0        0      501 2024-02-28 12:31:21.674209 webthing_client-0.2.9/webthing_client/input/from_to_input.py
+-rw-r--r--   0        0        0      284 2024-02-25 09:17:40.428692 webthing_client-0.2.9/webthing_client/input/iri_input.py
+-rw-r--r--   0        0        0      573 2024-02-29 08:15:42.300381 webthing_client-0.2.9/webthing_client/input/property_observations_input.py
+-rw-r--r--   0        0        0     1262 2024-04-11 11:55:16.307929 webthing_client-0.2.9/webthing_client/input/replay/replay_input.py
+-rw-r--r--   0        0        0     1497 2024-03-07 08:08:34.615412 webthing_client-0.2.9/webthing_client/model/action/action.py
+-rw-r--r--   0        0        0      483 2024-02-25 08:39:10.164817 webthing_client-0.2.9/webthing_client/model/action/base.py
+-rw-r--r--   0        0        0     5769 2024-03-07 08:10:40.389847 webthing_client-0.2.9/webthing_client/model/action/operation/operation.py
+-rw-r--r--   0        0        0     1354 2024-03-07 08:09:59.699008 webthing_client-0.2.9/webthing_client/model/action/request.py
+-rw-r--r--   0        0        0     2303 2024-04-02 09:37:23.149678 webthing_client-0.2.9/webthing_client/model/action/resolution.py
+-rw-r--r--   0        0        0     2576 2024-03-08 10:35:26.561490 webthing_client-0.2.9/webthing_client/model/event/event.py
+-rw-r--r--   0        0        0     2167 2024-03-07 08:11:29.041992 webthing_client-0.2.9/webthing_client/model/event/event_type.py
+-rw-r--r--   0        0        0     1078 2024-02-25 09:10:43.844340 webthing_client-0.2.9/webthing_client/model/event/feedback.py
+-rw-r--r--   0        0        0     2820 2024-04-19 07:01:04.451388 webthing_client-0.2.9/webthing_client/model/event/feedback_schema.py
+-rw-r--r--   0        0        0      845 2024-02-28 12:31:21.667211 webthing_client-0.2.9/webthing_client/model/event/observation.py
+-rw-r--r--   0        0        0     1276 2024-02-23 16:53:39.147090 webthing_client-0.2.9/webthing_client/model/event/stimulus.py
+-rw-r--r--   0        0        0      125 2024-03-07 08:09:17.428059 webthing_client-0.2.9/webthing_client/model/ontology.py
+-rw-r--r--   0        0        0      591 2024-02-29 09:01:40.135207 webthing_client-0.2.9/webthing_client/model/property/observable_property.py
+-rw-r--r--   0        0        0     3781 2024-04-16 06:59:05.967785 webthing_client-0.2.9/webthing_client/model/replay/replay.py
+-rw-r--r--   0        0        0      871 2024-02-25 08:42:01.491567 webthing_client-0.2.9/webthing_client/model/system/sensor.py
+-rw-r--r--   0        0        0      890 2024-02-25 08:41:34.495865 webthing_client-0.2.9/webthing_client/model/system/system.py
+-rw-r--r--   0        0        0     1635 2024-03-07 08:12:27.305511 webthing_client-0.2.9/webthing_client/model/user/user.py
+-rw-r--r--   0        0        0      900 2024-02-28 12:31:21.670210 webthing_client-0.2.9/webthing_client/model/webthing_observation.py
+-rw-r--r--   0        0        0        0 2021-11-19 14:10:06.477733 webthing_client-0.2.9/webthing_client/standard_api/__init__.py
+-rw-r--r--   0        0        0     9996 2023-06-07 11:34:51.827080 webthing_client-0.2.9/webthing_client/standard_api/api_handler.py
+-rw-r--r--   0        0        0     1651 2021-11-29 12:35:22.731824 webthing_client-0.2.9/webthing_client/standard_api/api_marshalling.py
+-rw-r--r--   0        0        0     6354 2024-03-20 12:02:38.241459 webthing_client-0.2.9/webthing_client/stomp.py
+-rw-r--r--   0        0        0     1897 2024-04-11 10:57:32.328600 webthing_client-0.2.9/webthing_client/utils.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 webthing_client-0.2.9/PKG-INFO
```

### Comparing `webthing_client-0.2.8/LICENSE` & `webthing_client-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/pyproject.toml` & `webthing_client-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webthing-client"
-version = "0.2.8"
+version = "0.2.9"
 description = "Client for the Dynamic Dashboard Webthings"
 authors = ["Emile Deman"]
 maintainers = [
     "Emile Deman <emile.deman@ugent.be>",
 	"Stef Pletinck <s@stefpletinck.be>"
 ]
 readme = "README.md"
```

### Comparing `webthing_client-0.2.8/webthing_client/client.py` & `webthing_client-0.2.9/webthing_client/client.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/input/action/event_input.py` & `webthing_client-0.2.9/webthing_client/input/action/event_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/input/action/event_type_input.py` & `webthing_client-0.2.9/webthing_client/input/action/event_type_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/input/action/from_to_user_input.py` & `webthing_client-0.2.9/webthing_client/input/action/from_to_user_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/input/action/resolution_input.py` & `webthing_client-0.2.9/webthing_client/input/action/resolution_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/input/property_observations_input.py` & `webthing_client-0.2.9/webthing_client/input/property_observations_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/input/replay/replay_input.py` & `webthing_client-0.2.9/webthing_client/input/replay/replay_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/action/action.py` & `webthing_client-0.2.9/webthing_client/model/action/action.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/action/operation/operation.py` & `webthing_client-0.2.9/webthing_client/model/action/operation/operation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/action/request.py` & `webthing_client-0.2.9/webthing_client/model/action/request.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/action/resolution.py` & `webthing_client-0.2.9/webthing_client/model/action/resolution.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/event/event.py` & `webthing_client-0.2.9/webthing_client/model/event/event.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/event/event_type.py` & `webthing_client-0.2.9/webthing_client/model/event/event_type.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/event/feedback.py` & `webthing_client-0.2.9/webthing_client/model/event/feedback.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/event/feedback_schema.py` & `webthing_client-0.2.9/webthing_client/model/event/feedback_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,10 @@
         schema: Dict[str, Any] = {
             '$schema': json_object['$schema'],
             'type': 'object',
             'properties': properties,
             'required': required
         }
         type: str = None
-        if '$class' in json_object:
-            type = json_object['$class']['const']
+        if '$class' in json_object['properties']:
+            type = json_object['properties']['$class']['const']
         return cls(type, schema)
```

### Comparing `webthing_client-0.2.8/webthing_client/model/event/observation.py` & `webthing_client-0.2.9/webthing_client/model/event/observation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/event/stimulus.py` & `webthing_client-0.2.9/webthing_client/model/event/stimulus.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/property/observable_property.py` & `webthing_client-0.2.9/webthing_client/model/property/observable_property.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/replay/replay.py` & `webthing_client-0.2.9/webthing_client/model/replay/replay.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/system/sensor.py` & `webthing_client-0.2.9/webthing_client/model/system/sensor.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/system/system.py` & `webthing_client-0.2.9/webthing_client/model/system/system.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/user/user.py` & `webthing_client-0.2.9/webthing_client/model/user/user.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/model/webthing_observation.py` & `webthing_client-0.2.9/webthing_client/model/webthing_observation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/standard_api/api_handler.py` & `webthing_client-0.2.9/webthing_client/standard_api/api_handler.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/standard_api/api_marshalling.py` & `webthing_client-0.2.9/webthing_client/standard_api/api_marshalling.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/stomp.py` & `webthing_client-0.2.9/webthing_client/stomp.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/webthing_client/utils.py` & `webthing_client-0.2.9/webthing_client/utils.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.8/PKG-INFO` & `webthing_client-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webthing-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: Client for the Dynamic Dashboard Webthings
 Home-page: https://github.com/predict-idlab/webthing-client-python
 Author: Emile Deman
 Maintainer: Emile Deman
 Maintainer-email: emile.deman@ugent.be
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```


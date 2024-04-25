# Comparing `tmp/multion-1.0.1.tar.gz` & `tmp/multion-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-1.0.1.tar", max compression
+gzip compressed data, was "multion-1.1.0.tar", max compression
```

## Comparing `multion-1.0.1.tar` & `multion-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,54 @@
--rw-r--r--   0        0        0     3937 2024-04-10 23:22:32.678930 multion-1.0.1/README.md
--rw-r--r--   0        0        0      592 2024-04-10 23:22:32.678930 multion-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1447 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/__init__.py
--rw-r--r--   0        0        0    16274 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/client.py
--rw-r--r--   0        0        0     1006 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/api_error.py
--rw-r--r--   0        0        0     1490 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/unchecked_base_model.py
--rw-r--r--   0        0        0      162 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/environment.py
--rw-r--r--   0        0        0      385 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/__init__.py
--rw-r--r--   0        0        0      301 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/bad_request_error.py
--rw-r--r--   0        0        0      333 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/internal_server_error.py
--rw-r--r--   0        0        0      308 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/py.typed
--rw-r--r--   0        0        0      427 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/__init__.py
--rw-r--r--   0        0        0    29484 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/client.py
--rw-r--r--   0        0        0      590 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/__init__.py
--rw-r--r--   0        0        0     1081 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/create_session_input_browser_params.py
--rw-r--r--   0        0        0     1105 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/sessions_close_response.py
--rw-r--r--   0        0        0     1010 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/sessions_list_response.py
--rw-r--r--   0        0        0     1024 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/sessions_screenshot_response.py
--rw-r--r--   0        0        0     1079 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/step_session_input_browser_params.py
--rw-r--r--   0        0        0     1062 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/__init__.py
--rw-r--r--   0        0        0     1147 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/bad_request_response.py
--rw-r--r--   0        0        0     1573 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/browse_output.py
--rw-r--r--   0        0        0     1009 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/http_validation_error.py
--rw-r--r--   0        0        0     1156 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/internal_server_error_response.py
--rw-r--r--   0        0        0     1231 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/metadata.py
--rw-r--r--   0        0        0     1152 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/payment_required_response.py
--rw-r--r--   0        0        0      906 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/remote_value.py
--rw-r--r--   0        0        0     1368 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/retrieve_output.py
--rw-r--r--   0        0        0     1417 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/session_created.py
--rw-r--r--   0        0        0     1421 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/session_step_success.py
--rw-r--r--   0        0        0     1149 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/unauthorized_response.py
--rw-r--r--   0        0        0     1028 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       75 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/version.py
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3937 2024-04-25 03:42:56.159605 multion-1.1.0/README.md
+-rw-r--r--   0        0        0      611 2024-04-25 03:42:56.159605 multion-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2193 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/__init__.py
+-rw-r--r--   0        0        0    16296 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/client.py
+-rw-r--r--   0        0        0     1006 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/api_error.py
+-rw-r--r--   0        0        0     1490 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      162 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/environment.py
+-rw-r--r--   0        0        0      385 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/errors/__init__.py
+-rw-r--r--   0        0        0      301 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/errors/bad_request_error.py
+-rw-r--r--   0        0        0      333 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/errors/internal_server_error.py
+-rw-r--r--   0        0        0      308 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/py.typed
+-rw-r--r--   0        0        0      523 2024-04-25 03:42:56.159605 multion-1.1.0/src/multion/sessions/__init__.py
+-rw-r--r--   0        0        0    38084 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/client.py
+-rw-r--r--   0        0        0      741 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/create_session_input_browser_params.py
+-rw-r--r--   0        0        0     1105 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/sessions_close_response.py
+-rw-r--r--   0        0        0     1010 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/sessions_list_response.py
+-rw-r--r--   0        0        0     1024 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/sessions_screenshot_response.py
+-rw-r--r--   0        0        0     1082 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/sessions_step_request_browser_params.py
+-rw-r--r--   0        0        0     1088 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/sessions/types/sessions_step_stream_request_browser_params.py
+-rw-r--r--   0        0        0     2015 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/bad_request_response.py
+-rw-r--r--   0        0        0     1573 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/browse_output.py
+-rw-r--r--   0        0        0     1009 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/http_validation_error.py
+-rw-r--r--   0        0        0     1156 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/internal_server_error_response.py
+-rw-r--r--   0        0        0     1231 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/metadata.py
+-rw-r--r--   0        0        0     1152 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/payment_required_response.py
+-rw-r--r--   0        0        0      906 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/remote_value.py
+-rw-r--r--   0        0        0     1368 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/retrieve_output.py
+-rw-r--r--   0        0        0     1417 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_created.py
+-rw-r--r--   0        0        0     1039 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_step_stream_chunk.py
+-rw-r--r--   0        0        0     1421 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_step_success.py
+-rw-r--r--   0        0        0     1220 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_stream_chunk_event.py
+-rw-r--r--   0        0        0     1165 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_stream_chunk_event_data.py
+-rw-r--r--   0        0        0     1177 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_stream_chunk_event_data_delta.py
+-rw-r--r--   0        0        0     1393 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_stream_chunk_final_event.py
+-rw-r--r--   0        0        0     1198 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_stream_chunk_final_event_data.py
+-rw-r--r--   0        0        0     1282 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/session_stream_chunk_final_event_data_delta.py
+-rw-r--r--   0        0        0     1149 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/unauthorized_response.py
+-rw-r--r--   0        0        0     1028 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       75 2024-04-25 03:42:56.163605 multion-1.1.0/src/multion/version.py
+-rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 multion-1.1.0/PKG-INFO
```

### Comparing `multion-1.0.1/README.md` & `multion-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/pyproject.toml` & `multion-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "multion"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "multion", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.21.2"
+httpx-sse = "0.4.0"
 pydantic = ">= 1.9.2"
 typing_extensions = ">= 4.0.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.8.0"
+mypy = "1.9.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
 python-dateutil = "^2.9.0"
 
 [tool.pytest.ini_options]
 testpaths = [ "tests" ]
 asyncio_mode = "auto"
```

### Comparing `multion-1.0.1/src/multion/client.py` & `multion-1.1.0/src/multion/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: MultiOnEnvironment = MultiOnEnvironment.DEFAULT,
         api_key: typing.Optional[str] = os.getenv("MULTION_API_KEY"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None,
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         if api_key is None:
             raise ApiError(
                 body="The client must be instantiated be either passing in api_key or setting MULTION_API_KEY"
             )
@@ -129,16 +129,16 @@
         if session_id is not OMIT:
             _request["session_id"] = session_id
         if max_steps is not OMIT:
             _request["max_steps"] = max_steps
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -212,15 +212,15 @@
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: MultiOnEnvironment = MultiOnEnvironment.DEFAULT,
         api_key: typing.Optional[str] = os.getenv("MULTION_API_KEY"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         if api_key is None:
             raise ApiError(
                 body="The client must be instantiated be either passing in api_key or setting MULTION_API_KEY"
             )
@@ -283,16 +283,16 @@
         if session_id is not OMIT:
             _request["session_id"] = session_id
         if max_steps is not OMIT:
             _request["max_steps"] = max_steps
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
```

### Comparing `multion-1.0.1/src/multion/core/__init__.py` & `multion-1.1.0/src/multion/core/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/core/client_wrapper.py` & `multion-1.1.0/src/multion/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "multion",
-            "X-Fern-SDK-Version": "1.0.1",
+            "X-Fern-SDK-Version": "1.1.0",
         }
         headers["X_MULTION_API_KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `multion-1.0.1/src/multion/core/datetime_utils.py` & `multion-1.1.0/src/multion/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/core/file.py` & `multion-1.1.0/src/multion/core/file.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/core/http_client.py` & `multion-1.1.0/src/multion/core/http_client.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/core/jsonable_encoder.py` & `multion-1.1.0/src/multion/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/core/request_options.py` & `multion-1.1.0/src/multion/core/request_options.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/core/unchecked_base_model.py` & `multion-1.1.0/src/multion/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/sessions/client.py` & `multion-1.1.0/src/multion/sessions/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import json
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
+import httpx_sse
+
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.session_created import SessionCreated
+from ..types.session_step_stream_chunk import SessionStepStreamChunk
 from ..types.session_step_success import SessionStepSuccess
 from .types.create_session_input_browser_params import CreateSessionInputBrowserParams
 from .types.sessions_close_response import SessionsCloseResponse
 from .types.sessions_list_response import SessionsListResponse
 from .types.sessions_screenshot_response import SessionsScreenshotResponse
-from .types.step_session_input_browser_params import StepSessionInputBrowserParams
+from .types.sessions_step_request_browser_params import SessionsStepRequestBrowserParams
+from .types.sessions_step_stream_request_browser_params import SessionsStepStreamRequestBrowserParams
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class SessionsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
@@ -64,16 +69,16 @@
         if local is not OMIT:
             _request["local"] = local
         if browser_params is not OMIT:
             _request["browser_params"] = browser_params
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -101,38 +106,129 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def step_stream(
+        self,
+        session_id: str,
+        *,
+        cmd: str,
+        url: typing.Optional[str] = OMIT,
+        browser_params: typing.Optional[SessionsStepStreamRequestBrowserParams] = OMIT,
+        include_screenshot: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> typing.Iterator[SessionStepStreamChunk]:
+        """
+        Allows for browsing the web using detailed natural language instructions in a step mode for a session with a given session ID
+
+        Parameters:
+            - session_id: str.
+
+            - cmd: str. A specific natural language instruction for the next step.
+
+            - url: typing.Optional[str]. The URL to create or continue session from.
+
+            - browser_params: typing.Optional[SessionsStepStreamRequestBrowserParams]. Object containing height and width for the browser screen size.
+
+            - include_screenshot: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from multion import SessionsStepStreamRequestBrowserParams
+        from multion.client import MultiOn
+
+        client = MultiOn(
+            api_key="YOUR_API_KEY",
+        )
+        client.sessions.step_stream(
+            session_id="string",
+            cmd="string",
+            url="string",
+            browser_params=SessionsStepStreamRequestBrowserParams(
+                height=1.1,
+                width=1.1,
+            ),
+            include_screenshot=True,
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd, "stream": True}
+        if url is not OMIT:
+            _request["url"] = url
+        if browser_params is not OMIT:
+            _request["browser_params"] = browser_params
+        if include_screenshot is not OMIT:
+            _request["include_screenshot"] = include_screenshot
+        with self._client_wrapper.httpx_client.stream(
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        ) as _response:
+            if 200 <= _response.status_code < 300:
+                _event_source = httpx_sse.EventSource(_response)
+                for _sse in _event_source.iter_sse():
+                    yield typing.cast(SessionStepStreamChunk, construct_type(type_=SessionStepStreamChunk, object_=json.loads(_sse.data)))  # type: ignore
+                return
+            _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
+            try:
+                _response_json = _response.json()
+            except JSONDecodeError:
+                raise ApiError(status_code=_response.status_code, body=_response.text)
+            raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def step(
         self,
         session_id: str,
         *,
         cmd: str,
         url: typing.Optional[str] = OMIT,
-        stream: typing.Optional[bool] = OMIT,
-        browser_params: typing.Optional[StepSessionInputBrowserParams] = OMIT,
+        browser_params: typing.Optional[SessionsStepRequestBrowserParams] = OMIT,
         include_screenshot: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SessionStepSuccess:
         """
         Allows for browsing the web using detailed natural language instructions in a step mode for a session with a given session ID
 
         Parameters:
             - session_id: str.
 
             - cmd: str. A specific natural language instruction for the next step.
 
             - url: typing.Optional[str]. The URL to create or continue session from.
 
-            - stream: typing.Optional[bool]. Boolean flag to stream results back to the client (Default: False)
-
-            - browser_params: typing.Optional[StepSessionInputBrowserParams]. Object containing height and width for the browser screen size.
+            - browser_params: typing.Optional[SessionsStepRequestBrowserParams]. Object containing height and width for the browser screen size.
 
             - include_screenshot: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import MultiOn
 
@@ -140,26 +236,26 @@
             api_key="YOUR_API_KEY",
         )
         client.sessions.step(
             session_id="session_id",
             cmd="cmd",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd, "stream": False}
         if url is not OMIT:
             _request["url"] = url
-        if stream is not OMIT:
-            _request["stream"] = stream
         if browser_params is not OMIT:
             _request["browser_params"] = browser_params
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -208,16 +304,18 @@
             api_key="YOUR_API_KEY",
         )
         client.sessions.close(
             session_id="session_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -260,16 +358,16 @@
             api_key="YOUR_API_KEY",
         )
         client.sessions.screenshot(
             session_id="session_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"screenshot/{jsonable_encoder(session_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -308,16 +406,16 @@
 
         client = MultiOn(
             api_key="YOUR_API_KEY",
         )
         client.sessions.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -380,16 +478,16 @@
         if local is not OMIT:
             _request["local"] = local
         if browser_params is not OMIT:
             _request["browser_params"] = browser_params
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -417,38 +515,129 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def step_stream(
+        self,
+        session_id: str,
+        *,
+        cmd: str,
+        url: typing.Optional[str] = OMIT,
+        browser_params: typing.Optional[SessionsStepStreamRequestBrowserParams] = OMIT,
+        include_screenshot: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> typing.AsyncIterator[SessionStepStreamChunk]:
+        """
+        Allows for browsing the web using detailed natural language instructions in a step mode for a session with a given session ID
+
+        Parameters:
+            - session_id: str.
+
+            - cmd: str. A specific natural language instruction for the next step.
+
+            - url: typing.Optional[str]. The URL to create or continue session from.
+
+            - browser_params: typing.Optional[SessionsStepStreamRequestBrowserParams]. Object containing height and width for the browser screen size.
+
+            - include_screenshot: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from multion import SessionsStepStreamRequestBrowserParams
+        from multion.client import AsyncMultiOn
+
+        client = AsyncMultiOn(
+            api_key="YOUR_API_KEY",
+        )
+        await client.sessions.step_stream(
+            session_id="string",
+            cmd="string",
+            url="string",
+            browser_params=SessionsStepStreamRequestBrowserParams(
+                height=1.1,
+                width=1.1,
+            ),
+            include_screenshot=True,
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd, "stream": True}
+        if url is not OMIT:
+            _request["url"] = url
+        if browser_params is not OMIT:
+            _request["browser_params"] = browser_params
+        if include_screenshot is not OMIT:
+            _request["include_screenshot"] = include_screenshot
+        async with self._client_wrapper.httpx_client.stream(
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        ) as _response:
+            if 200 <= _response.status_code < 300:
+                _event_source = httpx_sse.EventSource(_response)
+                async for _sse in _event_source.aiter_sse():
+                    yield typing.cast(SessionStepStreamChunk, construct_type(type_=SessionStepStreamChunk, object_=json.loads(_sse.data)))  # type: ignore
+                return
+            await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+                )
+            try:
+                _response_json = _response.json()
+            except JSONDecodeError:
+                raise ApiError(status_code=_response.status_code, body=_response.text)
+            raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def step(
         self,
         session_id: str,
         *,
         cmd: str,
         url: typing.Optional[str] = OMIT,
-        stream: typing.Optional[bool] = OMIT,
-        browser_params: typing.Optional[StepSessionInputBrowserParams] = OMIT,
+        browser_params: typing.Optional[SessionsStepRequestBrowserParams] = OMIT,
         include_screenshot: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> SessionStepSuccess:
         """
         Allows for browsing the web using detailed natural language instructions in a step mode for a session with a given session ID
 
         Parameters:
             - session_id: str.
 
             - cmd: str. A specific natural language instruction for the next step.
 
             - url: typing.Optional[str]. The URL to create or continue session from.
 
-            - stream: typing.Optional[bool]. Boolean flag to stream results back to the client (Default: False)
-
-            - browser_params: typing.Optional[StepSessionInputBrowserParams]. Object containing height and width for the browser screen size.
+            - browser_params: typing.Optional[SessionsStepRequestBrowserParams]. Object containing height and width for the browser screen size.
 
             - include_screenshot: typing.Optional[bool].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from multion.client import AsyncMultiOn
 
@@ -456,26 +645,26 @@
             api_key="YOUR_API_KEY",
         )
         await client.sessions.step(
             session_id="session_id",
             cmd="cmd",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
+        _request: typing.Dict[str, typing.Any] = {"cmd": cmd, "stream": False}
         if url is not OMIT:
             _request["url"] = url
-        if stream is not OMIT:
-            _request["stream"] = stream
         if browser_params is not OMIT:
             _request["browser_params"] = browser_params
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -524,16 +713,18 @@
             api_key="YOUR_API_KEY",
         )
         await client.sessions.close(
             session_id="session_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -576,16 +767,16 @@
             api_key="YOUR_API_KEY",
         )
         await client.sessions.screenshot(
             session_id="session_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"screenshot/{jsonable_encoder(session_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -624,16 +815,16 @@
 
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
         )
         await client.sessions.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
```

### Comparing `multion-1.0.1/src/multion/sessions/types/__init__.py` & `multion-1.1.0/src/multion/sessions/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .create_session_input_browser_params import CreateSessionInputBrowserParams
 from .sessions_close_response import SessionsCloseResponse
 from .sessions_list_response import SessionsListResponse
 from .sessions_screenshot_response import SessionsScreenshotResponse
-from .step_session_input_browser_params import StepSessionInputBrowserParams
+from .sessions_step_request_browser_params import SessionsStepRequestBrowserParams
+from .sessions_step_stream_request_browser_params import SessionsStepStreamRequestBrowserParams
 
 __all__ = [
     "CreateSessionInputBrowserParams",
     "SessionsCloseResponse",
     "SessionsListResponse",
     "SessionsScreenshotResponse",
-    "StepSessionInputBrowserParams",
+    "SessionsStepRequestBrowserParams",
+    "SessionsStepStreamRequestBrowserParams",
 ]
```

### Comparing `multion-1.0.1/src/multion/sessions/types/create_session_input_browser_params.py` & `multion-1.1.0/src/multion/sessions/types/create_session_input_browser_params.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/sessions/types/sessions_close_response.py` & `multion-1.1.0/src/multion/sessions/types/sessions_close_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/sessions/types/sessions_list_response.py` & `multion-1.1.0/src/multion/sessions/types/sessions_list_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/sessions/types/sessions_screenshot_response.py` & `multion-1.1.0/src/multion/sessions/types/sessions_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/sessions/types/step_session_input_browser_params.py` & `multion-1.1.0/src/multion/sessions/types/sessions_step_request_browser_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class StepSessionInputBrowserParams(UncheckedBaseModel):
+class SessionsStepRequestBrowserParams(UncheckedBaseModel):
     """
     Object containing height and width for the browser screen size.
     """
 
     height: typing.Optional[float] = None
     width: typing.Optional[float] = None
```

### Comparing `multion-1.0.1/src/multion/types/bad_request_response.py` & `multion-1.1.0/src/multion/types/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/browse_output.py` & `multion-1.1.0/src/multion/types/browse_output.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/http_validation_error.py` & `multion-1.1.0/src/multion/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/internal_server_error_response.py` & `multion-1.1.0/src/multion/types/internal_server_error_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/metadata.py` & `multion-1.1.0/src/multion/types/metadata.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/payment_required_response.py` & `multion-1.1.0/src/multion/types/payment_required_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/remote_value.py` & `multion-1.1.0/src/multion/types/remote_value.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/retrieve_output.py` & `multion-1.1.0/src/multion/types/retrieve_output.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/session_created.py` & `multion-1.1.0/src/multion/types/session_created.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/session_step_success.py` & `multion-1.1.0/src/multion/types/session_step_success.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/unauthorized_response.py` & `multion-1.1.0/src/multion/types/unauthorized_response.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/src/multion/types/validation_error.py` & `multion-1.1.0/src/multion/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.1/PKG-INFO` & `multion-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: multion
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
+Requires-Dist: httpx-sse (==0.4.0)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # MultiOn Python Library
 
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
```


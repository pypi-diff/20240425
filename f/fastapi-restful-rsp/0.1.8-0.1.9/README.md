# Comparing `tmp/fastapi_restful_rsp-0.1.8.tar.gz` & `tmp/fastapi_restful_rsp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_restful_rsp-0.1.8.tar", max compression
+gzip compressed data, was "fastapi_restful_rsp-0.1.9.tar", max compression
```

## Comparing `fastapi_restful_rsp-0.1.8.tar` & `fastapi_restful_rsp-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      600 2024-03-18 09:36:06.843585 fastapi_restful_rsp-0.1.8/README.md
--rw-r--r--   0        0        0      131 2024-03-18 09:36:06.843585 fastapi_restful_rsp-0.1.8/fastapi_restful_rsp/__init__.py
--rw-r--r--   0        0        0     5116 2024-03-18 09:36:06.843585 fastapi_restful_rsp-0.1.8/fastapi_restful_rsp/custom_decorator.py
--rw-r--r--   0        0        0      314 2024-03-18 09:36:06.843585 fastapi_restful_rsp-0.1.8/fastapi_restful_rsp/models.py
--rw-r--r--   0        0        0      216 2024-03-18 09:36:06.843585 fastapi_restful_rsp-0.1.8/fastapi_restful_rsp/restful_rsp.py
--rw-r--r--   0        0        0      584 2024-03-18 09:36:12.043577 fastapi_restful_rsp-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 fastapi_restful_rsp-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1009 2024-04-08 05:12:53.659990 fastapi_restful_rsp-0.1.9/README.md
+-rw-r--r--   0        0        0      210 2024-04-08 05:12:53.659990 fastapi_restful_rsp-0.1.9/fastapi_restful_rsp/__init__.py
+-rw-r--r--   0        0        0     4590 2024-04-08 05:12:53.659990 fastapi_restful_rsp-0.1.9/fastapi_restful_rsp/custom_decorator.py
+-rw-r--r--   0        0        0      300 2024-04-08 05:12:53.659990 fastapi_restful_rsp-0.1.9/fastapi_restful_rsp/models.py
+-rw-r--r--   0        0        0      216 2024-04-08 05:12:53.659990 fastapi_restful_rsp-0.1.9/fastapi_restful_rsp/restful_rsp.py
+-rw-r--r--   0        0        0      658 2024-04-08 05:13:04.304062 fastapi_restful_rsp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 fastapi_restful_rsp-0.1.9/PKG-INFO
```

### Comparing `fastapi_restful_rsp-0.1.8/fastapi_restful_rsp/custom_decorator.py` & `fastapi_restful_rsp-0.1.9/fastapi_restful_rsp/custom_decorator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import wraps
 import inspect
-from typing import Any, Callable, Generic, Optional, TypeVar, get_type_hints
+from typing import Any, Callable, Optional, get_type_hints
 
-from fastapi import HTTPException
+from fastapi import HTTPException, Response
 
 from fastapi.responses import JSONResponse
-from pydantic import BaseModel, create_model
+from pydantic import create_model
 
 from fastapi_restful_rsp.models import BaseRestFulRsp, DataT, RspGereric
 
 from logging import getLogger
 
 
 logger = getLogger("fastapi.restful_rsp")
@@ -50,71 +50,76 @@
     fields = {data_name: (DataT, None), message_name: (str, "")}
     if code_name:
         fields[code_name] = (get_type_hints(code_callback)["return"], 0)
     fields.update(param_dict)
 
     RestFulRsp = create_model("RestFulRsp", __base__=(RspGereric,), **fields)
 
-    def restful_response(func: Callable[..., DataT]) -> Callable[..., BaseRestFulRsp[DataT]]:
+    def handle_response(result, e=None):
+        if isinstance(result, Response):
+            return result
+        if e:
+            logger.exception(e)
+            ret = {
+                code_name: code_callback(e),
+                message_name: str(e.detail if isinstance(e, HTTPException) else e),
+            }
+            ret_data = RestFulRsp[DataT](**ret)
+            status_code = e.status_code if isinstance(e, HTTPException) else 500
+            return JSONResponse(content=ret_data.model_dump(), status_code=status_code)
+        else:
+            ret = {data_name: result, code_name: code_callback()}
+            return RestFulRsp[DataT](**ret)
+
+    def restful_response(
+        func: Callable[..., DataT],
+    ) -> Callable[..., BaseRestFulRsp[DataT]]:
         """
         Decorator function that wraps another function and converts its return value into a RestFulRsp object.
 
         Args:
             func (Callable[..., DataT]): The function to be decorated.
 
         Returns:
             Callable[..., BaseRestFulRsp[DataT]]: The decorated function that returns a RestFulRsp object.
 
         Raises:
             Exception: If an error occurs during the execution of the decorated function.
 
         """
-        # check func is a coroutine function
-        if inspect.iscoroutinefunction(func):
 
-            @wraps(func)
-            async def wrapper(*args, **kwargs):
-                try:
-                    result = await func(*args, **kwargs)
-                    ret = {data_name: result, code_name: code_callback()}
-                    return RestFulRsp[DataT](**ret)
-                except HTTPException as e:
-                    logger.exception(e)
-                    ret = {code_name: code_callback(e), message_name: str(e.detail)}
-                    ret_data = RestFulRsp[DataT](**ret)
-                    return JSONResponse(content=ret_data.model_dump(), status_code=e.status_code)
-                except Exception as e:
-                    logger.exception(e)
-                    ret = {code_name: code_callback(e), message_name: str(e)}
-                    ret_data = RestFulRsp[DataT](**ret)
-                    return JSONResponse(content=ret_data.model_dump(), status_code=500)
+        @wraps(func)
+        async def async_wrapper(*args, **kwargs):
+            try:
+                result = await func(*args, **kwargs)
+                return handle_response(result)
+            except Exception as e:
+                return handle_response(None, e)
+
+        @wraps(func)
+        def sync_wrapper(*args, **kwargs):
+            try:
+                result = func(*args, **kwargs)
+                return handle_response(result)
+            except Exception as e:
+                return handle_response(None, e)
 
+        if inspect.iscoroutinefunction(func):
+            wrapper = async_wrapper
         else:
-
-            @wraps(func)
-            def wrapper(*args, **kwargs):
-                try:
-                    result = func(*args, **kwargs)
-                    ret = {data_name: result, code_name: code_callback()}
-                    return RestFulRsp[DataT](**ret)
-                except HTTPException as e:
-                    logger.exception(e)
-                    ret = {code_name: code_callback(e), message_name: str(e.detail)}
-                    ret_data = RestFulRsp[DataT](**ret)
-                    return JSONResponse(content=ret_data.model_dump(), status_code=e.status_code)
-                except Exception as e:
-                    logger.exception(e)
-                    ret = {code_name: code_callback(e), message_name: str(e)}
-                    ret_data = RestFulRsp[DataT](**ret)
-                    return JSONResponse(content=ret_data.model_dump(), status_code=500)
+            wrapper = sync_wrapper
 
         # change the return type of the function to  -> RestFulRsp[DataT]
-        wrapper.__annotations__["return"] = RestFulRsp[wrapper.__annotations__.get("return", Any)]
+        wrapper.__annotations__["return"] = RestFulRsp[
+            wrapper.__annotations__.get("return", Any)
+        ]
         if hasattr(func, "__signature__"):
             # change return type of the function signature
             # see https://docs.python.org/3/library/inspect.html#inspect.signature
             # if has a __signature__ attribute, this function returns it without further computations
-            wrapper.__signature__ = func.__signature__.replace(return_annotation=wrapper.__annotations__["return"])
+            wrapper.__signature__ = func.__signature__.replace(
+                return_annotation=wrapper.__annotations__["return"]
+            )
 
         return wrapper
 
     return restful_response
```

### Comparing `fastapi_restful_rsp-0.1.8/pyproject.toml` & `fastapi_restful_rsp-0.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "fastapi-restful-rsp"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["paleneutron <paleneutron@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.110.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 pytest = "^8.0.2"
+pytest-asyncio = "^0.23.6"
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -26,7 +28,10 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.flake8]
 exclude = ".venv"
+
+[tool.pytest.ini_options]
+asyncio_mode="auto"
```

### Comparing `fastapi_restful_rsp-0.1.8/PKG-INFO` & `fastapi_restful_rsp-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: fastapi-restful-rsp
-Version: 0.1.8
-Summary: 
-Author: paleneutron
-Author-email: paleneutron@outlook.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fastapi (>=0.110.0,<0.111.0)
-Description-Content-Type: text/markdown
-
 # Wrap fastapi endpoints with RESTful API
 
 Modern frontend frameworks encourage backend developers to follow RESTful API design. This package wraps fastapi endpoints with following structure:
 
 ```json
 {
   "data": {
@@ -44,7 +30,21 @@
 
 @app.get("/foo/")
 @restful_response
 def foo()-> str:
     return "Hello World"
 ```
 
+### Custom response structure
+
+You can customize the response structure by passing `data_name`, `code_key`, `message_name` to `restful_response` decorator.
+
+```python
+restful_response = create_restful_rsp_decorator(
+    data_name="data", code_name="my_code", message_name="message", param_dict={"status": (str, "success")}
+)
+
+@app.get("/foo/")
+@restful_response
+def foo()-> str:
+    return "Hello World"
+```
```


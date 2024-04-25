# Comparing `tmp/fastapi_exceptionshandler-0.0.3.tar.gz` & `tmp/fastapi_exceptionshandler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_exceptionshandler-0.0.3.tar", last modified: Wed Oct  4 15:41:36 2023, max compression
+gzip compressed data, was "fastapi_exceptionshandler-0.1.0.tar", last modified: Thu Apr 25 19:26:24 2024, max compression
```

## Comparing `fastapi_exceptionshandler-0.0.3.tar` & `fastapi_exceptionshandler-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:41:36.675421 fastapi_exceptionshandler-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2023-10-04 15:41:36.675421 fastapi_exceptionshandler-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:41:36.675421 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:41:36.675421 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2023-10-04 15:41:36.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-10-04 15:41:36.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 15:41:36.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-04 15:41:36.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-04 15:41:36.000000 fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-10-04 15:41:26.000000 fastapi_exceptionshandler-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 15:41:36.675421 fastapi_exceptionshandler-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:26:24.944993 fastapi_exceptionshandler-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-25 19:26:24.944993 fastapi_exceptionshandler-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:26:24.940993 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:26:24.944993 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-25 19:26:24.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-25 19:26:24.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:26:24.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 19:26:24.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 19:26:24.000000 fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 19:26:20.000000 fastapi_exceptionshandler-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:26:24.944993 fastapi_exceptionshandler-0.1.0/setup.cfg
```

### Comparing `fastapi_exceptionshandler-0.0.3/PKG-INFO` & `fastapi_exceptionshandler-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_exceptionshandler
-Version: 0.0.3
+Version: 0.1.0
 Summary: Standardize and handle exceptions in FastAPI more elegantly
 Author-email: SirPaulO <me@sirpauloliver.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/SirPaulO/fastapi_exceptionshandler
 Project-URL: Bug Tracker, https://github.com/SirPaulO/fastapi_exceptionshandler/issues
 Project-URL: Repository, https://github.com/SirPaulO/fastapi_exceptionshandler.git
 Keywords: fastapi,middleware,exception,error,handler,response,api
@@ -24,63 +24,39 @@
 ```console
 $ pip install fastapi-exceptionshandler
 ```
 
 
 ## Example
 
-You can automatically handle **all** exceptions using [fastapi-routesmanager](https://github.com/SirPaulO/fastapi_routesmanager).
-Simply register the `APIExceptionManager` to the `RouteManagersRegistry`. _Don't forget to use the `ManagedAPIRouter`_
-
-**Note:** by default Validation errors are not captured. To do so, use `APIExceptionManager(capture_validation=True)` instead.
-
 ```python
 from fastapi import FastAPI
 
-from fastapi_routesmanager import RouteManagersRegistry, ManagedAPIRouter
-
-from fastapi_exceptionshandler import APIExceptionManager
-
-RouteManagersRegistry.register_route_manager(APIExceptionManager)  # Register manager
+from fastapi_exceptionshandler import APIExceptionMiddleware
 
 app = FastAPI()
 
-router = ManagedAPIRouter()
-
-@router.get("/")  # Use router instead of app
-def read_root():
-    return 1/0
-
-
-app.include_router(router)  # Include the router to the app
-
-```
-
-<details>
-<summary>Or you can handle exceptions manually...</summary>
-
-```python
-from fastapi import FastAPI
+# Register the middleware
+app.add_middleware(APIExceptionMiddleware, capture_unhandled=True)  # Capture all exceptions
 
+# You can also capture Validation errors, that are not captured by default
 from fastapi_exceptionshandler import APIExceptionHandler
 
-app = FastAPI()
+from pydantic import ValidationError
+app.add_exception_handler(ValidationError, APIExceptionHandler.unhandled)
+
+from fastapi.exceptions import RequestValidationError
+app.add_exception_handler(RequestValidationError, APIExceptionHandler.unhandled)
 
 @app.get("/")
 def read_root():
-    try:
-        return 1/0
-    except Exception as exc:
-        return await APIExceptionHandler.unhandled(exc)
+    return 1/0
 
 ```
-</details>
-
 
-Create a custom exception class and error code, then 
 
 ### Run it
 
 ```console
 $ uvicorn main:app --reload
 ```
 
@@ -90,48 +66,44 @@
 
 ```console
 {"errorCode": "InternalError", "message": "Internal Server Error"}
 ```
 
 ## Creating custom exceptions
 
-In order to create a custom exception you need to extend `APIException` and create an `Enum` class.
+In order to create a custom exception you need to extend `APIException` and `ErrorCodeBase` classes.
 
-**Note:** if you want to capture *only* `APIException` then use `APIExceptionManager(capture_unhandled=False)`
+**Note:** if you want to capture *only* `APIException` then don't send the `capture_unhandled` param, or set it to `False`
 
 ```python
-from enum import Enum
-
 from fastapi import FastAPI
 
-from fastapi_routesmanager import RouteManagersRegistry, ManagedAPIRouter
+from fastapi_exceptionshandler import APIExceptionMiddleware, APIException, ErrorCodeBase
 
-from fastapi_exceptionshandler import APIExceptionManager, APIException
+from starlette import status
 
-RouteManagersRegistry.register_route_manager(APIExceptionManager)  # Register manager
 
 app = FastAPI()
 
-router = ManagedAPIRouter()
+# Register the middleware
+app.add_middleware(APIExceptionMiddleware)
 
 
 class CustomException(APIException):
-    status_code = 401
+    status_code = status.HTTP_400_BAD_REQUEST
     
-    class ErrorCode(Enum):
-        CustomExceptionCode = "Custom Exception Message"
-
-
-@router.get("/")  # Use router instead of app
+    class ErrorCode(ErrorCodeBase):
+        CustomExceptionCode = "Custom Exception Message", status.HTTP_401_UNAUTHORIZED
+        CustomExceptionCodeWithDefaultStatusCode = "Custom Exception Message"
+        
+        
+@app.get("/")
 def read_root():
     raise CustomException(CustomException.ErrorCode.CustomExceptionCode)
 
-
-app.include_router(router)  # Include the router to the app
-
 ```
 
 Then you should get a `401` response with this body
 
 ```console
 {"errorCode": "CustomExceptionCode", "message": "Custom Exception Message"}
 ```
```

### Comparing `fastapi_exceptionshandler-0.0.3/README.md` & `fastapi_exceptionshandler-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,63 +7,39 @@
 ```console
 $ pip install fastapi-exceptionshandler
 ```
 
 
 ## Example
 
-You can automatically handle **all** exceptions using [fastapi-routesmanager](https://github.com/SirPaulO/fastapi_routesmanager).
-Simply register the `APIExceptionManager` to the `RouteManagersRegistry`. _Don't forget to use the `ManagedAPIRouter`_
-
-**Note:** by default Validation errors are not captured. To do so, use `APIExceptionManager(capture_validation=True)` instead.
-
 ```python
 from fastapi import FastAPI
 
-from fastapi_routesmanager import RouteManagersRegistry, ManagedAPIRouter
-
-from fastapi_exceptionshandler import APIExceptionManager
-
-RouteManagersRegistry.register_route_manager(APIExceptionManager)  # Register manager
+from fastapi_exceptionshandler import APIExceptionMiddleware
 
 app = FastAPI()
 
-router = ManagedAPIRouter()
-
-@router.get("/")  # Use router instead of app
-def read_root():
-    return 1/0
-
-
-app.include_router(router)  # Include the router to the app
-
-```
-
-<details>
-<summary>Or you can handle exceptions manually...</summary>
-
-```python
-from fastapi import FastAPI
+# Register the middleware
+app.add_middleware(APIExceptionMiddleware, capture_unhandled=True)  # Capture all exceptions
 
+# You can also capture Validation errors, that are not captured by default
 from fastapi_exceptionshandler import APIExceptionHandler
 
-app = FastAPI()
+from pydantic import ValidationError
+app.add_exception_handler(ValidationError, APIExceptionHandler.unhandled)
+
+from fastapi.exceptions import RequestValidationError
+app.add_exception_handler(RequestValidationError, APIExceptionHandler.unhandled)
 
 @app.get("/")
 def read_root():
-    try:
-        return 1/0
-    except Exception as exc:
-        return await APIExceptionHandler.unhandled(exc)
+    return 1/0
 
 ```
-</details>
-
 
-Create a custom exception class and error code, then 
 
 ### Run it
 
 ```console
 $ uvicorn main:app --reload
 ```
 
@@ -73,48 +49,44 @@
 
 ```console
 {"errorCode": "InternalError", "message": "Internal Server Error"}
 ```
 
 ## Creating custom exceptions
 
-In order to create a custom exception you need to extend `APIException` and create an `Enum` class.
+In order to create a custom exception you need to extend `APIException` and `ErrorCodeBase` classes.
 
-**Note:** if you want to capture *only* `APIException` then use `APIExceptionManager(capture_unhandled=False)`
+**Note:** if you want to capture *only* `APIException` then don't send the `capture_unhandled` param, or set it to `False`
 
 ```python
-from enum import Enum
-
 from fastapi import FastAPI
 
-from fastapi_routesmanager import RouteManagersRegistry, ManagedAPIRouter
+from fastapi_exceptionshandler import APIExceptionMiddleware, APIException, ErrorCodeBase
 
-from fastapi_exceptionshandler import APIExceptionManager, APIException
+from starlette import status
 
-RouteManagersRegistry.register_route_manager(APIExceptionManager)  # Register manager
 
 app = FastAPI()
 
-router = ManagedAPIRouter()
+# Register the middleware
+app.add_middleware(APIExceptionMiddleware)
 
 
 class CustomException(APIException):
-    status_code = 401
+    status_code = status.HTTP_400_BAD_REQUEST
     
-    class ErrorCode(Enum):
-        CustomExceptionCode = "Custom Exception Message"
-
-
-@router.get("/")  # Use router instead of app
+    class ErrorCode(ErrorCodeBase):
+        CustomExceptionCode = "Custom Exception Message", status.HTTP_401_UNAUTHORIZED
+        CustomExceptionCodeWithDefaultStatusCode = "Custom Exception Message"
+        
+        
+@app.get("/")
 def read_root():
     raise CustomException(CustomException.ErrorCode.CustomExceptionCode)
 
-
-app.include_router(router)  # Include the router to the app
-
 ```
 
 Then you should get a `401` response with this body
 
 ```console
 {"errorCode": "CustomExceptionCode", "message": "Custom Exception Message"}
 ```
```

### Comparing `fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception_handler.py` & `fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception_handler.py`

 * *Files identical despite different names*

### Comparing `fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception_manager.py` & `fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler/api_exception_middleware.py` & `fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler/api_exception_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_exceptionshandler-0.0.3/fastapi_exceptionshandler.egg-info/PKG-INFO` & `fastapi_exceptionshandler-0.1.0/fastapi_exceptionshandler.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastapi-exceptionshandler
-Version: 0.0.3
+Name: fastapi_exceptionshandler
+Version: 0.1.0
 Summary: Standardize and handle exceptions in FastAPI more elegantly
 Author-email: SirPaulO <me@sirpauloliver.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/SirPaulO/fastapi_exceptionshandler
 Project-URL: Bug Tracker, https://github.com/SirPaulO/fastapi_exceptionshandler/issues
 Project-URL: Repository, https://github.com/SirPaulO/fastapi_exceptionshandler.git
 Keywords: fastapi,middleware,exception,error,handler,response,api
@@ -24,63 +24,39 @@
 ```console
 $ pip install fastapi-exceptionshandler
 ```
 
 
 ## Example
 
-You can automatically handle **all** exceptions using [fastapi-routesmanager](https://github.com/SirPaulO/fastapi_routesmanager).
-Simply register the `APIExceptionManager` to the `RouteManagersRegistry`. _Don't forget to use the `ManagedAPIRouter`_
-
-**Note:** by default Validation errors are not captured. To do so, use `APIExceptionManager(capture_validation=True)` instead.
-
 ```python
 from fastapi import FastAPI
 
-from fastapi_routesmanager import RouteManagersRegistry, ManagedAPIRouter
-
-from fastapi_exceptionshandler import APIExceptionManager
-
-RouteManagersRegistry.register_route_manager(APIExceptionManager)  # Register manager
+from fastapi_exceptionshandler import APIExceptionMiddleware
 
 app = FastAPI()
 
-router = ManagedAPIRouter()
-
-@router.get("/")  # Use router instead of app
-def read_root():
-    return 1/0
-
-
-app.include_router(router)  # Include the router to the app
-
-```
-
-<details>
-<summary>Or you can handle exceptions manually...</summary>
-
-```python
-from fastapi import FastAPI
+# Register the middleware
+app.add_middleware(APIExceptionMiddleware, capture_unhandled=True)  # Capture all exceptions
 
+# You can also capture Validation errors, that are not captured by default
 from fastapi_exceptionshandler import APIExceptionHandler
 
-app = FastAPI()
+from pydantic import ValidationError
+app.add_exception_handler(ValidationError, APIExceptionHandler.unhandled)
+
+from fastapi.exceptions import RequestValidationError
+app.add_exception_handler(RequestValidationError, APIExceptionHandler.unhandled)
 
 @app.get("/")
 def read_root():
-    try:
-        return 1/0
-    except Exception as exc:
-        return await APIExceptionHandler.unhandled(exc)
+    return 1/0
 
 ```
-</details>
-
 
-Create a custom exception class and error code, then 
 
 ### Run it
 
 ```console
 $ uvicorn main:app --reload
 ```
 
@@ -90,48 +66,44 @@
 
 ```console
 {"errorCode": "InternalError", "message": "Internal Server Error"}
 ```
 
 ## Creating custom exceptions
 
-In order to create a custom exception you need to extend `APIException` and create an `Enum` class.
+In order to create a custom exception you need to extend `APIException` and `ErrorCodeBase` classes.
 
-**Note:** if you want to capture *only* `APIException` then use `APIExceptionManager(capture_unhandled=False)`
+**Note:** if you want to capture *only* `APIException` then don't send the `capture_unhandled` param, or set it to `False`
 
 ```python
-from enum import Enum
-
 from fastapi import FastAPI
 
-from fastapi_routesmanager import RouteManagersRegistry, ManagedAPIRouter
+from fastapi_exceptionshandler import APIExceptionMiddleware, APIException, ErrorCodeBase
 
-from fastapi_exceptionshandler import APIExceptionManager, APIException
+from starlette import status
 
-RouteManagersRegistry.register_route_manager(APIExceptionManager)  # Register manager
 
 app = FastAPI()
 
-router = ManagedAPIRouter()
+# Register the middleware
+app.add_middleware(APIExceptionMiddleware)
 
 
 class CustomException(APIException):
-    status_code = 401
+    status_code = status.HTTP_400_BAD_REQUEST
     
-    class ErrorCode(Enum):
-        CustomExceptionCode = "Custom Exception Message"
-
-
-@router.get("/")  # Use router instead of app
+    class ErrorCode(ErrorCodeBase):
+        CustomExceptionCode = "Custom Exception Message", status.HTTP_401_UNAUTHORIZED
+        CustomExceptionCodeWithDefaultStatusCode = "Custom Exception Message"
+        
+        
+@app.get("/")
 def read_root():
     raise CustomException(CustomException.ErrorCode.CustomExceptionCode)
 
-
-app.include_router(router)  # Include the router to the app
-
 ```
 
 Then you should get a `401` response with this body
 
 ```console
 {"errorCode": "CustomExceptionCode", "message": "Custom Exception Message"}
 ```
```

### Comparing `fastapi_exceptionshandler-0.0.3/pyproject.toml` & `fastapi_exceptionshandler-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'fastapi_exceptionshandler'
-version = "0.0.3"
+version = "0.1.0"
 license = {text = "MIT License"}
 authors = [
   { name="SirPaulO", email="me@sirpauloliver.com" },
 ]
 dependencies = [
     "fastapi>=0.95.2",
 ]
```


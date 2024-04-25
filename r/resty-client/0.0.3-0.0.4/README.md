# Comparing `tmp/resty_client-0.0.3.tar.gz` & `tmp/resty_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resty_client-0.0.3.tar", max compression
+gzip compressed data, was "resty_client-0.0.4.tar", max compression
```

## Comparing `resty_client-0.0.3.tar` & `resty_client-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.3/LICENSE
--rw-r--r--   0        0        0     1093 2024-04-23 18:45:23.095044 resty_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3108 2024-04-22 14:25:21.707143 resty_client-0.0.3/README.md
--rw-r--r--   0        0        0      126 2024-01-26 15:20:15.262707 resty_client-0.0.3/resty/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.249782 resty_client-0.0.3/resty/clients/__init__.py
--rw-r--r--   0        0        0      179 2024-04-22 14:23:32.487305 resty_client-0.0.3/resty/clients/httpx/__init__.py
--rw-r--r--   0        0        0     3351 2024-04-23 18:07:25.657688 resty_client-0.0.3/resty/clients/httpx/client.py
--rw-r--r--   0        0        0      557 2024-04-22 15:02:44.798358 resty_client-0.0.3/resty/constants.py
--rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.3/resty/enums.py
--rw-r--r--   0        0        0      729 2024-04-23 10:31:25.956591 resty_client-0.0.3/resty/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.3/resty/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.3/resty/ext/django/__init__.py
--rw-r--r--   0        0        0      200 2024-04-22 14:23:32.601297 resty_client-0.0.3/resty/ext/django/middlewares/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-23 16:28:55.203681 resty_client-0.0.3/resty/ext/django/middlewares/pagination.py
--rw-r--r--   0        0        0       69 2024-04-23 09:51:08.271071 resty_client-0.0.3/resty/managers/__init__.py
--rw-r--r--   0        0        0     4975 2024-04-23 18:07:25.719709 resty_client-0.0.3/resty/managers/manager.py
--rw-r--r--   0        0        0      328 2024-04-23 09:51:08.258984 resty_client-0.0.3/resty/middlewares/__init__.py
--rw-r--r--   0        0        0     1296 2024-04-23 16:28:55.207680 resty_client-0.0.3/resty/middlewares/manager.py
--rw-r--r--   0        0        0      264 2024-04-23 09:47:25.043213 resty_client-0.0.3/resty/middlewares/types.py
--rw-r--r--   0        0        0       81 2024-04-23 09:51:08.264970 resty_client-0.0.3/resty/serializers/__init__.py
--rw-r--r--   0        0        0     1390 2024-04-23 18:21:24.086198 resty_client-0.0.3/resty/serializers/serializer.py
--rw-r--r--   0        0        0     2861 2024-04-23 16:28:55.216676 resty_client-0.0.3/resty/types.py
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 resty_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1093 2024-04-25 08:58:55.181458 resty_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3194 2024-04-25 08:58:55.200458 resty_client-0.0.4/README.md
+-rw-r--r--   0        0        0      126 2024-01-26 15:20:15.262707 resty_client-0.0.4/resty/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 15:14:08.249782 resty_client-0.0.4/resty/clients/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-22 14:23:32.487305 resty_client-0.0.4/resty/clients/httpx/__init__.py
+-rw-r--r--   0        0        0     3351 2024-04-23 18:07:25.657688 resty_client-0.0.4/resty/clients/httpx/client.py
+-rw-r--r--   0        0        0      557 2024-04-22 15:02:44.798358 resty_client-0.0.4/resty/constants.py
+-rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.4/resty/enums.py
+-rw-r--r--   0        0        0      729 2024-04-23 10:31:25.956591 resty_client-0.0.4/resty/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.4/resty/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.4/resty/ext/django/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-22 14:23:32.601297 resty_client-0.0.4/resty/ext/django/middlewares/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-23 16:28:55.203681 resty_client-0.0.4/resty/ext/django/middlewares/pagination.py
+-rw-r--r--   0        0        0       69 2024-04-23 09:51:08.271071 resty_client-0.0.4/resty/managers/__init__.py
+-rw-r--r--   0        0        0     4988 2024-04-25 08:58:55.194460 resty_client-0.0.4/resty/managers/manager.py
+-rw-r--r--   0        0        0      328 2024-04-23 09:51:08.258984 resty_client-0.0.4/resty/middlewares/__init__.py
+-rw-r--r--   0        0        0     1296 2024-04-23 16:28:55.207680 resty_client-0.0.4/resty/middlewares/manager.py
+-rw-r--r--   0        0        0      264 2024-04-23 09:47:25.043213 resty_client-0.0.4/resty/middlewares/types.py
+-rw-r--r--   0        0        0       81 2024-04-23 09:51:08.264970 resty_client-0.0.4/resty/serializers/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-23 18:21:24.086198 resty_client-0.0.4/resty/serializers/serializer.py
+-rw-r--r--   0        0        0     2861 2024-04-23 16:28:55.216676 resty_client-0.0.4/resty/types.py
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 resty_client-0.0.4/PKG-INFO
```

### Comparing `resty_client-0.0.3/LICENSE` & `resty_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/pyproject.toml` & `resty_client-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resty-client"
-version = "0.0.3"
+version = "0.0.4"
 description = "RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "resty" },
 ]
```

### Comparing `resty_client-0.0.3/README.md` & `resty_client-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-# RestyClient
+# Resty-Client
 
 <p align="center">
-<img src="https://github.com/CrazyProger1/RestyClient/blob/master/docs/resty-cat.png" alt="resty lib logo">
+<img src="https://github.com/CrazyProger1/Resty-Client/blob/master/docs/resty-cat.png" alt="resty lib logo">
 </p>
 
 <p align="center">
-<a href="https://github.com/CrazyProger1/RestyClient/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/CrazyProger1/RestyClient"></a>
-<a href="https://github.com/CrazyProger1/RestyClient/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/RestyClient"></a>
+<a href="https://github.com/CrazyProger1/Resty-Client/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/CrazyProger1/Resty-Client"></a>
+<a href="https://github.com/CrazyProger1/Resty-Client/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/Resty-Client"></a>
 <a href="https://pypi.org/project/resty-client/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/resty-client"></a>
 <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style"></a>
 </p>
 
-RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data
+
+Resty-Client is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data
 validation and deserialization tools. This library provides an intuitive API that makes it easy to make HTTP requests
 and handle data on the client side.
 
 ## Features
 
 - Middleware system, which allows you to implement any pagination, filtering or authentication.
+- Powerful data validation & deserialization using Pydantic
+- Easy-to-Use
 
 ## Installation
 
 Using pip:
 
 ```shell
 pip install resty-client
@@ -115,12 +118,12 @@
 
     # Delete
     await ProductManager.delete(rest_client, my_product.id)
 ```
 
 ## Status
 
-``0.0.2`` - **RELEASED**
+``0.0.4`` - **RELEASED**
 
 ## Licence
 
-RestyClient is released under the MIT License. See the bundled [LICENSE](LICENSE) file for details.
+Resty-Client is released under the MIT License. See the bundled [LICENSE](LICENSE) file for details.
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-# RestyClient
+# Resty-Client
                                [resty lib logo]
     _[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_ _S_t_y_l_e_]
-RestyClient is a simple, easy-to-use Python library for interacting with REST
+Resty-Client is a simple, easy-to-use Python library for interacting with REST
 APIs using Pydantic's powerful data validation and deserialization tools. This
 library provides an intuitive API that makes it easy to make HTTP requests and
 handle data on the client side. ## Features - Middleware system, which allows
-you to implement any pagination, filtering or authentication. ## Installation
-Using pip: ```shell pip install resty-client ``` Using Poetry: ```shell poetry
-add resty-client ``` ## Getting-Started ### Schema ```python from pydantic
-import BaseModel class Product(BaseModel): id: int | None = None name: str
+you to implement any pagination, filtering or authentication. - Powerful data
+validation & deserialization using Pydantic - Easy-to-Use ## Installation Using
+pip: ```shell pip install resty-client ``` Using Poetry: ```shell poetry add
+resty-client ``` ## Getting-Started ### Schema ```python from pydantic import
+BaseModel class Product(BaseModel): id: int | None = None name: str
 description: str code: str ``` ### Serializer ```python from resty.serializers
 import Serializer class ProductSerializer(Serializer): schema = Product ``` ###
 Manager ```python from resty.enums import ( Endpoint, Field ) from
 resty.managers import Manager class ProductManager(Manager): serializer =
 ProductSerializer endpoints = { Endpoint.CREATE: '/products/', Endpoint.READ:
 '/products/', Endpoint.READ_ONE: '/products/{pk}/', Endpoint.UPDATE: '/
 products/{pk}/', Endpoint.DELETE: '/products/{pk}/', } fields =
@@ -21,10 +22,10 @@
 AsyncClient(base_url='http://localhost:8000/') rest_client = RESTClient
 (xclient=xclient) product = Product( name='First prod', description='My Desc',
 code='123W31Q' ) # Create created = await ProductManager.create(rest_client,
 product) # Read my_product = await ProductManager.read_one(rest_client,
 created.id) for prod in await ProductManager.read(rest_client): print
 (prod.name) # Update my_product.description = 'QWERTY' await
 ProductManager.update(rest_client, my_product) # Delete await
-ProductManager.delete(rest_client, my_product.id) ``` ## Status ``0.0.2`` -
-**RELEASED** ## Licence RestyClient is released under the MIT License. See the
+ProductManager.delete(rest_client, my_product.id) ``` ## Status ``0.0.4`` -
+**RELEASED** ## Licence Resty-Client is released under the MIT License. See the
 bundled [LICENSE](LICENSE) file for details.
```

### Comparing `resty_client-0.0.3/resty/clients/httpx/client.py` & `resty_client-0.0.4/resty/clients/httpx/client.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/resty/constants.py` & `resty_client-0.0.4/resty/constants.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/resty/exceptions.py` & `resty_client-0.0.4/resty/exceptions.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/resty/ext/django/middlewares/pagination.py` & `resty_client-0.0.4/resty/ext/django/middlewares/pagination.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/resty/managers/manager.py` & `resty_client-0.0.4/resty/managers/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         serializer = cls._get_serializer(**options)
         if many:
             return serializer.deserialize_many(data=data, **options)
         return serializer.deserialize(data=data, **options)
 
     @classmethod
     async def create(
-        cls, client: BaseRESTClient, obj: BaseModel, **kwargs
+            cls, client: BaseRESTClient, obj: BaseModel, **kwargs
     ) -> BaseModel:
 
         set_pk = kwargs.pop("set_pk", True)
 
         options = cls._prepare_options(
             endpoint=Endpoint.CREATE, method=Method.POST, **kwargs
         )
@@ -130,21 +130,21 @@
         response = await cls._make_request(client=client, **options)
 
         return cls._deserialize(data=response.data, many=False, **options)
 
     @classmethod
     async def update(cls, client: BaseRESTClient, obj: BaseModel, **kwargs) -> None:
         options = cls._prepare_options(
-            endpoint=Endpoint.READ, method=Method.GET, pk=cls._get_pk(obj), **kwargs
+            endpoint=Endpoint.UPDATE, method=Method.PATCH, pk=cls._get_pk(obj), **kwargs
         )
 
         options["json"] = cls._serialize(obj=obj, **options)
 
         await cls._make_request(client=client, **options)
 
     @classmethod
     async def delete(cls, client: BaseRESTClient, pk: any, **kwargs) -> None:
         options = cls._prepare_options(
-            endpoint=Endpoint.READ, method=Method.GET, pk=pk, **kwargs
+            endpoint=Endpoint.DELETE, method=Method.DELETE, pk=pk, **kwargs
         )
 
         await cls._make_request(client=client, **options)
```

### Comparing `resty_client-0.0.3/resty/middlewares/manager.py` & `resty_client-0.0.4/resty/middlewares/manager.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/resty/serializers/serializer.py` & `resty_client-0.0.4/resty/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/resty/types.py` & `resty_client-0.0.4/resty/types.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.3/PKG-INFO` & `resty_client-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: resty-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools.
 License: MIT
 Author: CrazyProger1
 Author-email: crazyproger1@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Description-Content-Type: text/markdown
 
-# RestyClient
+# Resty-Client
 
 <p align="center">
-<img src="https://github.com/CrazyProger1/RestyClient/blob/master/docs/resty-cat.png" alt="resty lib logo">
+<img src="https://github.com/CrazyProger1/Resty-Client/blob/master/docs/resty-cat.png" alt="resty lib logo">
 </p>
 
 <p align="center">
-<a href="https://github.com/CrazyProger1/RestyClient/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/CrazyProger1/RestyClient"></a>
-<a href="https://github.com/CrazyProger1/RestyClient/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/RestyClient"></a>
+<a href="https://github.com/CrazyProger1/Resty-Client/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/CrazyProger1/Resty-Client"></a>
+<a href="https://github.com/CrazyProger1/Resty-Client/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/Resty-Client"></a>
 <a href="https://pypi.org/project/resty-client/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/resty-client"></a>
 <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style"></a>
 </p>
 
-RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data
+
+Resty-Client is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data
 validation and deserialization tools. This library provides an intuitive API that makes it easy to make HTTP requests
 and handle data on the client side.
 
 ## Features
 
 - Middleware system, which allows you to implement any pagination, filtering or authentication.
+- Powerful data validation & deserialization using Pydantic
+- Easy-to-Use
 
 ## Installation
 
 Using pip:
 
 ```shell
 pip install resty-client
@@ -129,12 +132,12 @@
 
     # Delete
     await ProductManager.delete(rest_client, my_product.id)
 ```
 
 ## Status
 
-``0.0.2`` - **RELEASED**
+``0.0.4`` - **RELEASED**
 
 ## Licence
 
-RestyClient is released under the MIT License. See the bundled [LICENSE](LICENSE) file for details.
+Resty-Client is released under the MIT License. See the bundled [LICENSE](LICENSE) file for details.
```


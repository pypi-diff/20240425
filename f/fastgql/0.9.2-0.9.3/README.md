# Comparing `tmp/fastgql-0.9.2.tar.gz` & `tmp/fastgql-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgql-0.9.2.tar", max compression
+gzip compressed data, was "fastgql-0.9.3.tar", max compression
```

## Comparing `fastgql-0.9.2.tar` & `fastgql-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4956 2023-12-01 20:26:15.185531 fastgql-0.9.2/README.md
--rw-r--r--   0        0        0     1046 2023-11-01 07:13:53.449836 fastgql-0.9.2/fastgql/__init__.py
--rw-r--r--   0        0        0      506 2023-10-30 16:03:06.668946 fastgql-0.9.2/fastgql/context.py
--rw-r--r--   0        0        0      145 2023-10-25 22:03:21.089367 fastgql-0.9.2/fastgql/depends.py
--rw-r--r--   0        0        0        0 2023-10-25 22:13:51.498400 fastgql-0.9.2/fastgql/execute/__init__.py
--rw-r--r--   0        0        0     4328 2023-12-08 22:19:48.256761 fastgql-0.9.2/fastgql/execute/executor.py
--rw-r--r--   0        0        0    10899 2023-12-08 22:49:49.353160 fastgql-0.9.2/fastgql/execute/resolver.py
--rw-r--r--   0        0        0     4602 2023-11-10 00:20:47.396037 fastgql-0.9.2/fastgql/execute/utils.py
--rw-r--r--   0        0        0        0 2023-10-25 21:51:57.277314 fastgql-0.9.2/fastgql/gql_ast/__init__.py
--rw-r--r--   0        0        0     1192 2023-10-25 21:49:34.244208 fastgql-0.9.2/fastgql/gql_ast/models.py
--rw-r--r--   0        0        0    12496 2023-12-08 22:12:15.658524 fastgql-0.9.2/fastgql/gql_ast/translator.py
--rw-r--r--   0        0        0     1683 2023-12-08 22:20:24.768510 fastgql-0.9.2/fastgql/gql_models.py
--rw-r--r--   0        0        0      561 2023-10-30 16:09:33.748674 fastgql-0.9.2/fastgql/info.py
--rw-r--r--   0        0        0     6868 2023-11-15 23:36:59.643571 fastgql-0.9.2/fastgql/query_builders/edgedb/config.py
--rw-r--r--   0        0        0     5202 2023-12-08 21:36:55.883236 fastgql-0.9.2/fastgql/query_builders/edgedb/logic.py
--rw-r--r--   0        0        0      187 2023-10-26 15:37:10.657491 fastgql-0.9.2/fastgql/query_builders/edgedb/models.py
--rw-r--r--   0        0        0     7035 2023-10-26 15:10:57.180123 fastgql-0.9.2/fastgql/query_builders/edgedb/query_builder.py
--rw-r--r--   0        0        0     8127 2023-11-21 20:25:03.871659 fastgql-0.9.2/fastgql/query_builders/sql/config.py
--rw-r--r--   0        0        0     5565 2023-12-08 21:37:06.030561 fastgql-0.9.2/fastgql/query_builders/sql/logic.py
--rw-r--r--   0        0        0    16348 2023-12-06 16:35:01.996888 fastgql-0.9.2/fastgql/query_builders/sql/query_builder.py
--rw-r--r--   0        0        0     3163 2023-12-18 23:24:57.379618 fastgql-0.9.2/fastgql/scalars.py
--rw-r--r--   0        0        0    23680 2023-12-18 23:25:31.039108 fastgql-0.9.2/fastgql/schema_builder.py
--rw-r--r--   0        0        0     4503 2023-09-29 16:36:33.596831 fastgql-0.9.2/fastgql/static/graphiql.html
--rw-r--r--   0        0        0     1169 2023-11-01 07:25:22.024975 fastgql-0.9.2/fastgql/utils.py
--rw-r--r--   0        0        0     1623 2023-12-18 23:46:28.371050 fastgql-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 fastgql-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     4956 2023-12-01 20:26:15.185531 fastgql-0.9.3/README.md
+-rw-r--r--   0        0        0     1046 2023-11-01 07:13:53.449836 fastgql-0.9.3/fastgql/__init__.py
+-rw-r--r--   0        0        0      506 2023-10-30 16:03:06.668946 fastgql-0.9.3/fastgql/context.py
+-rw-r--r--   0        0        0      145 2023-10-25 22:03:21.089367 fastgql-0.9.3/fastgql/depends.py
+-rw-r--r--   0        0        0        0 2023-10-25 22:13:51.498400 fastgql-0.9.3/fastgql/execute/__init__.py
+-rw-r--r--   0        0        0     4328 2023-12-08 22:19:48.256761 fastgql-0.9.3/fastgql/execute/executor.py
+-rw-r--r--   0        0        0    10899 2023-12-08 22:49:49.353160 fastgql-0.9.3/fastgql/execute/resolver.py
+-rw-r--r--   0        0        0     4602 2023-11-10 00:20:47.396037 fastgql-0.9.3/fastgql/execute/utils.py
+-rw-r--r--   0        0        0        0 2023-10-25 21:51:57.277314 fastgql-0.9.3/fastgql/gql_ast/__init__.py
+-rw-r--r--   0        0        0     1192 2023-10-25 21:49:34.244208 fastgql-0.9.3/fastgql/gql_ast/models.py
+-rw-r--r--   0        0        0    12496 2023-12-08 22:12:15.658524 fastgql-0.9.3/fastgql/gql_ast/translator.py
+-rw-r--r--   0        0        0     1683 2023-12-08 22:20:24.768510 fastgql-0.9.3/fastgql/gql_models.py
+-rw-r--r--   0        0        0      561 2023-10-30 16:09:33.748674 fastgql-0.9.3/fastgql/info.py
+-rw-r--r--   0        0        0     6868 2023-11-15 23:36:59.643571 fastgql-0.9.3/fastgql/query_builders/edgedb/config.py
+-rw-r--r--   0        0        0     5202 2023-12-08 21:36:55.883236 fastgql-0.9.3/fastgql/query_builders/edgedb/logic.py
+-rw-r--r--   0        0        0      187 2023-10-26 15:37:10.657491 fastgql-0.9.3/fastgql/query_builders/edgedb/models.py
+-rw-r--r--   0        0        0     7035 2023-10-26 15:10:57.180123 fastgql-0.9.3/fastgql/query_builders/edgedb/query_builder.py
+-rw-r--r--   0        0        0     8127 2023-11-21 20:25:03.871659 fastgql-0.9.3/fastgql/query_builders/sql/config.py
+-rw-r--r--   0        0        0     5566 2023-12-19 16:54:52.014380 fastgql-0.9.3/fastgql/query_builders/sql/logic.py
+-rw-r--r--   0        0        0    16348 2023-12-06 16:35:01.996888 fastgql-0.9.3/fastgql/query_builders/sql/query_builder.py
+-rw-r--r--   0        0        0     3163 2023-12-18 23:24:57.379618 fastgql-0.9.3/fastgql/scalars.py
+-rw-r--r--   0        0        0    24987 2023-12-19 16:56:17.313617 fastgql-0.9.3/fastgql/schema_builder.py
+-rw-r--r--   0        0        0     4503 2023-09-29 16:36:33.596831 fastgql-0.9.3/fastgql/static/graphiql.html
+-rw-r--r--   0        0        0     1169 2023-11-01 07:25:22.024975 fastgql-0.9.3/fastgql/utils.py
+-rw-r--r--   0        0        0     1623 2023-12-19 16:37:09.667781 fastgql-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     6537 1970-01-01 00:00:00.000000 fastgql-0.9.3/PKG-INFO
```

### Comparing `fastgql-0.9.2/README.md` & `fastgql-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/__init__.py` & `fastgql-0.9.3/fastgql/__init__.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/execute/executor.py` & `fastgql-0.9.3/fastgql/execute/executor.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/execute/resolver.py` & `fastgql-0.9.3/fastgql/execute/resolver.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/execute/utils.py` & `fastgql-0.9.3/fastgql/execute/utils.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/gql_ast/models.py` & `fastgql-0.9.3/fastgql/gql_ast/models.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/gql_ast/translator.py` & `fastgql-0.9.3/fastgql/gql_ast/translator.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/gql_models.py` & `fastgql-0.9.3/fastgql/gql_models.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/info.py` & `fastgql-0.9.3/fastgql/info.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/query_builders/edgedb/config.py` & `fastgql-0.9.3/fastgql/query_builders/edgedb/config.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/query_builders/edgedb/logic.py` & `fastgql-0.9.3/fastgql/query_builders/edgedb/logic.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/query_builders/edgedb/query_builder.py` & `fastgql-0.9.3/fastgql/query_builders/edgedb/query_builder.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/query_builders/sql/config.py` & `fastgql-0.9.3/fastgql/query_builders/sql/config.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/query_builders/sql/logic.py` & `fastgql-0.9.3/fastgql/query_builders/sql/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     #     debug(gql_model._pydantic_model.qb_config_sql)
     print(
         f"[SQL QB CONFIG BUILDING] building the qb configs took: {(time.time() - start) * 1000} ms"
     )
 
 
 def root_type_s_from_annotation(
-    a: T.Any
+    a: T.Any,
 ) -> T.Type[BaseModel] | list[T.Type[BaseModel]]:
     if inspect.isclass(a):
         return a
     else:
         origin = T.get_origin(a)
         args = T.get_args(a)
         if origin is list or origin is types.UnionType or origin is T.Union:
```

### Comparing `fastgql-0.9.2/fastgql/query_builders/sql/query_builder.py` & `fastgql-0.9.3/fastgql/query_builders/sql/query_builder.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/scalars.py` & `fastgql-0.9.3/fastgql/scalars.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/schema_builder.py` & `fastgql-0.9.3/fastgql/schema_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import typing as T
 from dataclasses import dataclass
+from collections import OrderedDict
+import hashlib
 import time
 import types
 import datetime
 import enum
 import uuid
 import json
 import inspect
@@ -168,22 +170,26 @@
         cls,
         *,
         use_camel_case: bool = True,
         query_models: list[T.Type[GQL]],
         mutation_models: list[T.Type[GQL]] | None = None,
         allow_graphiql: bool = True,
         info_cls: T.Type[InfoType] | None = None,
+        introspection_cache_max_len: int | None = None,
     ):
         schema_builder = SchemaBuilder(
             use_camel_case=use_camel_case,
             query_models=query_models,
             mutation_models=mutation_models,
             info_cls=info_cls,
         )
-        return schema_builder._build_router(allow_graphiql=allow_graphiql)
+        return schema_builder._build_router(
+            allow_graphiql=allow_graphiql,
+            introspection_cache_max_len=introspection_cache_max_len,
+        )
 
     def snake_to_camel(self, s: str) -> str:
         if self.use_camel_case:
             return to_camel(s)
         return s
 
     @functools.cache
@@ -529,17 +535,19 @@
                         description=model.gql_description(),
                         interfaces=self.get_interfaces(model=model),
                     )
                 o._pydantic_model = model
             cache[model] = o
         return o
 
-    def _build_router(self, allow_graphiql: bool) -> APIRouter:
+    def _build_router(
+        self, allow_graphiql: bool, introspection_cache_max_len: int | None = None
+    ) -> APIRouter:
         router = APIRouter()
-
+        introspection_cache: OrderedDict[str, T.Any] = OrderedDict()
         if allow_graphiql:
 
             @router.get(
                 "",
                 responses={
                     200: {
                         "description": "The GraphiQL integrated development environment.",
@@ -581,20 +589,38 @@
 
             request.state.operation_name = request_data.operation_name
 
             if (
                 request_data.operation_name == "IntrospectionQuery"
                 or "IntrospectionQuery" in request_data.query
             ):
-                res = await graphql.graphql(
-                    schema=self.schema,
-                    source=request_data.query,
-                    variable_values=request_data.variables,
-                    operation_name=request_data.operation_name,
-                )
+                if introspection_cache_max_len:
+                    key = hashlib.sha256(
+                        f"{request_data.operation_name}{request_data.query}{request_data.variables}".encode()
+                    ).hexdigest()
+                    res = introspection_cache.get(key)
+                    if res:
+                        introspection_cache.move_to_end(key)
+                    else:
+                        res = await graphql.graphql(
+                            schema=self.schema,
+                            source=request_data.query,
+                            variable_values=request_data.variables,
+                            operation_name=request_data.operation_name,
+                        )
+                        if len(introspection_cache) > introspection_cache_max_len:
+                            introspection_cache.popitem(last=False)
+                        introspection_cache[key] = res
+                else:
+                    res = await graphql.graphql(
+                        schema=self.schema,
+                        source=request_data.query,
+                        variable_values=request_data.variables,
+                        operation_name=request_data.operation_name,
+                    )
             else:
                 res = await self.executor.execute(
                     source=request_data.query,
                     variable_values=request_data.variables,
                     operation_name=request_data.operation_name,
                     request=request,
                     response=response,
```

### Comparing `fastgql-0.9.2/fastgql/static/graphiql.html` & `fastgql-0.9.3/fastgql/static/graphiql.html`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/fastgql/utils.py` & `fastgql-0.9.3/fastgql/utils.py`

 * *Files identical despite different names*

### Comparing `fastgql-0.9.2/pyproject.toml` & `fastgql-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fastgql"
 packages = [{ include = "fastgql" }]
-version = "0.9.2"
+version = "0.9.3"
 description = "The easiest, fastest python GraphQL framework."
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jerber/fastgql"
 repository = "https://github.com/jerber/fastgql"
 documentation = "https://jerber.github.io/fastgql/"
```

### Comparing `fastgql-0.9.2/PKG-INFO` & `fastgql-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgql
-Version: 0.9.2
+Version: 0.9.3
 Summary: The easiest, fastest python GraphQL framework.
 Home-page: https://github.com/jerber/fastgql
 License: MIT
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```


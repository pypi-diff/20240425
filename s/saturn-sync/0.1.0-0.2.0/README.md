# Comparing `tmp/saturn_sync-0.1.0.tar.gz` & `tmp/saturn_sync-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn_sync-0.1.0.tar", max compression
+gzip compressed data, was "saturn_sync-0.2.0.tar", max compression
```

## Comparing `saturn_sync-0.1.0.tar` & `saturn_sync-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    16726 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/LICENSE
--rw-r--r--   0        0        0       71 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/README.md
--rw-r--r--   0        0        0     1478 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      564 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/__init__.py
--rw-r--r--   0        0        0      201 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/plugin/__init__.py
--rw-r--r--   0        0        0     1816 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/plugin/grpc_controller_pb2.py
--rw-r--r--   0        0        0      471 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/plugin/grpc_controller_pb2.pyi
--rw-r--r--   0        0        0     2942 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/plugin/grpc_controller_pb2_grpc.py
--rw-r--r--   0        0        0      201 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/protocol/__init__.py
--rw-r--r--   0        0        0      201 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/protocol/v1/__init__.py
--rw-r--r--   0        0        0     9139 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/protocol/v1/saturnsync_pb2.py
--rw-r--r--   0        0        0     8688 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/protocol/v1/saturnsync_pb2.pyi
--rw-r--r--   0        0        0    11910 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/protocol/v1/saturnsync_pb2_grpc.py
--rw-r--r--   0        0        0     7838 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/sdk.py
--rw-r--r--   0        0        0     1206 2024-03-22 19:33:23.907861 saturn_sync-0.1.0/saturn_sync/task.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 saturn_sync-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16726 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/LICENSE
+-rw-r--r--   0        0        0       71 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/README.md
+-rw-r--r--   0        0        0     1478 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/plugin/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/plugin/grpc_controller_pb2.py
+-rw-r--r--   0        0        0      471 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/plugin/grpc_controller_pb2.pyi
+-rw-r--r--   0        0        0     2942 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/plugin/grpc_controller_pb2_grpc.py
+-rw-r--r--   0        0        0      201 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/protocol/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/protocol/v1/__init__.py
+-rw-r--r--   0        0        0     6182 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/protocol/v1/saturnsync_pb2.py
+-rw-r--r--   0        0        0     4463 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/protocol/v1/saturnsync_pb2.pyi
+-rw-r--r--   0        0        0    11944 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/protocol/v1/saturnsync_pb2_grpc.py
+-rw-r--r--   0        0        0     5935 2024-04-25 10:55:31.063351 saturn_sync-0.2.0/saturn_sync/sdk.py
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 saturn_sync-0.2.0/PKG-INFO
```

### Comparing `saturn_sync-0.1.0/LICENSE` & `saturn_sync-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saturn_sync-0.1.0/pyproject.toml` & `saturn_sync-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [[tool.mypy.overrides]]
 module = "grpc_health.*"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "saturn-sync"
-version = "0.1.0"
+version = "0.2.0"
 description = "Synchronize and refactor repositories with ease."
 authors = ["Markus Meyer <hydrantanderwand@gmail.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/wndhydrnt/saturn-sync-protocol"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `saturn_sync-0.1.0/saturn_sync/plugin/grpc_controller_pb2.py` & `saturn_sync-0.2.0/saturn_sync/plugin/grpc_controller_pb2.py`

 * *Files identical despite different names*

### Comparing `saturn_sync-0.1.0/saturn_sync/plugin/grpc_controller_pb2_grpc.py` & `saturn_sync-0.2.0/saturn_sync/plugin/grpc_controller_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `saturn_sync-0.1.0/saturn_sync/protocol/v1/saturnsync_pb2_grpc.py` & `saturn_sync-0.2.0/saturn_sync/protocol/v1/saturnsync_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,71 +5,71 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from saturn_sync.protocol.v1 import saturnsync_pb2 as saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2
 
 
-class TaskServiceStub(object):
+class PluginServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.ExecuteActions = channel.unary_unary(
-                '/protocol.v1.TaskService/ExecuteActions',
+                '/protocol.v1.PluginService/ExecuteActions',
                 request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteActionsRequest.SerializeToString,
                 response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteActionsResponse.FromString,
                 )
         self.ExecuteFilters = channel.unary_unary(
-                '/protocol.v1.TaskService/ExecuteFilters',
+                '/protocol.v1.PluginService/ExecuteFilters',
                 request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteFiltersRequest.SerializeToString,
                 response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteFiltersResponse.FromString,
                 )
-        self.ListTasks = channel.unary_unary(
-                '/protocol.v1.TaskService/ListTasks',
-                request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ListTasksRequest.SerializeToString,
-                response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ListTasksResponse.FromString,
+        self.GetPlugin = channel.unary_unary(
+                '/protocol.v1.PluginService/GetPlugin',
+                request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.GetPluginRequest.SerializeToString,
+                response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.GetPluginResponse.FromString,
                 )
         self.OnPrClosed = channel.unary_unary(
-                '/protocol.v1.TaskService/OnPrClosed',
+                '/protocol.v1.PluginService/OnPrClosed',
                 request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrClosedRequest.SerializeToString,
                 response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrClosedResponse.FromString,
                 )
         self.OnPrCreated = channel.unary_unary(
-                '/protocol.v1.TaskService/OnPrCreated',
+                '/protocol.v1.PluginService/OnPrCreated',
                 request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrCreatedRequest.SerializeToString,
                 response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrCreatedResponse.FromString,
                 )
         self.OnPrMerged = channel.unary_unary(
-                '/protocol.v1.TaskService/OnPrMerged',
+                '/protocol.v1.PluginService/OnPrMerged',
                 request_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrMergedRequest.SerializeToString,
                 response_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrMergedResponse.FromString,
                 )
 
 
-class TaskServiceServicer(object):
+class PluginServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ExecuteActions(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ExecuteFilters(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListTasks(self, request, context):
+    def GetPlugin(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def OnPrClosed(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -86,30 +86,30 @@
     def OnPrMerged(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_TaskServiceServicer_to_server(servicer, server):
+def add_PluginServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ExecuteActions': grpc.unary_unary_rpc_method_handler(
                     servicer.ExecuteActions,
                     request_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteActionsRequest.FromString,
                     response_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteActionsResponse.SerializeToString,
             ),
             'ExecuteFilters': grpc.unary_unary_rpc_method_handler(
                     servicer.ExecuteFilters,
                     request_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteFiltersRequest.FromString,
                     response_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteFiltersResponse.SerializeToString,
             ),
-            'ListTasks': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListTasks,
-                    request_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ListTasksRequest.FromString,
-                    response_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ListTasksResponse.SerializeToString,
+            'GetPlugin': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPlugin,
+                    request_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.GetPluginRequest.FromString,
+                    response_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.GetPluginResponse.SerializeToString,
             ),
             'OnPrClosed': grpc.unary_unary_rpc_method_handler(
                     servicer.OnPrClosed,
                     request_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrClosedRequest.FromString,
                     response_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrClosedResponse.SerializeToString,
             ),
             'OnPrCreated': grpc.unary_unary_rpc_method_handler(
@@ -120,34 +120,34 @@
             'OnPrMerged': grpc.unary_unary_rpc_method_handler(
                     servicer.OnPrMerged,
                     request_deserializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrMergedRequest.FromString,
                     response_serializer=saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrMergedResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'protocol.v1.TaskService', rpc_method_handlers)
+            'protocol.v1.PluginService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class TaskService(object):
+class PluginService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def ExecuteActions(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/protocol.v1.TaskService/ExecuteActions',
+        return grpc.experimental.unary_unary(request, target, '/protocol.v1.PluginService/ExecuteActions',
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteActionsRequest.SerializeToString,
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteActionsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ExecuteFilters(request,
@@ -156,49 +156,49 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/protocol.v1.TaskService/ExecuteFilters',
+        return grpc.experimental.unary_unary(request, target, '/protocol.v1.PluginService/ExecuteFilters',
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteFiltersRequest.SerializeToString,
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ExecuteFiltersResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListTasks(request,
+    def GetPlugin(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/protocol.v1.TaskService/ListTasks',
-            saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ListTasksRequest.SerializeToString,
-            saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.ListTasksResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/protocol.v1.PluginService/GetPlugin',
+            saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.GetPluginRequest.SerializeToString,
+            saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.GetPluginResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def OnPrClosed(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/protocol.v1.TaskService/OnPrClosed',
+        return grpc.experimental.unary_unary(request, target, '/protocol.v1.PluginService/OnPrClosed',
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrClosedRequest.SerializeToString,
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrClosedResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def OnPrCreated(request,
@@ -207,15 +207,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/protocol.v1.TaskService/OnPrCreated',
+        return grpc.experimental.unary_unary(request, target, '/protocol.v1.PluginService/OnPrCreated',
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrCreatedRequest.SerializeToString,
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrCreatedResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def OnPrMerged(request,
@@ -224,12 +224,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/protocol.v1.TaskService/OnPrMerged',
+        return grpc.experimental.unary_unary(request, target, '/protocol.v1.PluginService/OnPrMerged',
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrMergedRequest.SerializeToString,
             saturn__sync_dot_protocol_dot_v1_dot_saturnsync__pb2.OnPrMergedResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `saturn_sync-0.1.0/saturn_sync/sdk.py` & `saturn_sync-0.2.0/saturn_sync/sdk.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,199 +1,172 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-import collections.abc
 import contextlib
 import errno
-import json
 import os
 import random
 import socket
 import sys
 import time
 from concurrent import futures
-from typing import Iterable, Iterator
+from typing import Iterator, Mapping
 
 import grpc
 from grpc_health.v1 import health_pb2, health_pb2_grpc
 from grpc_health.v1.health import HealthServicer
 
+from saturn_sync import Context
 from saturn_sync.plugin import grpc_controller_pb2_grpc
 from saturn_sync.protocol.v1 import saturnsync_pb2, saturnsync_pb2_grpc
-from saturn_sync.task import Task
 
 BIND_IP: str = "127.0.0.1"
 
 
-class Config(collections.abc.Mapping):
-    def __init__(self, data: dict[str, str]):
-        self._data = data
-
-    def __getitem__(self, item: str) -> str:
-        item_lower = item.lower()
-        return self._data.get(item_lower, "")
+class Plugin:
+    name: str
+    priority: int = 0
 
-    def __iter__(self):
-        return self._data.__iter__()
+    def init(self, config: Mapping[str, str]) -> None:
+        pass
 
-    def __len__(self):
-        return self._data.__len__()
+    def apply(self, ctx: Context) -> None:
+        return None
+
+    def filter(self, ctx: Context) -> bool:
+        return True
+
+    def on_pr_closed(self, ctx: Context):
+        pass
+
+    def on_pr_created(self, ctx: Context):
+        pass
+
+    def on_pr_merged(self, ctx: Context):
+        pass
 
 
 @contextlib.contextmanager
 def in_checkout_dir(d: str) -> Iterator[None]:
     current = os.getcwd()
     os.chdir(d)
     try:
         yield
     finally:
         os.chdir(current)
 
 
-class TaskService(saturnsync_pb2_grpc.TaskServiceServicer):
-    def __init__(self, tasks: Iterable[Task]):
-        self._tasks: dict[str, Task] = {}
-        for t in tasks:
-            self._tasks[t.name] = t
+class PluginService(saturnsync_pb2_grpc.PluginServiceServicer):
+    def __init__(self, p: Plugin):
+        self._plugin = p
 
     def ExecuteActions(
         self, request: saturnsync_pb2.ExecuteActionsRequest, context
     ) -> saturnsync_pb2.ExecuteActionsResponse:
         try:
             with in_checkout_dir(request.path):
-                task = self._tasks.get(request.task_name, None)
-                if task is None:
-                    return saturnsync_pb2.ExecuteActionsResponse(
-                        error=f"unknown task {request.task_name}"
-                    )
-
-                task.apply(ctx=request.context)
+                self._plugin.apply(ctx=request.context)
         except Exception as e:
             return saturnsync_pb2.ExecuteActionsResponse(
-                error=f"exception during apply of {request.task_name}: {e}"
+                error=f"failed to execute actions: {e}"
             )
 
         return saturnsync_pb2.ExecuteActionsResponse(error=None)
 
     def ExecuteFilters(
         self, request: saturnsync_pb2.ExecuteFiltersRequest, context
     ) -> saturnsync_pb2.ExecuteFiltersResponse:
         try:
-            task = self._tasks.get(request.task_name, None)
-            if task is None:
-                return saturnsync_pb2.ExecuteFiltersResponse(
-                    match=False, error=f"unknown task {request.task_name}"
-                )
-
-            result = task.filter(ctx=request.context)
+            result = self._plugin.filter(ctx=request.context)
             return saturnsync_pb2.ExecuteFiltersResponse(match=result, error=None)
         except Exception as e:
             return saturnsync_pb2.ExecuteFiltersResponse(
                 match=False,
-                error=f"exception during filtering of {request.task_name}: {e}",
+                error=f"failed to execute filters: {e}",
             )
 
-    def ListTasks(
-        self, request: saturnsync_pb2.ListTasksRequest, context
-    ) -> saturnsync_pb2.ListTasksResponse:
-        try:
-            config = Config(data=json.loads(request.custom_config))
-            proto_tasks: list[saturnsync_pb2.Task] = []
-            for t in self._tasks.values():
-                t.init(config)
-                proto_tasks.append(_to_proto_task(t))
-
-            return saturnsync_pb2.ListTasksResponse(tasks=proto_tasks)
+    def GetPlugin(
+        self, request: saturnsync_pb2.GetPluginRequest, context
+    ) -> saturnsync_pb2.GetPluginResponse:
+        try:
+            self._plugin.init(config=request.config)
+            return saturnsync_pb2.GetPluginResponse(
+                name=self._plugin.name, priority=self._plugin.priority, error=None
+            )
         except Exception as e:
-            return saturnsync_pb2.ListTasksResponse(error=f"cannot list tasks: {e}")
+            return saturnsync_pb2.GetPluginResponse(
+                error=f"plugin '{self._plugin.name}' failed during initialization: {e}"
+            )
 
     def OnPrClosed(
         self, request: saturnsync_pb2.OnPrClosedRequest, context
     ) -> saturnsync_pb2.OnPrClosedResponse:
         try:
-            task = self._tasks.get(request.task_name, None)
-            if task is None:
-                return saturnsync_pb2.OnPrClosedResponse(
-                    error=f"unknown task {request.task_name}"
-                )
-
-            task.on_pr_closed(request.context)
+            self._plugin.on_pr_closed(request.context)
             return saturnsync_pb2.OnPrClosedResponse(error=None)
         except Exception as e:
             return saturnsync_pb2.OnPrClosedResponse(
-                error=f"exception during execution: {e}"
+                error=f"failed to execute OnPrClosed event: {e}"
             )
 
     def OnPrCreated(
         self, request: saturnsync_pb2.OnPrCreatedRequest, context
     ) -> saturnsync_pb2.OnPrCreatedResponse:
         try:
-            task = self._tasks.get(request.task_name, None)
-            if task is None:
-                return saturnsync_pb2.OnPrCreatedResponse(
-                    error=f"unknown task {request.task_name}"
-                )
-
-            task.on_pr_created(request.context)
+            self._plugin.on_pr_created(request.context)
             return saturnsync_pb2.OnPrCreatedResponse(error=None)
         except Exception as e:
             return saturnsync_pb2.OnPrCreatedResponse(
-                error=f"exception during execution: {e}"
+                error=f"failed to execute OnPrCreated event: {e}"
             )
 
     def OnPrMerged(
         self, request: saturnsync_pb2.OnPrMergedRequest, context
     ) -> saturnsync_pb2.OnPrMergedResponse:
         try:
-            task = self._tasks.get(request.task_name, None)
-            if task is None:
-                return saturnsync_pb2.OnPrMergedResponse(
-                    error=f"unknown task {request.task_name}"
-                )
-
-            task.on_pr_merged(request.context)
+            self._plugin.on_pr_merged(request.context)
             return saturnsync_pb2.OnPrMergedResponse(error=None)
         except Exception as e:
             return saturnsync_pb2.OnPrMergedResponse(
-                error=f"exception during execution: {e}"
+                error=f"failed to execute OnPrMerged event: {e}"
             )
 
 
 class GRPCController(grpc_controller_pb2_grpc.GRPCControllerServicer):
     def __init__(self):
         self.is_shut_down = False
 
     def Shutdown(self, request, context):
         self.is_shut_down = True
 
 
-def serve(port: int, shutdown: GRPCController, tasks: Iterable[Task]):
+def serve(port: int, shutdown: GRPCController, plugin: Plugin):
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=10))
     server.add_insecure_port(f"{BIND_IP}:{port}")
 
-    saturnsync_pb2_grpc.add_TaskServiceServicer_to_server(
-        servicer=TaskService(tasks), server=server
+    saturnsync_pb2_grpc.add_PluginServiceServicer_to_server(
+        servicer=PluginService(plugin), server=server
     )
 
     grpc_controller_pb2_grpc.add_GRPCControllerServicer_to_server(
         servicer=shutdown, server=server
     )
 
     health = HealthServicer()
     health.set("plugin", health_pb2.HealthCheckResponse.ServingStatus.Value("SERVING"))
     health_pb2_grpc.add_HealthServicer_to_server(servicer=health, server=server)
     server.start()
     return server
 
 
-def serve_tasks(*tasks: Task) -> None:
+def serve_plugin(plugin: Plugin) -> None:
     port = _find_open_port()
     grpc_controller = GRPCController()
-    server = serve(port=port, shutdown=grpc_controller, tasks=tasks)
+    server = serve(port=port, shutdown=grpc_controller, plugin=plugin)
     print(f"1|1|tcp|{BIND_IP}:{port}|grpc")
     sys.stdout.flush()
     try:
         while True:
             time.sleep(0.1)
             if grpc_controller.is_shut_down is True:
                 server.stop(0)
@@ -211,26 +184,7 @@
             return port
         except socket.error as e:
             if e.errno != errno.EADDRINUSE:
                 raise e
         finally:
             if s is not None:
                 s.close()
-
-
-def _to_proto_task(task: Task) -> saturnsync_pb2.Task:
-    return saturnsync_pb2.Task(
-        name=task.name,
-        auto_merge=task.auto_merge,
-        auto_merge_after_seconds=task.auto_merge_after_seconds,
-        branch_name=task.branch_name,
-        change_limit=task.change_limit,
-        commit_message=task.commit_message,
-        create_only=task.create_only,
-        disabled=task.disabled,
-        filters=task.filters,
-        keep_branch_after_merge=task.keep_branch_after_merge,
-        labels=task.labels,
-        merge_once=task.merge_once,
-        pr_body=task.pr_body,
-        pr_title=task.pr_title,
-    )
```

### Comparing `saturn_sync-0.1.0/PKG-INFO` & `saturn_sync-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-sync
-Version: 0.1.0
+Version: 0.2.0
 Summary: Synchronize and refactor repositories with ease.
 Home-page: https://github.com/wndhydrnt/saturn-sync-protocol
 License: MPL-2.0
 Author: Markus Meyer
 Author-email: hydrantanderwand@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```


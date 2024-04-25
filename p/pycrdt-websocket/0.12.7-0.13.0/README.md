# Comparing `tmp/pycrdt_websocket-0.12.7.tar.gz` & `tmp/pycrdt_websocket-0.13.0.tar.gz`

## Comparing `pycrdt_websocket-0.12.7.tar` & `pycrdt_websocket-0.13.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/awareness.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/django_channels_consumer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/py.typed
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/websocket.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/websocket_provider.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/websocket_server.py
--rw-r--r--   0        0        0     8459 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/yroom.py
--rw-r--r--   0        0        0    15542 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/ystore.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pycrdt_websocket/yutils.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/conftest.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/package.json
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/test_asgi.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/test_pycrdt_yjs.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/test_ystore.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/yjs_client_0.js
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/tests/yjs_client_1.js
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/LICENSE
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/README.md
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/pyproject.toml
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 pycrdt_websocket-0.12.7/PKG-INFO
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/awareness.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/django_channels_consumer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/py.typed
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/websocket.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_provider.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_server.py
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/yroom.py
+-rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/ystore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/yutils.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/conftest.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/package.json
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/test_asgi.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/test_pycrdt_yjs.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/test_ystore.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/utils.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/yjs_client_0.js
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/yjs_client_1.js
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/PKG-INFO
```

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/asgi_server.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/awareness.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/awareness.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/django_channels_consumer.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/websocket.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/websocket_provider.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from contextlib import AsyncExitStack
 from functools import partial
 from logging import Logger, getLogger
 
 from anyio import (
     TASK_STATUS_IGNORED,
     Event,
+    Lock,
     create_memory_object_stream,
     create_task_group,
 )
 from anyio.abc import TaskGroup, TaskStatus
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
-from pycrdt import Doc
+from pycrdt import Doc, Subscription
 
 from .websocket import Websocket
 from .yutils import (
     YMessageType,
     create_update_message,
     process_sync_message,
     put_updates,
@@ -26,77 +27,61 @@
 
 class WebsocketProvider:
     """WebSocket provider."""
 
     _ydoc: Doc
     _update_send_stream: MemoryObjectSendStream
     _update_receive_stream: MemoryObjectReceiveStream
-    _started: Event | None
-    _starting: bool
-    _task_group: TaskGroup | None
+    _subscription: Subscription
+    _started: Event | None = None
+    _task_group: TaskGroup | None = None
+    __start_lock: Lock | None = None
 
     def __init__(self, ydoc: Doc, websocket: Websocket, log: Logger | None = None) -> None:
         """Initialize the object.
 
         The WebsocketProvider instance should preferably be used as an async context manager:
         ```py
         async with websocket_provider:
             ...
         ```
         However, a lower-level API can also be used:
         ```py
         task = asyncio.create_task(websocket_provider.start())
         await websocket_provider.started.wait()
         ...
-        websocket_provider.stop()
+        await websocket_provider.stop()
         ```
 
         Arguments:
             ydoc: The YDoc to connect through the WebSocket.
             websocket: The WebSocket through which to connect the YDoc.
             log: An optional logger.
         """
         self._ydoc = ydoc
         self._websocket = websocket
         self.log = log or getLogger(__name__)
         self._update_send_stream, self._update_receive_stream = create_memory_object_stream(
             max_buffer_size=65536
         )
-        self._started = None
-        self._starting = False
-        self._task_group = None
-        ydoc.observe(partial(put_updates, self._update_send_stream))
 
     @property
     def started(self) -> Event:
         """An async event that is set when the WebSocket provider has started."""
         if self._started is None:
             self._started = Event()
         return self._started
 
-    async def __aenter__(self) -> WebsocketProvider:
-        if self._task_group is not None:
-            raise RuntimeError("WebsocketProvider already running")
-
-        async with AsyncExitStack() as exit_stack:
-            tg = create_task_group()
-            self._task_group = await exit_stack.enter_async_context(tg)
-            self._exit_stack = exit_stack.pop_all()
-            tg.start_soon(self._run)
-            self.started.set()
-
         return self
 
-    async def __aexit__(self, exc_type, exc_value, exc_tb):
-        if self._task_group is None:
-            raise RuntimeError("WebsocketProvider not running")
-
-        self._task_group.cancel_scope.cancel()
-        self._task_group = None
-        return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
+    @property
+    def _start_lock(self) -> Lock:
+        if self.__start_lock is None:
+            self.__start_lock = Lock()
+        return self.__start_lock
 
     async def _run(self):
         await sync(self._ydoc, self._websocket, self.log)
         self._task_group.start_soon(self._send)
         async for message in self._websocket:
             if message[0] == YMessageType.SYNC:
                 await process_sync_message(message[1:], self._ydoc, self._websocket, self.log)
@@ -106,34 +91,61 @@
             async for update in self._update_receive_stream:
                 message = create_update_message(update)
                 try:
                     await self._websocket.send(message)
                 except Exception:
                     pass
 
-    async def start(self, *, task_status: TaskStatus[None] = TASK_STATUS_IGNORED):
+    async def __aenter__(self) -> WebsocketProvider:
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("WebsocketProvider already running")
+
+            async with AsyncExitStack() as exit_stack:
+                tg = create_task_group()
+                self._task_group = await exit_stack.enter_async_context(tg)
+                self._exit_stack = exit_stack.pop_all()
+                await tg.start(partial(self.start, from_context_manager=True))
+
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, exc_tb):
+        await self.stop()
+        return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
+
+    async def start(
+        self,
+        *,
+        task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
+        from_context_manager: bool = False,
+    ):
         """Start the WebSocket provider.
 
         Arguments:
             task_status: The status to set when the task has started.
         """
-        if self._starting:
-            return
-        else:
-            self._starting = True
+        self._subscription = self._ydoc.observe(partial(put_updates, self._update_send_stream))
 
-        if self._task_group is not None:
-            raise RuntimeError("WebsocketProvider already running")
-
-        async with create_task_group() as self._task_group:
-            self._task_group.start_soon(self._run)
-            self.started.set()
-            self._starting = False
+        if from_context_manager:
             task_status.started()
+            self.started.set()
+            assert self._task_group is not None
+            self._task_group.start_soon(self._run)
+            return
+
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("WebsocketProvider already running")
+
+            async with create_task_group() as self._task_group:
+                task_status.started()
+                self.started.set()
+                self._task_group.start_soon(self._run)
 
-    def stop(self):
+    async def stop(self):
         """Stop the WebSocket provider."""
         if self._task_group is None:
             raise RuntimeError("WebsocketProvider not running")
 
         self._task_group.cancel_scope.cancel()
         self._task_group = None
+        self._ydoc.unobserve(self._subscription)
```

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/websocket_server.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 from contextlib import AsyncExitStack
+from functools import partial
 from logging import Logger, getLogger
 
-from anyio import TASK_STATUS_IGNORED, Event, create_task_group
+from anyio import TASK_STATUS_IGNORED, Event, Lock, create_task_group
 from anyio.abc import TaskGroup, TaskStatus
 
 from .websocket import Websocket
 from .yroom import YRoom
 
 
 class WebsocketServer:
     """WebSocket server."""
 
     auto_clean_rooms: bool
     rooms: dict[str, YRoom]
-    _started: Event | None
-    _starting: bool
-    _task_group: TaskGroup | None
+    _started: Event | None = None
+    _task_group: TaskGroup | None = None
+    __start_lock: Lock | None = None
 
     def __init__(
         self, rooms_ready: bool = True, auto_clean_rooms: bool = True, log: Logger | None = None
     ) -> None:
         """Initialize the object.
 
         The WebsocketServer instance should preferably be used as an async context manager:
@@ -30,37 +31,40 @@
             ...
         ```
         However, a lower-level API can also be used:
         ```py
         task = asyncio.create_task(websocket_server.start())
         await websocket_server.started.wait()
         ...
-        websocket_server.stop()
+        await websocket_server.stop()
         ```
 
         Arguments:
             rooms_ready: Whether rooms are ready to be synchronized when opened.
             auto_clean_rooms: Whether rooms should be deleted when no client is there anymore.
             log: An optional logger.
         """
         self.rooms_ready = rooms_ready
         self.auto_clean_rooms = auto_clean_rooms
         self.log = log or getLogger(__name__)
         self.rooms = {}
-        self._started = None
-        self._starting = False
-        self._task_group = None
 
     @property
     def started(self) -> Event:
         """An async event that is set when the WebSocket server has started."""
         if self._started is None:
             self._started = Event()
         return self._started
 
+    @property
+    def _start_lock(self) -> Lock:
+        if self.__start_lock is None:
+            self.__start_lock = Lock()
+        return self.__start_lock
+
     async def get_room(self, name: str) -> YRoom:
         """Get or create a room with the given name, and start it.
 
         Arguments:
             name: The room name.
 
         Returns:
@@ -111,28 +115,28 @@
         if from_name is not None and from_room is not None:
             raise RuntimeError("Cannot pass from_name and from_room")
         if from_name is None:
             assert from_room is not None
             from_name = self.get_room_name(from_room)
         self.rooms[to_name] = self.rooms.pop(from_name)
 
-    def delete_room(self, *, name: str | None = None, room: YRoom | None = None) -> None:
+    async def delete_room(self, *, name: str | None = None, room: YRoom | None = None) -> None:
         """Delete a room.
 
         Arguments:
             name: The name of the room to delete (if `room` is not passed).
-            room: The room to delete ( if `name` is not passed).
+            room: The room to delete (if `name` is not passed).
         """
         if name is not None and room is not None:
             raise RuntimeError("Cannot pass name and room")
         if name is None:
             assert room is not None
             name = self.get_room_name(room)
         room = self.rooms.pop(name)
-        room.stop()
+        await room.stop()
 
     async def serve(self, websocket: Websocket) -> None:
         """Serve a client through a WebSocket.
 
         Arguments:
             websocket: The WebSocket through which to serve the client.
         """
@@ -147,58 +151,63 @@
 
     async def _serve(self, websocket: Websocket, tg: TaskGroup):
         room = await self.get_room(websocket.path)
         await self.start_room(room)
         await room.serve(websocket)
 
         if self.auto_clean_rooms and not room.clients:
-            self.delete_room(room=room)
+            await self.delete_room(room=room)
         tg.cancel_scope.cancel()
 
     async def __aenter__(self) -> WebsocketServer:
-        if self._task_group is not None:
-            raise RuntimeError("WebsocketServer already running")
-
-        async with AsyncExitStack() as exit_stack:
-            tg = create_task_group()
-            self._task_group = await exit_stack.enter_async_context(tg)
-            self._exit_stack = exit_stack.pop_all()
-            self.started.set()
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("WebsocketServer already running")
+
+            async with AsyncExitStack() as exit_stack:
+                tg = create_task_group()
+                self._task_group = await exit_stack.enter_async_context(tg)
+                self._exit_stack = exit_stack.pop_all()
+                await tg.start(partial(self.start, from_context_manager=True))
 
         return self
 
     async def __aexit__(self, exc_type, exc_value, exc_tb):
-        if self._task_group is None:
-            raise RuntimeError("WebsocketServer not running")
-
-        self._task_group.cancel_scope.cancel()
-        self._task_group = None
+        await self.stop()
         return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
 
-    async def start(self, *, task_status: TaskStatus[None] = TASK_STATUS_IGNORED):
+    async def start(
+        self,
+        *,
+        task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
+        from_context_manager: bool = False,
+    ):
         """Start the WebSocket server.
 
         Arguments:
             task_status: The status to set when the task has started.
         """
-        if self._starting:
+        if from_context_manager:
+            task_status.started()
+            self.started.set()
+            assert self._task_group is not None
+            # wait forever
+            self._task_group.start_soon(Event().wait)
             return
-        else:
-            self._starting = True
 
-        if self._task_group is not None:
-            raise RuntimeError("WebsocketServer already running")
-
-        # create the task group and wait forever
-        async with create_task_group() as self._task_group:
-            self._task_group.start_soon(Event().wait)
-            self.started.set()
-            self._starting = False
-            task_status.started()
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("WebsocketServer already running")
+
+            async with create_task_group() as self._task_group:
+                task_status.started()
+                self.started.set()
+                # wait forever
+                self._task_group.start_soon(Event().wait)
 
-    def stop(self) -> None:
+    async def stop(self) -> None:
         """Stop the WebSocket server."""
         if self._task_group is None:
             raise RuntimeError("WebsocketServer not running")
 
         self._task_group.cancel_scope.cancel()
         self._task_group = None
```

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/yroom.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/yroom.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from inspect import isawaitable
 from logging import Logger, getLogger
 from typing import Awaitable, Callable
 
 from anyio import (
     TASK_STATUS_IGNORED,
     Event,
+    Lock,
     create_memory_object_stream,
     create_task_group,
 )
 from anyio.abc import TaskGroup, TaskStatus
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
-from pycrdt import Doc
+from pycrdt import Doc, Subscription
 
 from .awareness import Awareness
 from .websocket import Websocket
 from .ystore import BaseYStore
 from .yutils import (
     YMessageType,
     create_update_message,
@@ -28,21 +29,22 @@
 )
 
 
 class YRoom:
     clients: list
     ydoc: Doc
     ystore: BaseYStore | None
+    ready_event: Event
     _on_message: Callable[[bytes], Awaitable[bool] | bool] | None
     _update_send_stream: MemoryObjectSendStream
     _update_receive_stream: MemoryObjectReceiveStream
-    _ready: bool
-    _task_group: TaskGroup | None
-    _started: Event | None
-    _starting: bool
+    _task_group: TaskGroup | None = None
+    _started: Event | None = None
+    __start_lock: Lock | None = None
+    _subscription: Subscription | None = None
 
     def __init__(
         self, ready: bool = True, ystore: BaseYStore | None = None, log: Logger | None = None
     ):
         """Initialize the object.
 
         The YRoom instance should preferably be used as an async context manager:
@@ -51,60 +53,66 @@
             ...
         ```
         However, a lower-level API can also be used:
         ```py
         task = asyncio.create_task(room.start())
         await room.started.wait()
         ...
-        room.stop()
+        await room.stop()
         ```
 
         Arguments:
             ready: Whether the internal YDoc is ready to be synchronized right away.
             ystore: An optional store in which to persist document updates.
             log: An optional logger.
         """
         self.ydoc = Doc()
         self.awareness = Awareness(self.ydoc)
         self._update_send_stream, self._update_receive_stream = create_memory_object_stream(
             max_buffer_size=65536
         )
-        self._ready = False
+        self.ready_event = Event()
         self.ready = ready
         self.ystore = ystore
         self.log = log or getLogger(__name__)
         self.clients = []
         self._on_message = None
-        self._started = None
-        self._starting = False
-        self._task_group = None
+
+    @property
+    def _start_lock(self) -> Lock:
+        if self.__start_lock is None:
+            self.__start_lock = Lock()
+        return self.__start_lock
 
     @property
     def started(self):
         """An async event that is set when the YRoom provider has started."""
         if self._started is None:
             self._started = Event()
         return self._started
 
     @property
     def ready(self) -> bool:
         """
         Returns:
             True is the internal YDoc is ready to be synchronized.
         """
-        return self._ready
+        return self.ready_event.is_set()
 
     @ready.setter
     def ready(self, value: bool) -> None:
         """
         Arguments:
             value: True if the internal YDoc is ready to be synchronized, False otherwise."""
-        self._ready = value
-        if value:
-            self.ydoc.observe(partial(put_updates, self._update_send_stream))
+        if value and not self.ready_event.is_set():
+            self.ready_event.set()
+
+    async def _watch_ready(self):
+        await self.ready_event.wait()
+        self._subscription = self.ydoc.observe(partial(put_updates, self._update_send_stream))
 
     @property
     def on_message(self) -> Callable[[bytes], Awaitable[bool] | bool] | None:
         """
         Returns:
             The optional callback to call when a message is received.
         """
@@ -134,61 +142,70 @@
                     message = create_update_message(update)
                     self._task_group.start_soon(client.send, message)
                 if self.ystore:
                     self.log.debug("Writing Y update to YStore")
                     self._task_group.start_soon(self.ystore.write, update)
 
     async def __aenter__(self) -> YRoom:
-        if self._task_group is not None:
-            raise RuntimeError("YRoom already running")
-
-        async with AsyncExitStack() as exit_stack:
-            tg = create_task_group()
-            self._task_group = await exit_stack.enter_async_context(tg)
-            self._exit_stack = exit_stack.pop_all()
-            tg.start_soon(self._broadcast_updates)
-            self.started.set()
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("YRoom already running")
+
+            async with AsyncExitStack() as exit_stack:
+                tg = create_task_group()
+                self._task_group = await exit_stack.enter_async_context(tg)
+                self._exit_stack = exit_stack.pop_all()
+                await tg.start(partial(self.start, from_context_manager=True))
 
         return self
 
     async def __aexit__(self, exc_type, exc_value, exc_tb):
-        if self._task_group is None:
-            raise RuntimeError("YRoom not running")
-
-        self._task_group.cancel_scope.cancel()
-        self._task_group = None
+        await self.stop()
         return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
 
-    async def start(self, *, task_status: TaskStatus[None] = TASK_STATUS_IGNORED):
+    async def start(
+        self,
+        *,
+        task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
+        from_context_manager: bool = False,
+    ):
         """Start the room.
 
         Arguments:
             task_status: The status to set when the task has started.
         """
-        if self._starting:
+        if from_context_manager:
+            task_status.started()
+            self.started.set()
+            assert self._task_group is not None
+            self._task_group.start_soon(self._broadcast_updates)
             return
-        else:
-            self._starting = True
 
-        if self._task_group is not None:
-            raise RuntimeError("YRoom already running")
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("YRoom already running")
+
+            async with create_task_group() as self._task_group:
+                task_status.started()
+                self.started.set()
+                self._task_group.start_soon(self._broadcast_updates)
+                self._task_group.start_soon(self._watch_ready)
 
-        async with create_task_group() as self._task_group:
-            self._task_group.start_soon(self._broadcast_updates)
-            self.started.set()
-            self._starting = False
-            task_status.started()
-
-    def stop(self):
+    async def stop(self) -> None:
         """Stop the room."""
         if self._task_group is None:
             raise RuntimeError("YRoom not running")
 
+        if self._task_group is None:
+            return
+
         self._task_group.cancel_scope.cancel()
         self._task_group = None
+        if self._subscription is not None:
+            self.ydoc.unobserve(self._subscription)
 
     async def serve(self, websocket: Websocket):
         """Serve a client.
 
         Arguments:
             websocket: The WebSocket through which to serve the client.
         """
```

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/ystore.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/ystore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,99 +1,107 @@
 from __future__ import annotations
 
 import struct
 import tempfile
 import time
 from abc import ABC, abstractmethod
 from contextlib import AsyncExitStack
+from functools import partial
 from inspect import isawaitable
 from logging import Logger, getLogger
 from pathlib import Path
 from typing import AsyncIterator, Awaitable, Callable, cast
 
-import aiosqlite
 import anyio
 from anyio import TASK_STATUS_IGNORED, Event, Lock, create_task_group
 from anyio.abc import TaskGroup, TaskStatus
 from pycrdt import Doc
+from sqlite_anyio import Connection, connect
 
 from .yutils import Decoder, get_new_path, write_var_uint
 
 
 class YDocNotFound(Exception):
     pass
 
 
 class BaseYStore(ABC):
     metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None
     version = 2
     _started: Event | None = None
-    _starting: bool = False
     _task_group: TaskGroup | None = None
+    __start_lock: Lock | None = None
 
     @abstractmethod
     def __init__(
         self, path: str, metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None
-    ):
-        ...
+    ): ...
 
     @abstractmethod
-    async def write(self, data: bytes) -> None:
-        ...
+    async def write(self, data: bytes) -> None: ...
 
     @abstractmethod
     async def read(self) -> AsyncIterator[tuple[bytes, bytes, float]]:
         if False:
             yield
 
     @property
     def started(self) -> Event:
         if self._started is None:
             self._started = Event()
         return self._started
 
-    async def __aenter__(self) -> BaseYStore:
-        if self._task_group is not None:
-            raise RuntimeError("YStore already running")
+    @property
+    def _start_lock(self) -> Lock:
+        if self.__start_lock is None:
+            self.__start_lock = Lock()
+        return self.__start_lock
 
-        async with AsyncExitStack() as exit_stack:
-            tg = create_task_group()
-            self._task_group = await exit_stack.enter_async_context(tg)
-            self._exit_stack = exit_stack.pop_all()
-            tg.start_soon(self.start)
+    async def __aenter__(self) -> BaseYStore:
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("YStore already running")
+
+            async with AsyncExitStack() as exit_stack:
+                tg = create_task_group()
+                self._task_group = await exit_stack.enter_async_context(tg)
+                self._exit_stack = exit_stack.pop_all()
+                await tg.start(partial(self.start, from_context_manager=True))
 
         return self
 
     async def __aexit__(self, exc_type, exc_value, exc_tb):
-        if self._task_group is None:
-            raise RuntimeError("YStore not running")
-
-        self._task_group.cancel_scope.cancel()
-        self._task_group = None
+        await self.stop()
         return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
 
-    async def start(self, *, task_status: TaskStatus[None] = TASK_STATUS_IGNORED):
+    async def start(
+        self,
+        *,
+        task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
+        from_context_manager: bool = False,
+    ):
         """Start the store.
 
         Arguments:
             task_status: The status to set when the task has started.
         """
-        if self._starting:
+        if from_context_manager:
+            task_status.started()
+            self.started.set()
             return
-        else:
-            self._starting = True
-
-        if self._task_group is not None:
-            raise RuntimeError("YStore already running")
 
-        self.started.set()
-        self._starting = False
-        task_status.started()
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("YStore already running")
+
+            async with create_task_group() as self._task_group:
+                task_status.started()
+                self.started.set()
 
-    def stop(self) -> None:
+    async def stop(self) -> None:
         """Stop the store."""
         if self._task_group is None:
             raise RuntimeError("YStore not running")
 
         self._task_group.cancel_scope.cancel()
         self._task_group = None
 
@@ -298,14 +306,15 @@
     # Determines the "time to live" for all documents, i.e. how recent the
     # latest update of a document must be before purging document history.
     # Defaults to never purging document history (None).
     document_ttl: int | None = None
     path: str
     lock: Lock
     db_initialized: Event
+    _db: Connection
 
     def __init__(
         self,
         path: str,
         metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None,
         log: Logger | None = None,
     ) -> None:
@@ -318,132 +327,148 @@
         """
         self.path = path
         self.metadata_callback = metadata_callback
         self.log = log or getLogger(__name__)
         self.lock = Lock()
         self.db_initialized = Event()
 
-    async def start(self, *, task_status: TaskStatus[None] = TASK_STATUS_IGNORED):
+    async def start(
+        self,
+        *,
+        task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
+        from_context_manager: bool = False,
+    ):
         """Start the SQLiteYStore.
 
         Arguments:
             task_status: The status to set when the task has started.
         """
-        if self._starting:
-            return
-        else:
-            self._starting = True
 
-        if self._task_group is not None:
-            raise RuntimeError("YStore already running")
-
-        async with create_task_group() as self._task_group:
+        self.db_initialized = Event()
+        if from_context_manager:
+            assert self._task_group is not None
             self._task_group.start_soon(self._init_db)
-            self.started.set()
-            self._starting = False
             task_status.started()
+            self.started.set()
+            return
+
+        async with self._start_lock:
+            if self._task_group is not None:
+                raise RuntimeError("YStore already running")
+            async with create_task_group() as self._task_group:
+                self._task_group.start_soon(self._init_db)
+                task_status.started()
+                self.started.set()
+
+    async def stop(self) -> None:
+        """Stop the store."""
+        if self.db_initialized.is_set():
+            await self._db.close()
+        await super().stop()
 
     async def _init_db(self):
         create_db = False
         move_db = False
         if not await anyio.Path(self.db_path).exists():
             create_db = True
         else:
             async with self.lock:
-                async with aiosqlite.connect(self.db_path) as db:
-                    cursor = await db.execute(
-                        "SELECT count(name) FROM sqlite_master "
-                        "WHERE type='table' and name='yupdates'"
-                    )
-                    table_exists = (await cursor.fetchone())[0]
-                    if table_exists:
-                        cursor = await db.execute("pragma user_version")
-                        version = (await cursor.fetchone())[0]
-                        if version != self.version:
-                            move_db = True
-                            create_db = True
-                    else:
+                db = await connect(self.db_path)
+                cursor = await db.cursor()
+                await cursor.execute(
+                    "SELECT count(name) FROM sqlite_master "
+                    "WHERE type='table' and name='yupdates'"
+                )
+                table_exists = (await cursor.fetchone())[0]
+                if table_exists:
+                    await cursor.execute("pragma user_version")
+                    version = (await cursor.fetchone())[0]
+                    if version != self.version:
+                        move_db = True
                         create_db = True
+                else:
+                    create_db = True
+                await db.close()
         if move_db:
             new_path = await get_new_path(self.db_path)
             self.log.warning("YStore version mismatch, moving %s to %s", self.db_path, new_path)
             await anyio.Path(self.db_path).rename(new_path)
         if create_db:
             async with self.lock:
-                async with aiosqlite.connect(self.db_path) as db:
-                    await db.execute(
-                        "CREATE TABLE yupdates (path TEXT NOT NULL, yupdate BLOB, "
-                        "metadata BLOB, timestamp REAL NOT NULL)"
-                    )
-                    await db.execute(
-                        "CREATE INDEX idx_yupdates_path_timestamp ON yupdates (path, timestamp)"
-                    )
-                    await db.execute(f"PRAGMA user_version = {self.version}")
-                    await db.commit()
+                db = await connect(self.db_path)
+                cursor = await db.cursor()
+                await cursor.execute(
+                    "CREATE TABLE yupdates (path TEXT NOT NULL, yupdate BLOB, "
+                    "metadata BLOB, timestamp REAL NOT NULL)"
+                )
+                await cursor.execute(
+                    "CREATE INDEX idx_yupdates_path_timestamp ON yupdates (path, timestamp)"
+                )
+                await cursor.execute(f"PRAGMA user_version = {self.version}")
+                await db.commit()
+                await db.close()
+        self._db = await connect(self.db_path)
         self.db_initialized.set()
 
     async def read(self) -> AsyncIterator[tuple[bytes, bytes, float]]:
         """Async iterator for reading the store content.
 
         Returns:
             A tuple of (update, metadata, timestamp) for each update.
         """
         await self.db_initialized.wait()
         try:
             async with self.lock:
-                async with aiosqlite.connect(self.db_path) as db:
-                    async with db.execute(
-                        "SELECT yupdate, metadata, timestamp FROM yupdates WHERE path = ?",
-                        (self.path,),
-                    ) as cursor:
-                        found = False
-                        async for update, metadata, timestamp in cursor:
-                            found = True
-                            yield update, metadata, timestamp
-                        if not found:
-                            raise YDocNotFound
+                cursor = await self._db.cursor()
+                await cursor.execute(
+                    "SELECT yupdate, metadata, timestamp FROM yupdates WHERE path = ?",
+                    (self.path,),
+                )
+                found = False
+                for update, metadata, timestamp in await cursor.fetchall():
+                    found = True
+                    yield update, metadata, timestamp
+                if not found:
+                    raise YDocNotFound
         except Exception:
             raise YDocNotFound
 
     async def write(self, data: bytes) -> None:
         """Store an update.
 
         Arguments:
             data: The update to store.
         """
         await self.db_initialized.wait()
         async with self.lock:
-            async with aiosqlite.connect(self.db_path) as db:
-                # first, determine time elapsed since last update
-                cursor = await db.execute(
-                    "SELECT timestamp FROM yupdates WHERE path = ? "
-                    "ORDER BY timestamp DESC LIMIT 1",
-                    (self.path,),
-                )
-                row = await cursor.fetchone()
-                diff = (time.time() - row[0]) if row else 0
-
-                if self.document_ttl is not None and diff > self.document_ttl:
-                    # squash updates
-                    ydoc = Doc()
-                    async with db.execute(
-                        "SELECT yupdate FROM yupdates WHERE path = ?", (self.path,)
-                    ) as cursor:
-                        async for (update,) in cursor:
-                            ydoc.apply_update(update)
-                    # delete history
-                    await db.execute("DELETE FROM yupdates WHERE path = ?", (self.path,))
-                    # insert squashed updates
-                    squashed_update = ydoc.get_update()
-                    metadata = await self.get_metadata()
-                    await db.execute(
-                        "INSERT INTO yupdates VALUES (?, ?, ?, ?)",
-                        (self.path, squashed_update, metadata, time.time()),
-                    )
-
-                # finally, write this update to the DB
+            # first, determine time elapsed since last update
+            cursor = await self._db.cursor()
+            await cursor.execute(
+                "SELECT timestamp FROM yupdates WHERE path = ? ORDER BY timestamp DESC LIMIT 1",
+                (self.path,),
+            )
+            row = await cursor.fetchone()
+            diff = (time.time() - row[0]) if row else 0
+
+            if self.document_ttl is not None and diff > self.document_ttl:
+                # squash updates
+                ydoc = Doc()
+                await cursor.execute("SELECT yupdate FROM yupdates WHERE path = ?", (self.path,))
+                for (update,) in await cursor.fetchall():
+                    ydoc.apply_update(update)
+                # delete history
+                await cursor.execute("DELETE FROM yupdates WHERE path = ?", (self.path,))
+                # insert squashed updates
+                squashed_update = ydoc.get_update()
                 metadata = await self.get_metadata()
-                await db.execute(
+                await cursor.execute(
                     "INSERT INTO yupdates VALUES (?, ?, ?, ?)",
-                    (self.path, data, metadata, time.time()),
+                    (self.path, squashed_update, metadata, time.time()),
                 )
-                await db.commit()
+
+            # finally, write this update to the DB
+            metadata = await self.get_metadata()
+            await cursor.execute(
+                "INSERT INTO yupdates VALUES (?, ?, ?, ?)",
+                (self.path, data, metadata, time.time()),
+            )
+            await self._db.commit()
```

### Comparing `pycrdt_websocket-0.12.7/pycrdt_websocket/yutils.py` & `pycrdt_websocket-0.13.0/pycrdt_websocket/yutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,13 @@
 
 
 async def get_new_path(path: str) -> str:
     p = Path(path)
     ext = p.suffix
     p_noext = p.with_suffix("")
     i = 1
-    dir_list = [p async for p in anyio.Path().iterdir()]
     while True:
         new_path = f"{p_noext}({i}){ext}"
-        if new_path not in dir_list:
+        if not await anyio.Path(new_path).exists():
             break
         i += 1
-    return str(new_path)
+    return new_path
```

### Comparing `pycrdt_websocket-0.12.7/tests/test_ystore.py` & `pycrdt_websocket-0.13.0/tests/test_ystore.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,126 @@
-import os
 import tempfile
 import time
 from pathlib import Path
 from unittest.mock import patch
 
-import aiosqlite
 import pytest
+from anyio import create_task_group
+from sqlite_anyio import connect
+from utils import StartStopContextManager, YDocTest
 
 from pycrdt_websocket.ystore import SQLiteYStore, TempFileYStore
 
+pytestmark = pytest.mark.anyio
+
+MY_SQLITE_YSTORE_DB_PATH = str(Path(tempfile.mkdtemp(prefix="test_sql_")) / "ystore.db")
+
 
 class MetadataCallback:
     def __init__(self):
         self.i = 0
 
     async def __call__(self):
         res = str(self.i).encode()
         self.i += 1
         return res
 
 
 class MyTempFileYStore(TempFileYStore):
     prefix_dir = "test_temp_"
 
-
-MY_SQLITE_YSTORE_DB_PATH = str(Path(tempfile.mkdtemp(prefix="test_sql_")) / "ystore.db")
+    def __init__(self, *args, delete=False, **kwargs):
+        super().__init__(*args, **kwargs)
+        if delete:
+            Path(self.path).unlink(missing_ok=True)
 
 
 class MySQLiteYStore(SQLiteYStore):
     db_path = MY_SQLITE_YSTORE_DB_PATH
     document_ttl = 1000
 
-    def __init__(self, *args, delete_db=False, **kwargs):
-        if delete_db:
-            os.remove(self.db_path)
+    def __init__(self, *args, delete=False, **kwargs):
+        if delete:
+            Path(self.db_path).unlink(missing_ok=True)
         super().__init__(*args, **kwargs)
 
 
-@pytest.mark.anyio
 @pytest.mark.parametrize("YStore", (MyTempFileYStore, MySQLiteYStore))
-async def test_ystore(YStore):
-    store_name = "my_store"
-    ystore = YStore(store_name, metadata_callback=MetadataCallback())
-    await ystore.start()
-    data = [b"foo", b"bar", b"baz"]
-    for d in data:
-        await ystore.write(d)
-
-    if YStore == MyTempFileYStore:
-        assert (Path(MyTempFileYStore.base_dir) / store_name).exists()
-    elif YStore == MySQLiteYStore:
-        assert Path(MySQLiteYStore.db_path).exists()
-    i = 0
-    async for d, m, t in ystore.read():
-        assert d == data[i]  # data
-        assert m == str(i).encode()  # metadata
-        i += 1
-
-    assert i == len(data)
-
-
-@pytest.mark.anyio
-async def test_document_ttl_sqlite_ystore(test_ydoc):
-    store_name = "my_store"
-    ystore = MySQLiteYStore(store_name, delete_db=True)
-    await ystore.start()
-    now = time.time()
-
-    for i in range(3):
-        # assert that adding a record before document TTL doesn't delete document history
-        with patch("time.time") as mock_time:
-            mock_time.return_value = now
-            await ystore.write(test_ydoc.update())
-            async with aiosqlite.connect(ystore.db_path) as db:
-                assert (await (await db.execute("SELECT count(*) FROM yupdates")).fetchone())[
+@pytest.mark.parametrize("ystore_api", ("ystore_context_manager", "ystore_start_stop"))
+async def test_ystore(YStore, ystore_api):
+    async with create_task_group() as tg:
+        store_name = f"my_store_with_api_{ystore_api}"
+        ystore = YStore(store_name, metadata_callback=MetadataCallback(), delete=True)
+        if ystore_api == "ystore_start_stop":
+            ystore = StartStopContextManager(ystore, tg)
+
+        async with ystore as ystore:
+            data = [b"foo", b"bar", b"baz"]
+            for d in data:
+                await ystore.write(d)
+
+            if YStore == MyTempFileYStore:
+                assert (Path(MyTempFileYStore.base_dir) / store_name).exists()
+            elif YStore == MySQLiteYStore:
+                assert Path(MySQLiteYStore.db_path).exists()
+            i = 0
+            async for d, m, t in ystore.read():
+                assert d == data[i]  # data
+                assert m == str(i).encode()  # metadata
+                i += 1
+
+            assert i == len(data)
+
+
+@pytest.mark.parametrize("ystore_api", ("ystore_context_manager", "ystore_start_stop"))
+async def test_document_ttl_sqlite_ystore(ystore_api):
+    async with create_task_group() as tg:
+        test_ydoc = YDocTest()
+        store_name = f"my_store_with_api_{ystore_api}"
+        ystore = MySQLiteYStore(store_name, delete=True)
+        if ystore_api == "ystore_start_stop":
+            ystore = StartStopContextManager(ystore, tg)
+
+        async with ystore as ystore:
+            now = time.time()
+            db = await connect(ystore.db_path)
+            cursor = await db.cursor()
+
+            for i in range(3):
+                # assert that adding a record before document TTL doesn't delete document history
+                with patch("time.time") as mock_time:
+                    mock_time.return_value = now
+                    await ystore.write(test_ydoc.update())
+                    assert (
+                        await (await cursor.execute("SELECT count(*) FROM yupdates")).fetchone()
+                    )[0] == i + 1
+
+            # assert that adding a record after document TTL deletes previous document history
+            with patch("time.time") as mock_time:
+                mock_time.return_value = now + ystore.document_ttl + 1
+                await ystore.write(test_ydoc.update())
+                # two updates in DB: one squashed update and the new update
+                assert (await (await cursor.execute("SELECT count(*) FROM yupdates")).fetchone())[
                     0
-                ] == i + 1
+                ] == 2
 
-    # assert that adding a record after document TTL deletes previous document history
-    with patch("time.time") as mock_time:
-        mock_time.return_value = now + ystore.document_ttl + 1
-        await ystore.write(test_ydoc.update())
-        async with aiosqlite.connect(ystore.db_path) as db:
-            # two updates in DB: one squashed update and the new update
-            assert (await (await db.execute("SELECT count(*) FROM yupdates")).fetchone())[0] == 2
+            await db.close()
 
 
-@pytest.mark.anyio
 @pytest.mark.parametrize("YStore", (MyTempFileYStore, MySQLiteYStore))
-async def test_version(YStore, caplog):
-    store_name = "my_store"
-    prev_version = YStore.version
-    YStore.version = -1
-    ystore = YStore(store_name)
-    await ystore.start()
-    await ystore.write(b"foo")
-    YStore.version = prev_version
-    assert "YStore version mismatch" in caplog.text
+@pytest.mark.parametrize("ystore_api", ("ystore_context_manager", "ystore_start_stop"))
+async def test_version(YStore, ystore_api, caplog):
+    async with create_task_group() as tg:
+        store_name = f"my_store_with_api_{ystore_api}"
+        prev_version = YStore.version
+        YStore.version = -1
+        ystore = YStore(store_name)
+        if ystore_api == "ystore_start_stop":
+            ystore = StartStopContextManager(ystore, tg)
+
+        async with ystore as ystore:
+            await ystore.write(b"foo")
+            assert "YStore version mismatch" in caplog.text
+
+        YStore.version = prev_version
+        async with ystore as ystore:
+            await ystore.write(b"bar")
```

### Comparing `pycrdt_websocket-0.12.7/.gitignore` & `pycrdt_websocket-0.13.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.12.7/LICENSE` & `pycrdt_websocket-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.12.7/README.md` & `pycrdt_websocket-0.13.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Pycrdt-websocket
 
-⚠️ This project is still in an **incubating** phase (i.e. it's not ready for production yet) ⚠️
-
 Pycrdt-websocket is an async WebSocket connector for pycrdt.
 
 [![Build Status](https://github.com/jupyter-server/pycrdt-websocket/workflows/CI/badge.svg)](https://github.com/jupyter-server/pycrdt-websocket/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
-**Documentation**: <a href="https://davidbrochart.github.io/pycrdt-websocket" target="_blank">https://davidbrochart.github.io/pycrdt-websocket</a>
+**Documentation**: <a href="https://jupyter-server.github.io/pycrdt-websocket" target="_blank">https://jupyter-server.github.io/pycrdt-websocket</a>
 
 **Source Code**: <a href="https://github.com/jupyter-server/pycrdt-websocket" target="_blank">https://github.com/jupyter-server/pycrdt-websocket</a>
 
 ---
 
 Pycrdt-websocket is a Python library for building WebSocket servers and clients that connect and synchronize shared documents.
 It can be used to create collaborative web applications.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-# Pycrdt-websocket â ï¸ This project is still in an **incubating** phase
-(i.e. it's not ready for production yet) â ï¸ Pycrdt-websocket is an async
-WebSocket connector for pycrdt. [![Build Status](https://github.com/jupyter-
-server/pycrdt-websocket/workflows/CI/badge.svg)](https://github.com/jupyter-
-server/pycrdt-websocket/actions) [![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg)](https://github.com/psf/black) --
-- **Documentation**: _h_t_t_p_s_:_/_/_d_a_v_i_d_b_r_o_c_h_a_r_t_._g_i_t_h_u_b_._i_o_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t **Source
-Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_j_u_p_y_t_e_r_-_s_e_r_v_e_r_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t --- Pycrdt-websocket
-is a Python library for building WebSocket servers and clients that connect and
-synchronize shared documents. It can be used to create collaborative web
-applications. The following diagram illustrates a typical architecture. The
-goal is to share a document among several clients. Each client has an instance
-of a `Doc`, representing their view of a document. A shared document also lives
-in a [room](./reference/Room.md) on the server side. Conceptually, a room can
-be seen as the place where clients collaborate on a document. The WebSocket to
-which a client connects points to the corresponding room through the endpoint
-path. In the example below, clients A and B connect to a WebSocket at path
-`room-1`, and thus both clients find themselves in a room called `room-1`. All
-the `Doc` synchronization logic is taken care of by the [WebsocketProvider](./
-reference/WebSocket_provider.md). Each update to a shared document can be
-persisted to disk using a [store](./reference/Store.md), which can be a file or
-a database. ```mermaid flowchart TD classDef room1 fill:#f96 classDef room2
-fill:#bbf A[Client A
+# Pycrdt-websocket Pycrdt-websocket is an async WebSocket connector for pycrdt.
+[![Build Status](https://github.com/jupyter-server/pycrdt-websocket/workflows/
+CI/badge.svg)](https://github.com/jupyter-server/pycrdt-websocket/actions) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) --- **Documentation**: _h_t_t_p_s_:_/_/
+_j_u_p_y_t_e_r_-_s_e_r_v_e_r_._g_i_t_h_u_b_._i_o_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_j_u_p_y_t_e_r_-_s_e_r_v_e_r_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t --- Pycrdt-websocket is a Python library for
+building WebSocket servers and clients that connect and synchronize shared
+documents. It can be used to create collaborative web applications. The
+following diagram illustrates a typical architecture. The goal is to share a
+document among several clients. Each client has an instance of a `Doc`,
+representing their view of a document. A shared document also lives in a [room]
+(./reference/Room.md) on the server side. Conceptually, a room can be seen as
+the place where clients collaborate on a document. The WebSocket to which a
+client connects points to the corresponding room through the endpoint path. In
+the example below, clients A and B connect to a WebSocket at path `room-1`, and
+thus both clients find themselves in a room called `room-1`. All the `Doc`
+synchronization logic is taken care of by the [WebsocketProvider](./reference/
+WebSocket_provider.md). Each update to a shared document can be persisted to
+disk using a [store](./reference/Store.md), which can be a file or a database.
+```mermaid flowchart TD classDef room1 fill:#f96 classDef room2 fill:#bbf A
+[Client A
 room-1]:::room1 <-->|WebSocket
 Provider| server(WebSocket Server) B[Client B
 room-1]:::room1 <-->|WebSocket
 Provider| server C[Client C
 room-2]:::room2 <-->|WebSocket
 Provider| server D[Client D
 room-2]:::room2 <-->|WebSocket
```

### Comparing `pycrdt_websocket-0.12.7/pyproject.toml` & `pycrdt_websocket-0.13.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,27 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "anyio >=3.6.2,<5",
-    "aiosqlite >=0.18.0,<1",
-    "pycrdt >=0.8.7,<0.9.0",
+    "sqlite-anyio >=0.2.0,<0.3.0",
+    "pycrdt >=0.8.16,<0.9.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "mypy",
     "pre-commit",
     "pytest",
-    "pytest-asyncio",
-    "websockets >=10.0",
-    "uvicorn",
+    "httpx-ws >=0.5.2",
+    "hypercorn >=0.16.0",
+    "trio >=0.25.0",
+    "sniffio",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings-python",
 ]
 django = [
@@ -64,15 +65,15 @@
 include = [
     "/pycrdt_websocket",
     "/tests",
 ]
 
 [tool.ruff]
 line-length = 99
-select = [
+lint.select = [
     "ASYNC",        # flake8-async
     "E", "F", "W",  # default Flake8
     "G",            # flake8-logging-format
     "I",            # isort
     "ISC",          # flake8-implicit-str-concat
     "PGH",          # pygrep-hooks
     "RUF100",       # unused noqa (yesqa)
```

### Comparing `pycrdt_websocket-0.12.7/PKG-INFO` & `pycrdt_websocket-0.13.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pycrdt-websocket
-Version: 0.12.7
+Version: 0.13.0
 Summary: WebSocket connector for pycrdt
 Project-URL: Homepage, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Source, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Issues, https://github.com/jupyter-server/pycrdt-websocket/issues
 Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT License
@@ -36,44 +36,43 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: aiosqlite<1,>=0.18.0
 Requires-Dist: anyio<5,>=3.6.2
-Requires-Dist: pycrdt<0.9.0,>=0.8.7
+Requires-Dist: pycrdt<0.9.0,>=0.8.16
+Requires-Dist: sqlite-anyio<0.3.0,>=0.2.0
 Provides-Extra: django
 Requires-Dist: channels; extra == 'django'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: test
+Requires-Dist: httpx-ws>=0.5.2; extra == 'test'
+Requires-Dist: hypercorn>=0.16.0; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-asyncio; extra == 'test'
-Requires-Dist: uvicorn; extra == 'test'
-Requires-Dist: websockets>=10.0; extra == 'test'
+Requires-Dist: sniffio; extra == 'test'
+Requires-Dist: trio>=0.25.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Pycrdt-websocket
 
-⚠️ This project is still in an **incubating** phase (i.e. it's not ready for production yet) ⚠️
-
 Pycrdt-websocket is an async WebSocket connector for pycrdt.
 
 [![Build Status](https://github.com/jupyter-server/pycrdt-websocket/workflows/CI/badge.svg)](https://github.com/jupyter-server/pycrdt-websocket/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
-**Documentation**: <a href="https://davidbrochart.github.io/pycrdt-websocket" target="_blank">https://davidbrochart.github.io/pycrdt-websocket</a>
+**Documentation**: <a href="https://jupyter-server.github.io/pycrdt-websocket" target="_blank">https://jupyter-server.github.io/pycrdt-websocket</a>
 
 **Source Code**: <a href="https://github.com/jupyter-server/pycrdt-websocket" target="_blank">https://github.com/jupyter-server/pycrdt-websocket</a>
 
 ---
 
 Pycrdt-websocket is a Python library for building WebSocket servers and clients that connect and synchronize shared documents.
 It can be used to create collaborative web applications.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycrdt-websocket Version: 0.12.7 Summary: WebSocket
+Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.0 Summary: WebSocket
 connector for pycrdt Project-URL: Homepage, https://github.com/jupyter-server/
 pycrdt-websocket Project-URL: Source, https://github.com/jupyter-server/pycrdt-
 websocket Project-URL: Issues, https://github.com/jupyter-server/pycrdt-
 websocket/issues Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart
 gmail.com> License: MIT License Copyright (c) 2022 David Brochart Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
@@ -21,46 +21,45 @@
 DEALINGS IN THE SOFTWARE. License-File: LICENSE Keywords: websocket,yjs
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
-Requires-Dist: aiosqlite<1,>=0.18.0 Requires-Dist: anyio<5,>=3.6.2 Requires-
-Dist: pycrdt<0.9.0,>=0.8.7 Provides-Extra: django Requires-Dist: channels;
-extra == 'django' Provides-Extra: docs Requires-Dist: mkdocs; extra == 'docs'
-Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist: mkdocstrings-
-python; extra == 'docs' Provides-Extra: test Requires-Dist: mypy; extra ==
-'test' Requires-Dist: pre-commit; extra == 'test' Requires-Dist: pytest; extra
-== 'test' Requires-Dist: pytest-asyncio; extra == 'test' Requires-Dist:
-uvicorn; extra == 'test' Requires-Dist: websockets>=10.0; extra == 'test'
-Description-Content-Type: text/markdown # Pycrdt-websocket â ï¸ This project
-is still in an **incubating** phase (i.e. it's not ready for production yet)
-â ï¸ Pycrdt-websocket is an async WebSocket connector for pycrdt. [![Build
-Status](https://github.com/jupyter-server/pycrdt-websocket/workflows/CI/
-badge.svg)](https://github.com/jupyter-server/pycrdt-websocket/actions) [![Code
-style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
-(https://github.com/psf/black) --- **Documentation**: _h_t_t_p_s_:_/_/
-_d_a_v_i_d_b_r_o_c_h_a_r_t_._g_i_t_h_u_b_._i_o_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_j_u_p_y_t_e_r_-_s_e_r_v_e_r_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t --- Pycrdt-websocket is a Python library for
-building WebSocket servers and clients that connect and synchronize shared
-documents. It can be used to create collaborative web applications. The
-following diagram illustrates a typical architecture. The goal is to share a
-document among several clients. Each client has an instance of a `Doc`,
-representing their view of a document. A shared document also lives in a [room]
-(./reference/Room.md) on the server side. Conceptually, a room can be seen as
-the place where clients collaborate on a document. The WebSocket to which a
-client connects points to the corresponding room through the endpoint path. In
-the example below, clients A and B connect to a WebSocket at path `room-1`, and
-thus both clients find themselves in a room called `room-1`. All the `Doc`
-synchronization logic is taken care of by the [WebsocketProvider](./reference/
-WebSocket_provider.md). Each update to a shared document can be persisted to
-disk using a [store](./reference/Store.md), which can be a file or a database.
-```mermaid flowchart TD classDef room1 fill:#f96 classDef room2 fill:#bbf A
-[Client A
+Requires-Dist: anyio<5,>=3.6.2 Requires-Dist: pycrdt<0.9.0,>=0.8.16 Requires-
+Dist: sqlite-anyio<0.3.0,>=0.2.0 Provides-Extra: django Requires-Dist:
+channels; extra == 'django' Provides-Extra: docs Requires-Dist: mkdocs; extra
+== 'docs' Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist:
+mkdocstrings-python; extra == 'docs' Provides-Extra: test Requires-Dist: httpx-
+ws>=0.5.2; extra == 'test' Requires-Dist: hypercorn>=0.16.0; extra == 'test'
+Requires-Dist: mypy; extra == 'test' Requires-Dist: pre-commit; extra == 'test'
+Requires-Dist: pytest; extra == 'test' Requires-Dist: sniffio; extra == 'test'
+Requires-Dist: trio>=0.25.0; extra == 'test' Description-Content-Type: text/
+markdown # Pycrdt-websocket Pycrdt-websocket is an async WebSocket connector
+for pycrdt. [![Build Status](https://github.com/jupyter-server/pycrdt-
+websocket/workflows/CI/badge.svg)](https://github.com/jupyter-server/pycrdt-
+websocket/actions) [![Code style: black](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black) --
+- **Documentation**: _h_t_t_p_s_:_/_/_j_u_p_y_t_e_r_-_s_e_r_v_e_r_._g_i_t_h_u_b_._i_o_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t **Source
+Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_j_u_p_y_t_e_r_-_s_e_r_v_e_r_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t --- Pycrdt-websocket
+is a Python library for building WebSocket servers and clients that connect and
+synchronize shared documents. It can be used to create collaborative web
+applications. The following diagram illustrates a typical architecture. The
+goal is to share a document among several clients. Each client has an instance
+of a `Doc`, representing their view of a document. A shared document also lives
+in a [room](./reference/Room.md) on the server side. Conceptually, a room can
+be seen as the place where clients collaborate on a document. The WebSocket to
+which a client connects points to the corresponding room through the endpoint
+path. In the example below, clients A and B connect to a WebSocket at path
+`room-1`, and thus both clients find themselves in a room called `room-1`. All
+the `Doc` synchronization logic is taken care of by the [WebsocketProvider](./
+reference/WebSocket_provider.md). Each update to a shared document can be
+persisted to disk using a [store](./reference/Store.md), which can be a file or
+a database. ```mermaid flowchart TD classDef room1 fill:#f96 classDef room2
+fill:#bbf A[Client A
 room-1]:::room1 <-->|WebSocket
 Provider| server(WebSocket Server) B[Client B
 room-1]:::room1 <-->|WebSocket
 Provider| server C[Client C
 room-2]:::room2 <-->|WebSocket
 Provider| server D[Client D
 room-2]:::room2 <-->|WebSocket
```


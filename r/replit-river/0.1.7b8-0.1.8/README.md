# Comparing `tmp/replit_river-0.1.7b8.tar.gz` & `tmp/replit_river-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.7b8.tar", max compression
+gzip compressed data, was "replit_river-0.1.8.tar", max compression
```

## Comparing `replit_river-0.1.7b8.tar` & `replit_river-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.7b8/LICENSE
--rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.7b8/README.md
--rw-r--r--   0        0        0     1749 2024-04-23 07:05:04.134001 replit_river-0.1.7b8/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.7b8/replit_river/__init__.py
--rw-r--r--   0        0        0     3860 2024-04-23 06:16:02.995607 replit_river-0.1.7b8/replit_river/client.py
--rw-r--r--   0        0        0    11280 2024-04-23 06:23:37.760393 replit_river-0.1.7b8/replit_river/client_session.py
--rw-r--r--   0        0        0     9848 2024-04-23 05:32:53.039645 replit_river-0.1.7b8/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.7b8/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.7b8/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.7b8/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.7b8/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5356 2024-04-23 00:45:40.473122 replit_river-0.1.7b8/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12624 2024-04-23 00:45:40.507714 replit_river-0.1.7b8/replit_river/codegen/server.py
--rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.7b8/replit_river/error_schema.py
--rw-r--r--   0        0        0        1 2024-04-22 19:50:44.357856 replit_river-0.1.7b8/replit_river/handshake.py
--rw-r--r--   0        0        0     1302 2024-04-23 06:42:16.393507 replit_river-0.1.7b8/replit_river/message_buffer.py
--rw-r--r--   0        0        0     2615 2024-04-23 05:36:58.812225 replit_river-0.1.7b8/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.7b8/replit_river/py.typed
--rw-r--r--   0        0        0     1827 2024-04-23 00:45:40.911579 replit_river-0.1.7b8/replit_river/rate_limiter.py
--rw-r--r--   0        0        0    12218 2024-04-22 19:50:44.358789 replit_river-0.1.7b8/replit_river/rpc.py
--rw-r--r--   0        0        0     2331 2024-04-23 07:04:46.123408 replit_river-0.1.7b8/replit_river/seq_manager.py
--rw-r--r--   0        0        0     2260 2024-04-23 05:03:13.892136 replit_river-0.1.7b8/replit_river/server.py
--rw-r--r--   0        0        0     7436 2024-04-23 06:23:37.760716 replit_river-0.1.7b8/replit_river/server_transport.py
--rw-r--r--   0        0        0    19701 2024-04-23 06:45:02.888697 replit_river-0.1.7b8/replit_river/session.py
--rw-r--r--   0        0        0     2336 2024-04-22 19:50:44.360278 replit_river-0.1.7b8/replit_river/task_manager.py
--rw-r--r--   0        0        0     1473 2024-04-23 01:20:15.732925 replit_river-0.1.7b8/replit_river/transport.py
--rw-r--r--   0        0        0     1432 2024-04-23 06:23:37.761014 replit_river-0.1.7b8/replit_river/transport_options.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.8/README.md
+-rw-r--r--   0        0        0     1742 2024-04-24 23:36:50.745203 replit_river-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.8/replit_river/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-24 23:10:35.786501 replit_river-0.1.8/replit_river/client.py
+-rw-r--r--   0        0        0    10717 2024-04-24 23:52:30.740117 replit_river-0.1.8/replit_river/client_session.py
+-rw-r--r--   0        0        0    12323 2024-04-24 23:49:21.694200 replit_river-0.1.8/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.8/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.8/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.8/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.8/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5354 2024-04-24 23:49:28.777220 replit_river-0.1.8/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12620 2024-04-24 23:49:28.805274 replit_river-0.1.8/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.8/replit_river/error_schema.py
+-rw-r--r--   0        0        0     1482 2024-04-24 23:40:20.838560 replit_river-0.1.8/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     2606 2024-04-24 22:30:56.712779 replit_river-0.1.8/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.8/replit_river/py.typed
+-rw-r--r--   0        0        0     3565 2024-04-24 23:49:26.772845 replit_river-0.1.8/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    12635 2024-04-24 23:47:43.465686 replit_river-0.1.8/replit_river/rpc.py
+-rw-r--r--   0        0        0     2293 2024-04-24 23:14:37.024811 replit_river-0.1.8/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2294 2024-04-24 23:09:28.482659 replit_river-0.1.8/replit_river/server.py
+-rw-r--r--   0        0        0     5916 2024-04-24 23:47:43.421824 replit_river-0.1.8/replit_river/server_transport.py
+-rw-r--r--   0        0        0    20444 2024-04-24 23:43:54.064753 replit_river-0.1.8/replit_river/session.py
+-rw-r--r--   0        0        0     3833 2024-04-24 23:37:26.072767 replit_river-0.1.8/replit_river/task_manager.py
+-rw-r--r--   0        0        0     5524 2024-04-24 23:48:34.430006 replit_river-0.1.8/replit_river/transport.py
+-rw-r--r--   0        0        0     1610 2024-04-24 23:39:46.272366 replit_river-0.1.8/replit_river/transport_options.py
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 replit_river-0.1.8/PKG-INFO
```

### Comparing `replit_river-0.1.7b8/LICENSE` & `replit_river-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b8/README.md` & `replit_river-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b8/pyproject.toml` & `replit_river-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.7-beta.8"
+version="0.1.8"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.7b8/replit_river/client.py` & `replit_river-0.1.8/replit_river/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             client_id=client_id,
             server_id=server_id,
             transport_options=transport_options,
         )
 
     async def close(self) -> None:
         logging.info(f"river client {self._client_id} start closing")
-        await self._transport.close_all_sessions()
+        await self._transport.close()
         logging.info(f"river client {self._client_id} closed")
 
     async def send_rpc(
         self,
         service_name: str,
         procedure_name: str,
         request: RequestType,
```

### Comparing `replit_river-0.1.7b8/replit_river/client_session.py` & `replit_river-0.1.8/replit_river/client_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import nanoid  # type: ignore
 from aiochannel import Channel
 from aiochannel.errors import ChannelClosed
 
 from replit_river.error_schema import ERROR_CODE_STREAM_CLOSED, RiverException
 from replit_river.session import Session
+from replit_river.transport_options import MAX_MESSAGE_BUFFER_SIZE
 
 from .rpc import (
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     ErrorType,
     InitType,
     RequestType,
@@ -44,32 +45,30 @@
             service_name=service_name,
             procedure_name=procedure_name,
         )
         # Handle potential errors during communication
         try:
             try:
                 response = await output.get()
-            except (RuntimeError, ChannelClosed) as e:
-                # if the stream is closed before we get a response, we will get a
-                # RuntimeError: RuntimeError: Event loop is closed
+            except ChannelClosed as e:
                 raise RiverException(
                     ERROR_CODE_STREAM_CLOSED, f"Stream closed before response {e}"
                 )
+            except RuntimeError as e:
+                raise RiverException(ERROR_CODE_STREAM_CLOSED, str(e))
             if not response.get("ok", False):
                 try:
                     error = error_deserializer(response["payload"])
                 except Exception as e:
                     raise RiverException("error_deserializer", str(e))
                 raise RiverException(error.code, error.message)
             return response_deserializer(response["payload"])
         except RiverException as e:
             raise e
         except Exception as e:
-            # Log the error and return an appropriate error response
-            logging.exception("Error during RPC communication")
             raise e
 
     async def send_upload(
         self,
         service_name: str,
         procedure_name: str,
         init: Optional[InitType],
@@ -96,15 +95,15 @@
                     control_flags=STREAM_OPEN_BIT,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     payload=init_serializer(init),
                 )
                 first_message = False
             # If this request is not closed and the session is killed, we should
-            # throws exception here
+            # throw exception here
             async for item in request:
                 control_flags = 0
                 if first_message:
                     control_flags = STREAM_OPEN_BIT
                     first_message = False
                 await self.send_message(
                     stream_id=stream_id,
@@ -119,33 +118,31 @@
         await self.send_close_stream(service_name, procedure_name, stream_id)
 
         # Handle potential errors during communication
         # TODO: throw a error when the transport is hard closed
         try:
             try:
                 response = await output.get()
-            except (RuntimeError, ChannelClosed):
-                # if the stream is closed before we get a response, we will get a
-                # RuntimeError: RuntimeError: Event loop is closed
+            except ChannelClosed:
                 raise RiverException(
                     ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
                 )
+            except RuntimeError as e:
+                raise RiverException(ERROR_CODE_STREAM_CLOSED, str(e))
             if not response.get("ok", False):
                 try:
                     error = error_deserializer(response["payload"])
                 except Exception as e:
                     raise RiverException("error_deserializer", str(e))
                 raise RiverException(error.code, error.message)
 
             return response_deserializer(response["payload"])
         except RiverException as e:
             raise e
         except Exception as e:
-            # Log the error and return an appropriate error response
-            logging.exception("Error during upload communication")
             raise e
 
     async def send_subscription(
         self,
         service_name: str,
         procedure_name: str,
         request: RequestType,
@@ -154,15 +151,15 @@
         error_deserializer: Callable[[Any], ErrorType],
     ) -> AsyncIterator[Union[ResponseType, ErrorType]]:
         """Sends a subscription request to the server.
 
         Expects the input and output be messages that will be msgpacked.
         """
         stream_id = nanoid.generate()
-        output: Channel[Any] = Channel(1024)
+        output: Channel[Any] = Channel(MAX_MESSAGE_BUFFER_SIZE)
         self._streams[stream_id] = output
         await self.send_message(
             ws=self._ws,
             service_name=service_name,
             procedure_name=procedure_name,
             stream_id=stream_id,
             control_flags=STREAM_OPEN_BIT,
@@ -184,16 +181,14 @@
                     continue
                 yield response_deserializer(item["payload"])
         except (RuntimeError, ChannelClosed):
             raise RiverException(
                 ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
         except Exception as e:
-            # Log the error and yield an appropriate error response
-            logging.exception(f"Error during subscription communication : {item}")
             raise e
 
     async def send_stream(
         self,
         service_name: str,
         procedure_name: str,
         init: Optional[InitType],
@@ -205,15 +200,15 @@
     ) -> AsyncIterator[Union[ResponseType, ErrorType]]:
         """Sends a subscription request to the server.
 
         Expects the input and output be messages that will be msgpacked.
         """
 
         stream_id = nanoid.generate()
-        output: Channel[Any] = Channel(1024)
+        output: Channel[Any] = Channel(MAX_MESSAGE_BUFFER_SIZE)
         self._streams[stream_id] = output
         try:
             if init and init_serializer:
                 await self.send_message(
                     ws=self._ws,
                     service_name=service_name,
                     procedure_name=procedure_name,
@@ -269,16 +264,14 @@
                     continue
                 yield response_deserializer(item["payload"])
         except (RuntimeError, ChannelClosed):
             raise RiverException(
                 ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
         except Exception as e:
-            # Log the error and yield an appropriate error response
-            logging.exception("Error during stream communication")
             raise e
 
     async def send_close_stream(
         self, service_name: str, procedure_name: str, stream_id: str
     ) -> None:
         # close stream
         await self.send_message(
```

### Comparing `replit_river-0.1.7b8/replit_river/client_transport.py` & `replit_river-0.1.8/replit_river/client_transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import logging
 from typing import Optional, Tuple
 
-import nanoid
 import websockets
 from pydantic import ValidationError
 from websockets import (
     WebSocketCommonProtocol,
 )
 from websockets.exceptions import ConnectionClosed
 
@@ -14,14 +13,15 @@
 from replit_river.error_schema import (
     ERROR_CODE_STREAM_CLOSED,
     ERROR_HANDSHAKE,
     ERROR_SESSION,
     RiverException,
 )
 from replit_river.messages import (
+    PROTOCOL_VERSION,
     FailedSendingMessageException,
     parse_transport_msg,
     send_transport_message,
 )
 from replit_river.rate_limiter import LeakyBucketRateLimit
 from replit_river.rpc import (
     ControlMessageHandshakeRequest,
@@ -29,15 +29,15 @@
     TransportMessage,
 )
 from replit_river.seq_manager import (
     IgnoreMessageException,
     InvalidMessageException,
 )
 from replit_river.session import Session
-from replit_river.transport import PROTOCOL_VERSION, Transport
+from replit_river.transport import Transport
 from replit_river.transport_options import TransportOptions
 
 
 class ClientTransport(Transport):
     def __init__(
         self,
         websocket_uri: str,
@@ -49,44 +49,38 @@
             transport_id=client_id,
             transport_options=transport_options,
             is_server=False,
         )
         self._websocket_uri = websocket_uri
         self._client_id = client_id
         self._server_id = server_id
-        self._instance_id = str(nanoid.generate())
         self._rate_limiter = LeakyBucketRateLimit(
             transport_options.connection_retry_options
         )
         # We want to make sure there's only one session creation at a time
         self._create_session_lock = asyncio.Lock()
         # Only one retry should happen at a time
         self._retry_ws_lock = asyncio.Lock()
 
     async def _on_session_closed(self, session: Session) -> None:
-        logging.info(f"Client session {session._instance_id} closed")
+        logging.info(f"Client session {session.advertised_session_id} closed")
         await self._delete_session(session)
 
-    async def _retry_session_connection(self, session_to_replace_ws: Session) -> None:
-        async with self._retry_ws_lock:
-            if await session_to_replace_ws.is_websocket_open():
-                # other retry successfully replaced the websocket,
-                return
-            if await session_to_replace_ws.is_session_open():
-                new_ws, hs_request, hs_response = await self._establish_new_connection()
-                await session_to_replace_ws.replace_with_new_websocket(new_ws)
+    async def close(self) -> None:
+        self._rate_limiter.close()
+        await self._close_all_sessions()
 
     async def _get_existing_session(self) -> Optional[ClientSession]:
         async with self._session_lock:
             if not self._sessions:
                 return None
             if len(self._sessions) > 1:
                 raise RiverException(
                     "session_error",
-                    "More than one session found in client, " + "should only be one",
+                    "More than one session found in client, should only be one",
                 )
             session = list(self._sessions.values())[0]
             if isinstance(session, ClientSession):
                 return session
             else:
                 raise RiverException(
                     "session_error", f"Client session type wrong, got {type(session)}"
@@ -98,88 +92,145 @@
         WebSocketCommonProtocol,
         ControlMessageHandshakeRequest,
         ControlMessageHandshakeResponse,
     ]:
         """Build a new websocket connection with retry logic."""
         rate_limit = self._rate_limiter
         max_retry = self._transport_options.connection_retry_options.max_retry
-        user_id = self._client_id
+        client_id = self._client_id
         for i in range(max_retry):
             if i > 0:
-                logging.info(f"Retrying build handshake {i} times")
-            if not rate_limit.has_budget(user_id):
-                logging.debug(
-                    f"No retry budget for {user_id}, waiting for budget restoration."
-                )
-                rate_limit.start_restoring_budget(user_id)
-                await asyncio.sleep(
-                    rate_limit.options.budget_restore_interval_ms / 1000.0
-                )
-                continue
+                logging.info(f"Retrying build handshake number {i} times")
+            if not rate_limit.has_budget(client_id):
+                logging.debug("No retry budget for %s.", client_id)
+                break
             try:
                 ws = await websockets.connect(self._websocket_uri)
+                existing_session = await self._get_existing_session()
+                session_id = (
+                    self.generate_session_id()
+                    if not existing_session
+                    else existing_session.session_id
+                )
+                rate_limit.consume_budget(client_id)
                 handshake_request, handshake_response = await self._establish_handshake(
-                    self._transport_id, self._server_id, self._instance_id, ws
+                    self._transport_id, self._server_id, session_id, ws
                 )
+                rate_limit.start_restoring_budget(client_id)
                 return ws, handshake_request, handshake_response
             except Exception as e:
-                backoff_time = rate_limit.get_backoff_ms(user_id)
+                backoff_time = rate_limit.get_backoff_ms(client_id)
                 logging.error(
                     f"Error creating session: {e}, start backoff {backoff_time} ms"
                 )
                 await asyncio.sleep(backoff_time / 1000)
         raise RiverException(
             ERROR_HANDSHAKE,
             "Failed to create session after retrying max number of times",
         )
 
+    async def _retry_session_connection(
+        self, session_to_replace_ws: Session
+    ) -> Session:
+        async with self._retry_ws_lock:
+            if await session_to_replace_ws.is_websocket_open():
+                # other retry successfully replaced the websocket,
+                return session_to_replace_ws
+            if not await session_to_replace_ws.is_session_open():
+                # If the session is already closing we don't retry connection
+                return session_to_replace_ws
+            new_ws, hs_request, hs_response = await self._establish_new_connection()
+            # If the server session id different, we create a new session.
+            if (
+                hs_response.status.sessionId
+                != session_to_replace_ws.advertised_session_id
+            ):
+                server_session_id = hs_response.status.sessionId
+                if not server_session_id:
+                    raise RiverException(
+                        ERROR_SESSION,
+                        "Server did not return a sessionId in successful handshake",
+                    )
+                new_session = ClientSession(
+                    transport_id=self._transport_id,
+                    to_id=self._server_id,
+                    session_id=hs_request.sessionId,
+                    advertised_session_id=server_session_id,
+                    websocket=new_ws,
+                    transport_options=self._transport_options,
+                    is_server=False,
+                    handlers={},
+                    close_session_callback=self._on_session_closed,
+                    retry_connection_callback=lambda x: self._retry_session_connection(
+                        x
+                    ),
+                )
+                return new_session
+            else:
+                # If the session is still active and aligns with the server session
+                # we replace the websocket in it.
+                await session_to_replace_ws.replace_with_new_websocket(new_ws)
+            return session_to_replace_ws
+
     async def _get_or_create_session(self) -> ClientSession:
         async with self._create_session_lock:
             existing_session = await self._get_existing_session()
             if existing_session:
                 if await existing_session.is_websocket_open():
                     return existing_session
                 else:
-                    await self._retry_session_connection(existing_session)
-                    return existing_session
+                    session = await self._retry_session_connection(existing_session)
+                    # This should never happen, adding here to make mypy happy
+                    if not isinstance(session, ClientSession):
+                        raise RiverException(
+                            ERROR_SESSION,
+                            f"Session type is not ClientSession, got {type(session)}",
+                        )
+                    return session
             else:
                 new_ws, hs_request, hs_response = await self._establish_new_connection()
+                advertised_session_id = hs_response.status.sessionId
+                if not advertised_session_id:
+                    raise RiverException(
+                        ERROR_SESSION,
+                        "Server did not return a sessionId in successful handshake",
+                    )
                 new_session = ClientSession(
                     transport_id=self._transport_id,
                     to_id=self._server_id,
-                    instance_id=self._instance_id,
+                    session_id=hs_request.sessionId,
+                    advertised_session_id=advertised_session_id,
                     websocket=new_ws,
                     transport_options=self._transport_options,
                     is_server=False,
                     handlers={},
                     close_session_callback=self._on_session_closed,
                     retry_connection_callback=lambda x: self._retry_session_connection(
                         x
                     ),
                 )
-                async with self._session_lock:
-                    self._sessions[self._server_id] = new_session
+                await self._set_session(new_session)
                 await new_session.start_serve_responses()
                 return new_session
 
     async def _send_handshake_request(
         self,
         transport_id: str,
         to_id: str,
-        instance_id: str,
+        session_id: str,
         websocket: WebSocketCommonProtocol,
     ) -> ControlMessageHandshakeRequest:
         handshake_request = ControlMessageHandshakeRequest(
             type="HANDSHAKE_REQ",
             protocolVersion=PROTOCOL_VERSION,
-            instanceId=instance_id,
+            sessionId=session_id,
         )
         stream_id = self.generate_nanoid()
 
-        def websocket_closed_callback():
+        def websocket_closed_callback() -> None:
             raise RiverException(ERROR_SESSION, "Session closed while sending")
 
         try:
             await send_transport_message(
                 TransportMessage(
                     from_=transport_id,
                     to=to_id,
@@ -194,58 +245,61 @@
                 prefix_bytes=self._transport_options.get_prefix_bytes(),
                 websocket_closed_callback=websocket_closed_callback,
             )
             return handshake_request
         except ConnectionClosed:
             raise RiverException(ERROR_HANDSHAKE, "Hand shake failed")
 
+    async def _get_handshake_response_msg(
+        self, websocket: WebSocketCommonProtocol
+    ) -> TransportMessage:
+        while True:
+            try:
+                data = await websocket.recv()
+            except ConnectionClosed as e:
+                logging.debug(
+                    "Connection closed during waiting for handshake response : %r", e
+                )
+                raise RiverException(ERROR_HANDSHAKE, "Hand shake failed")
+            try:
+                return parse_transport_msg(data, self._transport_options)
+            except IgnoreMessageException as e:
+                logging.debug("Ignoring transport message : %r", e)
+                continue
+            except InvalidMessageException as e:
+                raise RiverException(
+                    ERROR_HANDSHAKE,
+                    f"Got invalid transport message, closing connection : {e}",
+                )
+
     async def _establish_handshake(
         self,
         transport_id: str,
         to_id: str,
-        instance_id: str,
+        session_id: str,
         websocket: WebSocketCommonProtocol,
     ) -> Tuple[ControlMessageHandshakeRequest, ControlMessageHandshakeResponse]:
         try:
             handshake_request = await self._send_handshake_request(
                 transport_id=transport_id,
                 to_id=to_id,
-                instance_id=instance_id,
+                session_id=session_id,
                 websocket=websocket,
             )
         except FailedSendingMessageException:
             raise RiverException(
                 ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
         logging.debug("river client waiting for handshake response")
-        while True:
-            try:
-                logging.debug(f"websocket while waiting for response : {websocket.id}")
-                data = await websocket.recv()
-            except ConnectionClosed:
-                logging.debug(
-                    "Connection closed during waiting for handshake response : {e}"
-                )
-                raise RiverException(ERROR_HANDSHAKE, "Hand shake failed")
-            try:
-                first_message = parse_transport_msg(data, self._transport_options)
-            except IgnoreMessageException as e:
-                logging.debug(f"Ignoring transport message : {e}")
-                continue
-            except InvalidMessageException as e:
-                raise RiverException(
-                    ERROR_HANDSHAKE,
-                    f"Got invalid transport message, closing connection : {e}",
-                )
-            break
         try:
-            handshake_response = ControlMessageHandshakeResponse(
-                **first_message.payload
+            response_msg = await self._get_handshake_response_msg(websocket)
+            handshake_response = ControlMessageHandshakeResponse(**response_msg.payload)
+            logging.debug(
+                "river client get handshake response : %r", handshake_response
             )
-            logging.debug(f"river client get handshake response : {handshake_response}")
         except ValidationError as e:
             raise RiverException(
                 ERROR_HANDSHAKE, f"Failed to parse handshake response : {e}"
             )
         if not handshake_response.status.ok:
             raise RiverException(
                 ERROR_HANDSHAKE, f"Handshake failed: {handshake_response.status.reason}"
```

### Comparing `replit_river-0.1.7b8/replit_river/codegen/client.py` & `replit_river-0.1.8/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b8/replit_river/codegen/run.py` & `replit_river-0.1.8/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b8/replit_river/codegen/schema.py` & `replit_river-0.1.8/replit_river/codegen/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """Generates the type of a protobuf message into Typebox descriptions."""
     type: Dict[str, Any] = {
         "type": "object",
         "properties": {},
         "required": [],
     }
     # Non-oneof fields.
-    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
-        collections.defaultdict(list)
-    )
+    oneofs: DefaultDict[
+        int, List[descriptor_pb2.FieldDescriptorProto]
+    ] = collections.defaultdict(list)
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         if field.type == descriptor_pb2.FieldDescriptorProto.TYPE_MESSAGE:
             # TODO: implement
             pass
```

### Comparing `replit_river-0.1.7b8/replit_river/codegen/server.py` & `replit_river-0.1.8/replit_river/codegen/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         "  d: Mapping[str, Any],",
         f") -> {module_name}_pb2.{m.name}:",
         f"  m = {module_name}_pb2.{m.name}()",
         "  if d is None:",
         "    return m",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
-        collections.defaultdict(list)
-    )
+    oneofs: DefaultDict[
+        int, List[descriptor_pb2.FieldDescriptorProto]
+    ] = collections.defaultdict(list)
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         chunks.append(
             f"  if d.get('{to_camel_case(field.name)}') is not None:",
         )
@@ -153,17 +153,17 @@
     chunks = [
         f"def _{m.name}Encoder(",
         f"  e: {module_name}_pb2.{m.name}",
         ") -> Dict[str, Any]:",
         "  d: Dict[str, Any] = {}",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
-        collections.defaultdict(list)
-    )
+    oneofs: DefaultDict[
+        int, List[descriptor_pb2.FieldDescriptorProto]
+    ] = collections.defaultdict(list)
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         value: str
         if field.type_name == ".google.protobuf.Timestamp":
             value = f"_{field.name}.ToDatetime(tzinfo=datetime.timezone.utc)"
```

### Comparing `replit_river-0.1.7b8/replit_river/error_schema.py` & `replit_river-0.1.8/replit_river/error_schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b8/replit_river/message_buffer.py` & `replit_river-0.1.8/replit_river/message_buffer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 import logging
 from typing import Optional
 
 from replit_river.rpc import TransportMessage
+from replit_river.transport_options import MAX_MESSAGE_BUFFER_SIZE
 
 
 class MessageBuffer:
-    """A buffer to strore messages and support current updates"""
+    """A buffer to store messages and support current updates"""
 
-    def __init__(self, max_size: int = 1000):
-        self.max_size = max_size
+    def __init__(self, max_num_messages: int = MAX_MESSAGE_BUFFER_SIZE):
+        self.max_size = max_num_messages
         self.buffer: list[TransportMessage] = []
         self._lock = asyncio.Lock()
 
     async def empty(self) -> bool:
         """Check if the buffer is empty"""
         async with self._lock:
             return len(self.buffer) == 0
@@ -23,17 +24,17 @@
         async with self._lock:
             if len(self.buffer) >= self.max_size:
                 logging.error("Buffer is full, dropping message")
                 raise ValueError("Buffer is full")
             self.buffer.append(message)
 
     async def peek(self) -> Optional[TransportMessage]:
-        """Peek the first message in the buffer"""
+        """Peek the first message in the buffer, returns None if the buffer is empty."""
         async with self._lock:
             if len(self.buffer) == 0:
                 return None
             return self.buffer[0]
 
-    async def remove_old_messages(self, ack: int) -> None:
-        """Remove all messages in the buffer"""
+    async def remove_old_messages(self, min_seq: int) -> None:
+        """Remove messages in the buffer with a seq number less than min_seq."""
         async with self._lock:
-            self.buffer = [msg for msg in self.buffer if msg.seq >= ack]
+            self.buffer = [msg for msg in self.buffer if msg.seq >= min_seq]
```

### Comparing `replit_river-0.1.7b8/replit_river/messages.py` & `replit_river-0.1.8/replit_river/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 from replit_river.transport_options import TransportOptions
 
 
 class FailedSendingMessageException(Exception):
     pass
 
 
-PROTOCOL_VERSION = "v1"
+PROTOCOL_VERSION = "v1.1"
 
 CROSIS_PREFIX_BYTES = b"\x00\x00"
 PID2_PREFIX_BYTES = b"\xff\xff"
 
 
 async def send_transport_message(
     msg: TransportMessage,
     ws: WebSocketCommonProtocol,
     websocket_closed_callback: Callable[[], Coroutine[Any, Any, None]],
     prefix_bytes: bytes = b"",
 ) -> None:
-    logging.debug(f"sending a message {msg} to ws {ws.id}")
+    logging.debug("sending a message %r to ws %s", msg, ws)
     try:
         await ws.send(
             prefix_bytes
             + msgpack.packb(
                 msg.model_dump(by_alias=True, exclude_none=True), datetime=True
             )
         )
@@ -64,23 +64,23 @@
     if transport_options.use_prefix_bytes:
         if message.startswith(CROSIS_PREFIX_BYTES):
             raise IgnoreMessageException("Skip crosis message")
         elif message.startswith(PID2_PREFIX_BYTES):
             message = message[len(PID2_PREFIX_BYTES) :]
         else:
             raise InvalidMessageException(
-                "Got message without prefix bytes: " f"{formatted_bytes(message)}"
+                f"Got message without prefix bytes: {formatted_bytes(message)[:5]}"
             )
     try:
-        unpacked_message = msgpack.unpackb(message, timestamp=3)
+        unpacked_message = msgpack.unpackb(message)
     except (msgpack.UnpackException, msgpack.exceptions.ExtraData):
         raise InvalidMessageException("received non-msgpack message")
     try:
         msg = TransportMessage(**unpacked_message)
     except (
         ValidationError,
         ValueError,
         msgpack.UnpackException,
         PydanticCoreValidationError,
     ):
-        raise InvalidMessageException(f"failed to parse message:{message.decode()}")
+        raise InvalidMessageException(f"failed to parse message: {unpacked_message}")
     return msg
```

### Comparing `replit_river-0.1.7b8/replit_river/rpc.py` & `replit_river-0.1.8/replit_river/rpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from pydantic import BaseModel, ConfigDict, Field
 
 from replit_river.error_schema import (
     ERROR_CODE_STREAM_CLOSED,
     RiverError,
     RiverException,
 )
+from replit_river.task_manager import BackgroundTaskManager
+from replit_river.transport_options import MAX_MESSAGE_BUFFER_SIZE
 
 InitType = TypeVar("InitType")
 RequestType = TypeVar("RequestType")
 ResponseType = TypeVar("ResponseType")
 ErrorType = TypeVar("ErrorType", bound=RiverError)
 
 _MetadataType = Union[grpc.aio.Metadata, Sequence[Tuple[str, Union[str, bytes]]]]
@@ -45,32 +47,32 @@
 
 # Equivalent of https://github.com/replit/river/blob/c1345f1ff6a17a841d4319fad5c153b5bda43827/transport/message.ts#L23-L33
 
 
 class ControlMessageHandshakeRequest(BaseModel):
     type: Literal["HANDSHAKE_REQ"] = "HANDSHAKE_REQ"
     protocolVersion: str
-    instanceId: str
+    sessionId: str
 
 
 class HandShakeStatus(BaseModel):
     ok: bool
-    # Instance id should be server level id, each server have one
-    instanceId: Optional[str] = None
+    sessionId: Optional[str] = None
     # Reason for failure
     reason: Optional[str] = None
 
 
 class ControlMessageHandshakeResponse(BaseModel):
     type: Literal["HANDSHAKE_RESP"] = "HANDSHAKE_RESP"
     status: HandShakeStatus
 
 
 class TransportMessage(BaseModel):
     id: str
+    # from_ is used instead of from because from is a reserved keyword in Python
     from_: str = Field(..., alias="from")
     to: str
     seq: int
     ack: int
     serviceName: Optional[str] = None
     procedureName: Optional[str] = None
     streamId: str
@@ -272,17 +274,18 @@
     response_serializer: Callable[[ResponseType], Any],
 ) -> GenericRpcHandler:
     async def wrapped(
         peer: str,
         input: Channel[Any],
         output: Channel[Any],
     ) -> None:
+        task_manager = BackgroundTaskManager()
         try:
             context = GrpcContext(peer)
-            request: Channel[RequestType] = Channel(1024)
+            request: Channel[RequestType] = Channel(MAX_MESSAGE_BUFFER_SIZE)
 
             async def _convert_inputs() -> None:
                 try:
                     async for item in input:
                         await request.put(request_deserializer(item))
                 finally:
                     request.close()
@@ -305,29 +308,31 @@
                                 "message": f"{method.__name__} threw an exception: {e}",
                             },
                         }
                     )
                 finally:
                     output.close()
 
-            convert_inputs_task = asyncio.create_task(_convert_inputs())
-            convert_outputs_task = asyncio.create_task(_convert_outputs())
+            convert_inputs_task = await task_manager.create_task(_convert_inputs())
+            convert_outputs_task = await task_manager.create_task(_convert_outputs())
             await asyncio.wait((convert_inputs_task, convert_outputs_task))
+
         except Exception as e:
             logging.exception("Uncaught exception in upload")
             await output.put(
                 {
                     "ok": False,
                     "payload": {
                         "code": "UNCAUGHT_EXCEPTION",
                         "message": f"{method.__name__} threw an exception: {e}",
                     },
                 }
             )
         finally:
+            await task_manager.cancel_all_tasks()
             output.close()
 
     return wrapped
 
 
 def stream_method_handler(
     method: Callable[
@@ -338,17 +343,18 @@
     response_serializer: Callable[[ResponseType], Any],
 ) -> GenericRpcHandler:
     async def wrapped(
         peer: str,
         input: Channel[Any],
         output: Channel[Any],
     ) -> None:
+        task_manager = BackgroundTaskManager()
         try:
             context = GrpcContext(peer)
-            request: Channel[RequestType] = Channel(1024)
+            request: Channel[RequestType] = Channel(MAX_MESSAGE_BUFFER_SIZE)
 
             async def _convert_inputs() -> None:
                 try:
                     async for item in input:
                         await request.put(request_deserializer(item))
                 finally:
                     request.close()
@@ -360,16 +366,16 @@
                     async for item in response:
                         await output.put(
                             get_response_or_error_payload(item, response_serializer)
                         )
                 finally:
                     output.close()
 
-            convert_inputs_task = asyncio.create_task(_convert_inputs())
-            convert_outputs_task = asyncio.create_task(_convert_outputs())
+            convert_inputs_task = await task_manager.create_task(_convert_inputs())
+            convert_outputs_task = await task_manager.create_task(_convert_outputs())
             await asyncio.wait((convert_inputs_task, convert_outputs_task))
         except grpc.RpcError:
             logging.exception("RPC exception in stream")
             await output.put(
                 {
                     "ok": False,
                     "payload": {
@@ -387,10 +393,11 @@
                     "payload": {
                         "code": "UNCAUGHT_EXCEPTION",
                         "message": f"{method.__name__} threw an exception: {e}",
                     },
                 }
             )
         finally:
+            await task_manager.cancel_all_tasks()
             output.close()
 
     return wrapped
```

### Comparing `replit_river-0.1.7b8/replit_river/seq_manager.py` & `replit_river-0.1.8/replit_river/seq_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,21 +56,21 @@
                 if msg.seq < self.ack:
                     raise IgnoreMessageException(
                         f"{msg.from_} received duplicate msg, got {msg.seq}"
                         f" expected {self.ack}"
                     )
                 else:
                     logging.error(
-                        f"Out of order message received got {msg.seq} expected {self.ack}"
+                        f"Out of order message received got {msg.seq} expected "
+                        f"{self.ack}"
+                    )
+                    raise InvalidMessageException(
+                        f"{msg.from_} received out of order, got {msg.seq}"
+                        f" expected {self.ack}"
                     )
-                    # raise InvalidMessageException(
-                    #     f"{msg.from_} received out of order, got {msg.seq}"
-                    #     f" expected {self.ack}"
-                    # )
             self.receiver_ack = msg.ack
         await self._set_ack(msg.seq + 1)
-        # await self._set_ack(max(msg.seq + 1, self.ack))
 
     async def _set_ack(self, new_ack: int) -> int:
         async with self._ack_lock:
             self.ack = new_ack
             return self.ack
```

### Comparing `replit_river-0.1.7b8/replit_river/server.py` & `replit_river-0.1.8/replit_river/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,41 +20,43 @@
             transport_id=self._server_id,
             transport_options=transport_options,
             is_server=True,
         )
 
     async def close(self) -> None:
         logging.info(f"river server {self._server_id} start closing")
-        await self._transport.close_all_sessions()
+        await self._transport.close()
         logging.info(f"river server {self._server_id} closed")
 
     def add_rpc_handlers(
         self,
         rpc_handlers: Mapping[Tuple[str, str], Tuple[str, GenericRpcHandler]],
     ) -> None:
         self._transport._handlers.update(rpc_handlers)
 
     async def serve(self, websocket: WebSocketServerProtocol) -> None:
         logging.debug(
-            f"River server started establishing session with ws: {websocket.id}"
+            "River server started establishing session with ws: %s", websocket.id
         )
         try:
             session = await self._transport.handshake_to_get_session(websocket)
         except Exception as e:
-            logging.error(f"Error establishing handshake, closing websocket: {e}")
+            logging.error(
+                f"Error establishing handshake, closing websocket: {e}", exc_info=True
+            )
             await websocket.close()
             return
         logging.debug("River server session established, start serving messages")
 
         try:
             # Session serve will be closed in two cases
             #   1. websocket is closed
             #   2. exception thrown
             # session should be kept in order to be reused by the reconnect within the
             # grace period.
             await session.serve()
         except ConnectionClosed as e:
-            logging.debug(f"ConnectionClosed while serving {e}")
+            logging.debug("ConnectionClosed while serving %r", e)
             # We don't have to close the websocket here, it is already closed.
         except Exception as e:
             logging.error(f"River transport error in server {self._server_id}: {e}")
             await websocket.close()
```

### Comparing `replit_river-0.1.7b8/replit_river/session.py` & `replit_river-0.1.8/replit_river/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,60 +17,62 @@
 )
 from replit_river.seq_manager import (
     IgnoreMessageException,
     InvalidMessageException,
     SeqManager,
 )
 from replit_river.task_manager import BackgroundTaskManager
-from replit_river.transport_options import TransportOptions
+from replit_river.transport_options import MAX_MESSAGE_BUFFER_SIZE, TransportOptions
 
 from .rpc import (
     ACK_BIT,
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     GenericRpcHandler,
     TransportMessage,
 )
 
 
 class SessionState(enum.Enum):
     ACTIVE = 0
-    CLOSING = 3
-    CLOSED = 4
+    CLOSING = 1
+    CLOSED = 2
 
 
 class WsState(enum.Enum):
     OPEN = 0
-    CLOSING = 2
-    CLOSED = 3
+    CLOSING = 1
+    CLOSED = 2
 
 
 class Session(object):
     """A transport object that handles the websocket connection with a client."""
 
     def __init__(
         self,
         transport_id: str,
         to_id: str,
-        instance_id: str,
+        session_id: str,
+        advertised_session_id: str,
         websocket: websockets.WebSocketCommonProtocol,
         transport_options: TransportOptions,
         is_server: bool,
         handlers: Dict[Tuple[str, str], Tuple[str, GenericRpcHandler]],
         close_session_callback: Callable[["Session"], Coroutine[Any, Any, None]],
         retry_connection_callback: Optional[
             Callable[
                 ["Session"],
-                Coroutine[Any, Any, None],
+                Coroutine[Any, Any, Any],
             ]
         ] = None,
     ) -> None:
         self._transport_id = transport_id
         self._to_id = to_id
-        self._instance_id = instance_id
+        self.session_id = session_id
+        self.advertised_session_id = advertised_session_id
         self._handlers = handlers
         self._is_server = is_server
         self._transport_options = transport_options
 
         # session state, only modified during closing
         self._state = SessionState.ACTIVE
         self._state_lock = asyncio.Lock()
@@ -120,34 +122,35 @@
         websocket is closed.
         """
         logging.debug("begin_close_session_countdown")
         if self._close_session_after_time_secs is not None:
             # already in grace period, no need to set again
             return
         logging.debug(
-            f"websocket closed from {self._transport_id} to {self._to_id}, "
-            "begin grace period"
+            "websocket closed from %s to %s begin grace period",
+            self._transport_id,
+            self._to_id,
         )
         grace_period_ms = self._transport_options.session_disconnect_grace_ms
         self._close_session_after_time_secs = (
             await self._get_current_time() + grace_period_ms / 1000
         )
 
     async def serve(self) -> None:
         """Serve messages from the websocket."""
         try:
             async with asyncio.TaskGroup() as tg:
                 try:
                     await self._handle_messages_from_ws(self._ws, tg)
                 except ConnectionClosed as e:
                     await self._on_websocket_unexpected_close()
-                    logging.debug(f"ConnectionClosed while serving: {e}")
+                    logging.debug("ConnectionClosed while serving: %r", e)
                 except FailedSendingMessageException as e:
                     # Expected error if the connection is closed.
-                    logging.debug(f"FailedSendingMessageException while serving: {e}")
+                    logging.debug("FailedSendingMessageException while serving: %r", e)
                 except Exception:
                     logging.exception("caught exception at message iterator")
         except ExceptionGroup as eg:
             _, unhandled = eg.split(lambda e: isinstance(e, ConnectionClosed))
             if unhandled:
                 raise ExceptionGroup(
                     "Unhandled exceptions on River server", unhandled.exceptions
@@ -158,16 +161,17 @@
         await self._remove_acked_messages_in_buffer()
         self._reset_session_close_countdown()
 
     async def _handle_messages_from_ws(
         self, websocket: WebSocketCommonProtocol, tg: Optional[asyncio.TaskGroup] = None
     ) -> None:
         logging.debug(
-            f'{"server" if self._is_server else "client"} start handling messages from'
-            f" ws {websocket.id}"
+            "%s start handling messages from ws %s",
+            "server" if self._is_server else "client",
+            websocket.id,
         )
         try:
             async for message in websocket:
                 try:
                     msg = parse_transport_msg(message, self._transport_options)
 
                     logging.debug(f"{self._transport_id} got a message %r", msg)
@@ -191,15 +195,15 @@
 
                     if msg.controlFlags & STREAM_CLOSED_BIT != 0:
                         if stream:
                             stream.close()
                         async with self._stream_lock:
                             del self._streams[msg.streamId]
                 except IgnoreMessageException as e:
-                    logging.debug(f"Ignoring transport message : {e}")
+                    logging.debug("Ignoring transport message : %r", e)
                     continue
                 except InvalidMessageException as e:
                     logging.error(
                         f"Got invalid transport message, closing session : {e}"
                     )
                     await self.close(True)
                     return
@@ -249,35 +253,41 @@
         self,
     ) -> None:
         logging.debug("Start heartbeat")
         while True:
             await asyncio.sleep(self._transport_options.heartbeat_ms / 1000)
             if self._state != SessionState.ACTIVE:
                 logging.debug(
-                    f"Session is closed, no need to send heartbeat, state : "
-                    f"{self._state} close_session_after_this: "
-                    f"{self._close_session_after_time_secs}"
+                    "Session is closed, no need to send heartbeat, state : "
+                    "%r close_session_after_this: %r",
+                    {self._state},
+                    {self._close_session_after_time_secs},
                 )
                 # session is closing, no need to send heartbeat
                 continue
             try:
                 await self.send_message(
                     str(nanoid.generate()),
+                    # TODO: make this a message class
+                    # https://github.com/replit/river/blob/741b1ea6d7600937ad53564e9cf8cd27a92ec36a/transport/message.ts#L42
                     {
                         "ack": 0,
                     },
                     self._ws,
                     ACK_BIT,
                 )
                 self._heartbeat_misses += 1
                 if (
                     self._heartbeat_misses
                     >= self._transport_options.heartbeats_until_dead
                 ):
-                    logging.debug("closing websocket because of heartbeat misses")
+                    logging.debug(
+                        "%r closing websocket because of heartbeat misses",
+                        self.session_id,
+                    )
                     await self._on_websocket_unexpected_close()
                     await self.close_websocket(
                         self._ws, should_retry=not self._is_server
                     )
                     continue
             except FailedSendingMessageException:
                 # this is expected during websocket closed period
@@ -341,15 +351,16 @@
         try:
             # We need this lock to ensure the buffer order and message sending order
             # are the same.
             async with self._msg_lock:
                 try:
                     await self._buffer.put(msg)
                 except Exception:
-                    # We should close the session when there are too many messages in buffer
+                    # We should close the session when there are too many messages in
+                    # buffer
                     await self.close(True)
                     return
                 await self._send_transport_message(
                     msg,
                     ws,
                     prefix_bytes=self._transport_options.get_prefix_bytes(),
                 )
@@ -367,28 +378,33 @@
         self,
         stream_id: str,
         output: Channel[Any],
         is_streaming_output: bool,
     ) -> None:
         """Send serialized messages to the websockets."""
         try:
+            # TODO: This blocking is not ideal, we should close this task when websocket
+            # is closed, and start another one when websocket reconnects.
+            ws = None
             async for payload in output:
-                # TODO: what if the websocket changed during this?
                 ws = self._ws
                 while self._ws_state != WsState.OPEN:
                     await asyncio.sleep(
                         self._transport_options.close_session_check_interval_ms / 1000
                     )
                     ws = self._ws
                 if not is_streaming_output:
                     await self.send_message(stream_id, payload, ws, STREAM_CLOSED_BIT)
                     return
                 await self.send_message(stream_id, payload, ws)
-            logging.debug("sent an end of stream %r", stream_id)
-            await self.send_message(stream_id, {"type": "CLOSE"}, ws, STREAM_CLOSED_BIT)
+            if ws:
+                logging.debug("sent an end of stream %r", stream_id)
+                await self.send_message(
+                    stream_id, {"type": "CLOSE"}, ws, STREAM_CLOSED_BIT
+                )
         except FailedSendingMessageException as e:
             logging.error(f"Error while sending responses, {type(e)} : {e}")
         except (RuntimeError, ChannelClosed) as e:
             logging.error(f"Error while sending responses, {type(e)} : {e}")
         except Exception as e:
             logging.error(f"Unknown error while river sending responses back : {e}")
 
@@ -408,15 +424,15 @@
                 f"closing websocket {ws.id}"
             )
             self._ws_state = WsState.CLOSING
             if ws:
                 # TODO: should we wait here?
                 task = asyncio.create_task(ws.close())
                 task.add_done_callback(
-                    lambda _: logging.debug(f"old websocket {ws.id} closed.")
+                    lambda _: logging.debug("old websocket %s closed.", ws.id)
                 )
             self._ws_state = WsState.CLOSED
         if should_retry and self._retry_connection_callback:
             await self._retry_connection_callback(self)
 
     async def _open_stream_and_call_handler(
         self,
@@ -442,16 +458,20 @@
             "stream",
         )
         is_streaming_input = method_type in (
             "upload-stream",  # subscription
             "stream",
         )
         # New channel pair.
-        input_stream: Channel[Any] = Channel(1024 if is_streaming_input else 1)
-        output_stream: Channel[Any] = Channel(1024 if is_streaming_output else 1)
+        input_stream: Channel[Any] = Channel(
+            MAX_MESSAGE_BUFFER_SIZE if is_streaming_input else 1
+        )
+        output_stream: Channel[Any] = Channel(
+            MAX_MESSAGE_BUFFER_SIZE if is_streaming_output else 1
+        )
         try:
             await input_stream.put(msg.payload)
         except (RuntimeError, ChannelClosed) as e:
             raise InvalidMessageException(e)
         if not stream:
             async with self._stream_lock:
                 self._streams[msg.streamId] = input_stream
@@ -489,15 +509,15 @@
     async def start_serve_responses(self) -> None:
         await self._task_manager.create_task(self.serve())
 
     async def close(self, is_unexpected_close: bool) -> None:
         """Close the session and all associated streams."""
         logging.info(
             f"{self._transport_id} closing session "
-            f"to {self._to_id} current_state : {self._ws_state}"
+            f"to {self._to_id}, ws: {self._ws.id}, current_state : {self._ws_state}"
         )
         async with self._state_lock:
             if self._state != SessionState.ACTIVE:
                 # already closing
                 return
             self._state = SessionState.CLOSING
             self._reset_session_close_countdown()
```

### Comparing `replit_river-0.1.7b8/PKG-INFO` & `replit_river-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.7b8
+Version: 0.1.8
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```


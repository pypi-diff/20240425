# Comparing `tmp/bluetooth_auto_recovery-1.4.1.tar.gz` & `tmp/bluetooth_auto_recovery-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_auto_recovery-1.4.1.tar", max compression
+gzip compressed data, was "bluetooth_auto_recovery-1.4.2.tar", max compression
```

## Comparing `bluetooth_auto_recovery-1.4.1.tar` & `bluetooth_auto_recovery-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/LICENSE
--rw-r--r--   0        0        0     3840 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/README.md
--rw-r--r--   0        0        0     2618 2024-04-18 00:14:28.842423 bluetooth_auto_recovery-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1063 2024-04-18 00:14:28.794422 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/py.typed
--rw-r--r--   0        0        0    24748 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/recover.py
--rw-r--r--   0        0        0      225 2024-04-18 00:14:28.054413 bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/util.py
--rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-25 20:05:58.564504 bluetooth_auto_recovery-1.4.2/LICENSE
+-rw-r--r--   0        0        0     3840 2024-04-25 20:05:58.564504 bluetooth_auto_recovery-1.4.2/README.md
+-rw-r--r--   0        0        0     2618 2024-04-25 20:05:59.244514 bluetooth_auto_recovery-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1063 2024-04-25 20:05:59.220514 bluetooth_auto_recovery-1.4.2/src/bluetooth_auto_recovery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:05:58.568505 bluetooth_auto_recovery-1.4.2/src/bluetooth_auto_recovery/py.typed
+-rw-r--r--   0        0        0    25114 2024-04-25 20:05:58.568505 bluetooth_auto_recovery-1.4.2/src/bluetooth_auto_recovery/recover.py
+-rw-r--r--   0        0        0      225 2024-04-25 20:05:58.568505 bluetooth_auto_recovery-1.4.2/src/bluetooth_auto_recovery/util.py
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.4.2/PKG-INFO
```

### Comparing `bluetooth_auto_recovery-1.4.1/LICENSE` & `bluetooth_auto_recovery-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.4.1/README.md` & `bluetooth_auto_recovery-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.4.1/pyproject.toml` & `bluetooth_auto_recovery-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-auto-recovery"
-version = "1.4.1"
+version = "1.4.2"
 description = "Recover bluetooth adapters that are in an stuck state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-auto-recovery"
 documentation = "https://bluetooth-auto-recovery.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/__init__.py` & `bluetooth_auto_recovery-1.4.2/src/bluetooth_auto_recovery/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 import asyncio
 import importlib
 import sys
 from types import ModuleType
 
 _MODULE_CACHE: dict[str, ModuleType] = {}
```

### Comparing `bluetooth_auto_recovery-1.4.1/src/bluetooth_auto_recovery/recover.py` & `bluetooth_auto_recovery-1.4.2/src/bluetooth_auto_recovery/recover.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         self, timeout: float, connection_mode_future: asyncio.Future[None]
     ) -> None:
         """Initialize the protocol."""
         self.future: asyncio.Future[btmgmt_protocol.Response] | None = None
         self.transport: asyncio.Transport | None = None
         self.timeout = timeout
         self.connection_mode_future = connection_mode_future
+        self.loop = asyncio.get_running_loop()
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         """Handle connection made."""
         if not self.connection_mode_future.done():
             self.connection_mode_future.set_result(None)
         self.transport = cast(asyncio.Transport, transport)
 
@@ -151,23 +152,29 @@
             # ValueError: 47 is not a valid Events may happen on newer kernels
             # and we need to ignore these events
             _LOGGER.debug("Error parsing response: %s", ex)
 
     async def send(self, *args: Any) -> btmgmt_protocol.Response:
         """Send command."""
         pkt_objs = btmgmt_protocol.command(*args)
-        full_pkt = b""
-        for frame in pkt_objs:
-            if frame:
-                full_pkt += frame.octets
-        self.future = asyncio.Future()
+        self.future = self.loop.create_future()
         assert self.transport is not None  # nosec
-        self.transport.write(full_pkt)
-        async with asyncio_timeout(self.timeout):
+        self.transport.write(b"".join(frame.octets for frame in pkt_objs if frame))
+        cancel_timeout = self.loop.call_later(
+            self.timeout, self._timeout_future, self.future
+        )
+        try:
             return await self.future
+        finally:
+            cancel_timeout.cancel()
+            self.future = None
+
+    def _timeout_future(self, future: asyncio.Future[btmgmt_protocol.Response]) -> None:
+        if future and not future.done():
+            future.set_exception(asyncio.TimeoutError("Timeout waiting for response"))
 
     def connection_lost(self, exc: Exception | None) -> None:
         """Handle connection lost."""
         if exc:
             _LOGGER.warning("Bluetooth management socket connection lost: %s", exc)
         self.transport = None
```

### Comparing `bluetooth_auto_recovery-1.4.1/PKG-INFO` & `bluetooth_auto_recovery-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-auto-recovery
-Version: 1.4.1
+Version: 1.4.2
 Summary: Recover bluetooth adapters that are in an stuck state
 Home-page: https://github.com/bluetooth-devices/bluetooth-auto-recovery
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.4.2 Summary:
 Recover bluetooth adapters that are in an stuck state Home-page: https://
 github.com/bluetooth-devices/bluetooth-auto-recovery License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```


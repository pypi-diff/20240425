# Comparing `tmp/aio-intex-spa-0.9.0.tar.gz` & `tmp/aio_intex_spa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-intex-spa-0.9.0.tar", last modified: Mon Mar 11 20:41:04 2024, max compression
+gzip compressed data, was "aio_intex_spa-0.9.1.tar", last modified: Thu Apr 25 14:21:11 2024, max compression
```

## Comparing `aio-intex-spa-0.9.0.tar` & `aio_intex_spa-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:41:04.400218 aio-intex-spa-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-11 20:40:53.000000 aio-intex-spa-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-11 20:41:04.400218 aio-intex-spa-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-11 20:40:53.000000 aio-intex-spa-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:41:04.400218 aio-intex-spa-0.9.0/aio_intex_spa/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-11 20:40:53.000000 aio-intex-spa-0.9.0/aio_intex_spa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-03-11 20:41:03.000000 aio-intex-spa-0.9.0/aio_intex_spa/intex_spa.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-11 20:40:53.000000 aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-11 20:41:03.000000 aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_network_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-11 20:41:03.000000 aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_object_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-11 20:41:03.000000 aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_object_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-11 20:41:03.000000 aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:41:04.400218 aio-intex-spa-0.9.0/aio_intex_spa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-11 20:41:04.000000 aio-intex-spa-0.9.0/aio_intex_spa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-11 20:41:04.000000 aio-intex-spa-0.9.0/aio_intex_spa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 20:41:04.000000 aio-intex-spa-0.9.0/aio_intex_spa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-11 20:41:04.000000 aio-intex-spa-0.9.0/aio_intex_spa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-11 20:41:04.400218 aio-intex-spa-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-11 20:41:04.000000 aio-intex-spa-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:41:04.400218 aio-intex-spa-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-11 20:40:53.000000 aio-intex-spa-0.9.0/tests/test_intex_spa_query_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-11 20:40:53.000000 aio-intex-spa-0.9.0/tests/test_intex_spa_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:11.190267 aio_intex_spa-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-25 14:21:11.190267 aio_intex_spa-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:11.190267 aio_intex_spa-0.9.1/aio_intex_spa/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/intex_spa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_network_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_object_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_object_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:11.190267 aio_intex_spa-0.9.1/aio_intex_spa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-25 14:21:11.000000 aio_intex_spa-0.9.1/aio_intex_spa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-25 14:21:11.000000 aio_intex_spa-0.9.1/aio_intex_spa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:21:11.000000 aio_intex_spa-0.9.1/aio_intex_spa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 14:21:11.000000 aio_intex_spa-0.9.1/aio_intex_spa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 14:21:11.190267 aio_intex_spa-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:11.190267 aio_intex_spa-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/tests/test_intex_spa_query_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-25 14:21:05.000000 aio_intex_spa-0.9.1/tests/test_intex_spa_status.py
```

### Comparing `aio-intex-spa-0.9.0/LICENSE` & `aio_intex_spa-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-intex-spa-0.9.0/PKG-INFO` & `aio_intex_spa-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-intex-spa
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Intex Spa wifi interface
 Home-page: https://github.com/mathieu-mp/aio-intex-spa
 Author: Mathieu Payrol
 Author-email: aio-intex-spa@payrol.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,12 +74,12 @@
 For Changelog, please read [releases].
 
 <!-- links start -->
 
 [pypilink]: https://pypi.org/project/aio-intex-spa/
 [pypibadge]: https://badge.fury.io/py/aio-intex-spa.svg
 [releases]: https://github.com/mathieu-mp/aio-intex-spa/releases
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/mathieu-mp/aio-intex-spa
 [devcontainer-badge]: https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
 
 <!-- links end -->
```

### Comparing `aio-intex-spa-0.9.0/README.md` & `aio_intex_spa-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 For Changelog, please read [releases].
 
 <!-- links start -->
 
 [pypilink]: https://pypi.org/project/aio-intex-spa/
 [pypibadge]: https://badge.fury.io/py/aio-intex-spa.svg
 [releases]: https://github.com/mathieu-mp/aio-intex-spa/releases
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/mathieu-mp/aio-intex-spa
 [devcontainer-badge]: https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
 
 <!-- links end -->
```

### Comparing `aio-intex-spa-0.9.0/aio_intex_spa/intex_spa.py` & `aio_intex_spa-0.9.1/aio_intex_spa/intex_spa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""IntexSpa"""
+"""Load IntexSpa class."""
 
 import logging
 import asyncio
-import typing
 
 from .intex_spa_network_layer import IntexSpaNetworkLayer
 from .intex_spa_query import IntexSpaQuery
 from .intex_spa_object_status import IntexSpaStatus
 from .intex_spa_object_info import IntexSpaInfo
 from .intex_spa_exceptions import IntexSpaUnreachableException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class IntexSpa:
-    """
+    """Interface the user with Intex Spa.
+
     AsyncIO-enabled class to interface with Intex Spa wifi module
 
     Attributes
-    -------
+    ----------
     network : IntexSpaNetworkLayer
       The network layer object for communications with intex spa wifi module
     status : IntexSpaStatus
       The status object of the spa
     info : IntexSpaInfo
       The info object of the spa
+
     """
 
     def __init__(self, address: str = "SPA_DEVICE", port: str = "8990"):
-        """
-        Initialize IntexSpa instance
+        """Initialize IntexSpa object instance.
 
         Parameters
         ----------
         address : str, default = "SPA_DEVICE"
           The fqdn or IP of the intex spa wifi module
         port : str, default = "8990"
           The TCP service port the intex spa wifi module
+
         """
         _LOGGER.info("Initializing IntexSpa instance...")
         self.network = IntexSpaNetworkLayer(address, port)
         self._semaphore = asyncio.Semaphore(1)
         self.status = IntexSpaStatus()
         self.info = IntexSpaInfo()
         _LOGGER.info("IntexSpa instance initialized")
 
     async def _async_handle_intent(
-        self, intent: str = "status", expected_state: typing.Union[bool, int] = None
+        self, intent: str = "status", expected_state: bool | int = None
     ) -> IntexSpaStatus:
-        """
-        Handle any intent by conversing with the spa wifi module
+        """Handle any intent by conversing with the spa wifi module.
 
         An intent can be:
         * update: to refresh the status object of the spa
         * *command*: to change the function state or temperature preset on the spa
 
         A conversation with the spa is made of one or more queries:
         * A command intent always triggers a preliminary status update
@@ -67,14 +67,15 @@
         expected_state : bool | int, optional
           The expected state of the function or the temperature preset
 
         Returns
         -------
         status : IntexSpaStatus
           The status of the spa
+
         """
 
         _LOGGER.debug("'%s' intent: Handling new intent...", intent)
 
         # Trigger a preliminary update status intent if the provided intent is a command
         if intent != "status" and intent != "info":
             _LOGGER.debug(
@@ -123,16 +124,16 @@
 
                     except (AssertionError,):
                         _LOGGER.info("Malformed spa response during spa querying")
                         await asyncio.sleep(2)
                         continue
 
                     except (
+                        TimeoutError,
                         asyncio.IncompleteReadError,
-                        asyncio.TimeoutError,
                         ConnectionRefusedError,
                         ConnectionResetError,
                         ConnectionError,
                         OSError,
                     ):
                         _LOGGER.info("Network raised an exception during spa querying")
                         await self.network.async_force_disconnect()
@@ -147,116 +148,117 @@
                     raise IntexSpaUnreachableException("Spa is unreachable")
 
         # Return a status even when getattr(self.status, intent) == expected_state
         # Fixes mathieu-mp/aio-intex-spa#17
         return self.status
 
     async def async_update_status(self) -> IntexSpaStatus:
-        """Update known status of the spa
+        """Update known status of the spa.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self._async_handle_intent("status")
 
     async def async_set(
         self, parameter: str, expected_state: bool = True
     ) -> IntexSpaStatus:
-        """
-        Set specified parameter to `expected_state`
+        """Set specified parameter to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self._async_handle_intent(parameter, expected_state)
 
     async def async_set_power(self, expected_state: bool = True) -> IntexSpaStatus:
-        """
-        Set power function to `expected_state`
+        """Set power function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self.async_set("power", expected_state)
 
     async def async_set_filter(self, expected_state: bool = True) -> IntexSpaStatus:
-        """
-        Set filter function to `expected_state`
+        """Set filter function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self.async_set("filter", expected_state)
 
     async def async_set_heater(self, expected_state: bool = True) -> IntexSpaStatus:
-        """
-        Set heater function to `expected_state`
+        """Set heater function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self.async_set("heater", expected_state)
 
     async def async_set_jets(self, expected_state: bool = True) -> IntexSpaStatus:
-        """
-        Set jets function to `expected_state`
+        """Set jets function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self.async_set("jets", expected_state)
 
     async def async_set_bubbles(self, expected_state: bool = True) -> IntexSpaStatus:
-        """
-        Set bubbles function to `expected_state`
+        """Set bubbles function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self.async_set("bubbles", expected_state)
 
     async def async_set_sanitizer(self, expected_state: bool = True) -> IntexSpaStatus:
-        """
-        Set sanitizer function to `expected_state`
+        """Set sanitizer function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self.async_set("sanitizer", expected_state)
 
     async def async_set_preset_temp(self, expected_state: int) -> IntexSpaStatus:
-        """
-        Set preset_temp function to `expected_state`
+        """Set preset_temp function to `expected_state`.
 
         Returns
         -------
         status : IntexSpaStatus
           The updated spa status
+
         """
         return await self._async_handle_intent("preset_temp", expected_state)
 
     async def async_update_info(self) -> IntexSpaInfo:
-        """
-        Update known info of the spa
+        """Update known info from the spa.
 
         Returns
         -------
         info : IntexSpaInfo
           The updated spa info
+
         """
         return await self._async_handle_intent("info")
```

### Comparing `aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_network_layer.py` & `aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_network_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-"""IntexSpa"""
+"""Load IntexSpaNetworkLayer class."""
 
 import logging
 import asyncio
 import socket
 
 from .intex_spa_exceptions import IntexSpaDnsException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class IntexSpaNetworkLayer:
-    """
+    """Manage Network-layer communications.
+
     AsyncIO-enabled class to manage network-layer communications with Intex Spa wifi module
 
     Attributes
-    -------
+    ----------
     address : str
         The fqdn or IP of the intex spa wifi module
     port : str
         The TCP service port the intex spa wifi module
     reader : asyncio.StreamReader
         The StreamReader connected to the spa
     writer : asyncio.StreamWriter
         The StreamWriter connected to the spa
+
     """
 
     def __init__(self, address: str, port: str):
-        """
-        Initialize IntexSpaNetworkLayer class
+        """Initialize IntexSpaNetworkLayer class.
 
         Parameters
         ----------
         address : str
             The fqdn or IP of the intex spa wifi module
         port : str
             The TCP service port of the intex spa wifi module
+
         """
         self.address = address
         self.port = port
 
         self.reader: asyncio.StreamReader = None
         self.writer: asyncio.StreamWriter = None
 
     async def _async_connect(self) -> None:
-        """Initialize a connection to the spa"""
+        """Initialize a connection to the spa."""
         _LOGGER.debug(
             "Opening TCP connection with the spa at %s:%s with asyncio...",
             self.address,
             self.port,
         )
         try:
             self.reader, self.writer = await asyncio.open_connection(
@@ -63,15 +65,15 @@
                 raise socket.gaierror(err) from err
 
         _LOGGER.info(
             "TCP connection established with the spa",
         )
 
     async def _async_disconnect(self) -> None:
-        """Close the connection to the spa"""
+        """Close the connection to the spa."""
         # If there is a writer to send a disconnect message
         try:
             _LOGGER.debug("Closing previous TCP connection to the spa with asyncio...")
             self.writer.close()
             await self.writer.wait_closed()
             _LOGGER.info("Previous TCP connection closed with the spa")
         except AttributeError:
@@ -81,29 +83,29 @@
                 "Failure while closing previous TCP connection to the spa, dumping it"
             )
         finally:
             self.reader = None
             self.writer = None
 
     async def async_force_disconnect(self) -> None:
-        """Force reconnecting to the spa"""
+        """Force reconnecting to the spa."""
         await self._async_disconnect()
 
     async def async_send(self, bytes_to_write: bytes = None) -> None:
-        """Send command to the spa"""
+        """Send command to the spa."""
         if self.writer is None or self.reader is None:
             _LOGGER.info("Not connected to the spa, trying to connect...")
             await self._async_connect()
         elif self.writer.is_closing() or self.reader.at_eof():
             _LOGGER.info("Connection with the spa seems to be broken")
             await self._async_disconnect()
             await self._async_connect()
 
         _LOGGER.debug("Sending bytes to the spa: %s", bytes_to_write)
         self.writer.write(bytes_to_write)
         await self.writer.drain()
 
     async def async_receive(self) -> None:
-        """Receive response from the spa"""
+        """Receive response from the spa."""
         response_as_bytes = await self.reader.readline()
         _LOGGER.debug("Receiving bytes from the spa: %s", response_as_bytes)
         return response_as_bytes
```

### Comparing `aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_object_info.py` & `aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_object_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""IntexSpaInfo"""
+"""Load IntexSpaInfo class."""
 
 import logging
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class IntexSpaInfo:
-    """
-    Class to represent Intex Spa info
+    """Hold and expose the info response objects.
 
     Attributes
-    -------
+    ----------
     dtype : str
         The spa dtype, provided by the spa
     ip : str
         The spa ip, provided by the spa
     uid : str
         The spa uid, provided by the spa
+
     """
 
     def __init__(self, raw_info: str = None):
-        """
-        Initialize IntexSpaInfo class
+        """Initialize IntexSpaInfo class.
 
         Parameters
         ----------
-        raw_status : int, optional
+        raw_info : int, optional
             The raw response data received from the spa
+
         """
         if raw_info is not None:
             self.update(raw_info)
 
     def update(self, raw_info: dict):
-        """
-        Update the attributes value
+        """Update the attributes value.
 
         Parameters
         ----------
         raw_info : dict
             The response data received from the spa
+
         """
         self.ip: str = raw_info["ip"]  # pylint: disable=invalid-name
         self.uid: str = raw_info["uid"]
         self.dtype: str = raw_info["dtype"]
         _LOGGER.debug("Spa info: '%s'", self)
 
     def as_dict(self) -> dict:
-        """
-        Return main attributes only, as dict
+        """Return main attributes only, as dict.
 
         Returns
         -------
         info_attributes : dict
             IntexSpaInfo main attributes as dict
+
         """
         try:
             return {
                 "ip": self.ip,
                 "uid": self.uid,
                 "dtype": self.dtype,
             }
@@ -65,11 +65,9 @@
             return {
                 "ip": None,
                 "uid": None,
                 "dtype": None,
             }
 
     def __repr__(self) -> str:
-        """
-        Represent IntexSpaInfo main attributes
-        """
+        """Represent IntexSpaInfo main attributes."""
         return repr(self.as_dict())
```

### Comparing `aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_object_status.py` & `aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_object_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-"""IntexSpaStatus"""
+"""Load IntexSpaStatus."""
 
 import logging
-import typing
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class IntexSpaStatus:
-    """
-    Class to represent Intex Spa status
+    """Hold and expose the status response objects.
 
     Attributes
-    -------
+    ----------
     _raw_status : int
         The raw integer-encoded status data, as received from the spa
     power : bool
     filter : bool
     heater : bool
     jets : bool
     bubbles : bool
     sanitizer : bool
     unit : str
     current_temp : int
     preset_temp : int
+
     """
 
     @property
     def power(self) -> bool:
-        """Power state of the spa"""
+        """Power state of the spa."""
         return bool((self._raw_status >> 104) & 0b1)
 
     @property
     def filter(self) -> bool:
-        """State of the filter function"""
+        """State of the filter function."""
         return bool((self._raw_status >> 105) & 0b1)
 
     @property
     def heater(self) -> bool:
-        """State of the heater function"""
+        """State of the heater function."""
         return bool((self._raw_status >> 106) & 0b1)
 
     @property
     def jets(self) -> bool:
-        """State of the jets function"""
+        """State of the jets function."""
         return bool((self._raw_status >> 107) & 0b1)
 
     @property
     def bubbles(self) -> bool:
-        """State of the bubbles function"""
+        """State of the bubbles function."""
         return bool((self._raw_status >> 108) & 0b1)
 
     @property
     def sanitizer(self) -> bool:
-        """State of sanitizer function"""
+        """State of sanitizer function."""
         return bool((self._raw_status >> 109) & 0b1)
 
     @property
     def unit(self) -> str:
-        """Temperature measurement unit
-        *"°C" for Celsius*
-        *"°F" for Farenheit*
+        """Unit of the temperature values.
+
+        * "°C" for Celsius*
+        * "°F" for Farenheit*
         """
         if self.preset_temp <= 40:
             return "°C"
         else:
             return "°F"
 
     @property
-    def current_temp(self) -> typing.Union[int, bool]:
-        """Current temperature of the water, expressed in `unit`"""
+    def current_temp(self) -> int | bool:
+        """Current temperature of the water, expressed in `unit`."""
         raw_current_temp = (self._raw_status >> 88) & 0xFF
 
         # If current_temp encodes a temperature, return the temperature
         if raw_current_temp < 181:
             return raw_current_temp
         # Else if current_temp encodes an error (E81, ...), return False
         else:
             return False
 
     @property
-    def error_code(self) -> typing.Union[int, bool]:
-        """Current error code of the spa"""
+    def error_code(self) -> int | bool:
+        """Current error code of the spa."""
         raw_current_temp = (self._raw_status >> 88) & 0xFF
 
         # If current_temp encodes an error (E81, ...), return the error code
         if raw_current_temp >= 181:
             error_no = raw_current_temp - 100
             return f"E{error_no}"
         # Else if current_temp encodes a temperature, return False
         else:
             return False
 
     @property
     def preset_temp(self) -> int:
-        """Preset temperature of the water, expressed in `unit`"""
+        """Preset temperature of the water, expressed in `unit`."""
         return (self._raw_status >> 24) & 0xFF
 
     def __init__(self, raw_status: int = None):
-        """
-        Initialize IntexSpaStatus class
+        """Initialize IntexSpaStatus class.
 
         Parameters
         ----------
         raw_status : int, optional
             The raw response data received from the spa
+
         """
         if raw_status is not None:
             self.update(raw_status)
 
     def update(self, raw_status: int):
-        """
-        Update the raw_status
+        """Update the status of the spa from the received raw response.
 
         Parameters
         ----------
         raw_status : int
             The raw response data received from the spa
+
         """
         self._raw_status = raw_status
         _LOGGER.debug("Spa status: '%s'", self)
 
     def as_dict(self) -> dict:
-        """
-        Return main status attributes only, as dict
+        """Return main status attributes only, as dict.
 
         Returns
         -------
         status_attributes : dict
             IntexSpaStatus main status attributes as dict
+
         """
         try:
             return {
                 "power": self.power,
                 "filter": self.filter,
                 "heater": self.heater,
                 "jets": self.jets,
@@ -154,11 +154,9 @@
                 "unit": None,
                 "current_temp": None,
                 "preset_temp": None,
                 "error_code": None,
             }
 
     def __repr__(self) -> str:
-        """
-        Represent IntexSpaStatus main attributes
-        """
+        """Represent IntexSpaStatus main attributes."""
         return repr(self.as_dict())
```

### Comparing `aio-intex-spa-0.9.0/aio_intex_spa/intex_spa_query.py` & `aio_intex_spa-0.9.1/aio_intex_spa/intex_spa_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""IntexSpaQuery"""
+"""Load IntexSpaQuery class."""
 
 import time
 import json
 
 TYPE: dict = {
     "command": 1,
     "status": 2,
@@ -46,49 +46,49 @@
         "request": "",
         "type": TYPE["info"],
     },
 }
 
 
 def checksum_as_int(data: str) -> int:
-    """Return integer checksum for the given data, as expected by Intex Spa protocol"""
+    """Return integer checksum for the given data, as expected by Intex Spa protocol."""
     calculated_checksum = 0xFF
     for index in range(0, len(data), 2):
         calculated_checksum = calculated_checksum - (
             int("0x" + data[index : index + 2], 16)
         )
     calculated_checksum = calculated_checksum % 0xFF
     # Fix: https://github.com/mathieu-mp/aio-intex-spa/issues/27
     if calculated_checksum == 0x00:
         calculated_checksum = 0xFF
     return calculated_checksum
 
 
 def checksum_as_str(data: str) -> str:
-    """Return string checksum for the given data, as expected by Intex Spa protocol"""
+    """Return string checksum for the given data, as expected by Intex Spa protocol."""
     # Return checksum as a hex string without 0x prefix
     return hex(checksum_as_int(data))[2:].upper()
 
 
 class IntexSpaQuery:
-    """
-    Class to manage one application-layer query with Intex Spa wifi module
+    """Manage one application-layer query with Intex Spa wifi module.
 
-    Manages encoding and decoding of one request and its response messages
+    For a specific query, manage encoding and decoding of the request and its response messages
 
     Attributes
-    -------
+    ----------
     intex_timestamp : str
         The 10th of milliseconds timestamp, as expected by Intex Spa protocol
     request : str
         The request data to send, as expected by Intex Spa protocol
     request_bytes : bytes
         The full message request to send, as expected by Intex Spa protocol, encoded as bytes
     response_data
         The rendered response data
+
     """
 
     def __init__(self, intent: str, preset_temp: int = None):
         """Init."""
         self.intex_timestamp = str(int(time.time() * 10000))
 
         self.request: str = COMMAND[intent]["request"]
@@ -97,35 +97,35 @@
 
         self.type: int = COMMAND[intent]["type"]
 
         self.response_data: int
 
     @property
     def request_bytes(self) -> bytes:
-        """The full message request to send, as expected by Intex Spa protocol, encoded as bytes"""
+        """The full message request to send, as expected by Intex Spa protocol, encoded as bytes."""
         request_dict = {
             "data": self.request + checksum_as_str(self.request),
             "sid": self.intex_timestamp,
             "type": self.type,
         }
         return json.dumps(request_dict).encode()
 
     def render_response_data(self, received_bytes: bytes):
-        """
-        Render response data from `received_bytes` from Intex Spa wifi module
+        """Render response data from `received_bytes` from Intex Spa wifi module.
 
         Parameters
         ----------
         received_bytes : bytes
             The response received from Intex Spa wifi module, as bytes
 
         Returns
-        ----------
+        -------
         response_data : int
             The new data, rendered from the spa response
+
         """
         response = json.loads(received_bytes.decode())
 
         # Timestamp correspondance check
         assert response["sid"] == self.intex_timestamp
         assert response["result"] == "ok"
```

### Comparing `aio-intex-spa-0.9.0/aio_intex_spa.egg-info/PKG-INFO` & `aio_intex_spa-0.9.1/aio_intex_spa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-intex-spa
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Intex Spa wifi interface
 Home-page: https://github.com/mathieu-mp/aio-intex-spa
 Author: Mathieu Payrol
 Author-email: aio-intex-spa@payrol.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,12 +74,12 @@
 For Changelog, please read [releases].
 
 <!-- links start -->
 
 [pypilink]: https://pypi.org/project/aio-intex-spa/
 [pypibadge]: https://badge.fury.io/py/aio-intex-spa.svg
 [releases]: https://github.com/mathieu-mp/aio-intex-spa/releases
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/mathieu-mp/aio-intex-spa
 [devcontainer-badge]: https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
 
 <!-- links end -->
```

### Comparing `aio-intex-spa-0.9.0/setup.py` & `aio_intex_spa-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Setup configuration."""
 
 from setuptools import setup, find_packages
 
 
-with open("README.md", "r") as fh:
+with open("README.md") as fh:
     README = fh.read()
 setup(
     name="aio-intex-spa",
-    version="0.9.0",
+    version="0.9.1",
     author="Mathieu Payrol",
     author_email="aio-intex-spa@payrol.fr",
     description="Python client for Intex Spa wifi interface",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mathieu-mp/aio-intex-spa",
     packages=find_packages(),
```

### Comparing `aio-intex-spa-0.9.0/tests/test_intex_spa_query_checksum.py` & `aio_intex_spa-0.9.1/tests/test_intex_spa_query_checksum.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Load checksum tests."""
+
 from aio_intex_spa.intex_spa_query import IntexSpaQuery
 
 import pytest
 
 valid_status_responses = [
     b'{"sid":"12345678901234","data":"FFFF110F010700220000000080808022000012","result":"ok","type":2}\n',
     b'{"sid":"12345678901234","data":"FFFF110F01070064000000008080806700008A","result":"ok","type":2}\n',  # From https://github.com/mathieu-mp/aio-intex-spa/issues/27
@@ -11,18 +13,20 @@
     b'{"sid":"12345678901234","data":"FFFF110F010700220000000080808022000044","result":"ok","type":2}\n',  # Arbitrary false checksum
     b'{"sid":"12345678901234","data":"00000000000000000000000000000000000000","result":"ok","type":2}\n',  # Checksum 0x00 means no checksum calculation
 ]
 
 
 @pytest.mark.parametrize("status_response", valid_status_responses)
 def test_valid_intex_spa_checksums(status_response):
+    """Assert provided checksums are considered valid."""
     query = IntexSpaQuery(intent="status")
     query.intex_timestamp = "12345678901234"
     query.render_response_data(received_bytes=status_response)
 
 
 @pytest.mark.parametrize("status_response", invalid_status_responses)
 def test_invalid_intex_spa_checksums(status_response):
+    """Assert provided checksums are considered invalid."""
     query = IntexSpaQuery(intent="status")
     query.intex_timestamp = "12345678901234"
     with pytest.raises(AssertionError):
         query.render_response_data(received_bytes=status_response)
```

### Comparing `aio-intex-spa-0.9.0/tests/test_intex_spa_status.py` & `aio_intex_spa-0.9.1/tests/test_intex_spa_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Load Status parsing tests."""
+
 from aio_intex_spa.intex_spa_object_status import IntexSpaStatus
 
 
 def test_intex_spa_status():
     """Test function for IntexSpaStatus with standard input status."""
     status_str = "FFFF110F010700220000000080808022000012"
     status_int = int("0x" + status_str, 16)
```


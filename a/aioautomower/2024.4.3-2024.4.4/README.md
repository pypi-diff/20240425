# Comparing `tmp/aioautomower-2024.4.3.tar.gz` & `tmp/aioautomower-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2024.4.3.tar", max compression
+gzip compressed data, was "aioautomower-2024.4.4.tar", max compression
```

## Comparing `aioautomower-2024.4.3.tar` & `aioautomower-2024.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1152 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/README.md
--rw-r--r--   0        0        0     8231 2024-04-22 15:58:17.783814 aioautomower-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0      138 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/__init__.py
--rw-r--r--   0        0        0      108 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/_secrets.yaml
--rw-r--r--   0        0        0     7233 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/auth.py
--rw-r--r--   0        0        0     5812 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/const.py
--rw-r--r--   0        0        0     5091 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/example.py
--rw-r--r--   0        0        0      970 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/exceptions.py
--rw-r--r--   0        0        0    11130 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/model.py
--rw-r--r--   0        0        0        0 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/py.typed
--rw-r--r--   0        0        0    14104 2024-04-22 15:58:02.711799 aioautomower-2024.4.3/src/aioautomower/session.py
--rw-r--r--   0        0        0     3659 2024-04-22 15:58:02.715799 aioautomower-2024.4.3/src/aioautomower/utils.py
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 aioautomower-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2001 2024-04-25 17:42:50.257138 aioautomower-2024.4.4/README.md
+-rw-r--r--   0        0        0     8299 2024-04-25 17:43:09.336976 aioautomower-2024.4.4/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/_secrets.yaml
+-rw-r--r--   0        0        0     7241 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/auth.py
+-rw-r--r--   0        0        0     5812 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/const.py
+-rw-r--r--   0        0        0     5087 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/example.py
+-rw-r--r--   0        0        0      970 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/exceptions.py
+-rw-r--r--   0        0        0    11236 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/py.typed
+-rw-r--r--   0        0        0    14281 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/session.py
+-rw-r--r--   0        0        0     3659 2024-04-25 17:42:50.261138 aioautomower-2024.4.4/src/aioautomower/utils.py
+-rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 aioautomower-2024.4.4/PKG-INFO
```

### Comparing `aioautomower-2024.4.3/pyproject.toml` & `aioautomower-2024.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aioautomower"
 # The version is set by GH action on release
-version = "2024.4.3"
+version = "2024.4.4"
 description = "MPython module to talk to Husqvarna Automower."
 authors = ["Thomas55555"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "aioautomower", from = "src" },
 ]
@@ -25,28 +25,28 @@
 aiohttp = "^3.9.3"
 mashumaro = "^3.12"
 PyJWT = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
-coverage = {version = "7.4.4", extras = ["toml"]}
+coverage = {version = "7.5.0", extras = ["toml"]}
 mypy = "1.9.0"
 pre-commit = "3.7.0"
 pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
 pytest = "8.1.1"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
 ruff = "0.4.1"
 safety = "3.1.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
-freezegun = "1.4.0"
+freezegun = "1.5.0"
 pyyaml = "6.0.1"
 types-pyyaml = "^6.0.12.20240311"
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
@@ -226,13 +226,17 @@
 
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
+# strict rules
+disallow_untyped_calls = true
+warn_no_return = true
+
 [tool.coverage.report]
 show_missing = true
 fail_under = 50
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
```

### Comparing `aioautomower-2024.4.3/src/aioautomower/auth.py` & `aioautomower-2024.4.4/src/aioautomower/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         message = ["Error from API", f"{resp.status}"]
         if STATUS in error:
             message.append(f"{error[STATUS]}")
         if MESSAGE in error:
             message.append(error[MESSAGE])
         return message
 
-    async def websocket_connect(self):
+    async def websocket_connect(self) -> None:
         """Start a websocket connection."""
         token = await self._async_get_access_token()
         try:
             self.ws = await self._websession.ws_connect(
                 url=WS_URL,
                 headers={"Authorization": AUTH_HEADER_FMT.format(token)},
                 heartbeat=60,
```

### Comparing `aioautomower-2024.4.3/src/aioautomower/const.py` & `aioautomower-2024.4.4/src/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.3/src/aioautomower/example.py` & `aioautomower-2024.4.4/src/aioautomower/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     async def async_ensure_token_valid(self) -> None:
         """Ensure that the current token is valid."""
         if self.valid_token:
             return
         self.token = await async_get_access_token(CLIENT_ID, CLIENT_SECRET)
 
 
-async def main():
+async def main() -> None:
     """Establish connection to mower and print states for 5 minutes."""
     websession = ClientSession()
     automower_api = AutomowerSession(AsyncTokenAuth(websession), poll=True)
     await asyncio.sleep(1)
     await automower_api.connect()
     api_task = asyncio.create_task(_client_listen(automower_api))
     ping_pong_task = asyncio.create_task(_send_messages(automower_api))
@@ -92,16 +92,16 @@
         # Uncomment the line above to let all your mowers resume their schedule.
         await asyncio.sleep(5)
         # await automower_api.pause_mowing(_mower_id)
         # Uncomment the line above to let all your mowers pause.
     await asyncio.sleep(3000)
     # The close() will stop the websocket and the token refresh tasks
     await automower_api.close()
-    await api_task.cancel()
-    await ping_pong_task.cancel()
+    api_task.cancel()
+    ping_pong_task.cancel()
     await websession.close()
 
 
 def callback(ws_data: dict[str, MowerAttributes]):
     """Process websocket callbacks and write them to the DataUpdateCoordinator."""
     for mower_id in ws_data:
         print(ws_data[mower_id])
```

### Comparing `aioautomower-2024.4.3/src/aioautomower/exceptions.py` & `aioautomower-2024.4.4/src/aioautomower/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.3/src/aioautomower/model.py` & `aioautomower-2024.4.4/src/aioautomower/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,23 +291,27 @@
 
 
 @dataclass
 class _WorkAreas(DataClassDictMixin):
     """DataClass for WorkAreas values."""
 
     work_area_id: int = field(metadata=field_options(alias="workAreaId"))
-    name: str
+    name: str = field(
+        metadata=field_options(
+            deserialize=lambda x: "my_lawn" if x == "" else x,
+        ),
+    )
     cutting_height: int = field(metadata=field_options(alias="cuttingHeight"))
 
 
 @dataclass
 class WorkArea(DataClassDictMixin):
     """DataClass for WorkAreas values."""
 
-    name: str | None
+    name: str
     cutting_height: int
 
 
 @dataclass
 class MowerAttributes(DataClassDictMixin):
     """DataClass for MowerAttributes."""
 
@@ -328,15 +332,15 @@
     stay_out_zones: StayOutZones | None = field(
         metadata=field_options(alias="stayOutZones"), default=None
     )
     work_areas: dict[int, WorkArea] | None = field(
         metadata=field_options(
             deserialize=lambda workarea_list: {
                 area.work_area_id: WorkArea(
-                    name=area.name or None, cutting_height=area.cutting_height
+                    name=area.name, cutting_height=area.cutting_height
                 )
                 for area in map(_WorkAreas.from_dict, workarea_list)
             },
             alias="workAreas",
         ),
         default=None,
     )
```

### Comparing `aioautomower-2024.4.3/src/aioautomower/session.py` & `aioautomower-2024.4.4/src/aioautomower/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module to connect to Automower with websocket."""
 
 import asyncio
 import contextlib
 import datetime
 import logging
 from dataclasses import dataclass
-from typing import Literal
+from typing import Any, Literal, Mapping
 
 from aiohttp import WSMsgType
 
 from .auth import AbstractAuth
 from .const import EVENT_TYPES, REST_POLL_CYCLE
 from .exceptions import NoDataAvailableException, TimeoutException
 from .model import HeadlightModes, MowerAttributes
@@ -64,77 +64,82 @@
         poll: bool = False,
     ) -> None:
         """Create a session.
 
         :param class auth: The AbstractAuth class from aioautomower.auth.
         :param bool poll: Poll data with rest if True.
         """
-        self._data: dict[str, str] = {}
+        self._data: Mapping[Any, Any] = {}
         self.auth = auth
         self.pong_cbs: list = []
         self.data_update_cbs: list = []
         self.data: dict[str, MowerAttributes] = {}
         self.last_ws_message: datetime.datetime
         self.loop = asyncio.get_running_loop()
         self.poll = poll
         self.rest_task: asyncio.Task | None = None
         self.token = None
         self.token_task = None
         self.token_update_cbs: list = []
 
-    def register_data_callback(self, callback):
+    def register_data_callback(self, callback) -> None:
         """Register a data update callback."""
         if callback not in self.data_update_cbs:
             self.data_update_cbs.append(callback)
 
-    def _schedule_data_callback(self, cb):
+    def _schedule_data_callback(self, cb) -> None:
+        """Schedule a data callback."""
         if self.poll and self.data is None:
             raise NoDataAvailableException
         self.loop.call_soon_threadsafe(cb, self.data)
 
     def _schedule_data_callbacks(self) -> None:
+        """Schedule a data callbacks."""
         for cb in self.data_update_cbs:
             self._schedule_data_callback(cb)
 
-    def unregister_data_callback(self, callback):
+    def unregister_data_callback(self, callback) -> None:
         """Unregister a data update callback.
 
         :param func callback: Takes one function, which should be unregistered.
         """
         if callback in self.data_update_cbs:
             self.data_update_cbs.remove(callback)
 
-    def register_pong_callback(self, pong_callback):
-        """Register a data update callback."""
+    def register_pong_callback(self, pong_callback) -> None:
+        """Register a pong callback.
+
+        It's not real ping/pong, but a way to check if the websocket
+        is still alive, by receiving an empty message.
+        """
         if pong_callback not in self.pong_cbs:
             self.pong_cbs.append(pong_callback)
 
-    def _schedule_pong_callback(self, cb):
+    def _schedule_pong_callback(self, cb) -> None:
+        """Schedule a pong callback."""
         self.loop.call_soon_threadsafe(cb, self.last_ws_message)
 
     def _schedule_pong_callbacks(self) -> None:
+        """Schedule pong callbacks."""
         for cb in self.pong_cbs:
             self._schedule_pong_callback(cb)
 
-    def unregister_pong_callback(self, pong_callback):
-        """Unregister a data update callback.
+    def unregister_pong_callback(self, pong_callback) -> None:
+        """Unregister a pong update callback.
 
         :param func callback: Takes one function, which should be unregistered.
         """
         if pong_callback in self.pong_cbs:
             self.pong_cbs.remove(pong_callback)
 
     async def connect(self) -> None:
         """Connect to the API.
 
-        This method handles the login and starts a task that keep the access
-        token constantly fresh. Also a REST task will be started, which
-        periodically polls the REST endpoint. This method works only, if the
-        token is created with the Authorization Code Grant. Call this method
-        before any other methods.
+        This method handles the login. Also a REST task will be started, which
+        periodically polls the REST endpoint, when polling is set to true.
         """
         self._schedule_data_callbacks()
 
         if self.poll:
             await self.get_status()
             self.rest_task = asyncio.create_task(self._rest_task())
 
@@ -330,15 +335,15 @@
 
     async def error_confirm(self, mower_id: str):
         """Confirm non-fatal mower error."""
         body = {}  # type: dict[str, str]
         url = AutomowerEndpoint.error_confirm.format(mower_id=mower_id)
         await self.auth.post_json(url, json=body)
 
-    def _update_data(self, new_data):
+    def _update_data(self, new_data) -> None:
         if self._data is None:
             raise NoDataAvailableException
         if self._data is not None:
             for datum in self._data["data"]:
                 if datum["type"] == "mower" and datum["id"] == new_data["id"]:
                     for attrib in new_data["attributes"]:
                         try:
```

### Comparing `aioautomower-2024.4.3/src/aioautomower/utils.py` & `aioautomower-2024.4.4/src/aioautomower/utils.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.3/PKG-INFO` & `aioautomower-2024.4.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: MPython module to talk to Husqvarna Automower.
 Home-page: https://github.com/Thomas55555/aioautomower
 License: Apache 2.0
 Author: Thomas55555
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,49 @@
 but should be easy to incorporate using Husqvarna's authentication examples. See
 Husqvarna's [Authentication API](https://developer.husqvarnagroup.cloud/apis/authentication-api) for details.
 
 You will implement `AbstractAuth` to provide an access token. Your implementation
 will handle any necessary refreshes. You can invoke the service with your auth implementation
 to access the API.
 
+You need at least:
+
+- Python 3.11+
+- [Poetry][poetry-install]
+
 For a first start you can run the `example.py`, by doing the following steps
 
 - `git clone https://github.com/Thomas55555/aioautomower.git`
-- `pip install -e ./`
-- Enter your personal `client_id` and `client_secret` in the `example.py`
-- Run with `python3 ./aioautomower/example.py`
+- `cd aioautomower`
+- `poetry install`
+- Enter your personal `client_id` and `client_secret` in the `_secrets.yaml` and rename it to `secrets.yaml`
+- Run with `poetry run ./src/aioautomower/example.py`
+
+## Contributing
+
+This is an active open-source project. We are always open to people who want to use the code or contribute to it.
+This Python project is fully managed using the [Poetry][poetry] dependency manager.
+
+As this repository uses the [pre-commit][pre-commit] framework, all changes
+are linted and tested with each commit. You can run all checks and tests
+manually, using the following command:
+
+```bash
+poetry run pre-commit run --all-files
+```
+
+To run just the Python tests:
+
+```bash
+poetry run pytest
+```
+
+To update snapshots:
+
+```bash
+poetry run pytest --snapshot-update
+```
+
+[poetry-install]: https://python-poetry.org/docs/#installation
+[poetry]: https://python-poetry.org
+[pre-commit]: https://pre-commit.com/
```


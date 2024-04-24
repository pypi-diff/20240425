# Comparing `tmp/kumaone-0.0.1a4.tar.gz` & `tmp/kumaone-0.0.1a5.tar.gz`

## Comparing `kumaone-0.0.1a4.tar` & `kumaone-0.0.1a5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/__init__.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/configs.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/connection.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/event_handlers.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/ioevents.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/main.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/monitors.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/notification_settings.py
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/notifications.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/payload_handler.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/settings.py
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/status_pages.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/utils.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/cli/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/cli/config_cli.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/cli/monitor_cli.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/cli/notification_cli.py
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/src/kumaone/cli/status_page_cli.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/.gitignore
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/AUTHORS.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/LICENSE
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/README.md
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 kumaone-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/__init__.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/configs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/connection.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/event_handlers.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/ioevents.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/main.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/monitors.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/notification_settings.py
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/notifications.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/payload_handler.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/settings.py
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/status_pages.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/cli/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/cli/config_cli.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/cli/monitor_cli.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/cli/notification_cli.py
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/src/kumaone/cli/status_page_cli.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/.gitignore
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/AUTHORS.md
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/LICENSE
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/README.md
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 kumaone-0.0.1a5/PKG-INFO
```

### Comparing `kumaone-0.0.1a4/src/kumaone/configs.py` & `kumaone-0.0.1a5/src/kumaone/configs.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/connection.py` & `kumaone-0.0.1a5/src/kumaone/connection.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/event_handlers.py` & `kumaone-0.0.1a5/src/kumaone/event_handlers.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/ioevents.py` & `kumaone-0.0.1a5/src/kumaone/ioevents.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/main.py` & `kumaone-0.0.1a5/src/kumaone/main.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/monitors.py` & `kumaone-0.0.1a5/src/kumaone/monitors.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/notification_settings.py` & `kumaone-0.0.1a5/src/kumaone/notification_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 """Notification settings module for kumaone"""
 
 # Source code meta data
 __author__ = "Dalwar Hossain"
 __email__ = "dalwar23@pm.me"
 
 notification_providers = {
+    "opsgenie":{
+        "opsgeniePriority": "",
+        "opsgenieRegion": "",
+        "opsgenieApiKey": "",
+    },
     "rocket.chat": {
         "rocketchannel": "",
         "rocketusername": "",
         "rocketiconemo": "",
         "rocketwebhookURL": "",
     },
     "slack": {
```

### Comparing `kumaone-0.0.1a4/src/kumaone/notifications.py` & `kumaone-0.0.1a5/src/kumaone/notifications.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/payload_handler.py` & `kumaone-0.0.1a5/src/kumaone/payload_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     :return: (dict) Python dictionary for payload
     """
 
     if accepted_statuscodes is None:
         accepted_statuscodes = ["200-299"]
 
     if notificationIDList is None:
-        notificationIDList = []
+        notificationIDList = {}
 
     monitor_data = {
         "type": type,
         "name": name,
         "interval": interval,
         "retryInterval": retryInterval,
         "maxretries": maxretries,
```

### Comparing `kumaone-0.0.1a4/src/kumaone/settings.py` & `kumaone-0.0.1a5/src/kumaone/settings.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/status_pages.py` & `kumaone-0.0.1a5/src/kumaone/status_pages.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/utils.py` & `kumaone-0.0.1a5/src/kumaone/utils.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/cli/config_cli.py` & `kumaone-0.0.1a5/src/kumaone/cli/config_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/cli/monitor_cli.py` & `kumaone-0.0.1a5/src/kumaone/cli/monitor_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/cli/notification_cli.py` & `kumaone-0.0.1a5/src/kumaone/cli/notification_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/src/kumaone/cli/status_page_cli.py` & `kumaone-0.0.1a5/src/kumaone/cli/status_page_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/.gitignore` & `kumaone-0.0.1a5/.gitignore`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/LICENSE` & `kumaone-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a4/README.md` & `kumaone-0.0.1a5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,18 @@
 - [x] Add status pages from file(s).
 - [x] Delete single status page by slug.
 - [x] Delete status page from file(s).
 
 ### Notification
 
 - Supported notification providers (tested)
+    [x] Opsgenie
   - [x] Rocket.Chat
   - [x] Slack
-  - [x] MS Teams
+  - [x] Teams
   - [x] Webhook
 - [x] List all `notification`(s).
 - [x] See details of a `single notification` by name/id.
 - [ ] Add new notification (interactive).
 - [x] Add notifications from single file.
 - [x] Delete notification by name.
 - [x] Delete notification by id.
```

### Comparing `kumaone-0.0.1a4/pyproject.toml` & `kumaone-0.0.1a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "python-socketio[client] >= 5.11.0",
   "pyyaml >= 6.0.1",
   "requests >= 2.31.0",
-  "typer[all] >= 0.9.0",
+  "typer >= 0.12.3",
   "validators >= 0.22.0"
 ]
 
 [project.urls]
 Documentation = "https://kumaone.rtfd.io/"
 Issues = "https://github.com/dalwar23/kumaone/issues"
 Source = "https://github.com/dalwar23/kumaone"
@@ -178,15 +178,15 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.bumpversion]
-current_version = "0.0.1-alpha.4"
+current_version = "0.0.1-alpha.5"
 #parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 #serialize = ["{major}.{minor}.{patch}"]
 parse = """(?x)
     (?P<major>[0-9]+)
     \\.(?P<minor>[0-9]+)
     \\.(?P<patch>[0-9]+)
     (?:
```

### Comparing `kumaone-0.0.1a4/PKG-INFO` & `kumaone-0.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: kumaone
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: CLI helper for uptime kuma
 Project-URL: Documentation, https://kumaone.rtfd.io/
 Project-URL: Issues, https://github.com/dalwar23/kumaone/issues
 Project-URL: Source, https://github.com/dalwar23/kumaone
 Author-email: Dalwar Hossain <dalwar23@pm.me>
 License-Expression: BSD-3-Clause
 License-File: AUTHORS.md
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: python-socketio[client]>=5.11.0
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: requests>=2.31.0
-Requires-Dist: typer[all]>=0.9.0
+Requires-Dist: typer>=0.12.3
 Requires-Dist: validators>=0.22.0
 Description-Content-Type: text/markdown
 
 # kumaone
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![PyPI - Version](https://img.shields.io/pypi/v/kumaone.svg)](https://pypi.org/project/kumaone)
@@ -129,17 +129,18 @@
 - [x] Add status pages from file(s).
 - [x] Delete single status page by slug.
 - [x] Delete status page from file(s).
 
 ### Notification
 
 - Supported notification providers (tested)
+    [x] Opsgenie
   - [x] Rocket.Chat
   - [x] Slack
-  - [x] MS Teams
+  - [x] Teams
   - [x] Webhook
 - [x] List all `notification`(s).
 - [x] See details of a `single notification` by name/id.
 - [ ] Add new notification (interactive).
 - [x] Add notifications from single file.
 - [x] Delete notification by name.
 - [x] Delete notification by id.
```


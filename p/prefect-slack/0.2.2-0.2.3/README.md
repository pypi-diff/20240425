# Comparing `tmp/prefect-slack-0.2.2.tar.gz` & `tmp/prefect_slack-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-slack-0.2.2.tar", last modified: Wed Nov 29 19:53:27 2023, max compression
+gzip compressed data, was "prefect_slack-0.2.3.tar", last modified: Thu Apr 25 19:20:18 2024, max compression
```

## Comparing `prefect-slack-0.2.2.tar` & `prefect_slack-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/prefect_slack/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/prefect_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/prefect_slack/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/prefect_slack/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/prefect_slack/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/prefect_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2023-11-29 19:53:27.000000 prefect-slack-0.2.2/prefect_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-11-29 19:53:27.000000 prefect-slack-0.2.2/prefect_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:53:27.000000 prefect-slack-0.2.2/prefect_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-29 19:53:27.000000 prefect-slack-0.2.2/prefect_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-29 19:53:27.000000 prefect-slack-0.2.2/prefect_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-29 19:53:27.000000 prefect-slack-0.2.2/prefect_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:27.768370 prefect-slack-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-29 19:52:44.000000 prefect-slack-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.033281 prefect_slack-0.2.3/prefect_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/prefect_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/prefect_slack/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/prefect_slack/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/prefect_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 19:20:18.000000 prefect_slack-0.2.3/prefect_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 19:20:17.000000 prefect_slack-0.2.3/prefect_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:18.037281 prefect_slack-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 19:20:04.000000 prefect_slack-0.2.3/tests/test_version.py
```

### Comparing `prefect-slack-0.2.2/prefect_slack/messages.py` & `prefect_slack-0.2.3/prefect_slack/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Tasks for sending Slack messages."""
+"""Tasks for sending Slack messages"""
+
 from typing import TYPE_CHECKING, Dict, Optional, Sequence, Union
 
 from prefect import get_run_logger, task
-
 from prefect_slack.credentials import SlackCredentials, SlackWebhook
 
 if TYPE_CHECKING:  # pragma: no cover
     import slack_sdk.models.attachments
     import slack_sdk.models.blocks
 
 
@@ -19,38 +19,38 @@
         Sequence[Union[Dict, "slack_sdk.models.attachments.Attachment"]]
     ] = None,
     slack_blocks: Optional[
         Sequence[Union[Dict, "slack_sdk.models.blocks.Block"]]
     ] = None,
 ) -> Dict:
     """
-    Sends a message to a Slack channel.
+    Sends a message to a Slack channel
 
     Args:
-        channel: The name of the channel in which to post the chat messsage
-            (e.g. #general).
+        channel: The name of the channel in which to post the chat message
+            (e.g. #general)
         slack_credentials: Instance of `SlackCredentials` initialized with a Slack
-            bot token.
+            bot token
         text: Contents of the message. It's a best practice to always provide a `text`
             argument when posting a message. The `text` argument is used in places where
             content cannot be rendered such as: system push notifications, assistive
             technology such as screen readers, etc.
         attachments: List of objects defining secondary context in the posted Slack
             message. The [Slack API docs](https://api.slack.com/messaging/composing/layouts#building-attachments)
             provide guidance on building attachments.
         slack_blocks: List of objects defining the layout and formatting of the posted
             message. The [Slack API docs](https://api.slack.com/block-kit/building)
             provide guidance on building messages with blocks.
 
     Returns:
         Dict: Response from the Slack API. Example response structures can be found in
-            the [Slack API docs](https://api.slack.com/methods/chat.postMessage#examples).
+            the [Slack API docs](https://api.slack.com/methods/chat.postMessage#examples)
 
-    Example:
-        Post a message at the end of a flow run.
+    Examples:
+        Post a message at the end of a flow run
 
         ```python
         from prefect import flow
         from prefect.context import get_run_context
         from prefect_slack import SlackCredentials
         from prefect_slack.messages import send_chat_message
 
@@ -89,15 +89,15 @@
         Sequence[Union[Dict, "slack_sdk.models.attachments.Attachment"]]
     ] = None,
     slack_blocks: Optional[
         Sequence[Union[Dict, "slack_sdk.models.blocks.Block"]]
     ] = None,
 ) -> None:
     """
-    Sends a message via an incoming webhook.
+    Sends a message via an incoming webhook
 
     Args:
         slack_webhook: Instance of `SlackWebhook` initialized with a Slack
             webhook URL.
         text: Contents of the message. It's a best practice to always provide a `text`
             argument when posting a message. The `text` argument is used in places where
             content cannot be rendered such as: system push notifications, assistive
@@ -105,16 +105,16 @@
         attachments: List of objects defining secondary context in the posted Slack
             message. The [Slack API docs](https://api.slack.com/messaging/composing/layouts#building-attachments)
             provide guidance on building attachments.
         slack_blocks: List of objects defining the layout and formatting of the posted
             message. The [Slack API docs](https://api.slack.com/block-kit/building)
             provide guidance on building messages with blocks.
 
-    Example:
-        Post a message at the end of a flow run.
+    Examples:
+        Post a message at the end of a flow run
 
         ```python
         from prefect import flow
         from prefect_slack import SlackWebhook
         from prefect_slack.messages import send_incoming_webhook_message
```

### Comparing `prefect-slack-0.2.2/tests/test_messages.py` & `prefect_slack-0.2.3/tests/test_messages.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from itertools import product
 
 import pytest
-from prefect import flow
-
 from prefect_slack.messages import send_chat_message, send_incoming_webhook_message
 
+from prefect import flow
+
 CHANNELS = ["#random", "#general"]
 TEXT = ["hello", "goodbye"]
 ATTACHMENTS = [
     None,
     [
         {
             "text": "This is an attachment",
```


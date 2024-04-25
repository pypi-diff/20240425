# Comparing `tmp/ops_py_azure_key_vault_alert-4.6.1.tar.gz` & `tmp/ops_py_azure_key_vault_alert-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_alert-4.6.1.tar", last modified: Fri Apr 19 14:13:24 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_alert-4.7.0.tar", last modified: Thu Apr 25 07:30:27 2024, max compression
```

## Comparing `ops_py_azure_key_vault_alert-4.6.1.tar` & `ops_py_azure_key_vault_alert-4.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:13:24.499633 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8903 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1648 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/slack_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:30:27.942043 ops_py_azure_key_vault_alert-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 07:30:25.000000 ops_py_azure_key_vault_alert-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-25 07:30:27.942043 ops_py_azure_key_vault_alert-4.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:30:27.942043 ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-25 07:30:22.000000 ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10826 2024-04-25 07:30:22.000000 ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2531 2024-04-25 07:30:22.000000 ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/slack_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2281 2024-04-25 07:30:22.000000 ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/teams_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:30:27.942043 ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-25 07:30:27.000000 ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 07:30:27.000000 ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:30:27.000000 ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 07:30:27.000000 ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 07:30:27.000000 ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-25 07:30:25.000000 ops_py_azure_key_vault_alert-4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-25 07:30:25.000000 ops_py_azure_key_vault_alert-4.7.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 07:30:22.000000 ops_py_azure_key_vault_alert-4.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:30:27.942043 ops_py_azure_key_vault_alert-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 07:30:25.000000 ops_py_azure_key_vault_alert-4.7.0/setup.py
```

### Comparing `ops_py_azure_key_vault_alert-4.6.1/LICENSE` & `ops_py_azure_key_vault_alert-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/azure_key_vault_alert.py` & `ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import os
 import logging
 import argparse
 import json
+import re
 from azure_key_vault_report import azure_key_vault_report
 from azure_key_vault_report import az_cmd
 from message_handler import message_handler
 from .slack_post import slack_post
 from .teams_alert import teams_alert
 
 ########################################################################################################################
@@ -17,22 +18,22 @@
     logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
 
     # The list of key vaults to check passed as command line arguments
     parser = argparse.ArgumentParser()
     parser.add_argument("-v", "--vaults", nargs='+',
                         help="List of key vaults to check. E.g. kv-dev kv-test")
 
-    parser.add_argument("-c", "--critical_threshold", type=int,
+    parser.add_argument("-c", "--alert_threshold", type=int,
                         help="If set then only records that are +/- this value in days till expire/expired "
                              "will be alerted. Records will be alerted as individual Slack messages. "
                              "Summary report and other reports will not be posted.")
 
     parser.add_argument("-e", "--expire_threshold", type=int,
-                        help="If a value (int) is set. The days to the record's Expiration Date must be above "
-                             "this threshold (Default: not set)")
+                        help="If a value (int) is set. The days to the record's Expiration Date must be below "
+                             "this threshold in order to be included in the report (Default: not set).")
 
     parser.add_argument("-a", "--include_all", action='store_true',
                         help="Include all records in output (verbose) if provided.")
 
     parser.add_argument("-i", "--include_no_expiration", action='store_false',
                         help="Also include records which has no Expiration Date set.")
 
@@ -60,43 +61,47 @@
     parser.add_argument("-s", "--silence", action='store_true',
                         help="If provided the workflow will run and log, but no messages to Slack or MS Teams and "
                              "no print to stdout.")
 
     args = parser.parse_args()
     vaults = args.vaults
     expire_threshold = args.expire_threshold
-    critical_threshold = args.critical_threshold
+    alert_threshold = args.alert_threshold
     include_all = args.include_all
     ignore_no_expiration = args.include_no_expiration
     title = args.title
     record_types = args.record_types
     slack_split_chars = args.slack_split_chars
     teams_max_chars = args.teams_max_chars
     stdout_only = args.stdout_only
     workflow_output_file = args.workflow_output_file
     silence = args.silence
 
+    # Each argparse argument is logged
     for k, v in sorted(vars(args).items()):
         logging.info(f"Argument '{k}': '{v}'")
 
+    # Exit if no vaults are specified
     if not vaults:
         logging.error("No vaults specified.")
         exit(2)
 
-    # If only one key vault to check, it is ensured that it is treated as a list
+    # If only one key vault to check, ensure it is treated as a list
     if isinstance(vaults, str):
         vaults = [vaults]
 
     # The different kind of alert outputs are initially set to False.
     # Will be updated according to value of WEBHOOK_REPORT
+    # Success is also set to False and will only be True if one or more messages are posted.
     slack_app = False
     teams_output = False
     msg_handler = None
     success = False
 
+    # Determines if a webhook is set, and if it is for a Slack App or a Slack Workflow. If not we assume for MS Teams.
     if not WEBHOOK_REPORT:
         logging.warning("'WEBHOOK_REPORT' not provided. Report will not be posted to message handler.")
     else:
         if "slack.com/services" in WEBHOOK_REPORT:
             logging.info("Slack services webhook detected.")
             slack_app = True
         elif "slack.com" not in WEBHOOK_REPORT:
@@ -113,65 +118,83 @@
     kv_report = azure_key_vault_report.AzureKeyVaultReport(az_results)
     kv_report.parse_results()
     kv_report.add_summary()
     kv_report.add_report(expire_threshold=expire_threshold,
                          ignore_no_expiration=ignore_no_expiration,
                          include_all=include_all,
                          teams_json=teams_output,
-                         critical_threshold=critical_threshold)
+                         critical_threshold=alert_threshold)
 
-    # Get the full report which will be logged for future references.
-    # Azure resource information are added.
+    # Get the full report which will be written to file, and may be used for future references (logging / monitoring).
+    # The name of the Workflow and Azure resource information are added to the json object.
     report_full = kv_report.get_report_full()
     if isinstance(report_full, dict):
         workflow_output_name = str(WORKFLOW_OUTPUT_NAME).strip().lower().replace(" ", "_")[:40]
         report_full["name"] = workflow_output_name
         report_full["client_id"] = AZURE_CLIENT_ID
         report_full["subscription_id"] = AZURE_SUBSCRIPTION_ID
         report_full["tenant_id"] = AZURE_TENANT_ID
 
-        # Write full report as json to file
-        if not isinstance(workflow_output_file, str):
+        # Ensure a valid filename is set. If that is not the case, then 'output.json' is used as default.
+        workflow_output_file = str(workflow_output_file.lower()).replace(" ", "_")
+        if not bool(re.match("^[a-z0-9_-]*$", workflow_output_file)):
             workflow_output_file = "output.json"
 
+        # Write full report as json to file
         with open(workflow_output_file, 'w') as f:
             json.dump(report_full, f)
 
+    # If the 'silence' argument is provided, then we are done once the json output file is written
     if silence:
         return
 
-    if stdout_only:
+    # If the 'stdout_only' argument is provided, the plain text markdown reports are printed to stdout, and then exit.
+    # If 'teams_output', the 'stdout_only' is handled by the 'teams_alert' function instead.
+    if stdout_only and not teams_output:
         report = kv_report.get_report_summary_markdown()
         print(title)
         print(report)
         return
 
     # Initializes the Message Handler
     if WEBHOOK_REPORT:
         msg_handler = message_handler.MessageHandler(WEBHOOK_REPORT)
 
-    if teams_output and not success:
+    # If the webhook is previously determined to be an MS Teams webhook, the teams_alert function is called
+    if teams_output:
         success = teams_alert(title, kv_report, teams_max_chars, stdout_only=stdout_only, msg_handler=msg_handler)
 
-    if msg_handler and not teams_output and not success:
-        if slack_app and not success:
-            if not isinstance(critical_threshold, int):
+    # If the webhook is previously determined NOT to be an MS Teams webhook
+    if msg_handler and not teams_output:
+
+        # If the webhook is previously determined to be a Slack App webhook
+        if slack_app:
+            if not isinstance(alert_threshold, int):
+                # If an 'alert_threshold' is NOT provided, Slack report payloads will be used
                 payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars)
             else:
+                # If an 'alert_threshold' is provided, Slack alert payloads will be used
                 payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, md=True)
 
+            # If payloads, the slack_post function is called
             if payloads:
                 success = slack_post(msg_handler, payloads=payloads)
 
-        if not slack_app and not isinstance(critical_threshold, int) and not success:
+        # Proceed if the webhook is previously determined to NOT be a Slack App webhook (but a Slack Workflow webhook)
+        # and no 'alert_threshold' is specified (Slack Workflow is not supported for this) and
+        # that we do not post if we already have a success from an earlier post.
+        if not slack_app and not isinstance(alert_threshold, int) and not success:
             posts = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, app=False)
             if posts:
+                # The slack_post function is called
                 success = slack_post(msg_handler, posts=posts)
 
-        if isinstance(critical_threshold, int) and not slack_app and not success:
+        # If the only option left is to post alert messages to a Slack Workflow (which is not supported),
+        # a message regarding info about not supported is posted instead.
+        if isinstance(alert_threshold, int) and not slack_app and not success:
             error_msg = "Posting individual critical messages to Slack Workflow is not supported."
             logging.error(error_msg)
             success = slack_post(msg_handler, posts=[(f"ERROR - {title}", error_msg)])
 
     # If success and 'WEBHOOK_NOTIFY' is provided
     # an additional notify will be posted to the 'WEBHOOK_NOTIFY' webhook
     if success and WEBHOOK_NOTIFY:
```

### Comparing `ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/teams_alert.py` & `ops_py_azure_key_vault_alert-4.7.0/azure_key_vault_alert/teams_alert.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,18 +45,19 @@
     if len(payload) > max_chars:
         warning_msg = f"The {title} length is above the character limit count of {max_chars}"
         logging.warning(warning_msg)
         title = f"WARNING! {warning_msg}"
         text = "The html report have been omitted from the report due to size limits."
         payload = kv.get_teams_payload(title, text=text)
 
-    # The payload is set and posted and return code set
+    # The payload is set and ready to be posted
     logging.info(f"Using payload: {payload}")
 
+    # Proceed with posting the payload to Message Handler if the 'msg_handler' was provided
     if msg_handler:
         msg_handler.set_payload(payload)
         msg_handler.post_payload()
         response_code = msg_handler.get_response_code()
 
         # Return True if response code is 200
         if isinstance(response_code, int) and response_code == 200:
-            return True
+            return True
```

### Comparing `ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/requires.txt` & `ops_py_azure_key_vault_alert-4.7.0/ops_py_azure_key_vault_alert.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-backports.tarfile==1.0.0
+backports.tarfile==1.1.1
 build==1.2.1
 certifi==2024.2.2
 charset-normalizer==3.3.2
-docutils==0.21.1
+docutils==0.21.2
 idna==3.6
 importlib_metadata==7.1.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
-jaraco.functools==4.0.0
+jaraco.functools==4.0.1
 keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
 ops-py-azure-key-vault-report==5.0.3
 ops-py-generate-pyproject==2.2.3
```

### Comparing `ops_py_azure_key_vault_alert-4.6.1/requirements.txt` & `ops_py_azure_key_vault_alert-4.7.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-backports.tarfile==1.0.0
+backports.tarfile==1.1.1
 build==1.2.1
 certifi==2024.2.2
 charset-normalizer==3.3.2
-docutils==0.21.1
+docutils==0.21.2
 idna==3.6
 importlib_metadata==7.1.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
-jaraco.functools==4.0.0
+jaraco.functools==4.0.1
 keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
 ops-py-azure-key-vault-report==5.0.3
 ops-py-generate-pyproject==2.2.3
```


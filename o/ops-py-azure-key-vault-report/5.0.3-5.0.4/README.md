# Comparing `tmp/ops_py_azure_key_vault_report-5.0.3.tar.gz` & `tmp/ops_py_azure_key_vault_report-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_report-5.0.3.tar", last modified: Fri Apr 19 13:57:41 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_report-5.0.4.tar", last modified: Thu Apr 25 09:24:29 2024, max compression
```

## Comparing `ops_py_azure_key_vault_report-5.0.3.tar` & `ops_py_azure_key_vault_report-5.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:41.855461 ops_py_azure_key_vault_report-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-19 13:57:41.855461 ops_py_azure_key_vault_report-5.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:41.851461 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25592 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/set_timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7390 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/slack_payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:41.851461 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:57:41.855461 ops_py_azure_key_vault_report-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:24:29.385945 ops_py_azure_key_vault_report-5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 09:24:26.000000 ops_py_azure_key_vault_report-5.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-25 09:24:29.385945 ops_py_azure_key_vault_report-5.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:24:29.381945 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25559 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/set_timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7390 2024-04-25 09:24:19.000000 ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/slack_payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:24:29.385945 ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-25 09:24:29.000000 ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 09:24:29.000000 ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:24:29.000000 ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 09:24:29.000000 ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 09:24:26.000000 ops_py_azure_key_vault_report-5.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-25 09:24:26.000000 ops_py_azure_key_vault_report-5.0.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:24:29.385945 ops_py_azure_key_vault_report-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 09:24:26.000000 ops_py_azure_key_vault_report-5.0.4/setup.py
```

### Comparing `ops_py_azure_key_vault_report-5.0.3/LICENSE` & `ops_py_azure_key_vault_report-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/PKG-INFO` & `ops_py_azure_key_vault_report-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 5.0.3
+Version: 5.0.4
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 5.0.3
+Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 5.0.4
 Summary: Output a Key Vault Secrets report License: MIT License Copyright (c)
 2024 Equinor Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/az_cmd.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/azure_key_vault_report.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
                     continue
 
             # If the record has Expiration Date set, check if it should be alerted and/or reported on
             if isinstance(expires_age, int):
 
                 # The record has not expired yet, but it is logged.
                 if expires_age < 0:
-                    logging.info(f"{record_name} has not expired yet. "
+                    logging.info(f"{record_name} - has not expired yet. "
                                  f"It will expire in {abs(expires_age)} days ({expires}).")
 
                 # Check if soon expiring OR expired recently (the critical_threshold range)
                 # If so, a Slack Markdown Payload of current row will be created
                 # and added to the list of Slack Markdown payloads,
                 if isinstance(critical_threshold, int):
                     slack_md = False
@@ -415,32 +415,31 @@
                         logging.info(f"{record_name} - critical_threshold is set to '{critical_threshold}'.")
                         logging.info(f"{record_name} - will be alerted to Slack.")
                         slack_md_payload = self.get_slack_md(row)
                         if slack_md_payload:
                             logging.info(f"{record_name} - Slack Markdown payload created.")
                             self.slack_rows_md.append(slack_md_payload)
 
-                    # Handle those within the valid 'expire_threshold' range
-                    # Those record will not be included in the standard report.
-                    # They will only be included in the full report or if 'include_all' is set to True
-                    if isinstance(expire_threshold, int) and expire_threshold < abs(expires_age):
-                        logging.info(
-                            f"'{record_name}' - Expiration Date is within the valid specified threshold of "
-                            f"{expire_threshold} days. This record will start to be "
-                            f"reported in {abs(expires_age) - expire_threshold} days.")
-
-                        # This record is within the valid 'expire_threshold' range so the loop will
-                        # not proceed with adding the row the list of rows
-                        # unless if 'include_all' is set to True, then the row will be added.
-                        if not include_all:
-                            continue
+                # Handle those within the valid 'expire_threshold' range
+                # Those record will not be included in the standard report.
+                # They will only be included in the full report or if 'include_all' is set to True
+                if isinstance(expire_threshold, int) and expire_threshold < abs(expires_age) and expires_age > 0:
+                    logging.info(
+                        f"{record_name} - Expiration Date is within the valid specified threshold of "
+                        f"{expire_threshold} days. This record will start to be "
+                        f"reported in {abs(expires_age) - expire_threshold} days.")
+
+                    # This record is within the valid 'expire_threshold' range so the loop will
+                    # not proceed with adding the row the list of rows
+                    # unless if 'include_all' is set to True, then the row will be added.
+                    if not include_all:
+                        continue
 
             # Then finally add the row to the rows which will be reported on
             rows.append(row)
-
             # If the teams_json argument was set to True, a html_table was created.
             # If so, then the row is also added to the html table, which are used in the MS Teams payload.
             if self.html_table:
                 self.html_table.add_html_row(*row)
 
         ################################################################################################################
         # All the rows are now processed. Only the wanted rows are kept and will be used to create the reports
```

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/config.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/config.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/html_table.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/html_table.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/markdown.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/markdown.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/ms_teams_json.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/set_timestamp.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/slack_payloads.py` & `ops_py_azure_key_vault_report-5.0.4/azure_key_vault_report/slack_payloads.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/PKG-INFO` & `ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 5.0.3
+Version: 5.0.4
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 5.0.3
+Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 5.0.4
 Summary: Output a Key Vault Secrets report License: MIT License Copyright (c)
 2024 Equinor Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops_py_azure_key_vault_report-5.0.4/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.3/readme.md` & `ops_py_azure_key_vault_report-5.0.4/readme.md`

 * *Files identical despite different names*


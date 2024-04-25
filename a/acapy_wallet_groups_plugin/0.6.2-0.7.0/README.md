# Comparing `tmp/acapy_wallet_groups_plugin-0.6.2.tar.gz` & `tmp/acapy_wallet_groups_plugin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapy_wallet_groups_plugin-0.6.2.tar", max compression
+gzip compressed data, was "acapy_wallet_groups_plugin-0.7.0.tar", max compression
```

## Comparing `acapy_wallet_groups_plugin-0.6.2.tar` & `acapy_wallet_groups_plugin-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11334 2024-02-05 15:34:25.025375 acapy_wallet_groups_plugin-0.6.2/LICENSE.md
--rw-r--r--   0        0        0      195 2024-02-05 15:34:25.025375 acapy_wallet_groups_plugin-0.6.2/acapy_wallet_groups_plugin/definition.py
--rw-r--r--   0        0        0     1420 2024-02-05 15:34:25.025375 acapy_wallet_groups_plugin-0.6.2/acapy_wallet_groups_plugin/v1_0/__init__.py
--rw-r--r--   0        0        0    10300 2024-02-05 15:34:25.025375 acapy_wallet_groups_plugin-0.6.2/acapy_wallet_groups_plugin/v1_0/routes.py
--rw-r--r--   0        0        0      522 2024-02-05 15:34:25.025375 acapy_wallet_groups_plugin-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 acapy_wallet_groups_plugin-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11334 2024-03-08 15:33:27.515241 acapy_wallet_groups_plugin-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0      195 2024-03-08 15:33:27.515241 acapy_wallet_groups_plugin-0.7.0/acapy_wallet_groups_plugin/definition.py
+-rw-r--r--   0        0        0     1420 2024-03-08 15:33:27.515241 acapy_wallet_groups_plugin-0.7.0/acapy_wallet_groups_plugin/v1_0/__init__.py
+-rw-r--r--   0        0        0    10525 2024-03-08 15:33:27.515241 acapy_wallet_groups_plugin-0.7.0/acapy_wallet_groups_plugin/v1_0/routes.py
+-rw-r--r--   0        0        0      522 2024-03-08 15:33:27.515241 acapy_wallet_groups_plugin-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 acapy_wallet_groups_plugin-0.7.0/PKG-INFO
```

### Comparing `acapy_wallet_groups_plugin-0.6.2/LICENSE.md` & `acapy_wallet_groups_plugin-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.6.2/acapy_wallet_groups_plugin/v1_0/__init__.py` & `acapy_wallet_groups_plugin-0.7.0/acapy_wallet_groups_plugin/v1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.6.2/acapy_wallet_groups_plugin/v1_0/routes.py` & `acapy_wallet_groups_plugin-0.7.0/acapy_wallet_groups_plugin/v1_0/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,14 +176,17 @@
     if label:
         settings["default_label"] = label
     if image_url:
         settings["image_url"] = image_url
     if key_derivation:  # allow lower levels to handle default
         settings["wallet.key_derivation_method"] = key_derivation
 
+    if group_id is not None:
+        settings["wallet.group_id"] = group_id  # add group_id to wallet settings
+
     try:
         multitenant_mgr = context.profile.inject(BaseMultitenantManager)
 
         wallet_record = await multitenant_mgr.create_wallet(
             settings, key_management_mode
         )
 
@@ -247,14 +250,18 @@
         settings["wallet.webhook_urls"] = wallet_webhook_urls
     if wallet_dispatch_type is not None:
         settings["wallet.dispatch_type"] = wallet_dispatch_type
     if label is not None:
         settings["default_label"] = label
     if image_url is not None:
         settings["image_url"] = image_url
+
+    if group_id is not None:
+        settings["wallet.group_id"] = group_id  # add group_id to wallet settings
+
     extra_subwallet_setting = get_extra_settings_dict_per_tenant(extra_settings)
     settings.update(extra_subwallet_setting)
 
     try:
         multitenant_mgr = context.profile.inject(BaseMultitenantManager)
         wallet_record = await multitenant_mgr.update_wallet(wallet_id, settings)
```

### Comparing `acapy_wallet_groups_plugin-0.6.2/pyproject.toml` & `acapy_wallet_groups_plugin-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acapy_wallet_groups_plugin"
-version = "0.6.2"
+version = "0.7.0"
 description = "Agent plugin to add a group id to a wallet"
 authors = ["Berend Sliedrecht <berend@animo.id>"]
 packages = [{ include = "acapy_wallet_groups_plugin" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0.0"
 aries-cloudagent = "0.11.0"
```

### Comparing `acapy_wallet_groups_plugin-0.6.2/PKG-INFO` & `acapy_wallet_groups_plugin-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapy_wallet_groups_plugin
-Version: 0.6.2
+Version: 0.7.0
 Summary: Agent plugin to add a group id to a wallet
 Author: Berend Sliedrecht
 Author-email: berend@animo.id
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


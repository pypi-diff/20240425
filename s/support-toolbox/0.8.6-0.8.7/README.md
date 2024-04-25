# Comparing `tmp/support-toolbox-0.8.6.tar.gz` & `tmp/support-toolbox-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "support-toolbox-0.8.6.tar", last modified: Thu Mar 14 22:59:42 2024, max compression
+gzip compressed data, was "support-toolbox-0.8.7.tar", last modified: Thu Apr 25 15:01:52 2024, max compression
```

## Comparing `support-toolbox-0.8.6.tar` & `support-toolbox-0.8.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:42.497202 support-toolbox-0.8.6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      249 2024-03-14 22:59:42.497202 support-toolbox-0.8.6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-14 22:59:42.497202 support-toolbox-0.8.6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:42.493203 support-toolbox-0.8.6/support_toolbox/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:42.493203 support-toolbox-0.8.6/support_toolbox/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4522 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/entitlements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/org.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2377 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/site.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2022 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/api/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:42.493203 support-toolbox-0.8.6/support_toolbox/app_handler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/app_handler/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/app_handler/app.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/app_handler/app_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/app_handler/auto_updater.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/app_handler/token_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/clear_user_layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/delete_users.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/deploy_browse_card.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/deploy_ctk_service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/deploy_integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18651 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/deploy_pi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/onboard_ctk_orgs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/revert_soft_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/update_saml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:42.497202 support-toolbox-0.8.6/support_toolbox/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/utils/api_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/utils/csv_to_iris.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6826 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/utils/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/utils/resource_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-03-14 22:59:34.000000 support-toolbox-0.8.6/support_toolbox/utils/saml_parser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-14 22:59:42.493203 support-toolbox-0.8.6/support_toolbox.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      249 2024-03-14 22:59:42.000000 support-toolbox-0.8.6/support_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-03-14 22:59:42.000000 support-toolbox-0.8.6/support_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-14 22:59:42.000000 support-toolbox-0.8.6/support_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-03-14 22:59:42.000000 support-toolbox-0.8.6/support_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-03-14 22:59:42.000000 support-toolbox-0.8.6/support_toolbox.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-03-14 22:59:42.000000 support-toolbox-0.8.6/support_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.849060 support-toolbox-0.8.7/support_toolbox/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.849060 support-toolbox-0.8.7/support_toolbox/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4522 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/entitlements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/org.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2377 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/site.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2022 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/support_toolbox/app_handler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/app.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/app_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/auto_updater.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/token_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/clear_user_layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/delete_users.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_browse_card.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_ctk_service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_integrations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_pi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/onboard_ctk_orgs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/revert_soft_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/update_saml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/support_toolbox/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/api_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/csv_to_iris.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6826 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/resource_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/saml_parser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/support_toolbox.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/top_level.txt
```

### Comparing `support-toolbox-0.8.6/README.md` & `support-toolbox-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/setup.py` & `support-toolbox-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/entitlements.py` & `support-toolbox-0.8.7/support_toolbox/api/entitlements.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/file.py` & `support-toolbox-0.8.7/support_toolbox/api/file.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/org.py` & `support-toolbox-0.8.7/support_toolbox/api/org.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/project.py` & `support-toolbox-0.8.7/support_toolbox/api/project.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/service_account.py` & `support-toolbox-0.8.7/support_toolbox/api/service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/site.py` & `support-toolbox-0.8.7/support_toolbox/api/site.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/api/user.py` & `support-toolbox-0.8.7/support_toolbox/api/user.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/app_handler/app.py` & `support-toolbox-0.8.7/support_toolbox/app_handler/app.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/app_handler/auto_updater.py` & `support-toolbox-0.8.7/support_toolbox/app_handler/auto_updater.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/app_handler/token_manager.py` & `support-toolbox-0.8.7/support_toolbox/app_handler/token_manager.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/clear_user_layer.py` & `support-toolbox-0.8.7/support_toolbox/clear_user_layer.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/delete_users.py` & `support-toolbox-0.8.7/support_toolbox/delete_users.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/deploy_browse_card.py` & `support-toolbox-0.8.7/support_toolbox/deploy_browse_card.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/deploy_ctk_service_account.py` & `support-toolbox-0.8.7/support_toolbox/deploy_ctk_service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/deploy_integrations.py` & `support-toolbox-0.8.7/support_toolbox/deploy_integrations.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/deploy_pi.py` & `support-toolbox-0.8.7/support_toolbox/deploy_pi.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from support_toolbox.api.org import authorize_access_to_org, deauthorize_access_to_org, validate_org_input
 from support_toolbox.onboard_ctk_orgs import deploy_ctk, CTK_STACK
 from support_toolbox.api.entitlements import update_org_entitlements, get_entitlements, get_default_values, update_default_plan, ORG_DEFAULT_ENTITLEMENTS, ORG_ADDON_ENTITLEMENTS, USER_DEFAULT_ENTITLEMENTS
 from support_toolbox.api.site import create_site
 from support_toolbox.api.service_account import deploy_service_accounts
 from support_toolbox.utils.metrics import deploy_metrics
 from support_toolbox.api.project import create_project, create_saved_query
+from support_toolbox.api.dataset import set_dataset_ingest
 
 # TODO: Remove if Service Account creation is sunset from deploy_pi
 # Get the path to the user's home directory
 user_home = os.path.expanduser("~")
 
 # Construct the full path to the configuration file
 tokens_file_path = os.path.join(user_home, ".tokens.ini")
@@ -181,15 +182,15 @@
         email = values["email"]
 
         create_user(api_url, admin_token, agent_id, display_name, email)
         update_user_roles(api_url, admin_token, agent_id, ALLOWED_SUPPORT_ROLES)
         authorize_access_to_org(api_url, admin_token, org_id="datadotworldsupport", party="agent:" + agent_id)
 
 
-def setup_implementation_project(admin_token, org_id, public_slug, visibility):
+def setup_implementation_project(api_url, admin_token, org_id, public_slug, visibility):
     IMPLEMENTATION_QUERIES = [
         {
             "name": "01. First Login",
             "content": """
     SELECT
     displayname as UserID,
     onboard_date as Firstlogin
@@ -418,14 +419,16 @@
     project_title = f"{public_slug} Implementation Project"
     create_project(admin_token, org_id, project_title, visibility, summary)
 
     project_id = project_title.replace(" ", "-").lower()
     for q in IMPLEMENTATION_QUERIES:
         create_saved_query(admin_token, q, org_id, project_id)
 
+    set_dataset_ingest(api_url, admin_token, org_id, project_id)
+
 
 def run():
     api_url = get_api_url_location()
 
     while True:
         user_input = input("Enter the URL slug: ")
         public_slug = sanitize_public_slug(user_input)
@@ -439,19 +442,19 @@
 
         if selection == 'y':
             entity_id = SAML_PLACEHOLDER['entity_id']
             sso_url = SAML_PLACEHOLDER['sso_url']
             x509_cert = SAML_PLACEHOLDER['x509_cert']
 
             # Create site
-            admin_token = input("Enter your active admin token for the community site to begin deployment: ")
+            admin_token = input("Enter your active adminToken to begin deployment (US-community/EU-admingatewayeu): ")
             create_site(admin_token, entity_id, public_slug, sso_url, x509_cert, api_url)
 
             # Get the users active admin_token to complete the deployment using Private APIs
-            admin_token = input(f"Enter your active admin token for the {public_slug} site: ")
+            admin_token = input(f"Enter your active adminToken for the {public_slug} site: ")
 
             # Configure site
             config_default_orgs(api_url, admin_token)
             config_default_org_plan(api_url, admin_token)
             config_default_user_plan(api_url, admin_token)
 
             # Deploy CTK using the entered 'main' org as the Display Name
@@ -479,15 +482,15 @@
 
             cleanup_site_creation(api_url, admin_token, metrics_org)
 
             print("Adding the Support Team to the PI...")
             add_support(api_url, admin_token)
 
             print("Setting up Implementation Project...")
-            setup_implementation_project(admin_token, "data-catalog-team", public_slug, "OPEN")
+            setup_implementation_project(api_url, admin_token, "data-catalog-team", public_slug, "OPEN")
             break
 
         # preview URL denied
         elif selection == 'n':
             continue
 
         else:
```

### Comparing `support-toolbox-0.8.6/support_toolbox/onboard_ctk_orgs.py` & `support-toolbox-0.8.7/support_toolbox/onboard_ctk_orgs.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/revert_soft_delete.py` & `support-toolbox-0.8.7/support_toolbox/revert_soft_delete.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/update_saml.py` & `support-toolbox-0.8.7/support_toolbox/update_saml.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/utils/api_url.py` & `support-toolbox-0.8.7/support_toolbox/utils/api_url.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/utils/metrics.py` & `support-toolbox-0.8.7/support_toolbox/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/utils/resource_type.py` & `support-toolbox-0.8.7/support_toolbox/utils/resource_type.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox/utils/saml_parser.py` & `support-toolbox-0.8.7/support_toolbox/utils/saml_parser.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.6/support_toolbox.egg-info/SOURCES.txt` & `support-toolbox-0.8.7/support_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/eam_b2c_helper-0.1.0.tar.gz` & `tmp/eam_b2c_helper-0.1.1.tar.gz`

## Comparing `eam_b2c_helper-0.1.0.tar` & `eam_b2c_helper-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/src/eam_b2c_helper/__init__.py
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/src/eam_b2c_helper/b2c.py
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/tests/test_b2c.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/LICENSE
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/README.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/src/eam_b2c_helper/__init__.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/src/eam_b2c_helper/b2c.py
+-rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/tests/test_b2c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/README.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 eam_b2c_helper-0.1.1/PKG-INFO
```

### Comparing `eam_b2c_helper-0.1.0/src/eam_b2c_helper/b2c.py` & `eam_b2c_helper-0.1.1/src/eam_b2c_helper/b2c.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import requests
 
 LOGGER = logging.getLogger("azure")
 LOGGER.setLevel(logging.WARN)
 
 
-def build_user_object(user_details: dict, extension_id: str, b2c_prefix: str) -> dict:
+def build_local_user_object(user_details: dict, b2c_prefix: str, extension_id: str) -> dict:
     """Builds a user object to be used in the creation or update of a user in Azure AD B2C"""
     if user_details['role'] == '8amAdmin':
         user_details['password'] = 'eightamAdmin!23'
     else:
         user_details['password'] = 'eightam!23'
 
     return {
@@ -34,88 +34,105 @@
         f"extension_{extension_id}_OrganizationID": user_details['company_id'],
         f"extension_{extension_id}_SignUpCode": user_details['sign_up_code'],
         f"extension_{extension_id}_UserRoles": user_details['role'],
         f"extension_{extension_id}_mustResetPassword": user_details['reset_password']
     }
 
 
+def build_federated_user_object(user_details: dict, extension_id: str) -> dict:
+    """Builds a federated user object to be used in the creation or update of a user in Azure AD B2C"""
+    return {
+        "accountEnabled": True,
+        "displayName": f"{user_details['firstName']} {user_details['lastName']}",
+        "mailNickname": user_details['firstName'],
+        "otherMails": [user_details['email']],
+        "mobilePhone": user_details['phone'],
+        f"extension_{extension_id}_OrganizationID": user_details['company_id'],
+        f"extension_{extension_id}_SignUpCode": user_details['sign_up_code'],
+        f"extension_{extension_id}_UserRoles": user_details['role'],
+        f"extension_{extension_id}_mustResetPassword": user_details['reset_password']
+    }
+
+
+def build_user_object(user_details: dict, extension_id: str, b2c_prefix: str) -> dict:
+    """Builds a user object to be used in the creation or update of a user in Azure AD B2C"""
+    if ('signInType' in user_details) and (user_details['signInType'] == 'federated'):
+        return build_federated_user_object(user_details, extension_id)
+    else:
+        return build_local_user_object(user_details, b2c_prefix, extension_id)
+
+
 class B2CHelper:
     """Class providing functionality to interact with Azure AD B2C via the Microsoft Graph API"""
+
     def __init__(self, token_request_data) -> None:
         self.token_request_data = {
             'grant_type': token_request_data['grant_type'],
             'client_id': token_request_data['user_mgmt_client_id'],
             'scope': token_request_data['scope'],
             'client_secret': token_request_data['user_mgmt_client_secret'],
             'b2c_tenant_id': token_request_data['tenant_id'],
             'extension_id': token_request_data['ext_app_client_id']
         }
 
-
     def get_token(self) -> str:
         """Gets an access token from Azure AD B2C
         using the token_request_data provided in the constructor."""
         return requests.post(
-            f"https://login.microsoftonline.com/" \
+            f"https://login.microsoftonline.com/"
             f"{self.token_request_data['b2c_tenant_id']}/oauth2/v2.0/token",
             data=self.token_request_data,
             timeout=30).json()['access_token']
 
-
     def get_auth_header(self) -> dict:
         """Returns a dictionary containing the authorization header"""
         return {
             'Authorization': f'Bearer {self.get_token()}',
             'Content-type': 'application/json',
         }
 
-
     @staticmethod
     def create_item(auth_header: dict, item: dict) -> requests.Response:
         """Creates a user in Azure AD B2C using the provided item and authorization header."""
         return requests.post(
             "https://graph.microsoft.com/beta/users",
             headers=auth_header,
             data=json.dumps(item),
             timeout=30
         )
 
-
     @staticmethod
     def update_item(auth_header: dict, item: dict, item_id: str) -> requests.Response:
         """Updates a user in Azure AD B2C using the provided item and authorization header."""
         del item['passwordProfile']
         return requests.patch(
             f"https://graph.microsoft.com/beta/users/{item_id}",
             headers=auth_header,
             data=json.dumps(item),
             timeout=30
         )
 
-
     @staticmethod
     def delete_item(auth_header: dict, user_id: dict) -> requests.Response:
         """Deletes a user in Azure AD B2C using the provided user_id and authorization header."""
         return requests.delete(
             f"https://graph.microsoft.com/beta/users/{user_id}",
             headers=auth_header,
             timeout=30
         )
 
-
     def get_user(self, user_id: str) -> dict:
         """Gets a user in Azure AD B2C using the provided user_id."""
         user = requests.get(
             f"https://graph.microsoft.com/beta/users/{user_id}", headers=self.get_auth_header(),
             timeout=30
         ).json()
         del user["@odata.context"]
         return user
 
-
     def compile_entire_user_list(self, filter_extension: str) -> list:
         """Compiles the entire list of users in Azure AD B2C using the provided filter_extension."""
         users = requests.get(
             f"https://graph.microsoft.com/beta/users{filter_extension}",
             headers=self.get_auth_header(),
             timeout=30
         )
@@ -138,80 +155,73 @@
             if '@odata.nextLink' in users_next.json():
                 next_link = users_next.json()["@odata.nextLink"]
             else:
                 next_link = None
 
         return return_list
 
-
     def get_users(self, company_id: str = None, role_type: str = None) -> list:
         """Gets a list of users in Azure AD B2C using the provided company_id or role_type."""
         if company_id is not None:
             filter_extension = f"?$filter=" \
-            f"extension_{self.token_request_data['extension_id']}_OrganizationID eq '{company_id}'"
+                f"extension_{self.token_request_data['extension_id']}_OrganizationID eq '{company_id}'"
 
             users = self.compile_entire_user_list(filter_extension)
 
         elif role_type is not None:
             filter_extension = f"?$filter=" \
-            f"extension_{self.token_request_data['extension_id']}_UserRoles eq '{role_type}'"
+                f"extension_{self.token_request_data['extension_id']}_UserRoles eq '{role_type}'"
             users = self.compile_entire_user_list(filter_extension)
         else:
             filter_extension = ''
             users = [
-                x for x in self.compile_entire_user_list(filter_extension) \
+                x for x in self.compile_entire_user_list(filter_extension)
                 if x['mailNickname'] != 'Daveg_8amsolutions.com#EXT#'
             ]
 
         return users
 
-
     def create_user(self, user_details: dict, b2c_prefix: str) -> dict:
         """Creates a user in Azure AD B2C using the provided user_details and b2c_prefix."""
         user = build_user_object(
             user_details, self.token_request_data['extension_id'], b2c_prefix)
         return self.create_item(self.get_auth_header(), user)
 
-
     def create_users(self, user_details_list: list, b2c_prefix: str) -> list:
         """Creates a list of users in Azure AD B2C
         using the provided user_details_list and b2c_prefix."""
         auth_header = self.get_auth_header()
         results = []
         for user_detail in user_details_list:
             user = build_user_object(
                 user_detail, self.token_request_data['extension_id'], b2c_prefix)
             results.append(self.create_item(auth_header, user))
         return results
 
-
     def update_user(self, user_details: dict, b2c_prefix: str) -> dict:
         """Updates a user in Azure AD B2C using the provided user_details and b2c_prefix."""
         user = build_user_object(
             user_details, self.token_request_data['extension_id'], b2c_prefix)
         return self.update_item(self.get_auth_header(), user, user_details['id'])
 
-
     def update_users(self, user_details_list: list, b2c_prefix: str) -> list:
         """Updates a list of users in Azure AD B2C"""
         auth_header = self.get_auth_header()
         results = []
         for user_detail in user_details_list:
             user = build_user_object(
                 user_detail, self.token_request_data['extension_id'], b2c_prefix)
             results.append(self.update_item(
                 auth_header, user, user_detail['id']))
         return results
 
-
     def delete_user(self, user_id: str) -> dict:
         """Deletes a user in Azure AD B2C using the provided user_id."""
         return self.delete_item(self.get_auth_header(), user_id)
 
-
     def delete_users(self, user_id_list) -> list:
         """Deletes a list of users in Azure AD B2C using the provided user_id_list."""
         auth_header = self.get_auth_header()
         results = []
         for user_id in user_id_list:
             results.append(self.delete_item(auth_header, user_id))
         return results
```

### Comparing `eam_b2c_helper-0.1.0/tests/test_b2c.py` & `eam_b2c_helper-0.1.1/tests/test_b2c.py`

 * *Files identical despite different names*

### Comparing `eam_b2c_helper-0.1.0/LICENSE` & `eam_b2c_helper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eam_b2c_helper-0.1.0/README.md` & `eam_b2c_helper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eam_b2c_helper-0.1.0/PKG-INFO` & `eam_b2c_helper-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: eam_b2c_helper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to interact with ms graph /users functionality
 Author-email: Dave Gunn <daveg@8amsolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```


# Comparing `tmp/trustauthx-0.8.1.tar.gz` & `tmp/trustauthx-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.8.1.tar", last modified: Thu Apr 18 14:36:46 2024, max compression
+gzip compressed data, was "trustauthx-0.8.3.tar", last modified: Thu Apr 25 15:31:15 2024, max compression
```

## Comparing `trustauthx-0.8.1.tar` & `trustauthx-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.079297 trustauthx-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 14:36:37.000000 trustauthx-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-18 14:36:46.079297 trustauthx-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-18 14:36:37.000000 trustauthx-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:36:46.079297 trustauthx-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-18 14:36:37.000000 trustauthx-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.075297 trustauthx-0.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 14:36:37.000000 trustauthx-0.8.1/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.079297 trustauthx-0.8.1/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41392 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-18 14:36:37.000000 trustauthx-0.8.1/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:36:46.079297 trustauthx-0.8.1/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 14:36:46.000000 trustauthx-0.8.1/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.623471 trustauthx-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:31:06.000000 trustauthx-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-25 15:31:15.623471 trustauthx-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-25 15:31:06.000000 trustauthx-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:31:15.623471 trustauthx-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-25 15:31:06.000000 trustauthx-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.619471 trustauthx-0.8.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 15:31:06.000000 trustauthx-0.8.3/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.623471 trustauthx-0.8.3/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41517 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-25 15:31:06.000000 trustauthx-0.8.3/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:15.623471 trustauthx-0.8.3/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 15:31:15.000000 trustauthx-0.8.3/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.8.1/LICENSE` & `trustauthx-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.1/PKG-INFO` & `trustauthx-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.8.1
+Version: 0.8.3
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.8.1/README.md` & `trustauthx-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.1/setup.py` & `trustauthx-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="trustauthx",
-    version="0.8.1",
+    version="0.8.3",
     description="Official connector SDK for TrustAuthx",
     long_description=long_description,
     long_description_content_type="text/markdown",  # This is important!
     author="moonlightnexus",
     author_email="nexus@trustauthx.com",
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.8.1/trustauthx/authlite.py` & `trustauthx-0.8.3/trustauthx/authlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,15 @@
             "rol_id": rol_id,
             "permissions": permissions,
         }
         response = requests.delete(
             url, headers=headers, params=params, data=json.dumps(data)
         )
         self.reinitialize_all(foreground)
-        return response.json()
+        return DeletePermissionResponse(**response.json())
 
 
 class AuthLiteClient:
     instances = []
     """
     AuthLiteClient is a Python client for the TrustAuthX authentication service.
 
@@ -597,14 +597,15 @@
         )
         self._secret_key = secret_key
         self._api_key = api_key
         self.org_id = org_id
         self._signed_key = self.jwt_encode(
             key=self._secret_key, data={"api_key": self._api_key}
         )
+        # print(f"{(self._api_key, self.org_id, self._signed_key)}")
         self.API_BASE_URL = API_BASE_URL
         self.in_memory = in_memory
         self.Roles: _Roles = _Roles(
             roles=self._set_edge_roles(),
             org_id=self.org_id,
             api_key=self._api_key,
             signed_key=self._signed_key,
@@ -713,17 +714,17 @@
         if response.status_code == 200:
             rtn = self.jwt_decode(self._secret_key, response.json())
             sub = json.loads(rtn["sub"])
             rtn.pop("sub")
             rtn["email"] = sub["email"]
             rtn["uid"] = sub["uid"]
             if not return_class:
-                return User(rtn).to_dict()
+                return rtn
             else:
-                return User(rtn)
+                return User(**rtn)
         else:
             raise HTTPError(
                 "Request failed with status code : {} \n this code contains a msg : {}".format(
                     response.status_code, response.text
                 )
             )
 
@@ -894,15 +895,16 @@
         headers = {"accept": "application/json"}
         params = {
             "org_id": f"{self.org_id}",
             "api_key": f"{self._api_key}",
             "signed_key": f"{self._signed_key}",
         }
         response = requests.get(url, headers=headers, params=params)
-        roles = [Role(**role_data) for role_data in response.json()]
+        response_text = response.json()
+        roles = [Role(**role_data) for role_data in response_text]
         roles = GetAllRolesResponse(
             roles_list=roles, roles_json_list=[asdict(role) for role in roles]
         )
         # print(roles.roles_json_list)
         return roles.roles_json_list
 
     def _re_init_roles(self) -> _Roles:
@@ -955,36 +957,36 @@
         }
         params = {
             "org_id": self.org_id,
             "api_key": self._api_key,
             "signed_key": self._signed_key,
         }
         rols = []
-        if isinstance(rol_ids) == str:
+        if isinstance(rol_ids, str):
             rols.append(rol_ids)
-        elif isinstance(rol_ids) == list:
+        elif isinstance(rol_ids, list):
             rols = [i for i in rol_ids]
         else:
             raise TypeError()
         data = {
             "uid": uid,
             "rol_id": rol_ids,
             "inplace": [],
             "signoff_session_and_assign": signoff_session_and_assign,
             "AccessToken": access_token,
             "RefreshToken": refresh_token,
         }
         response = requests.post(url, headers=headers, params=params, json=data)
-        if signoff_session_and_assign:
+        if not signoff_session_and_assign:
             return response.json()
         else:
             if return_class:
-                return SignOffSessionReplace(response.json())
+                return SignOffSessionReplace(**response.json())
             else:
-                return SignOffSessionReplace(response.json()).to_dict()
+                return SignOffSessionReplace(**response.json()).to_dict()
 
     def remove_role(
         self,
         uid: str,
         rol_ids: Union[str, list],
         signoff_session_and_assign=False,
         refresh_token=None,
@@ -1020,36 +1022,36 @@
         }
         params = {
             "org_id": self.org_id,
             "api_key": self._api_key,
             "signed_key": self._signed_key,
         }
         rols = []
-        if isinstance(rol_ids) == str:
+        if isinstance(rol_ids, str):
             rols.append(rol_ids)
-        elif isinstance(rol_ids) == list:
+        elif isinstance(rol_ids, list):
             rols = [i for i in rol_ids]
         else:
             raise TypeError()
         data = {
             "uid": uid,
             "rol_id": [],
             "inplace": rol_ids,
             "signoff_session_and_assign": signoff_session_and_assign,
             "AccessToken": access_token,
             "RefreshToken": refresh_token,
         }
         response = requests.post(url, headers=headers, params=params, json=data)
-        if signoff_session_and_assign:
+        if not signoff_session_and_assign:
             return response.json()
         else:
             if return_class:
-                return SignOffSessionReplace(response.json())
+                return SignOffSessionReplace(**response.json())
             else:
-                return SignOffSessionReplace(response.json()).to_dict()
+                return SignOffSessionReplace(**response.json()).to_dict()
 
     def update_role(
         self,
         uid: str,
         rol_ids_to_add: Union[str, list],
         rol_ids_to_remove: Union[str, list],
         signoff_session_and_assign=False,
@@ -1087,24 +1089,24 @@
         }
         params = {
             "org_id": self.org_id,
             "api_key": self._api_key,
             "signed_key": self._signed_key,
         }
         rols_add = []
-        if isinstance(rol_ids_to_add) == str:
+        if isinstance(rol_ids_to_add, str):
             rols_add.append(rol_ids_to_add)
-        elif isinstance(rol_ids_to_add) == list:
+        elif isinstance(rol_ids_to_add, list):
             rols_add = [i for i in rol_ids_to_add]
         else:
             raise TypeError()
         rols_rem = []
-        if isinstance(rol_ids_to_remove) == str:
+        if isinstance(rol_ids_to_remove, str):
             rols_rem.append(rol_ids_to_remove)
-        elif isinstance(rol_ids_to_remove) == list:
+        elif isinstance(rol_ids_to_remove, list):
             rols_rem = [i for i in rol_ids_to_remove]
         else:
             raise TypeError()
         data = {
             "uid": uid,
             "rol_id": rols_add,
             "inplace": rols_rem,
@@ -1113,10 +1115,10 @@
             "RefreshToken": refresh_token,
         }
         response = requests.post(url, headers=headers, params=params, json=data)
         if signoff_session_and_assign:
             return response.json()
         else:
             if return_class:
-                return SignOffSessionReplace(response.json())
+                return SignOffSessionReplace(**response.json())
             else:
-                return SignOffSessionReplace(response.json()).to_dict()
+                return SignOffSessionReplace(**response.json()).to_dict()
```

### Comparing `trustauthx-0.8.1/trustauthx/cli.py` & `trustauthx-0.8.3/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.1/trustauthx/llmai.py` & `trustauthx-0.8.3/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.1/trustauthx/scheme.py` & `trustauthx-0.8.3/trustauthx/scheme.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.8.1/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.8.3/trustauthx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.8.1
+Version: 0.8.3
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


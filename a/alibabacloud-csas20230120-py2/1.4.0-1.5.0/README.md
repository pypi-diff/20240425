# Comparing `tmp/alibabacloud_csas20230120_py2-1.4.0.tar.gz` & `tmp/alibabacloud_csas20230120_py2-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120_py2-1.4.0.tar", last modified: Mon Apr 15 03:01:33 2024, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120_py2-1.5.0.tar", last modified: Thu Apr 25 05:40:25 2024, max compression
```

## Comparing `alibabacloud_csas20230120_py2-1.4.0.tar` & `alibabacloud_csas20230120_py2-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68633 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   398633 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2024-04-15 03:01:33.000000 alibabacloud_csas20230120_py2-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)      648 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83714 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   464018 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-25 05:40:25.000000 alibabacloud_csas20230120_py2-1.5.0/setup.py
```

### Comparing `alibabacloud_csas20230120_py2-1.4.0/ChangeLog.md` & `alibabacloud_csas20230120_py2-1.5.0/ChangeLog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-15 Version: 1.4.0
+- Support API ListUsers.
+- Support API UpdateUsersStatus.
+
+
 2024-01-25 Version: 1.3.0
 - Generated python2 2023-01-20 for csas.
 
 2023-11-15 Version: 1.2.1
 - Generated python2 2023-01-20 for csas.
 
 2023-09-14 Version: 1.2.0
```

### Comparing `alibabacloud_csas20230120_py2-1.4.0/LICENSE` & `alibabacloud_csas20230120_py2-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.4.0/PKG-INFO` & `alibabacloud_csas20230120_py2-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120_py2
-Version: 1.4.0
+Version: 1.5.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120_py2-1.4.0/README-CN.md` & `alibabacloud_csas20230120_py2-1.5.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.4.0/README.md` & `alibabacloud_csas20230120_py2-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,14 +60,54 @@
             self.call_api(params, req, runtime)
         )
 
     def attach_application_2connector(self, request):
         runtime = util_models.RuntimeOptions()
         return self.attach_application_2connector_with_options(request, runtime)
 
+    def create_client_user_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.department_id):
+            query['DepartmentId'] = request.department_id
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.email):
+            query['Email'] = request.email
+        if not UtilClient.is_unset(request.idp_config_id):
+            query['IdpConfigId'] = request.idp_config_id
+        if not UtilClient.is_unset(request.mobile_number):
+            query['MobileNumber'] = request.mobile_number
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.username):
+            query['Username'] = request.username
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateClientUser',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.CreateClientUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_client_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_client_user_with_options(request, runtime)
+
     def create_dynamic_route_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
@@ -109,14 +149,44 @@
             self.call_api(params, req, runtime)
         )
 
     def create_dynamic_route(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_dynamic_route_with_options(request, runtime)
 
+    def create_idp_department_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.department_name):
+            query['DepartmentName'] = request.department_name
+        if not UtilClient.is_unset(request.idp_config_id):
+            query['IdpConfigId'] = request.idp_config_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateIdpDepartment',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.CreateIdpDepartmentResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_idp_department(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_idp_department_with_options(request, runtime)
+
     def create_private_access_application_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.addresses):
             body_flat['Addresses'] = request.addresses
         if not UtilClient.is_unset(request.description):
@@ -327,14 +397,42 @@
             self.call_api(params, req, runtime)
         )
 
     def create_user_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_user_group_with_options(request, runtime)
 
+    def delete_client_user_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.id):
+            query['Id'] = request.id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteClientUser',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.DeleteClientUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_client_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_client_user_with_options(request, runtime)
+
     def delete_dynamic_route_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dynamic_route_id):
             query['DynamicRouteId'] = request.dynamic_route_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
@@ -355,14 +453,44 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_dynamic_route(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_dynamic_route_with_options(request, runtime)
 
+    def delete_idp_department_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.department_id):
+            query['DepartmentId'] = request.department_id
+        if not UtilClient.is_unset(request.idp_config_id):
+            query['IdpConfigId'] = request.idp_config_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteIdpDepartment',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.DeleteIdpDepartmentResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_idp_department(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_idp_department_with_options(request, runtime)
+
     def delete_private_access_application_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
@@ -532,14 +660,62 @@
             self.call_api(params, req, runtime)
         )
 
     def detach_application_2connector(self, request):
         runtime = util_models.RuntimeOptions()
         return self.detach_application_2connector_with_options(request, runtime)
 
+    def get_active_idp_config_with_options(self, runtime):
+        req = open_api_models.OpenApiRequest()
+        params = open_api_models.Params(
+            action='GetActiveIdpConfig',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.GetActiveIdpConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_active_idp_config(self):
+        runtime = util_models.RuntimeOptions()
+        return self.get_active_idp_config_with_options(runtime)
+
+    def get_client_user_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetClientUser',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.GetClientUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_client_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_client_user_with_options(request, runtime)
+
     def get_dynamic_route_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -558,14 +734,40 @@
             self.call_api(params, req, runtime)
         )
 
     def get_dynamic_route(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_dynamic_route_with_options(request, runtime)
 
+    def get_idp_config_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetIdpConfig',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.GetIdpConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_idp_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_idp_config_with_options(request, runtime)
+
     def get_private_access_application_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -740,14 +942,40 @@
             self.call_api(params, req, runtime)
         )
 
     def list_applications_for_private_access_tag(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_applications_for_private_access_tag_with_options(request, runtime)
 
+    def list_client_users_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListClientUsers',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListClientUsersResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_client_users(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_client_users_with_options(request, runtime)
+
     def list_connectors_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -840,14 +1068,66 @@
             self.call_api(params, req, runtime)
         )
 
     def list_excessive_device_registration_applications(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_excessive_device_registration_applications_with_options(request, runtime)
 
+    def list_idp_configs_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListIdpConfigs',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListIdpConfigsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_idp_configs(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_idp_configs_with_options(request, runtime)
+
+    def list_idp_departments_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListIdpDepartments',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.ListIdpDepartmentsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_idp_departments(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_idp_departments_with_options(request, runtime)
+
     def list_polices_for_private_access_application_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -1334,14 +1614,112 @@
             self.call_api(params, req, runtime)
         )
 
     def list_users(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_users_with_options(request, runtime)
 
+    def update_client_user_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.department_id):
+            query['DepartmentId'] = request.department_id
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.email):
+            query['Email'] = request.email
+        if not UtilClient.is_unset(request.id):
+            query['Id'] = request.id
+        if not UtilClient.is_unset(request.mobile_number):
+            query['MobileNumber'] = request.mobile_number
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateClientUser',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.UpdateClientUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def update_client_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_client_user_with_options(request, runtime)
+
+    def update_client_user_password_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.id):
+            query['Id'] = request.id
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.username):
+            query['Username'] = request.username
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateClientUserPassword',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.UpdateClientUserPasswordResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def update_client_user_password(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_client_user_password_with_options(request, runtime)
+
+    def update_client_user_status_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.id):
+            query['Id'] = request.id
+        if not UtilClient.is_unset(request.status):
+            query['Status'] = request.status
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateClientUserStatus',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.UpdateClientUserStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def update_client_user_status(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_client_user_status_with_options(request, runtime)
+
     def update_dynamic_route_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
@@ -1420,14 +1798,46 @@
             self.call_api(params, req, runtime)
         )
 
     def update_excessive_device_registration_applications_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_excessive_device_registration_applications_status_with_options(request, runtime)
 
+    def update_idp_department_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.department_id):
+            query['DepartmentId'] = request.department_id
+        if not UtilClient.is_unset(request.department_name):
+            query['DepartmentName'] = request.department_name
+        if not UtilClient.is_unset(request.idp_config_id):
+            query['IdpConfigId'] = request.idp_config_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateIdpDepartment',
+            version='2023-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            csas_20230120_models.UpdateIdpDepartmentResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def update_idp_department(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.update_idp_department_with_options(request, runtime)
+
     def update_private_access_application_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.addresses):
             body_flat['Addresses'] = request.addresses
         if not UtilClient.is_unset(request.application_id):
```

### Comparing `alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -119,14 +119,134 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AttachApplication2ConnectorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateClientUserRequest(TeaModel):
+    def __init__(self, department_id=None, description=None, email=None, idp_config_id=None, mobile_number=None,
+                 password=None, username=None):
+        self.department_id = department_id  # type: str
+        self.description = description  # type: str
+        self.email = email  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+        self.mobile_number = mobile_number  # type: str
+        self.password = password  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateClientUserRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.mobile_number is not None:
+            result['MobileNumber'] = self.mobile_number
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('MobileNumber') is not None:
+            self.mobile_number = m.get('MobileNumber')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class CreateClientUserResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateClientUserResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateClientUserResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateClientUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateClientUserResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateClientUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateDynamicRouteRequest(TeaModel):
     def __init__(self, application_ids=None, application_type=None, description=None, dynamic_route_type=None,
                  name=None, next_hop=None, priority=None, region_ids=None, status=None, tag_ids=None):
         self.application_ids = application_ids  # type: list[str]
         self.application_type = application_type  # type: str
         self.description = description  # type: str
         self.dynamic_route_type = dynamic_route_type  # type: str
@@ -254,14 +374,108 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDynamicRouteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateIdpDepartmentRequest(TeaModel):
+    def __init__(self, department_name=None, idp_config_id=None):
+        self.department_name = department_name  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateIdpDepartmentRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_name is not None:
+            result['DepartmentName'] = self.department_name
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DepartmentName') is not None:
+            self.department_name = m.get('DepartmentName')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        return self
+
+
+class CreateIdpDepartmentResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateIdpDepartmentResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateIdpDepartmentResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateIdpDepartmentResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateIdpDepartmentResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateIdpDepartmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreatePrivateAccessApplicationRequestPortRanges(TeaModel):
     def __init__(self, begin=None, end=None):
         self.begin = begin  # type: int
         self.end = end  # type: int
 
     def validate(self):
         pass
@@ -1288,14 +1502,98 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteClientUserRequest(TeaModel):
+    def __init__(self, id=None):
+        self.id = id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteClientUserRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class DeleteClientUserResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteClientUserResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteClientUserResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteClientUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteClientUserResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteClientUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteDynamicRouteRequest(TeaModel):
     def __init__(self, dynamic_route_id=None):
         self.dynamic_route_id = dynamic_route_id  # type: str
 
     def validate(self):
         pass
 
@@ -1372,14 +1670,103 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteDynamicRouteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteIdpDepartmentRequest(TeaModel):
+    def __init__(self, department_id=None, idp_config_id=None):
+        self.department_id = department_id  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteIdpDepartmentRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        return self
+
+
+class DeleteIdpDepartmentResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteIdpDepartmentResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteIdpDepartmentResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteIdpDepartmentResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteIdpDepartmentResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteIdpDepartmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeletePrivateAccessApplicationRequest(TeaModel):
     def __init__(self, application_id=None):
         self.application_id = application_id  # type: str
 
     def validate(self):
         pass
 
@@ -1912,14 +2299,317 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DetachApplication2ConnectorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetActiveIdpConfigResponseBodyData(TeaModel):
+    def __init__(self, description=None, id=None, name=None, type=None):
+        self.description = description  # type: str
+        self.id = id  # type: str
+        self.name = name  # type: str
+        self.type = type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetActiveIdpConfigResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetActiveIdpConfigResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: GetActiveIdpConfigResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(GetActiveIdpConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetActiveIdpConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetActiveIdpConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetActiveIdpConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetActiveIdpConfigResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetActiveIdpConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetClientUserRequest(TeaModel):
+    def __init__(self, idp_config_id=None, username=None):
+        self.idp_config_id = idp_config_id  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetClientUserRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class GetClientUserResponseBodyDataDepartment(TeaModel):
+    def __init__(self, id=None, name=None):
+        self.id = id  # type: str
+        self.name = name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetClientUserResponseBodyDataDepartment, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class GetClientUserResponseBodyData(TeaModel):
+    def __init__(self, department=None, department_id=None, description=None, email=None, id=None,
+                 idp_config_id=None, mobile_number=None, status=None, user_id=None, username=None):
+        self.department = department  # type: GetClientUserResponseBodyDataDepartment
+        self.department_id = department_id  # type: str
+        self.description = description  # type: str
+        self.email = email  # type: str
+        self.id = id  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+        self.mobile_number = mobile_number  # type: str
+        self.status = status  # type: str
+        self.user_id = user_id  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        if self.department:
+            self.department.validate()
+
+    def to_map(self):
+        _map = super(GetClientUserResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department is not None:
+            result['Department'] = self.department.to_map()
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.mobile_number is not None:
+            result['MobileNumber'] = self.mobile_number
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Department') is not None:
+            temp_model = GetClientUserResponseBodyDataDepartment()
+            self.department = temp_model.from_map(m['Department'])
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('MobileNumber') is not None:
+            self.mobile_number = m.get('MobileNumber')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class GetClientUserResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: GetClientUserResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(GetClientUserResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetClientUserResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetClientUserResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetClientUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetClientUserResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetClientUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDynamicRouteRequest(TeaModel):
     def __init__(self, dynamic_route_id=None):
         self.dynamic_route_id = dynamic_route_id  # type: str
 
     def validate(self):
         pass
 
@@ -2084,14 +2774,219 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetDynamicRouteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetIdpConfigRequest(TeaModel):
+    def __init__(self, id=None):
+        self.id = id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetIdpConfigRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class GetIdpConfigResponseBodyData(TeaModel):
+    def __init__(self, access_key=None, access_key_secret=None, description=None, get_group_url=None, id=None,
+                 idp_metadata=None, mfa_config_type=None, mobile_login_type=None, mobile_mfa_config_type=None,
+                 multi_idp_info=None, name=None, pc_login_type=None, status=None, type=None, update_time=None, verify_aes_key=None,
+                 verify_token=None, verify_url=None):
+        # AccessKey ID
+        self.access_key = access_key  # type: str
+        # AccessKey Secret
+        self.access_key_secret = access_key_secret  # type: str
+        self.description = description  # type: str
+        self.get_group_url = get_group_url  # type: str
+        self.id = id  # type: str
+        self.idp_metadata = idp_metadata  # type: str
+        self.mfa_config_type = mfa_config_type  # type: str
+        self.mobile_login_type = mobile_login_type  # type: str
+        self.mobile_mfa_config_type = mobile_mfa_config_type  # type: str
+        self.multi_idp_info = multi_idp_info  # type: str
+        self.name = name  # type: str
+        self.pc_login_type = pc_login_type  # type: str
+        self.status = status  # type: str
+        self.type = type  # type: str
+        self.update_time = update_time  # type: str
+        self.verify_aes_key = verify_aes_key  # type: str
+        self.verify_token = verify_token  # type: str
+        self.verify_url = verify_url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetIdpConfigResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_key is not None:
+            result['AccessKey'] = self.access_key
+        if self.access_key_secret is not None:
+            result['AccessKeySecret'] = self.access_key_secret
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.get_group_url is not None:
+            result['GetGroupUrl'] = self.get_group_url
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.idp_metadata is not None:
+            result['IdpMetadata'] = self.idp_metadata
+        if self.mfa_config_type is not None:
+            result['MfaConfigType'] = self.mfa_config_type
+        if self.mobile_login_type is not None:
+            result['MobileLoginType'] = self.mobile_login_type
+        if self.mobile_mfa_config_type is not None:
+            result['MobileMfaConfigType'] = self.mobile_mfa_config_type
+        if self.multi_idp_info is not None:
+            result['MultiIdpInfo'] = self.multi_idp_info
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.pc_login_type is not None:
+            result['PcLoginType'] = self.pc_login_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.type is not None:
+            result['Type'] = self.type
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        if self.verify_aes_key is not None:
+            result['VerifyAesKey'] = self.verify_aes_key
+        if self.verify_token is not None:
+            result['VerifyToken'] = self.verify_token
+        if self.verify_url is not None:
+            result['VerifyUrl'] = self.verify_url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AccessKey') is not None:
+            self.access_key = m.get('AccessKey')
+        if m.get('AccessKeySecret') is not None:
+            self.access_key_secret = m.get('AccessKeySecret')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('GetGroupUrl') is not None:
+            self.get_group_url = m.get('GetGroupUrl')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdpMetadata') is not None:
+            self.idp_metadata = m.get('IdpMetadata')
+        if m.get('MfaConfigType') is not None:
+            self.mfa_config_type = m.get('MfaConfigType')
+        if m.get('MobileLoginType') is not None:
+            self.mobile_login_type = m.get('MobileLoginType')
+        if m.get('MobileMfaConfigType') is not None:
+            self.mobile_mfa_config_type = m.get('MobileMfaConfigType')
+        if m.get('MultiIdpInfo') is not None:
+            self.multi_idp_info = m.get('MultiIdpInfo')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('PcLoginType') is not None:
+            self.pc_login_type = m.get('PcLoginType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        if m.get('VerifyAesKey') is not None:
+            self.verify_aes_key = m.get('VerifyAesKey')
+        if m.get('VerifyToken') is not None:
+            self.verify_token = m.get('VerifyToken')
+        if m.get('VerifyUrl') is not None:
+            self.verify_url = m.get('VerifyUrl')
+        return self
+
+
+class GetIdpConfigResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: GetIdpConfigResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(GetIdpConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetIdpConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetIdpConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetIdpConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetIdpConfigResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetIdpConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetPrivateAccessApplicationRequest(TeaModel):
     def __init__(self, application_id=None):
         self.application_id = application_id  # type: str
 
     def validate(self):
         pass
 
@@ -3655,14 +4550,279 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListApplicationsForPrivateAccessTagResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListClientUsersRequest(TeaModel):
+    def __init__(self, current_page=None, department_id=None, email=None, idp_config_id=None, mobile_number=None,
+                 page_size=None, status=None, username=None):
+        self.current_page = current_page  # type: long
+        self.department_id = department_id  # type: str
+        self.email = email  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+        self.mobile_number = mobile_number  # type: str
+        self.page_size = page_size  # type: long
+        self.status = status  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListClientUsersRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.mobile_number is not None:
+            result['MobileNumber'] = self.mobile_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('MobileNumber') is not None:
+            self.mobile_number = m.get('MobileNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class ListClientUsersResponseBodyDataDataListDepartment(TeaModel):
+    def __init__(self, id=None, name=None):
+        self.id = id  # type: str
+        self.name = name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListClientUsersResponseBodyDataDataListDepartment, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class ListClientUsersResponseBodyDataDataList(TeaModel):
+    def __init__(self, department=None, department_id=None, description=None, email=None, id=None,
+                 idp_config_id=None, mobile_number=None, status=None, user_id=None, username=None):
+        self.department = department  # type: ListClientUsersResponseBodyDataDataListDepartment
+        self.department_id = department_id  # type: str
+        self.description = description  # type: str
+        self.email = email  # type: str
+        self.id = id  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+        self.mobile_number = mobile_number  # type: str
+        self.status = status  # type: str
+        self.user_id = user_id  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        if self.department:
+            self.department.validate()
+
+    def to_map(self):
+        _map = super(ListClientUsersResponseBodyDataDataList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department is not None:
+            result['Department'] = self.department.to_map()
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.mobile_number is not None:
+            result['MobileNumber'] = self.mobile_number
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Department') is not None:
+            temp_model = ListClientUsersResponseBodyDataDataListDepartment()
+            self.department = temp_model.from_map(m['Department'])
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('MobileNumber') is not None:
+            self.mobile_number = m.get('MobileNumber')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class ListClientUsersResponseBodyData(TeaModel):
+    def __init__(self, data_list=None, total_num=None):
+        self.data_list = data_list  # type: list[ListClientUsersResponseBodyDataDataList]
+        self.total_num = total_num  # type: long
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListClientUsersResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DataList'] = []
+        if self.data_list is not None:
+            for k in self.data_list:
+                result['DataList'].append(k.to_map() if k else None)
+        if self.total_num is not None:
+            result['TotalNum'] = self.total_num
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.data_list = []
+        if m.get('DataList') is not None:
+            for k in m.get('DataList'):
+                temp_model = ListClientUsersResponseBodyDataDataList()
+                self.data_list.append(temp_model.from_map(k))
+        if m.get('TotalNum') is not None:
+            self.total_num = m.get('TotalNum')
+        return self
+
+
+class ListClientUsersResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: ListClientUsersResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(ListClientUsersResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ListClientUsersResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListClientUsersResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListClientUsersResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListClientUsersResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListClientUsersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListConnectorsRequest(TeaModel):
     def __init__(self, connector_ids=None, current_page=None, name=None, page_size=None, status=None,
                  switch_status=None):
         self.connector_ids = connector_ids  # type: list[str]
         self.current_page = current_page  # type: int
         self.name = name  # type: str
         self.page_size = page_size  # type: int
@@ -4488,14 +5648,399 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListExcessiveDeviceRegistrationApplicationsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListIdpConfigsRequest(TeaModel):
+    def __init__(self, current_page=None, include=None, page_size=None):
+        self.current_page = current_page  # type: long
+        self.include = include  # type: str
+        self.page_size = page_size  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListIdpConfigsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.include is not None:
+            result['Include'] = self.include
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('Include') is not None:
+            self.include = m.get('Include')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        return self
+
+
+class ListIdpConfigsResponseBodyDataDataList(TeaModel):
+    def __init__(self, description=None, id=None, mfa=None, mobile_login_type=None, mobile_mfa_config_type=None,
+                 multi_idp_info=None, name=None, pc_login_type=None, status=None, type=None, update_time=None):
+        self.description = description  # type: str
+        self.id = id  # type: str
+        self.mfa = mfa  # type: str
+        self.mobile_login_type = mobile_login_type  # type: str
+        self.mobile_mfa_config_type = mobile_mfa_config_type  # type: str
+        self.multi_idp_info = multi_idp_info  # type: str
+        self.name = name  # type: str
+        self.pc_login_type = pc_login_type  # type: str
+        self.status = status  # type: str
+        self.type = type  # type: str
+        self.update_time = update_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListIdpConfigsResponseBodyDataDataList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.mfa is not None:
+            result['Mfa'] = self.mfa
+        if self.mobile_login_type is not None:
+            result['MobileLoginType'] = self.mobile_login_type
+        if self.mobile_mfa_config_type is not None:
+            result['MobileMfaConfigType'] = self.mobile_mfa_config_type
+        if self.multi_idp_info is not None:
+            result['MultiIdpInfo'] = self.multi_idp_info
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.pc_login_type is not None:
+            result['PcLoginType'] = self.pc_login_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.type is not None:
+            result['Type'] = self.type
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Mfa') is not None:
+            self.mfa = m.get('Mfa')
+        if m.get('MobileLoginType') is not None:
+            self.mobile_login_type = m.get('MobileLoginType')
+        if m.get('MobileMfaConfigType') is not None:
+            self.mobile_mfa_config_type = m.get('MobileMfaConfigType')
+        if m.get('MultiIdpInfo') is not None:
+            self.multi_idp_info = m.get('MultiIdpInfo')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('PcLoginType') is not None:
+            self.pc_login_type = m.get('PcLoginType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        return self
+
+
+class ListIdpConfigsResponseBodyData(TeaModel):
+    def __init__(self, data_list=None, total_num=None):
+        self.data_list = data_list  # type: list[ListIdpConfigsResponseBodyDataDataList]
+        self.total_num = total_num  # type: long
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListIdpConfigsResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DataList'] = []
+        if self.data_list is not None:
+            for k in self.data_list:
+                result['DataList'].append(k.to_map() if k else None)
+        if self.total_num is not None:
+            result['TotalNum'] = self.total_num
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.data_list = []
+        if m.get('DataList') is not None:
+            for k in m.get('DataList'):
+                temp_model = ListIdpConfigsResponseBodyDataDataList()
+                self.data_list.append(temp_model.from_map(k))
+        if m.get('TotalNum') is not None:
+            self.total_num = m.get('TotalNum')
+        return self
+
+
+class ListIdpConfigsResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: ListIdpConfigsResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(ListIdpConfigsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ListIdpConfigsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListIdpConfigsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListIdpConfigsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListIdpConfigsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListIdpConfigsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListIdpDepartmentsRequest(TeaModel):
+    def __init__(self, current_page=None, idp_config_id=None, page_size=None):
+        self.current_page = current_page  # type: long
+        self.idp_config_id = idp_config_id  # type: str
+        self.page_size = page_size  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListIdpDepartmentsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page is not None:
+            result['CurrentPage'] = self.current_page
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CurrentPage') is not None:
+            self.current_page = m.get('CurrentPage')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        return self
+
+
+class ListIdpDepartmentsResponseBodyDataDataList(TeaModel):
+    def __init__(self, id=None, idp_config_id=None, name=None):
+        self.id = id  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+        self.name = name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListIdpDepartmentsResponseBodyDataDataList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class ListIdpDepartmentsResponseBodyData(TeaModel):
+    def __init__(self, data_list=None, total_num=None):
+        self.data_list = data_list  # type: list[ListIdpDepartmentsResponseBodyDataDataList]
+        self.total_num = total_num  # type: long
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListIdpDepartmentsResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DataList'] = []
+        if self.data_list is not None:
+            for k in self.data_list:
+                result['DataList'].append(k.to_map() if k else None)
+        if self.total_num is not None:
+            result['TotalNum'] = self.total_num
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.data_list = []
+        if m.get('DataList') is not None:
+            for k in m.get('DataList'):
+                temp_model = ListIdpDepartmentsResponseBodyDataDataList()
+                self.data_list.append(temp_model.from_map(k))
+        if m.get('TotalNum') is not None:
+            self.total_num = m.get('TotalNum')
+        return self
+
+
+class ListIdpDepartmentsResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: ListIdpDepartmentsResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(ListIdpDepartmentsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ListIdpDepartmentsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListIdpDepartmentsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListIdpDepartmentsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListIdpDepartmentsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListIdpDepartmentsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListPolicesForPrivateAccessApplicationRequest(TeaModel):
     def __init__(self, application_ids=None):
         self.application_ids = application_ids  # type: list[str]
 
     def validate(self):
         pass
 
@@ -8793,14 +10338,301 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateClientUserRequest(TeaModel):
+    def __init__(self, department_id=None, description=None, email=None, id=None, mobile_number=None):
+        self.department_id = department_id  # type: str
+        self.description = description  # type: str
+        self.email = email  # type: str
+        self.id = id  # type: str
+        self.mobile_number = mobile_number  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateClientUserRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.mobile_number is not None:
+            result['MobileNumber'] = self.mobile_number
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('MobileNumber') is not None:
+            self.mobile_number = m.get('MobileNumber')
+        return self
+
+
+class UpdateClientUserResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateClientUserResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateClientUserResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateClientUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateClientUserResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateClientUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateClientUserPasswordRequest(TeaModel):
+    def __init__(self, id=None, password=None, username=None):
+        self.id = id  # type: str
+        self.password = password  # type: str
+        self.username = username  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateClientUserPasswordRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.username is not None:
+            result['Username'] = self.username
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class UpdateClientUserPasswordResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateClientUserPasswordResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateClientUserPasswordResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateClientUserPasswordResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateClientUserPasswordResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateClientUserPasswordResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateClientUserStatusRequest(TeaModel):
+    def __init__(self, id=None, status=None):
+        self.id = id  # type: str
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateClientUserStatusRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class UpdateClientUserStatusResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateClientUserStatusResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateClientUserStatusResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateClientUserStatusResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateClientUserStatusResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateClientUserStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateDynamicRouteRequest(TeaModel):
     def __init__(self, application_ids=None, application_type=None, description=None, dynamic_route_id=None,
                  dynamic_route_type=None, modify_type=None, name=None, next_hop=None, priority=None, region_ids=None, status=None,
                  tag_ids=None):
         self.application_ids = application_ids  # type: list[str]
         self.application_type = application_type  # type: str
         self.description = description  # type: str
@@ -9116,14 +10948,108 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateExcessiveDeviceRegistrationApplicationsStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateIdpDepartmentRequest(TeaModel):
+    def __init__(self, department_id=None, department_name=None, idp_config_id=None):
+        self.department_id = department_id  # type: str
+        self.department_name = department_name  # type: str
+        self.idp_config_id = idp_config_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateIdpDepartmentRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.department_id is not None:
+            result['DepartmentId'] = self.department_id
+        if self.department_name is not None:
+            result['DepartmentName'] = self.department_name
+        if self.idp_config_id is not None:
+            result['IdpConfigId'] = self.idp_config_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('DepartmentName') is not None:
+            self.department_name = m.get('DepartmentName')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        return self
+
+
+class UpdateIdpDepartmentResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateIdpDepartmentResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateIdpDepartmentResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateIdpDepartmentResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateIdpDepartmentResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateIdpDepartmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdatePrivateAccessApplicationRequestPortRanges(TeaModel):
     def __init__(self, begin=None, end=None):
         self.begin = begin  # type: int
         self.end = end  # type: int
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_csas20230120_py2-1.4.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO` & `alibabacloud_csas20230120_py2-1.5.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120-py2
-Version: 1.4.0
+Version: 1.5.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120_py2-1.4.0/setup.py` & `alibabacloud_csas20230120_py2-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120_py2.
 
-Created on 15/04/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python2"
```


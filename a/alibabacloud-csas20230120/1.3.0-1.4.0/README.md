# Comparing `tmp/alibabacloud_csas20230120-1.3.0.tar.gz` & `tmp/alibabacloud_csas20230120-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120-1.3.0.tar", last modified: Mon Apr 15 03:02:10 2024, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120-1.4.0.tar", last modified: Thu Apr 25 05:40:29 2024, max compression
```

## Comparing `alibabacloud_csas20230120-1.3.0.tar` & `alibabacloud_csas20230120-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      489 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171706 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   393460 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2024-04-15 03:02:10.000000 alibabacloud_csas20230120-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   210038 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   458459 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/setup.py
```

### Comparing `alibabacloud_csas20230120-1.3.0/LICENSE` & `alibabacloud_csas20230120-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.3.0/PKG-INFO` & `alibabacloud_csas20230120-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120-1.3.0/README-CN.md` & `alibabacloud_csas20230120-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.3.0/README.md` & `alibabacloud_csas20230120-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -119,14 +119,108 @@
     async def attach_application_2connector_async(
         self,
         request: csas_20230120_models.AttachApplication2ConnectorRequest,
     ) -> csas_20230120_models.AttachApplication2ConnectorResponse:
         runtime = util_models.RuntimeOptions()
         return await self.attach_application_2connector_with_options_async(request, runtime)
 
+    def create_client_user_with_options(
+        self,
+        request: csas_20230120_models.CreateClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.CreateClientUserResponse:
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
+    async def create_client_user_with_options_async(
+        self,
+        request: csas_20230120_models.CreateClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.CreateClientUserResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_client_user(
+        self,
+        request: csas_20230120_models.CreateClientUserRequest,
+    ) -> csas_20230120_models.CreateClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_client_user_with_options(request, runtime)
+
+    async def create_client_user_async(
+        self,
+        request: csas_20230120_models.CreateClientUserRequest,
+    ) -> csas_20230120_models.CreateClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_client_user_with_options_async(request, runtime)
+
     def create_dynamic_route_with_options(
         self,
         request: csas_20230120_models.CreateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateDynamicRouteResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -231,14 +325,88 @@
     async def create_dynamic_route_async(
         self,
         request: csas_20230120_models.CreateDynamicRouteRequest,
     ) -> csas_20230120_models.CreateDynamicRouteResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_dynamic_route_with_options_async(request, runtime)
 
+    def create_idp_department_with_options(
+        self,
+        request: csas_20230120_models.CreateIdpDepartmentRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.CreateIdpDepartmentResponse:
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
+    async def create_idp_department_with_options_async(
+        self,
+        request: csas_20230120_models.CreateIdpDepartmentRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.CreateIdpDepartmentResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_idp_department(
+        self,
+        request: csas_20230120_models.CreateIdpDepartmentRequest,
+    ) -> csas_20230120_models.CreateIdpDepartmentResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_idp_department_with_options(request, runtime)
+
+    async def create_idp_department_async(
+        self,
+        request: csas_20230120_models.CreateIdpDepartmentRequest,
+    ) -> csas_20230120_models.CreateIdpDepartmentResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_idp_department_with_options_async(request, runtime)
+
     def create_private_access_application_with_options(
         self,
         request: csas_20230120_models.CreatePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessApplicationResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -737,14 +905,84 @@
     async def create_user_group_async(
         self,
         request: csas_20230120_models.CreateUserGroupRequest,
     ) -> csas_20230120_models.CreateUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_user_group_with_options_async(request, runtime)
 
+    def delete_client_user_with_options(
+        self,
+        request: csas_20230120_models.DeleteClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.DeleteClientUserResponse:
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
+    async def delete_client_user_with_options_async(
+        self,
+        request: csas_20230120_models.DeleteClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.DeleteClientUserResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_client_user(
+        self,
+        request: csas_20230120_models.DeleteClientUserRequest,
+    ) -> csas_20230120_models.DeleteClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_client_user_with_options(request, runtime)
+
+    async def delete_client_user_async(
+        self,
+        request: csas_20230120_models.DeleteClientUserRequest,
+    ) -> csas_20230120_models.DeleteClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_client_user_with_options_async(request, runtime)
+
     def delete_dynamic_route_with_options(
         self,
         request: csas_20230120_models.DeleteDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteDynamicRouteResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -807,14 +1045,88 @@
     async def delete_dynamic_route_async(
         self,
         request: csas_20230120_models.DeleteDynamicRouteRequest,
     ) -> csas_20230120_models.DeleteDynamicRouteResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_dynamic_route_with_options_async(request, runtime)
 
+    def delete_idp_department_with_options(
+        self,
+        request: csas_20230120_models.DeleteIdpDepartmentRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
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
+    async def delete_idp_department_with_options_async(
+        self,
+        request: csas_20230120_models.DeleteIdpDepartmentRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_idp_department(
+        self,
+        request: csas_20230120_models.DeleteIdpDepartmentRequest,
+    ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_idp_department_with_options(request, runtime)
+
+    async def delete_idp_department_async(
+        self,
+        request: csas_20230120_models.DeleteIdpDepartmentRequest,
+    ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_idp_department_with_options_async(request, runtime)
+
     def delete_private_access_application_with_options(
         self,
         request: csas_20230120_models.DeletePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessApplicationResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1245,14 +1557,130 @@
     async def detach_application_2connector_async(
         self,
         request: csas_20230120_models.DetachApplication2ConnectorRequest,
     ) -> csas_20230120_models.DetachApplication2ConnectorResponse:
         runtime = util_models.RuntimeOptions()
         return await self.detach_application_2connector_with_options_async(request, runtime)
 
+    def get_active_idp_config_with_options(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.GetActiveIdpConfigResponse:
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
+    async def get_active_idp_config_with_options_async(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.GetActiveIdpConfigResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_active_idp_config(self) -> csas_20230120_models.GetActiveIdpConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_active_idp_config_with_options(runtime)
+
+    async def get_active_idp_config_async(self) -> csas_20230120_models.GetActiveIdpConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_active_idp_config_with_options_async(runtime)
+
+    def get_client_user_with_options(
+        self,
+        request: csas_20230120_models.GetClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.GetClientUserResponse:
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
+    async def get_client_user_with_options_async(
+        self,
+        request: csas_20230120_models.GetClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.GetClientUserResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_client_user(
+        self,
+        request: csas_20230120_models.GetClientUserRequest,
+    ) -> csas_20230120_models.GetClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_client_user_with_options(request, runtime)
+
+    async def get_client_user_async(
+        self,
+        request: csas_20230120_models.GetClientUserRequest,
+    ) -> csas_20230120_models.GetClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_client_user_with_options_async(request, runtime)
+
     def get_dynamic_route_with_options(
         self,
         request: csas_20230120_models.GetDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetDynamicRouteResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -1311,14 +1739,80 @@
     async def get_dynamic_route_async(
         self,
         request: csas_20230120_models.GetDynamicRouteRequest,
     ) -> csas_20230120_models.GetDynamicRouteResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_dynamic_route_with_options_async(request, runtime)
 
+    def get_idp_config_with_options(
+        self,
+        request: csas_20230120_models.GetIdpConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.GetIdpConfigResponse:
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
+    async def get_idp_config_with_options_async(
+        self,
+        request: csas_20230120_models.GetIdpConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.GetIdpConfigResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_idp_config(
+        self,
+        request: csas_20230120_models.GetIdpConfigRequest,
+    ) -> csas_20230120_models.GetIdpConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_idp_config_with_options(request, runtime)
+
+    async def get_idp_config_async(
+        self,
+        request: csas_20230120_models.GetIdpConfigRequest,
+    ) -> csas_20230120_models.GetIdpConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_idp_config_with_options_async(request, runtime)
+
     def get_private_access_application_with_options(
         self,
         request: csas_20230120_models.GetPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetPrivateAccessApplicationResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -1773,14 +2267,80 @@
     async def list_applications_for_private_access_tag_async(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_applications_for_private_access_tag_with_options_async(request, runtime)
 
+    def list_client_users_with_options(
+        self,
+        request: csas_20230120_models.ListClientUsersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListClientUsersResponse:
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
+    async def list_client_users_with_options_async(
+        self,
+        request: csas_20230120_models.ListClientUsersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListClientUsersResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_client_users(
+        self,
+        request: csas_20230120_models.ListClientUsersRequest,
+    ) -> csas_20230120_models.ListClientUsersResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_client_users_with_options(request, runtime)
+
+    async def list_client_users_async(
+        self,
+        request: csas_20230120_models.ListClientUsersRequest,
+    ) -> csas_20230120_models.ListClientUsersResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_client_users_with_options_async(request, runtime)
+
     def list_connectors_with_options(
         self,
         request: csas_20230120_models.ListConnectorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListConnectorsResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -2021,14 +2581,146 @@
     async def list_excessive_device_registration_applications_async(
         self,
         request: csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsRequest,
     ) -> csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_excessive_device_registration_applications_with_options_async(request, runtime)
 
+    def list_idp_configs_with_options(
+        self,
+        request: csas_20230120_models.ListIdpConfigsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListIdpConfigsResponse:
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
+    async def list_idp_configs_with_options_async(
+        self,
+        request: csas_20230120_models.ListIdpConfigsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListIdpConfigsResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_idp_configs(
+        self,
+        request: csas_20230120_models.ListIdpConfigsRequest,
+    ) -> csas_20230120_models.ListIdpConfigsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_idp_configs_with_options(request, runtime)
+
+    async def list_idp_configs_async(
+        self,
+        request: csas_20230120_models.ListIdpConfigsRequest,
+    ) -> csas_20230120_models.ListIdpConfigsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_idp_configs_with_options_async(request, runtime)
+
+    def list_idp_departments_with_options(
+        self,
+        request: csas_20230120_models.ListIdpDepartmentsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListIdpDepartmentsResponse:
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
+    async def list_idp_departments_with_options_async(
+        self,
+        request: csas_20230120_models.ListIdpDepartmentsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.ListIdpDepartmentsResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_idp_departments(
+        self,
+        request: csas_20230120_models.ListIdpDepartmentsRequest,
+    ) -> csas_20230120_models.ListIdpDepartmentsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_idp_departments_with_options(request, runtime)
+
+    async def list_idp_departments_async(
+        self,
+        request: csas_20230120_models.ListIdpDepartmentsRequest,
+    ) -> csas_20230120_models.ListIdpDepartmentsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_idp_departments_with_options_async(request, runtime)
+
     def list_polices_for_private_access_application_with_options(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -3275,14 +3967,252 @@
     async def list_users_async(
         self,
         request: csas_20230120_models.ListUsersRequest,
     ) -> csas_20230120_models.ListUsersResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_users_with_options_async(request, runtime)
 
+    def update_client_user_with_options(
+        self,
+        request: csas_20230120_models.UpdateClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateClientUserResponse:
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
+    async def update_client_user_with_options_async(
+        self,
+        request: csas_20230120_models.UpdateClientUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateClientUserResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_client_user(
+        self,
+        request: csas_20230120_models.UpdateClientUserRequest,
+    ) -> csas_20230120_models.UpdateClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_client_user_with_options(request, runtime)
+
+    async def update_client_user_async(
+        self,
+        request: csas_20230120_models.UpdateClientUserRequest,
+    ) -> csas_20230120_models.UpdateClientUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_client_user_with_options_async(request, runtime)
+
+    def update_client_user_password_with_options(
+        self,
+        request: csas_20230120_models.UpdateClientUserPasswordRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
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
+    async def update_client_user_password_with_options_async(
+        self,
+        request: csas_20230120_models.UpdateClientUserPasswordRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_client_user_password(
+        self,
+        request: csas_20230120_models.UpdateClientUserPasswordRequest,
+    ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_client_user_password_with_options(request, runtime)
+
+    async def update_client_user_password_async(
+        self,
+        request: csas_20230120_models.UpdateClientUserPasswordRequest,
+    ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_client_user_password_with_options_async(request, runtime)
+
+    def update_client_user_status_with_options(
+        self,
+        request: csas_20230120_models.UpdateClientUserStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateClientUserStatusResponse:
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
+    async def update_client_user_status_with_options_async(
+        self,
+        request: csas_20230120_models.UpdateClientUserStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateClientUserStatusResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_client_user_status(
+        self,
+        request: csas_20230120_models.UpdateClientUserStatusRequest,
+    ) -> csas_20230120_models.UpdateClientUserStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_client_user_status_with_options(request, runtime)
+
+    async def update_client_user_status_async(
+        self,
+        request: csas_20230120_models.UpdateClientUserStatusRequest,
+    ) -> csas_20230120_models.UpdateClientUserStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_client_user_status_with_options_async(request, runtime)
+
     def update_dynamic_route_with_options(
         self,
         request: csas_20230120_models.UpdateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateDynamicRouteResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -3475,14 +4405,92 @@
     async def update_excessive_device_registration_applications_status_async(
         self,
         request: csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusRequest,
     ) -> csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.update_excessive_device_registration_applications_status_with_options_async(request, runtime)
 
+    def update_idp_department_with_options(
+        self,
+        request: csas_20230120_models.UpdateIdpDepartmentRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
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
+    async def update_idp_department_with_options_async(
+        self,
+        request: csas_20230120_models.UpdateIdpDepartmentRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_idp_department(
+        self,
+        request: csas_20230120_models.UpdateIdpDepartmentRequest,
+    ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.update_idp_department_with_options(request, runtime)
+
+    async def update_idp_department_async(
+        self,
+        request: csas_20230120_models.UpdateIdpDepartmentRequest,
+    ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.update_idp_department_with_options_async(request, runtime)
+
     def update_private_access_application_with_options(
         self,
         request: csas_20230120_models.UpdatePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdatePrivateAccessApplicationResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -136,14 +136,151 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AttachApplication2ConnectorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateClientUserRequest(TeaModel):
+    def __init__(
+        self,
+        department_id: str = None,
+        description: str = None,
+        email: str = None,
+        idp_config_id: str = None,
+        mobile_number: str = None,
+        password: str = None,
+        username: str = None,
+    ):
+        self.department_id = department_id
+        self.description = description
+        self.email = email
+        self.idp_config_id = idp_config_id
+        self.mobile_number = mobile_number
+        self.password = password
+        self.username = username
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: str = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateClientUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateClientUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         description: str = None,
         dynamic_route_type: str = None,
@@ -291,14 +428,121 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDynamicRouteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateIdpDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        department_name: str = None,
+        idp_config_id: str = None,
+    ):
+        self.department_name = department_name
+        self.idp_config_id = idp_config_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DepartmentName') is not None:
+            self.department_name = m.get('DepartmentName')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        return self
+
+
+class CreateIdpDepartmentResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: str = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateIdpDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateIdpDepartmentResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         begin: int = None,
         end: int = None,
     ):
         self.begin = begin
@@ -1468,14 +1712,109 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteClientUserRequest(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+    ):
+        self.id = id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class DeleteClientUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteClientUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteClientUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         dynamic_route_id: str = None,
     ):
         self.dynamic_route_id = dynamic_route_id
 
@@ -1563,14 +1902,115 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteDynamicRouteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteIdpDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        department_id: str = None,
+        idp_config_id: str = None,
+    ):
+        self.department_id = department_id
+        self.idp_config_id = idp_config_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DepartmentId') is not None:
+            self.department_id = m.get('DepartmentId')
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        return self
+
+
+class DeleteIdpDepartmentResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteIdpDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteIdpDepartmentResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         application_id: str = None,
     ):
         self.application_id = application_id
 
@@ -2174,14 +2614,360 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DetachApplication2ConnectorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetActiveIdpConfigResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        id: str = None,
+        name: str = None,
+        type: str = None,
+    ):
+        self.description = description
+        self.id = id
+        self.name = name
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: GetActiveIdpConfigResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetActiveIdpConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        idp_config_id: str = None,
+        username: str = None,
+    ):
+        self.idp_config_id = idp_config_id
+        self.username = username
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('IdpConfigId') is not None:
+            self.idp_config_id = m.get('IdpConfigId')
+        if m.get('Username') is not None:
+            self.username = m.get('Username')
+        return self
+
+
+class GetClientUserResponseBodyDataDepartment(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+        name: str = None,
+    ):
+        self.id = id
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class GetClientUserResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        department: GetClientUserResponseBodyDataDepartment = None,
+        department_id: str = None,
+        description: str = None,
+        email: str = None,
+        id: str = None,
+        idp_config_id: str = None,
+        mobile_number: str = None,
+        status: str = None,
+        user_id: str = None,
+        username: str = None,
+    ):
+        self.department = department
+        self.department_id = department_id
+        self.description = description
+        self.email = email
+        self.id = id
+        self.idp_config_id = idp_config_id
+        self.mobile_number = mobile_number
+        self.status = status
+        self.user_id = user_id
+        self.username = username
+
+    def validate(self):
+        if self.department:
+            self.department.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: GetClientUserResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetClientUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         dynamic_route_id: str = None,
     ):
         self.dynamic_route_id = dynamic_route_id
 
@@ -2370,14 +3156,248 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetDynamicRouteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetIdpConfigRequest(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+    ):
+        self.id = id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['Id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        return self
+
+
+class GetIdpConfigResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        access_key: str = None,
+        access_key_secret: str = None,
+        description: str = None,
+        get_group_url: str = None,
+        id: str = None,
+        idp_metadata: str = None,
+        mfa_config_type: str = None,
+        mobile_login_type: str = None,
+        mobile_mfa_config_type: str = None,
+        multi_idp_info: str = None,
+        name: str = None,
+        pc_login_type: str = None,
+        status: str = None,
+        type: str = None,
+        update_time: str = None,
+        verify_aes_key: str = None,
+        verify_token: str = None,
+        verify_url: str = None,
+    ):
+        # AccessKey ID
+        self.access_key = access_key
+        # AccessKey Secret
+        self.access_key_secret = access_key_secret
+        self.description = description
+        self.get_group_url = get_group_url
+        self.id = id
+        self.idp_metadata = idp_metadata
+        self.mfa_config_type = mfa_config_type
+        self.mobile_login_type = mobile_login_type
+        self.mobile_mfa_config_type = mobile_mfa_config_type
+        self.multi_idp_info = multi_idp_info
+        self.name = name
+        self.pc_login_type = pc_login_type
+        self.status = status
+        self.type = type
+        self.update_time = update_time
+        self.verify_aes_key = verify_aes_key
+        self.verify_token = verify_token
+        self.verify_url = verify_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: GetIdpConfigResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetIdpConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         application_id: str = None,
     ):
         self.application_id = application_id
 
@@ -4154,14 +5174,316 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListApplicationsForPrivateAccessTagResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListClientUsersRequest(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        department_id: str = None,
+        email: str = None,
+        idp_config_id: str = None,
+        mobile_number: str = None,
+        page_size: int = None,
+        status: str = None,
+        username: str = None,
+    ):
+        self.current_page = current_page
+        self.department_id = department_id
+        self.email = email
+        self.idp_config_id = idp_config_id
+        self.mobile_number = mobile_number
+        self.page_size = page_size
+        self.status = status
+        self.username = username
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        id: str = None,
+        name: str = None,
+    ):
+        self.id = id
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class ListClientUsersResponseBodyDataDataList(TeaModel):
+    def __init__(
+        self,
+        department: ListClientUsersResponseBodyDataDataListDepartment = None,
+        department_id: str = None,
+        description: str = None,
+        email: str = None,
+        id: str = None,
+        idp_config_id: str = None,
+        mobile_number: str = None,
+        status: str = None,
+        user_id: str = None,
+        username: str = None,
+    ):
+        self.department = department
+        self.department_id = department_id
+        self.description = description
+        self.email = email
+        self.id = id
+        self.idp_config_id = idp_config_id
+        self.mobile_number = mobile_number
+        self.status = status
+        self.user_id = user_id
+        self.username = username
+
+    def validate(self):
+        if self.department:
+            self.department.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data_list: List[ListClientUsersResponseBodyDataDataList] = None,
+        total_num: int = None,
+    ):
+        self.data_list = data_list
+        self.total_num = total_num
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: ListClientUsersResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListClientUsersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         connector_ids: List[str] = None,
         current_page: int = None,
         name: str = None,
         page_size: int = None,
@@ -5104,14 +6426,452 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListExcessiveDeviceRegistrationApplicationsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListIdpConfigsRequest(TeaModel):
+    def __init__(
+        self,
+        current_page: int = None,
+        include: str = None,
+        page_size: int = None,
+    ):
+        self.current_page = current_page
+        self.include = include
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        description: str = None,
+        id: str = None,
+        mfa: str = None,
+        mobile_login_type: str = None,
+        mobile_mfa_config_type: str = None,
+        multi_idp_info: str = None,
+        name: str = None,
+        pc_login_type: str = None,
+        status: str = None,
+        type: str = None,
+        update_time: str = None,
+    ):
+        self.description = description
+        self.id = id
+        self.mfa = mfa
+        self.mobile_login_type = mobile_login_type
+        self.mobile_mfa_config_type = mobile_mfa_config_type
+        self.multi_idp_info = multi_idp_info
+        self.name = name
+        self.pc_login_type = pc_login_type
+        self.status = status
+        self.type = type
+        self.update_time = update_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data_list: List[ListIdpConfigsResponseBodyDataDataList] = None,
+        total_num: int = None,
+    ):
+        self.data_list = data_list
+        self.total_num = total_num
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: ListIdpConfigsResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListIdpConfigsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        current_page: int = None,
+        idp_config_id: str = None,
+        page_size: int = None,
+    ):
+        self.current_page = current_page
+        self.idp_config_id = idp_config_id
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        id: str = None,
+        idp_config_id: str = None,
+        name: str = None,
+    ):
+        self.id = id
+        self.idp_config_id = idp_config_id
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data_list: List[ListIdpDepartmentsResponseBodyDataDataList] = None,
+        total_num: int = None,
+    ):
+        self.data_list = data_list
+        self.total_num = total_num
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        data: ListIdpDepartmentsResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListIdpDepartmentsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         application_ids: List[str] = None,
     ):
         self.application_ids = application_ids
 
@@ -9982,14 +11742,341 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateClientUserRequest(TeaModel):
+    def __init__(
+        self,
+        department_id: str = None,
+        description: str = None,
+        email: str = None,
+        id: str = None,
+        mobile_number: str = None,
+    ):
+        self.department_id = department_id
+        self.description = description
+        self.email = email
+        self.id = id
+        self.mobile_number = mobile_number
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateClientUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateClientUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        id: str = None,
+        password: str = None,
+        username: str = None,
+    ):
+        self.id = id
+        self.password = password
+        self.username = username
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateClientUserPasswordResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateClientUserPasswordResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        id: str = None,
+        status: str = None,
+    ):
+        self.id = id
+        self.status = status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class UpdateClientUserStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateClientUserStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateClientUserStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         application_ids: List[str] = None,
         application_type: str = None,
         description: str = None,
         dynamic_route_id: str = None,
@@ -10351,14 +12438,121 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateExcessiveDeviceRegistrationApplicationsStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateIdpDepartmentRequest(TeaModel):
+    def __init__(
+        self,
+        department_id: str = None,
+        department_name: str = None,
+        idp_config_id: str = None,
+    ):
+        self.department_id = department_id
+        self.department_name = department_name
+        self.idp_config_id = idp_config_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateIdpDepartmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateIdpDepartmentResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         begin: int = None,
         end: int = None,
     ):
         self.begin = begin
```

### Comparing `alibabacloud_csas20230120-1.3.0/alibabacloud_csas20230120.egg-info/PKG-INFO` & `alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120-1.3.0/setup.py` & `alibabacloud_csas20230120-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120.
 
-Created on 15/04/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python"
```


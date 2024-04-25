# Comparing `tmp/alibabacloud_ecd20201002-1.1.0.tar.gz` & `tmp/alibabacloud_ecd20201002-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ecd20201002-1.1.0.tar", last modified: Thu Mar 21 17:14:20 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ecd20201002-1.1.1.tar", last modified: Thu Apr 25 17:16:09 2024, max compression
```

## Comparing `alibabacloud_ecd20201002-1.1.0.tar` & `alibabacloud_ecd20201002-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123600 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002/client.py
--rw-r--r--   0 root         (0) root         (0)   177566 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-21 17:14:20.000000 alibabacloud_ecd20201002-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-03-21 17:14:19.000000 alibabacloud_ecd20201002-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      204 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   124392 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002/client.py
+-rw-r--r--   0 root         (0) root         (0)   181043 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 17:16:09.000000 alibabacloud_ecd20201002-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-25 17:16:08.000000 alibabacloud_ecd20201002-1.1.1/setup.py
```

### Comparing `alibabacloud_ecd20201002-1.1.0/LICENSE` & `alibabacloud_ecd20201002-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20201002-1.1.0/PKG-INFO` & `alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_ecd20201002
-Version: 1.1.0
+Name: alibabacloud-ecd20201002
+Version: 1.1.1
 Summary: Alibaba Cloud ecd (20201002) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20201002-1.1.0/README-CN.md` & `alibabacloud_ecd20201002-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20201002-1.1.0/README.md` & `alibabacloud_ecd20201002-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002/client.py` & `alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1493,14 +1493,16 @@
             query['LoginToken'] = request.login_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.session_token):
             query['SessionToken'] = request.session_token
+        if not UtilClient.is_unset(request.uuid):
+            query['Uuid'] = request.uuid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RebootDesktops',
             version='2020-10-02',
             protocol='HTTPS',
@@ -1537,14 +1539,16 @@
             query['LoginToken'] = request.login_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
         if not UtilClient.is_unset(request.session_token):
             query['SessionToken'] = request.session_token
+        if not UtilClient.is_unset(request.uuid):
+            query['Uuid'] = request.uuid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RebootDesktops',
             version='2020-10-02',
             protocol='HTTPS',
@@ -2320,15 +2324,15 @@
 
     def start_desktops_with_options(
         self,
         request: ecd_20201002_models.StartDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20201002_models.StartDesktopsResponse:
         """
-        The ID of the client.
+        The cloud computers that you want to start must be in the Stopped state. After you call this operation, the cloud computers enter the Running state.
         
         @param request: StartDesktopsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartDesktopsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2344,14 +2348,16 @@
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.login_token):
             query['LoginToken'] = request.login_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
+        if not UtilClient.is_unset(request.uuid):
+            query['Uuid'] = request.uuid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDesktops',
             version='2020-10-02',
             protocol='HTTPS',
@@ -2369,15 +2375,15 @@
 
     async def start_desktops_with_options_async(
         self,
         request: ecd_20201002_models.StartDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20201002_models.StartDesktopsResponse:
         """
-        The ID of the client.
+        The cloud computers that you want to start must be in the Stopped state. After you call this operation, the cloud computers enter the Running state.
         
         @param request: StartDesktopsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartDesktopsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2393,14 +2399,16 @@
             query['DesktopId'] = request.desktop_id
         if not UtilClient.is_unset(request.login_token):
             query['LoginToken'] = request.login_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.session_id):
             query['SessionId'] = request.session_id
+        if not UtilClient.is_unset(request.uuid):
+            query['Uuid'] = request.uuid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartDesktops',
             version='2020-10-02',
             protocol='HTTPS',
@@ -2417,28 +2425,28 @@
         )
 
     def start_desktops(
         self,
         request: ecd_20201002_models.StartDesktopsRequest,
     ) -> ecd_20201002_models.StartDesktopsResponse:
         """
-        The ID of the client.
+        The cloud computers that you want to start must be in the Stopped state. After you call this operation, the cloud computers enter the Running state.
         
         @param request: StartDesktopsRequest
         @return: StartDesktopsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_desktops_with_options(request, runtime)
 
     async def start_desktops_async(
         self,
         request: ecd_20201002_models.StartDesktopsRequest,
     ) -> ecd_20201002_models.StartDesktopsResponse:
         """
-        The ID of the client.
+        The cloud computers that you want to start must be in the Stopped state. After you call this operation, the cloud computers enter the Running state.
         
         @param request: StartDesktopsRequest
         @return: StartDesktopsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_desktops_with_options_async(request, runtime)
 
@@ -2542,15 +2550,15 @@
 
     def stop_desktops_with_options(
         self,
         request: ecd_20201002_models.StopDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20201002_models.StopDesktopsResponse:
         """
-        The cloud desktops that you want to stop by calling this operation must be in the Running state. If the call is successful, the cloud desktops enter the Stopped state.
+        The cloud computers that you want to stop must be in the Running state. After you call this operation, the cloud computers enter the Stopped state.
         
         @param request: StopDesktopsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopDesktopsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2593,15 +2601,15 @@
 
     async def stop_desktops_with_options_async(
         self,
         request: ecd_20201002_models.StopDesktopsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ecd_20201002_models.StopDesktopsResponse:
         """
-        The cloud desktops that you want to stop by calling this operation must be in the Running state. If the call is successful, the cloud desktops enter the Stopped state.
+        The cloud computers that you want to stop must be in the Running state. After you call this operation, the cloud computers enter the Stopped state.
         
         @param request: StopDesktopsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopDesktopsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2643,28 +2651,28 @@
         )
 
     def stop_desktops(
         self,
         request: ecd_20201002_models.StopDesktopsRequest,
     ) -> ecd_20201002_models.StopDesktopsResponse:
         """
-        The cloud desktops that you want to stop by calling this operation must be in the Running state. If the call is successful, the cloud desktops enter the Stopped state.
+        The cloud computers that you want to stop must be in the Running state. After you call this operation, the cloud computers enter the Stopped state.
         
         @param request: StopDesktopsRequest
         @return: StopDesktopsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.stop_desktops_with_options(request, runtime)
 
     async def stop_desktops_async(
         self,
         request: ecd_20201002_models.StopDesktopsRequest,
     ) -> ecd_20201002_models.StopDesktopsResponse:
         """
-        The cloud desktops that you want to stop by calling this operation must be in the Running state. If the call is successful, the cloud desktops enter the Stopped state.
+        The cloud computers that you want to stop must be in the Running state. After you call this operation, the cloud computers enter the Stopped state.
         
         @param request: StopDesktopsRequest
         @return: StopDesktopsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.stop_desktops_with_options_async(request, runtime)
```

### Comparing `alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002/models.py` & `alibabacloud_ecd20201002-1.1.1/alibabacloud_ecd20201002/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2789,28 +2789,74 @@
         if m.get('TokenCode') is not None:
             self.token_code = m.get('TokenCode')
         if m.get('Uuid') is not None:
             self.uuid = m.get('Uuid')
         return self
 
 
+class GetLoginTokenResponseBodyRiskVerifyInfo(TeaModel):
+    def __init__(
+        self,
+        email: str = None,
+        last_lock_duration: int = None,
+        locked: str = None,
+        phone: str = None,
+    ):
+        self.email = email
+        self.last_lock_duration = last_lock_duration
+        self.locked = locked
+        self.phone = phone
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
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.last_lock_duration is not None:
+            result['LastLockDuration'] = self.last_lock_duration
+        if self.locked is not None:
+            result['Locked'] = self.locked
+        if self.phone is not None:
+            result['Phone'] = self.phone
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('LastLockDuration') is not None:
+            self.last_lock_duration = m.get('LastLockDuration')
+        if m.get('Locked') is not None:
+            self.locked = m.get('Locked')
+        if m.get('Phone') is not None:
+            self.phone = m.get('Phone')
+        return self
+
+
 class GetLoginTokenResponseBody(TeaModel):
     def __init__(
         self,
         email: str = None,
         end_user_id: str = None,
         industry: str = None,
         keep_alive_token: str = None,
         label: str = None,
         login_token: str = None,
         next_stage: str = None,
         phone: str = None,
         props: Dict[str, str] = None,
         qr_code_png: str = None,
         request_id: str = None,
+        risk_verify_info: GetLoginTokenResponseBodyRiskVerifyInfo = None,
         secret: str = None,
         session_id: str = None,
         tenant_id: int = None,
         window_display_mode: str = None,
     ):
         # The email address of the user. The system returns the email address in the return value of the LoginToken parameter after the user logs on to the client.
         # 
@@ -2837,29 +2883,31 @@
         self.props = props
         # The QR code that is generated when the virtual MFA device is bound. The value is encoded in Base64. This parameter can be empty. This parameter is required only when the CurrentStage parameter is set to `MFABind`.
         # 
         # > For more information about each authentication stage, see the parameter description of the request parameter `CurrentStage`.
         self.qr_code_png = qr_code_png
         # The ID of the request.
         self.request_id = request_id
+        self.risk_verify_info = risk_verify_info
         # The key that is generated when you bind the virtual MFA device. This parameter is required when the CurrentStage parameter is set to `MFABind`.
         # 
         # > For more information about each authentication stage, see the parameter description of the request parameter `CurrentStage`.
         self.secret = secret
         # The ID of the session. The ID is returned the first time you call the `GetLoginToken` operation in the session. If MFA is required, you must specify this parameter in subsequent stages.
         # 
         # > For more information about each authentication stage, see the parameter description of the request parameter `CurrentStage`.
         self.session_id = session_id
         # The ID of the Alibaba Cloud account. The ID is used for hardware client authentication.
         self.tenant_id = tenant_id
         # > This is a parameter only for internal use.
         self.window_display_mode = window_display_mode
 
     def validate(self):
-        pass
+        if self.risk_verify_info:
+            self.risk_verify_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2881,14 +2929,16 @@
             result['Phone'] = self.phone
         if self.props is not None:
             result['Props'] = self.props
         if self.qr_code_png is not None:
             result['QrCodePng'] = self.qr_code_png
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.risk_verify_info is not None:
+            result['RiskVerifyInfo'] = self.risk_verify_info.to_map()
         if self.secret is not None:
             result['Secret'] = self.secret
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.tenant_id is not None:
             result['TenantId'] = self.tenant_id
         if self.window_display_mode is not None:
@@ -2915,14 +2965,17 @@
             self.phone = m.get('Phone')
         if m.get('Props') is not None:
             self.props = m.get('Props')
         if m.get('QrCodePng') is not None:
             self.qr_code_png = m.get('QrCodePng')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('RiskVerifyInfo') is not None:
+            temp_model = GetLoginTokenResponseBodyRiskVerifyInfo()
+            self.risk_verify_info = temp_model.from_map(m['RiskVerifyInfo'])
         if m.get('Secret') is not None:
             self.secret = m.get('Secret')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('TenantId') is not None:
             self.tenant_id = m.get('TenantId')
         if m.get('WindowDisplayMode') is not None:
@@ -3246,33 +3299,35 @@
         client_token: str = None,
         client_version: str = None,
         desktop_id: List[str] = None,
         login_token: str = None,
         region_id: str = None,
         session_id: str = None,
         session_token: str = None,
+        uuid: str = None,
     ):
         # The client ID. The system generates a unique ID for each client.
         self.client_id = client_id
-        # The client OS.
+        # The operating system (OS) of the device that runs the Alibaba Cloud Workspace client (hereinafter referred to as WUYING client).
         self.client_os = client_os
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [How do I ensure the idempotence of a request?](~~25693~~)
         self.client_token = client_token
-        # The client version.
+        # The client version. If you use a WUYING client, you can view the client version in the **About** dialog box on the client logon page.
         self.client_version = client_version
-        # The cloud desktop IDs. You can specify 1 to 20 IDs.
+        # The IDs of the cloud computers. You can specify the IDs of 1 to 20 cloud computers.
         self.desktop_id = desktop_id
         # The logon token.
         self.login_token = login_token
-        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the most recent region list.
+        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the regions supported by WUYING Workspace.
         self.region_id = region_id
         # The session ID.
         self.session_id = session_id
         # The logon token.
         self.session_token = session_token
+        self.uuid = uuid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -3293,14 +3348,16 @@
             result['LoginToken'] = self.login_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.session_id is not None:
             result['SessionId'] = self.session_id
         if self.session_token is not None:
             result['SessionToken'] = self.session_token
+        if self.uuid is not None:
+            result['Uuid'] = self.uuid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientId') is not None:
             self.client_id = m.get('ClientId')
         if m.get('ClientOS') is not None:
@@ -3315,14 +3372,16 @@
             self.login_token = m.get('LoginToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
         if m.get('SessionToken') is not None:
             self.session_token = m.get('SessionToken')
+        if m.get('Uuid') is not None:
+            self.uuid = m.get('Uuid')
         return self
 
 
 class RebootDesktopsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
@@ -4452,29 +4511,33 @@
         client_os: str = None,
         client_token: str = None,
         client_version: str = None,
         desktop_id: List[str] = None,
         login_token: str = None,
         region_id: str = None,
         session_id: str = None,
+        uuid: str = None,
     ):
-        # The ID of the request.
+        # The ID of the Alibaba Cloud Workspace client (hereinafter referred to as WUYING client). The system generates a unique ID for each client.
         self.client_id = client_id
-        # The OS used by the client.
+        # The operating system (OS) of the device that run the client.
         self.client_os = client_os
+        # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [How to ensure idempotence](~~25693~~).
         self.client_token = client_token
-        # StartDesktops
+        # The client version. If you use a WUYING client, you can click **About** on the client logon page to view the version of the client.
         self.client_version = client_version
+        # The IDs of the cloud computers. You can specify the IDs of 1 to 20 cloud computers.
         self.desktop_id = desktop_id
-        # The ID of cloud desktop N. You can specify one or more IDs of cloud desktops. Valid values of N: 1 to 20.
+        # The logon token.
         self.login_token = login_token
-        # The logon credential.
+        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the regions supported by WUYING Workspace.
         self.region_id = region_id
-        # The operation that you want to perform. Set the value to StartDesktops.
+        # The session ID.
         self.session_id = session_id
+        self.uuid = uuid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -4493,14 +4556,16 @@
             result['DesktopId'] = self.desktop_id
         if self.login_token is not None:
             result['LoginToken'] = self.login_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.session_id is not None:
             result['SessionId'] = self.session_id
+        if self.uuid is not None:
+            result['Uuid'] = self.uuid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientId') is not None:
             self.client_id = m.get('ClientId')
         if m.get('ClientOS') is not None:
@@ -4513,22 +4578,25 @@
             self.desktop_id = m.get('DesktopId')
         if m.get('LoginToken') is not None:
             self.login_token = m.get('LoginToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SessionId') is not None:
             self.session_id = m.get('SessionId')
+        if m.get('Uuid') is not None:
+            self.uuid = m.get('Uuid')
         return self
 
 
 class StartDesktopsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4736,25 +4804,25 @@
         login_token: str = None,
         region_id: str = None,
         session_id: str = None,
         session_token: str = None,
     ):
         # The client ID. The system generates a unique ID for each client.
         self.client_id = client_id
-        # The client OS.
+        # The operating system (OS) of the device that runs the Alibaba Cloud Workspace client (hereinafter referred to as WUYING client).
         self.client_os = client_os
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. For more information, see [How do I ensure the idempotence of a request?](~~25693~~)
         self.client_token = client_token
-        # The client version.
+        # The client version. If you use a WUYING client, you can view the client version in the **About** dialog box on the client logon page.
         self.client_version = client_version
-        # The cloud desktop IDs. You can specify 1 to 20 IDs.
+        # The IDs of the cloud computers. You can specify the IDs of 1 to 20 cloud computers.
         self.desktop_id = desktop_id
         # The logon token.
         self.login_token = login_token
-        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the most recent region list.
+        # The region ID. You can call the [DescribeRegions](~~196646~~) operation to query the regions supported by WUYING Workspace.
         self.region_id = region_id
         # The session ID.
         self.session_id = session_id
         # The logon token.
         self.session_token = session_token
 
     def validate(self):
```

### Comparing `alibabacloud_ecd20201002-1.1.0/alibabacloud_ecd20201002.egg-info/PKG-INFO` & `alibabacloud_ecd20201002-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-ecd20201002
-Version: 1.1.0
+Name: alibabacloud_ecd20201002
+Version: 1.1.1
 Summary: Alibaba Cloud ecd (20201002) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20201002-1.1.0/setup.py` & `alibabacloud_ecd20201002-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ecd20201002.
 
-Created on 21/03/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ecd20201002"
 NAME = "alibabacloud_ecd20201002" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ecd (20201002) SDK Library for Python"
```


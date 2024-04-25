# Comparing `tmp/alibabacloud_cloudauth-intl20220809-1.4.5.tar.gz` & `tmp/alibabacloud_cloudauth-intl20220809-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809-1.4.5.tar", last modified: Sun Feb  4 02:16:55 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth-intl20220809-2.0.0.tar", last modified: Thu Apr 25 07:57:14 2024, max compression
```

## Comparing `alibabacloud_cloudauth-intl20220809-1.4.5.tar` & `alibabacloud_cloudauth-intl20220809-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/
--rw-r--r--   0 root         (0) root         (0)     1524 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1224 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80506 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809/client.py
--rw-r--r--   0 root         (0) root         (0)   149672 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 02:16:55.000000 alibabacloud_cloudauth-intl20220809-1.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2668 2024-02-04 02:16:54.000000 alibabacloud_cloudauth-intl20220809-1.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1860 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809/client.py
+-rw-r--r--   0 root         (0) root         (0)   144064 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 07:57:14.000000 alibabacloud_cloudauth-intl20220809-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-25 07:57:13.000000 alibabacloud_cloudauth-intl20220809-2.0.0/setup.py
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/LICENSE` & `alibabacloud_cloudauth-intl20220809-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/PKG-INFO` & `alibabacloud_cloudauth-intl20220809-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth-intl20220809
-Version: 1.4.5
+Version: 2.0.0
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/README-CN.md` & `alibabacloud_cloudauth-intl20220809-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/README.md` & `alibabacloud_cloudauth-intl20220809-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809/client.py` & `alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,88 +259,14 @@
     async def check_result_async(
         self,
         request: cloudauth_intl_20220809_models.CheckResultRequest,
     ) -> cloudauth_intl_20220809_models.CheckResultResponse:
         runtime = util_models.RuntimeOptions()
         return await self.check_result_with_options_async(request, runtime)
 
-    def delete_picture_with_options(
-        self,
-        request: cloudauth_intl_20220809_models.DeletePictureRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> cloudauth_intl_20220809_models.DeletePictureResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.delete_pic_after_query):
-            query['DeletePicAfterQuery'] = request.delete_pic_after_query
-        if not UtilClient.is_unset(request.transaction_id):
-            query['TransactionId'] = request.transaction_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeletePicture',
-            version='2022-08-09',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            cloudauth_intl_20220809_models.DeletePictureResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_picture_with_options_async(
-        self,
-        request: cloudauth_intl_20220809_models.DeletePictureRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> cloudauth_intl_20220809_models.DeletePictureResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.delete_pic_after_query):
-            query['DeletePicAfterQuery'] = request.delete_pic_after_query
-        if not UtilClient.is_unset(request.transaction_id):
-            query['TransactionId'] = request.transaction_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DeletePicture',
-            version='2022-08-09',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            cloudauth_intl_20220809_models.DeletePictureResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_picture(
-        self,
-        request: cloudauth_intl_20220809_models.DeletePictureRequest,
-    ) -> cloudauth_intl_20220809_models.DeletePictureResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.delete_picture_with_options(request, runtime)
-
-    async def delete_picture_async(
-        self,
-        request: cloudauth_intl_20220809_models.DeletePictureRequest,
-    ) -> cloudauth_intl_20220809_models.DeletePictureResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.delete_picture_with_options_async(request, runtime)
-
     def delete_verify_result_with_options(
         self,
         request: cloudauth_intl_20220809_models.DeleteVerifyResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_intl_20220809_models.DeleteVerifyResultResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1664,48 +1590,40 @@
             query['Crop'] = request.crop
         if not UtilClient.is_unset(request.doc_scan_mode):
             query['DocScanMode'] = request.doc_scan_mode
         if not UtilClient.is_unset(request.doc_type):
             query['DocType'] = request.doc_type
         if not UtilClient.is_unset(request.face_picture_url):
             query['FacePictureUrl'] = request.face_picture_url
-        if not UtilClient.is_unset(request.flow_type):
-            query['FlowType'] = request.flow_type
         if not UtilClient.is_unset(request.id_face_quality):
             query['IdFaceQuality'] = request.id_face_quality
         if not UtilClient.is_unset(request.id_spoof):
             query['IdSpoof'] = request.id_spoof
         if not UtilClient.is_unset(request.language_config):
             query['LanguageConfig'] = request.language_config
         if not UtilClient.is_unset(request.merchant_biz_id):
             query['MerchantBizId'] = request.merchant_biz_id
         if not UtilClient.is_unset(request.merchant_user_id):
             query['MerchantUserId'] = request.merchant_user_id
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
         if not UtilClient.is_unset(request.ocr):
             query['Ocr'] = request.ocr
-        if not UtilClient.is_unset(request.operation_mode):
-            query['OperationMode'] = request.operation_mode
-        if not UtilClient.is_unset(request.pages):
-            query['Pages'] = request.pages
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
-        if not UtilClient.is_unset(request.product_config):
-            query['ProductConfig'] = request.product_config
         if not UtilClient.is_unset(request.product_flow):
             query['ProductFlow'] = request.product_flow
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_code):
             query['SceneCode'] = request.scene_code
         if not UtilClient.is_unset(request.security_level):
             query['SecurityLevel'] = request.security_level
-        if not UtilClient.is_unset(request.service_level):
-            query['ServiceLevel'] = request.service_level
+        if not UtilClient.is_unset(request.style_config):
+            query['StyleConfig'] = request.style_config
         body = {}
         if not UtilClient.is_unset(request.face_picture_base_64):
             body['FacePictureBase64'] = request.face_picture_base_64
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1742,48 +1660,40 @@
             query['Crop'] = request.crop
         if not UtilClient.is_unset(request.doc_scan_mode):
             query['DocScanMode'] = request.doc_scan_mode
         if not UtilClient.is_unset(request.doc_type):
             query['DocType'] = request.doc_type
         if not UtilClient.is_unset(request.face_picture_url):
             query['FacePictureUrl'] = request.face_picture_url
-        if not UtilClient.is_unset(request.flow_type):
-            query['FlowType'] = request.flow_type
         if not UtilClient.is_unset(request.id_face_quality):
             query['IdFaceQuality'] = request.id_face_quality
         if not UtilClient.is_unset(request.id_spoof):
             query['IdSpoof'] = request.id_spoof
         if not UtilClient.is_unset(request.language_config):
             query['LanguageConfig'] = request.language_config
         if not UtilClient.is_unset(request.merchant_biz_id):
             query['MerchantBizId'] = request.merchant_biz_id
         if not UtilClient.is_unset(request.merchant_user_id):
             query['MerchantUserId'] = request.merchant_user_id
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
         if not UtilClient.is_unset(request.ocr):
             query['Ocr'] = request.ocr
-        if not UtilClient.is_unset(request.operation_mode):
-            query['OperationMode'] = request.operation_mode
-        if not UtilClient.is_unset(request.pages):
-            query['Pages'] = request.pages
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
-        if not UtilClient.is_unset(request.product_config):
-            query['ProductConfig'] = request.product_config
         if not UtilClient.is_unset(request.product_flow):
             query['ProductFlow'] = request.product_flow
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_code):
             query['SceneCode'] = request.scene_code
         if not UtilClient.is_unset(request.security_level):
             query['SecurityLevel'] = request.security_level
-        if not UtilClient.is_unset(request.service_level):
-            query['ServiceLevel'] = request.service_level
+        if not UtilClient.is_unset(request.style_config):
+            query['StyleConfig'] = request.style_config
         body = {}
         if not UtilClient.is_unset(request.face_picture_base_64):
             body['FacePictureBase64'] = request.face_picture_base_64
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809/models.py` & `alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,169 +418,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CheckResultResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DeletePictureRequest(TeaModel):
-    def __init__(
-        self,
-        delete_pic_after_query: str = None,
-        transaction_id: str = None,
-    ):
-        self.delete_pic_after_query = delete_pic_after_query
-        self.transaction_id = transaction_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.delete_pic_after_query is not None:
-            result['DeletePicAfterQuery'] = self.delete_pic_after_query
-        if self.transaction_id is not None:
-            result['TransactionId'] = self.transaction_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('DeletePicAfterQuery') is not None:
-            self.delete_pic_after_query = m.get('DeletePicAfterQuery')
-        if m.get('TransactionId') is not None:
-            self.transaction_id = m.get('TransactionId')
-        return self
-
-
-class DeletePictureResponseBodyResult(TeaModel):
-    def __init__(
-        self,
-        delete_result: str = None,
-        transaction_id: str = None,
-    ):
-        self.delete_result = delete_result
-        self.transaction_id = transaction_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.delete_result is not None:
-            result['DeleteResult'] = self.delete_result
-        if self.transaction_id is not None:
-            result['TransactionId'] = self.transaction_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('DeleteResult') is not None:
-            self.delete_result = m.get('DeleteResult')
-        if m.get('TransactionId') is not None:
-            self.transaction_id = m.get('TransactionId')
-        return self
-
-
-class DeletePictureResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        message: str = None,
-        request_id: str = None,
-        result: DeletePictureResponseBodyResult = None,
-    ):
-        self.code = code
-        self.message = message
-        # Id of the request
-        self.request_id = request_id
-        self.result = result
-
-    def validate(self):
-        if self.result:
-            self.result.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.result is not None:
-            result['Result'] = self.result.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Result') is not None:
-            temp_model = DeletePictureResponseBodyResult()
-            self.result = temp_model.from_map(m['Result'])
-        return self
-
-
-class DeletePictureResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: DeletePictureResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = DeletePictureResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DeleteVerifyResultRequest(TeaModel):
     def __init__(
         self,
         delete_after_query: str = None,
         delete_type: str = None,
         transaction_id: str = None,
     ):
@@ -4098,58 +3943,50 @@
         callback_token: str = None,
         callback_url: str = None,
         crop: str = None,
         doc_scan_mode: str = None,
         doc_type: str = None,
         face_picture_base_64: str = None,
         face_picture_url: str = None,
-        flow_type: str = None,
         id_face_quality: str = None,
         id_spoof: str = None,
         language_config: str = None,
         merchant_biz_id: str = None,
         merchant_user_id: str = None,
         meta_info: str = None,
         ocr: str = None,
-        operation_mode: str = None,
-        pages: str = None,
         product_code: str = None,
-        product_config: str = None,
         product_flow: str = None,
         return_url: str = None,
         scene_code: str = None,
         security_level: str = None,
-        service_level: str = None,
+        style_config: str = None,
     ):
         self.authorize = authorize
         self.callback_token = callback_token
         self.callback_url = callback_url
         self.crop = crop
         self.doc_scan_mode = doc_scan_mode
         self.doc_type = doc_type
         self.face_picture_base_64 = face_picture_base_64
         self.face_picture_url = face_picture_url
-        self.flow_type = flow_type
         self.id_face_quality = id_face_quality
         self.id_spoof = id_spoof
         self.language_config = language_config
         self.merchant_biz_id = merchant_biz_id
         self.merchant_user_id = merchant_user_id
         self.meta_info = meta_info
         # OCR。
         self.ocr = ocr
-        self.operation_mode = operation_mode
-        self.pages = pages
         self.product_code = product_code
-        self.product_config = product_config
         self.product_flow = product_flow
         self.return_url = return_url
         self.scene_code = scene_code
         self.security_level = security_level
-        self.service_level = service_level
+        self.style_config = style_config
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -4168,48 +4005,40 @@
             result['DocScanMode'] = self.doc_scan_mode
         if self.doc_type is not None:
             result['DocType'] = self.doc_type
         if self.face_picture_base_64 is not None:
             result['FacePictureBase64'] = self.face_picture_base_64
         if self.face_picture_url is not None:
             result['FacePictureUrl'] = self.face_picture_url
-        if self.flow_type is not None:
-            result['FlowType'] = self.flow_type
         if self.id_face_quality is not None:
             result['IdFaceQuality'] = self.id_face_quality
         if self.id_spoof is not None:
             result['IdSpoof'] = self.id_spoof
         if self.language_config is not None:
             result['LanguageConfig'] = self.language_config
         if self.merchant_biz_id is not None:
             result['MerchantBizId'] = self.merchant_biz_id
         if self.merchant_user_id is not None:
             result['MerchantUserId'] = self.merchant_user_id
         if self.meta_info is not None:
             result['MetaInfo'] = self.meta_info
         if self.ocr is not None:
             result['Ocr'] = self.ocr
-        if self.operation_mode is not None:
-            result['OperationMode'] = self.operation_mode
-        if self.pages is not None:
-            result['Pages'] = self.pages
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
-        if self.product_config is not None:
-            result['ProductConfig'] = self.product_config
         if self.product_flow is not None:
             result['ProductFlow'] = self.product_flow
         if self.return_url is not None:
             result['ReturnUrl'] = self.return_url
         if self.scene_code is not None:
             result['SceneCode'] = self.scene_code
         if self.security_level is not None:
             result['SecurityLevel'] = self.security_level
-        if self.service_level is not None:
-            result['ServiceLevel'] = self.service_level
+        if self.style_config is not None:
+            result['StyleConfig'] = self.style_config
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Authorize') is not None:
             self.authorize = m.get('Authorize')
         if m.get('CallbackToken') is not None:
@@ -4222,48 +4051,40 @@
             self.doc_scan_mode = m.get('DocScanMode')
         if m.get('DocType') is not None:
             self.doc_type = m.get('DocType')
         if m.get('FacePictureBase64') is not None:
             self.face_picture_base_64 = m.get('FacePictureBase64')
         if m.get('FacePictureUrl') is not None:
             self.face_picture_url = m.get('FacePictureUrl')
-        if m.get('FlowType') is not None:
-            self.flow_type = m.get('FlowType')
         if m.get('IdFaceQuality') is not None:
             self.id_face_quality = m.get('IdFaceQuality')
         if m.get('IdSpoof') is not None:
             self.id_spoof = m.get('IdSpoof')
         if m.get('LanguageConfig') is not None:
             self.language_config = m.get('LanguageConfig')
         if m.get('MerchantBizId') is not None:
             self.merchant_biz_id = m.get('MerchantBizId')
         if m.get('MerchantUserId') is not None:
             self.merchant_user_id = m.get('MerchantUserId')
         if m.get('MetaInfo') is not None:
             self.meta_info = m.get('MetaInfo')
         if m.get('Ocr') is not None:
             self.ocr = m.get('Ocr')
-        if m.get('OperationMode') is not None:
-            self.operation_mode = m.get('OperationMode')
-        if m.get('Pages') is not None:
-            self.pages = m.get('Pages')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
-        if m.get('ProductConfig') is not None:
-            self.product_config = m.get('ProductConfig')
         if m.get('ProductFlow') is not None:
             self.product_flow = m.get('ProductFlow')
         if m.get('ReturnUrl') is not None:
             self.return_url = m.get('ReturnUrl')
         if m.get('SceneCode') is not None:
             self.scene_code = m.get('SceneCode')
         if m.get('SecurityLevel') is not None:
             self.security_level = m.get('SecurityLevel')
-        if m.get('ServiceLevel') is not None:
-            self.service_level = m.get('ServiceLevel')
+        if m.get('StyleConfig') is not None:
+            self.style_config = m.get('StyleConfig')
         return self
 
 
 class InitializeResponseBodyResult(TeaModel):
     def __init__(
         self,
         client_cfg: str = None,
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO` & `alibabacloud_cloudauth-intl20220809-2.0.0/alibabacloud_cloudauth_intl20220809.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth-intl20220809
-Version: 1.4.5
+Version: 2.0.0
 Summary: Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth-intl20220809-1.4.5/setup.py` & `alibabacloud_cloudauth-intl20220809-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth-intl20220809.
 
-Created on 02/02/2024
+Created on 25/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth_intl20220809"
 NAME = "alibabacloud_cloudauth-intl20220809" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloudauth-intl (20220809) SDK Library for Python"
```


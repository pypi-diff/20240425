# Comparing `tmp/latch_cloud_clients-0.1.4.tar.gz` & `tmp/latch_cloud_clients-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_cloud_clients-0.1.4.tar", max compression
+gzip compressed data, was "latch_cloud_clients-0.1.5.tar", max compression
```

## Comparing `latch_cloud_clients-0.1.4.tar` & `latch_cloud_clients-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.4/LICENSE
--rw-r--r--   0        0        0      121 2024-04-23 21:26:46.040298 latch_cloud_clients-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.4/latch_cloud_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.4/latch_cloud_clients/aws/__init__.py
--rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.4/latch_cloud_clients/aws/aws.py
--rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.4/latch_cloud_clients/aws/client_pool.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/__init__.py
--rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/client_pool.py
--rw-r--r--   0        0        0     3369 2024-04-23 22:28:19.034702 latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/pubsub.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/py.typed
--rw-r--r--   0        0        0    13709 2024-04-24 02:15:44.861789 latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/storage.py
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.4/latch_cloud_clients/py.typed
--rw-r--r--   0        0        0    24434 2024-04-24 00:05:21.984419 latch_cloud_clients-0.1.4/latch_cloud_clients/storage_clients.py
--rw-r--r--   0        0        0     1455 2024-04-24 02:16:05.060109 latch_cloud_clients-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.5/LICENSE
+-rw-r--r--   0        0        0      121 2024-04-24 21:08:53.493221 latch_cloud_clients-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.5/latch_cloud_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.5/latch_cloud_clients/aws/__init__.py
+-rw-r--r--   0        0        0    14297 2024-04-25 15:28:32.366171 latch_cloud_clients-0.1.5/latch_cloud_clients/aws/storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.5/latch_cloud_clients/gcp/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-24 18:33:31.527944 latch_cloud_clients-0.1.5/latch_cloud_clients/gcp/client_pool.py
+-rw-r--r--   0        0        0    14808 2024-04-25 16:51:37.323692 latch_cloud_clients-0.1.5/latch_cloud_clients/gcp/storage.py
+-rw-r--r--   0        0        0     9534 2024-04-25 16:52:13.344438 latch_cloud_clients-0.1.5/latch_cloud_clients/gcp/storage_client.py
+-rw-r--r--   0        0        0      790 2024-04-24 21:40:21.430232 latch_cloud_clients-0.1.5/latch_cloud_clients/get_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.5/latch_cloud_clients/py.typed
+-rw-r--r--   0        0        0     2944 2024-04-25 01:41:32.831875 latch_cloud_clients-0.1.5/latch_cloud_clients/utils.py
+-rw-r--r--   0        0        0     1502 2024-04-25 16:52:28.721249 latch_cloud_clients-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.5/PKG-INFO
```

### Comparing `latch_cloud_clients-0.1.4/LICENSE` & `latch_cloud_clients-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/client_pool.py` & `latch_cloud_clients-0.1.5/latch_cloud_clients/gcp/client_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from collections.abc import AsyncGenerator
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
 
 import aiohttp
 from opentelemetry.trace import get_tracer
 
-from .pubsub import AsyncPubsubClient
 from .storage import AsyncStorageClient
 
 tracer = get_tracer(__name__)
 
 
 class AsyncGCPClient:
     def __init__(self, session: aiohttp.ClientSession):
@@ -19,17 +18,14 @@
 
     def __aexit__(self, exc_type, exc_val, exc_tb):
         return self.session.__aexit__(exc_type, exc_val, exc_tb)
 
     def storage_client(self):
         return AsyncStorageClient(self.session)
 
-    def pubsub_client(self, project_id: str, subscription: str):
-        return AsyncPubsubClient(self.session, project_id, subscription)
-
 
 @dataclass
 class ClientList:
     sema: BoundedSemaphore
     client_add_sema: BoundedSemaphore
     clients: list[AsyncGCPClient]
```

### Comparing `latch_cloud_clients-0.1.4/latch_cloud_clients/gcp/storage.py` & `latch_cloud_clients-0.1.5/latch_cloud_clients/gcp/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, TypedDict
-from urllib.parse import urljoin
+from urllib.parse import quote, urljoin
 from xml.etree import ElementTree as ET
 
 import aiohttp
 import xmltodict
-from dateutil.parser import parse
 from google.api_core.exceptions import (
     BadRequest,
     Forbidden,
     NotFound,
     ServerError,
     TooManyRequests,
     Unauthorized,
@@ -27,25 +26,25 @@
     name: str
     id: str
     creation_time: str
     update_time: str
     project_number: str
 
 
-@dataclass(frozen=True)
+@dataclass(kw_only=True)
 class Object:
     id: str
     name: str
     bucket: str
-    media_link: str
-    generation: str
-    content_type: str
     size: int
-    creation_time: datetime
-    update_time: datetime
+    media_link: str | None
+    generation: str | None
+    content_type: str | None
+    creation_time: datetime | None
+    update_time: datetime | None
 
 
 CompletedPartTypeDef = TypedDict(
     "CompletedPartTypeDef",
     {
         "ETag": str,
         "ChecksumCRC32": str,
@@ -54,62 +53,14 @@
         "ChecksumSHA256": str,
         "PartNumber": int,
     },
     total=False,
 )
 
 
-class AsyncHTTPIterator:
-    def __init__(self, url: str, headers: dict, params: dict, storage_client):
-        self.url = url
-        self.headers = headers
-        self.params = params
-        self.next_page_token = None
-        self.prefixes = list()
-        self.items = []
-        self.storage_client = storage_client
-
-    def __aiter__(self):
-        return self
-
-    async def __anext__(self):
-        if not self.items and self.next_page_token == "":
-            raise StopAsyncIteration
-
-        if self.items:
-            obj = self.items.pop()
-            return Object(
-                id=obj["id"],
-                name=obj["name"],
-                bucket=obj["bucket"],
-                media_link=obj["mediaLink"],
-                generation=obj["generation"],
-                content_type=obj["contentType"],
-                size=int(obj["size"]),
-                creation_time=parse(obj["timeCreated"]),
-                update_time=parse(obj["updated"]),
-            )
-
-        if self.next_page_token:
-            self.params["pageToken"] = self.next_page_token
-
-        res = await self.storage_client._make_api_request(
-            "GET", self.url, headers=self.headers, params=self.params, return_json=True
-        )
-
-        if "items" not in res:
-            raise StopAsyncIteration
-
-        self.items = res.get("items", [])
-        self.prefixes.extend(res.get("prefixes", []))
-        self.next_page_token = res.get("nextPageToken", "")
-
-        return await self.__anext__()
-
-
 class AsyncStorageClient:
     credentials, _ = default(scopes=["https://www.googleapis.com/auth/cloud-platform"])
 
     def __init__(self, session: aiohttp.ClientSession):
         self.api_url = "https://storage.googleapis.com/storage/v1/"
         self.upload_api_url = "https://storage.googleapis.com/upload/storage/v1/"
         self.session = session
@@ -130,15 +81,17 @@
         data: Any | None = None,
         headers: dict | None = None,
         params: dict | None = None,
         return_bytes=False,
         return_json=False,
         return_response=False,
     ) -> Any:
-        headers = headers or {}
+        if headers is None:
+            headers = {}
+
         headers["Authorization"] = f"Bearer {AsyncStorageClient.get_auth_token()}"
 
         async with self.session.request(
             method,
             url,
             headers=headers,
             params=params,
@@ -188,87 +141,90 @@
             project_number=res["projectNumber"],
         )
 
     async def get_blob_meta(self, bucket_name: str, key: str):
         try:
             res = await self._make_api_request(
                 "GET",
-                urljoin(self.api_url, f"b/{bucket_name}/o/{key}"),
+                urljoin(self.api_url, f"b/{bucket_name}/o/{quote(key, safe='')}"),
                 return_json=True,
             )
         except NotFound:
             return None
 
         return Object(
             name=res["name"],
             id=res["id"],
             bucket=res["bucket"],
             media_link=res["mediaLink"],
             generation=res["generation"],
             content_type=res["contentType"],
             size=int(res["size"]),
-            creation_time=parse(res["timeCreated"]),
-            update_time=parse(res["updated"]),
+            creation_time=datetime.fromisoformat(res["timeCreated"]),
+            update_time=datetime.fromisoformat(res["updated"]),
         )
 
     def list_blobs(
         self,
         bucket_name: str,
         prefix: str | None = None,
         delimiter: str = "/",
         match_glob: str | None = None,
-        page_size: int = 1000,
         page_token: str | None = None,
         include_trailing_delimeter: bool | None = None,
         include_folders_as_prefixes: bool | None = None,
+        max_items: int | None = None,
     ):
         if match_glob is not None and delimiter != "/":
             raise ValueError("match_glob is only supported with delimeter='/'")
 
         if include_folders_as_prefixes and delimiter != "/":
             raise ValueError(
                 "include_folders_as_prefixes is only supported with delimeter='/'"
             )
 
         params = {
+            "bucket": bucket_name,
             "prefix": prefix,
             "delimiter": delimiter,
             "matchGlob": match_glob,
-            "maxResults": page_size,
+            "maxResults": 1000,
             "pageToken": page_token,
             "includeTrailingDelimeter": include_trailing_delimeter,
             "includeFoldersAsPrefixes": include_folders_as_prefixes,
         }
 
         params = {k: str(v) for k, v in params.items() if v is not None}
 
         return AsyncHTTPIterator(
             url=urljoin(self.api_url, f"b/{bucket_name}/o"),
             headers={},
             params=params,
             storage_client=self,
+            max_items=max_items,
         )
 
     async def get_blob_bytes(
         self,
         bucket_name: str,
         key: str,
         start: int | None = None,
         end: int | None = None,
     ):
         headers = {}
-        start = start if start is not None else 0
+        if start is None:
+            start = 0
 
         if end is not None:
             headers["Range"] = f"bytes={start}-{end}"
 
         return bytes(
             await self._make_api_request(
                 "GET",
-                urljoin(self.api_url, f"b/{bucket_name}/o/{key}"),
+                urljoin(self.api_url, f"b/{bucket_name}/o/{quote(key, safe='')}"),
                 params={"alt": "media"},
                 headers=headers,
                 return_bytes=True,
             )
         )
 
     async def put_blob(
@@ -294,16 +250,16 @@
             id=resp["id"],
             name=resp["name"],
             bucket=resp["bucket"],
             media_link=resp["mediaLink"],
             generation=resp["generation"],
             content_type=resp["contentType"],
             size=int(resp["size"]),
-            creation_time=parse(resp["timeCreated"]),
-            update_time=parse(resp["updated"]),
+            creation_time=datetime.fromisoformat(resp["timeCreated"]),
+            update_time=datetime.fromisoformat(resp["updated"]),
         )
 
     async def copy_blob(
         self,
         src_bucket_name: str,
         src_bucket_key: str,
         dest_bucket_name: str,
@@ -317,15 +273,15 @@
                 if rewrite_token:
                     params = {"rewriteToken": rewrite_token}
 
                 resp = await self._make_api_request(
                     "POST",
                     urljoin(
                         self.api_url,
-                        f"b/{src_bucket_name}/o/{src_bucket_key}/rewriteTo/b/{dest_bucket_name}/o/{dest_bucket_key}",
+                        f"b/{src_bucket_name}/o/{quote(src_bucket_key,safe='')}/rewriteTo/b/{dest_bucket_name}/o/{quote(dest_bucket_key, safe='')}",
                     ),
                     params=params,
                     headers={"Content-Type": "application/json"},
                     return_json=True,
                 )
 
                 done = resp["done"]
@@ -338,19 +294,19 @@
     ):
         params = {}
         if generation is not None:
             params["generation"] = generation
 
         await self._make_api_request(
             "DELETE",
-            urljoin(self.api_url, f"b/{bucket_name}/o/{key}"),
+            urljoin(self.api_url, f"b/{bucket_name}/o/{quote(key, safe='')}"),
             params=params,
         )
 
-    def get_signed_url(
+    def get_signed_download_url(
         self,
         bucket_name: str,
         key: str | None,
         content_disposition: str | None = None,
         content_type: str | None = None,
     ):
         # note(taras): this constructs a blob object and signs download url without making requests
@@ -360,29 +316,25 @@
             version="v4",
             expiration=max_presigned_url_age,
             method="GET",
             content_type=content_type,
             response_disposition=content_disposition,
         )
 
-    async def get_signed_upload_url(
+    async def get_signed_part_upload_url(
         self,
         bucket_name: str,
-        key: str,
+        bucket_key: str,
         upload_id: str,
         part_number: int,
     ):
 
-        meta = await self.get_blob_meta(bucket_name, key)
-        if meta is None:
-            await self.put_blob(bucket_name, key, b"")
-
         # note(taras): this constructs a blob object and signs
         # upload url without making syncronous requests
-        blob = storage.Client().bucket(bucket_name).blob(key)
+        blob = storage.Client().bucket(bucket_name).blob(bucket_key)
 
         return blob.generate_signed_url(
             version="v4",
             expiration=max_presigned_url_age,
             method="PUT",
             query_parameters={
                 "partNumber": part_number,
@@ -392,14 +344,18 @@
 
     async def multipart_initiate_upload(
         self,
         bucket_name: str,
         bucket_key: str,
         content_type: str = "text/plain",
     ):
+        meta = await self.get_blob_meta(bucket_name, bucket_key)
+        if meta is None:
+            await self.put_blob(bucket_name, bucket_key, b"")
+
         # note(taras): multipart uploads use XML api instead of JSON
         resp = await self._make_api_request(
             "POST",
             f"https://storage.googleapis.com/{bucket_name}/{bucket_key}?uploads",
             headers={
                 "Content-Type": content_type,
             },
@@ -410,15 +366,15 @@
     async def multipart_upload_part(
         self,
         bucket_name: str,
         bucket_key: str,
         upload_id: str,
         part_number: int,
         data: bytes,
-    ):
+    ) -> str:
         resp = await self._make_api_request(
             "PUT",
             f"https://storage.googleapis.com/{bucket_name}/{bucket_key}?uploadId={upload_id}&partNumber={part_number}",
             data=data,
             return_response=True,
         )
 
@@ -426,15 +382,15 @@
 
     async def multipart_complete_upload(
         self,
         bucket_name: str,
         bucket_key: str,
         upload_id: str,
         parts: list[CompletedPartTypeDef],
-    ):
+    ) -> str:
         root = ET.Element("CompleteMultipartUpload")
 
         for part in parts:
             if "PartNumber" not in part:
                 raise ValueError("PartNumber is required")
             if "ETag" not in part:
                 raise ValueError("ETag is required")
@@ -447,10 +403,85 @@
             "POST",
             f"https://storage.googleapis.com/{bucket_name}/{bucket_key}?uploadId={upload_id}",
             data=ET.tostring(root),
         )
 
         blob = await self.get_blob_meta(bucket_name, bucket_key)
         if blob is None:
-            raise ServerError("Failed to complete multipart upload. Can't find blob")
+            raise ServerError("Failed to complete multipart upload: can't find blob")
+        if blob.generation is None:
+            raise ServerError("The uploaded blob has no generation")
 
         return blob.generation
+
+
+class AsyncHTTPIterator:
+    def __init__(
+        self,
+        url: str,
+        headers: dict,
+        params: dict,
+        storage_client: AsyncStorageClient,
+        max_items: int | None = None,
+    ):
+        self.url = url
+        self.headers = headers
+        self.params = params
+        self.next_page_token = None
+        self.prefixes: set[str] = set()
+        self.items = []
+        self.storage_client = storage_client
+
+        self.cur_item = 0
+        self.max_items = max_items
+
+    def __aiter__(self):
+        return self
+
+    async def __anext__(self):
+        if (self.max_items is not None and self.cur_item >= self.max_items) or (
+            len(self.items) == 0 and self.next_page_token == ""
+        ):
+            raise StopAsyncIteration
+
+        if len(self.items) > 0:
+            obj = self.items.pop()
+            self.cur_item = self.cur_item + 1
+
+            creation_time = obj.get("timeCreated")
+            if creation_time is not None:
+                creation_time = datetime.fromisoformat(creation_time)
+
+            update_time = obj.get("updated")
+            if update_time is not None:
+                update_time = datetime.fromisoformat(update_time)
+
+            return Object(
+                id=obj["id"],
+                name=obj["name"],
+                bucket=obj["bucket"],
+                media_link=obj.get("mediaLink"),
+                generation=obj.get("generation"),
+                content_type=obj["contentType"],
+                size=int(obj["size"]),
+                creation_time=creation_time,
+                update_time=update_time,
+            )
+
+        if self.next_page_token:
+            self.params["pageToken"] = self.next_page_token
+
+        res = await self.storage_client._make_api_request(
+            "GET", self.url, headers=self.headers, params=self.params, return_json=True
+        )
+
+        self.items = res.get("items", [])
+        prefixes = res.get("prefixes", [])
+        self.next_page_token = res.get("nextPageToken", "")
+
+        for prefix in prefixes:
+            self.prefixes.add(prefix)
+
+        if "items" not in res:
+            raise StopAsyncIteration
+
+        return await self.__anext__()
```

### Comparing `latch_cloud_clients-0.1.4/latch_cloud_clients/storage_clients.py` & `latch_cloud_clients-0.1.5/latch_cloud_clients/aws/storage_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,179 +1,141 @@
 import asyncio
 import math
 from collections.abc import AsyncGenerator, Coroutine
-from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 import botocore.exceptions
-from google.api_core.exceptions import (
-    NotFound,
-)
-from latch_o11y.o11y import trace_function_with_span
-from opentelemetry.trace import Span, get_tracer
+from latch_aws.aws import max_presigned_url_age
+from latch_aws.client_pool import s3_pool
+
+# from latch_o11y.o11y import trace_function_with_span
+# from opentelemetry.trace import Span, get_tracer
 from types_aiobotocore_s3.type_defs import (
     CompletedPartTypeDef,
 )
 
-from .aws.aws import max_presigned_url_age
-from .aws.client_pool import s3_pool
-from .gcp.client_pool import gcp_pool
-
-tracer = get_tracer(__name__)
-
-MP_THRESHOLD = 25000000
-MP_CHUNK_SIZE = 25000000
-
-
-class EmptyMountResponseError(Exception):
-    pass
+from ..utils import MP_CHUNK_SIZE, BlobMeta, EmptyMountResponseError, StorageClient
 
 
-@dataclass
-class BlobMeta:
-    bucket: str
-    key: str
-    content_type: Any
-    size: int
-    version: Any
-    update_time: datetime | None
-
-
-class S3MountClient:
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def head(s: Span, bucket_name: str, key: str) -> BlobMeta:
-        s.set_attributes({"bucket_name": bucket_name, "key": key})
+class S3StorageClient(StorageClient):
+    async def head(self, bucket_name: str, key: str) -> BlobMeta:
+        # s.set_attributes({"bucket_name": bucket_name, "key": key})
         blob = None
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
             try:
                 obj = await s3.head_object(Bucket=bucket_name, Key=key)
                 if key.endswith("/"):
                     obj["ContentType"] = "dir"
                     obj["ContentLength"] = 0
             except botocore.exceptions.ClientError as e:
-                s.record_exception(e)
+                # s.record_exception(e)
                 res = e.response
                 if res.get("Error", {}).get("Code") != "404":
                     raise e
 
                 try:
                     res = await s3.list_objects_v2(
                         Bucket=bucket_name,
                         Prefix=key,
                         MaxKeys=1,
                     )
-                    if "Contents" in res:
-                        key = key.rstrip("/") + "/"
-                        obj = {
-                            "ContentType": "dir",
-                            "ContentLength": 0,
-                            "LastModified": None,
-                            "VersionId": None,
-                        }
-                    else:
+                    if "Contents" not in res:
                         raise EmptyMountResponseError()
+
+                    key = key.rstrip("/") + "/"
+                    obj = {
+                        "ContentType": "dir",
+                        "ContentLength": 0,
+                        "LastModified": None,
+                        "VersionId": None,
+                    }
                 except botocore.exceptions.ClientError as e:
-                    s.record_exception(e)
+                    # s.record_exception(e)
                     raise EmptyMountResponseError from e
 
             blob = BlobMeta(
                 bucket=bucket_name,
                 key=key,
                 content_type=obj["ContentType"],
                 size=obj["ContentLength"],
                 version=obj.get("VersionId"),
                 update_time=obj.get("LastModified"),
             )
         return blob
 
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def get_blob_bytes(
-        s: Span,
+        self,
         bucket_name: str,
         key: str,
         start: int | None = None,
         end: int | None = None,
     ) -> bytes:
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
-            meta = await S3MountClient.head(bucket_name=bucket_name, key=key)
+            meta = await self.head(bucket_name=bucket_name, key=key)
 
             start = start if start is not None else 0
             end = end if end is not None else meta.size - 1
 
             response = await s3.get_object(
                 Bucket=bucket_name,
                 Key=key,
                 Range=f"bytes={start}-{end}",
             )
 
             return await response["Body"].read()
 
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def list_keys(
-        s: Span,
+        self,
         bucket_name: str,
         prefix: str | None = None,
         delimiter: str = "/",
-        page_size: int = 100,
-    ) -> AsyncGenerator[list[str], Any]:
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "prefix": str(prefix),
-                "delimeter": delimiter,
-                "page_size": page_size,
-            }
-        )
+    ) -> AsyncGenerator[str, Any]:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "prefix": str(prefix),
+        #         "delimeter": delimiter,
+        #         "page_size": page_size,
+        #     }
+        # )
 
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
             paginator = s3.get_paginator("list_objects_v2")
 
             params = {
                 "Bucket": bucket_name,
                 "Delimiter": delimiter,
             }
             if prefix is not None:
                 params["Prefix"] = prefix
 
-            data: list[str] = []
             async for page in paginator.paginate(**params):
                 for x in [y["Key"] for y in page.get("Contents", [])] + [
                     y["Prefix"] for y in page.get("CommonPrefixes", [])
                 ]:
                     if prefix is None or x.rstrip("/") != prefix.rstrip("/"):
-                        data.append(x)
-
-                    if len(data) > page_size:
-                        yield data
-                        data = []
+                        yield x
 
-            yield data
-
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def put_blob(
-        s: Span,
+        self,
         bucket_name: str,
         key: str,
         body: bytes = b"",
         content_type: str = "text/plain",
         acl: str = "bucket-owner-full-control",
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "key": key,
-                "body": body,
-                "content_type": str(content_type),
-            }
-        )
+    ) -> BlobMeta:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "key": key,
+        #         "body": body,
+        #         "content_type": str(content_type),
+        #     }
+        # )
 
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
             res = await s3.put_object(
                 Bucket=bucket_name,
                 Key=key,
                 Body=body,
                 ContentType=content_type,
@@ -185,79 +147,75 @@
                 key=key,
                 content_type=content_type,
                 size=len(body),
                 version=res["VersionId"],
                 update_time=datetime.now(),
             )
 
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def copy_blob(
-        s: Span,
+        self,
         src_key: str,
         src_bucket: str,
         dest_key: str,
         dest_bucket: str,
-    ):
-        s.set_attributes(
-            {
-                "src_key": src_key,
-                "src_bucket": src_bucket,
-                "dest_key": dest_key,
-                "dest_bucket": dest_bucket,
-            }
-        )
+    ) -> None:
+        # s.set_attributes(
+        #     {
+        #         "src_key": src_key,
+        #         "src_bucket": src_bucket,
+        #         "dest_key": dest_key,
+        #         "dest_bucket": dest_bucket,
+        #     }
+        # )
 
-        blob = await S3MountClient.head(src_bucket, src_key)
+        blob = await self.head(src_bucket, src_key)
         if blob is None:
             return
         async with s3_pool.s3_client_for_bucket(dest_bucket) as s3:
             await s3.copy_object(
                 CopySource={
                     "Bucket": src_bucket,
                     "Key": src_key,
                 },
                 Bucket=dest_bucket,
                 Key=dest_key,
                 ContentType=blob.content_type,
                 ACL="bucket-owner-full-control",
             )
 
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def multipart_copy_blob(
-        s: Span,
+    async def copy_blob_multipart(
+        self,
         src_key: str,
         src_bucket: str,
         dest_key: str,
         dest_bucket: str,
-    ):
-        s.set_attributes(
-            {
-                "src_key": src_key,
-                "src_bucket": src_bucket,
-                "dest_key": dest_key,
-                "dest_bucket": dest_bucket,
-            }
-        )
+    ) -> None:
+        # s.set_attributes(
+        #     {
+        #         "src_key": src_key,
+        #         "src_bucket": src_bucket,
+        #         "dest_key": dest_key,
+        #         "dest_bucket": dest_bucket,
+        #     }
+        # )
 
-        blob = await S3MountClient.head(src_bucket, src_key)
+        blob = await self.head(src_bucket, src_key)
         if blob is None:
             raise EmptyMountResponseError()
 
         async with s3_pool.s3_client_for_bucket(dest_bucket) as s3:
-            upload_id = await S3MountClient.multipart_initiate_upload(
+            upload_id = await self.multipart_initiate_upload(
                 dest_bucket,
                 dest_key,
                 blob.content_type,
                 "bucket-owner-full-control",
             )
 
             parts = math.ceil(blob.size / MP_CHUNK_SIZE)
-            s.set_attribute("copy.nrof_parts", parts)
+            # s.set_attribute("copy.nrof_parts", parts)
 
             async def run_upload_chunk(
                 byte_range: str, index: int
             ) -> CompletedPartTypeDef:
                 res = await s3.upload_part_copy(
                     CopySource={
                         "Bucket": src_bucket,
@@ -292,59 +250,55 @@
                     upload_chunk_responses.extend(
                         await asyncio.gather(*upload_chunk_requests)
                     )
                     upload_chunk_requests = []
 
             upload_chunk_responses.extend(await asyncio.gather(*upload_chunk_requests))
 
-            await S3MountClient.multipart_complete_upload(
+            await self.multipart_complete_upload(
                 dest_bucket, dest_key, upload_id, upload_chunk_responses
             )
 
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def delete_blob(
-        s: Span,
+        self,
         bucket_name: str,
         key: str,
-    ):
-        s.set_attributes({"bucket_name": bucket_name, "key": key})
+    ) -> None:
+        # s.set_attributes({"bucket_name": bucket_name, "key": key})
         try:
             async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
                 await s3.delete_object(
                     Bucket=bucket_name,
                     Key=key,
                 )
         except botocore.exceptions.ClientError as e:
             res = e.response
             if res.get("Error", {}).get("Code") != "404":
                 raise e
 
             return
 
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def generate_presigned_url(
-        s: Span,
+    async def generate_signed_download_url(
+        self,
         bucket_name: str,
         key: str | None,
         content_disposition: str | None = None,
         content_type: str | None = None,
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "key": str(key),
-                "content_disposition": str(content_disposition),
-                "content_type": str(content_type),
-            }
-        )
+    ) -> str:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "key": str(key),
+        #         "content_disposition": str(content_disposition),
+        #         "content_type": str(content_type),
+        #     }
+        # )
 
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
-            return s3.generate_presigned_url(
+            return await s3.generate_presigned_url(
                 "get_object",
                 Params={
                     "Bucket": bucket_name,
                     "Key": key,
                     # todo(maximsmol): add extra validation
                     # "ExpectedBucketOwner": "",
                     # "IfMatch": "",
@@ -359,117 +313,109 @@
                     {"ResponseContentType": content_type}
                     if content_type is not None
                     else {}
                 ),
                 ExpiresIn=max_presigned_url_age,
             )
 
-    @staticmethod
-    @trace_function_with_span(tracer)
+    async def generate_signed_part_upload_url(
+        self,
+        bucket_name: str,
+        bucket_key: str,
+        upload_id: str,
+        part_number: int,
+    ) -> str:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "bucket_key": bucket_key,
+        #         "part_number": part_number,
+        #     }
+        # )
+
+        async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
+            return await s3.generate_presigned_url(
+                "upload_part",
+                Params={
+                    "Bucket": bucket_name,
+                    "Key": bucket_key,
+                    "UploadId": upload_id,
+                    "PartNumber": part_number,
+                    # todo(maximsmol): add extra validation
+                    # "ExpectedBucketOwner": "",
+                },
+                ExpiresIn=max_presigned_url_age,
+            )
+
     async def multipart_initiate_upload(
-        s: Span,
+        self,
         bucket_name: str,
         bucket_key: str,
         content_type: str,
         acl: str = "bucket-owner-full-control",
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-                "content_type": content_type,
-                "acl": acl,
-            }
-        )
+    ) -> str:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "bucket_key": bucket_key,
+        #         "content_type": content_type,
+        #         "acl": acl,
+        #     }
+        # )
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
             multipart_res = await s3.create_multipart_upload(
                 Bucket=bucket_name,
                 Key=bucket_key,
                 ACL=acl,
                 ContentType=content_type,
                 # todo(maximsmol): add extra validation
                 # "ExpectedBucketOwner": "",
             )
             return multipart_res["UploadId"]
 
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def multipart_upload_part(
-        s: Span,
+        self,
         bucket_name: str,
         bucket_key: str,
         upload_id: str,
         part_number: int,
         data: bytes,
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-                "part_number": part_number,
-            }
-        )
+    ) -> str:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "bucket_key": bucket_key,
+        #         "part_number": part_number,
+        #     }
+        # )
 
         async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
             ret = await s3.upload_part(
                 Bucket=bucket_name,
                 Key=bucket_key,
                 UploadId=upload_id,
                 PartNumber=part_number,
                 Body=data,
             )
             return ret["ETag"]
 
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def generate_presigned_part_upload_url(
-        s: Span,
-        bucket_name: str,
-        bucket_key: str,
-        upload_id: str,
-        part_number: int,
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-                "part_number": part_number,
-            }
-        )
-
-        async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
-            return await s3.generate_presigned_url(
-                "upload_part",
-                Params={
-                    "Bucket": bucket_name,
-                    "Key": bucket_key,
-                    "UploadId": upload_id,
-                    "PartNumber": part_number,
-                    # todo(maximsmol): add extra validation
-                    # "ExpectedBucketOwner": "",
-                },
-                ExpiresIn=max_presigned_url_age,
-            )
-
-    @staticmethod
-    @trace_function_with_span(tracer)
     async def multipart_complete_upload(
-        s: Span,
+        self,
         bucket_name: str,
         bucket_key: str,
         upload_id: str,
         parts: list[CompletedPartTypeDef],
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-                "upload_id": upload_id,
-            }
-        )
+    ) -> str:
+        # s.set_attributes(
+        #     {
+        #         "bucket_name": bucket_name,
+        #         "bucket_key": bucket_key,
+        #         "upload_id": upload_id,
+        #     }
+        # )
 
         try:
             async with s3_pool.s3_client_for_bucket(bucket_name) as s3:
                 res = await s3.complete_multipart_upload(
                     Bucket=bucket_name,
                     Key=bucket_key,
                     UploadId=upload_id,
@@ -487,312 +433,7 @@
             if "Code" not in err_res["Error"]:
                 raise e
 
             if err_res["Error"]["Code"] != "EntityTooSmall":
                 raise e
 
             raise ValueError("Upload size is less than minimum allowed") from e
-
-
-class GCPMountClient:
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def head(s: Span, bucket_name: str, key: str) -> BlobMeta:
-        s.set_attributes({"bucket_name": bucket_name, "key": key})
-        async with gcp_pool.gcp_client() as gcp:
-            client = gcp.storage_client()
-            blob = await client.get_blob_meta(bucket_name, key)
-
-            if blob is None:
-                raise EmptyMountResponseError()
-
-            blob = BlobMeta(
-                bucket=bucket_name,
-                key=key,
-                content_type=blob.content_type,
-                size=blob.size,
-                version=blob.generation,
-                update_time=blob.update_time,
-            )
-
-            return blob
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def get_blob_bytes(
-        s: Span,
-        bucket_name: str,
-        key: str,
-        start: int | None = None,
-        end: int | None = None,
-    ) -> bytes:
-        s.set_attributes({"bucket_name": bucket_name, "key": key})
-        async with gcp_pool.gcp_client() as gcp:
-            client = gcp.storage_client()
-
-            try:
-                return await client.get_blob_bytes(
-                    bucket_name, key, start=start, end=end
-                )
-            except NotFound as e:
-                raise EmptyMountResponseError() from e
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def list_keys(
-        s: Span,
-        bucket_name: str,
-        prefix: str | None = None,
-        delimiter: str = "/",
-        page_size: int = 100,
-    ) -> AsyncGenerator[list[str], Any]:
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "prefix": str(prefix),
-                "delimeter": delimiter,
-                "page_size": page_size,
-            }
-        )
-        async with gcp_pool.gcp_client() as gcp:
-            client = gcp.storage_client()
-
-            iterator = client.list_blobs(
-                bucket_name,
-                prefix=prefix,
-                delimiter=delimiter,
-            )
-
-            data = []
-            async for obj in iterator:
-                # don't add the prefix itself to the list
-                if prefix is None or obj.name.rstrip("/") != prefix.rstrip("/"):
-                    data.append(obj.name)
-
-                if len(data) >= page_size:
-                    yield data
-                    data = []
-
-            # all the prefixes are present after executing iterator above
-            blob_prefixes = set(iterator.prefixes)
-
-            for p in blob_prefixes:
-                if prefix is None or p.rstrip("/") != prefix.rstrip("/"):
-                    data.append(obj)
-                if len(data) >= page_size:
-                    yield data
-                    data = []
-
-            if len(data) > 0:
-                yield data
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def put_blob(
-        s: Span,
-        bucket_name: str,
-        key: str,
-        body: bytes = b"",
-        content_type: str | None = None,
-        acl: str = "bucket-owner-full-control",
-    ):
-        s.set_attributes({"bucket_name": bucket_name, "key": key})
-
-        async with gcp_pool.gcp_client() as gcp:
-            client = gcp.storage_client()
-
-            content_type = content_type if content_type else "text/plain"
-
-            obj = await client.put_blob(
-                bucket_name, key, body, content_type=content_type
-            )
-
-            return BlobMeta(
-                bucket=bucket_name,
-                key=key,
-                content_type=content_type,
-                size=len(body),
-                version=obj.generation,
-                update_time=obj.update_time,
-            )
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def copy_blob(
-        s: Span,
-        src_key: str,
-        src_bucket_name: str,
-        dest_key: str,
-        dest_bucket_name: str,
-    ):
-        s.set_attributes(
-            {
-                "src_key": src_key,
-                "src_bucket_name": src_bucket_name,
-                "dest_key": dest_key,
-                "dest_bucket_name": dest_bucket_name,
-            }
-        )
-
-        async with gcp_pool.gcp_client() as gcp:
-            client = gcp.storage_client()
-
-            try:
-                await client.copy_blob(
-                    src_bucket_name=src_bucket_name,
-                    src_bucket_key=src_key,
-                    dest_bucket_name=dest_bucket_name,
-                    dest_bucket_key=dest_key,
-                )
-            except NotFound as e:
-                s.record_exception(e)
-                raise EmptyMountResponseError from e
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def multipart_copy_blob(
-        s: Span,
-        src_key: str,
-        src_bucket: str,
-        dest_key: str,
-        dest_bucket: str,
-    ):
-        s.set_attributes(
-            {
-                "src_key": src_key,
-                "src_bucket": src_bucket,
-                "dest_key": dest_key,
-                "dest_bucket": dest_bucket,
-            }
-        )
-        await GCPMountClient.copy_blob(src_key, src_bucket, dest_key, dest_bucket)
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def delete_blob(
-        s: Span,
-        bucket_name: str,
-        key: str,
-    ):
-        s.set_attributes({"bucket_name": bucket_name, "key": key})
-        async with gcp_pool.gcp_client() as gcp:
-            await gcp.storage_client().delete_blob(bucket_name, key)
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def generate_presigned_url(
-        s: Span,
-        bucket_name: str,
-        key: str | None,
-        content_disposition: str | None = None,
-        content_type: str | None = None,
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "key": str(key),
-                "content_disposition": str(content_disposition),
-                "content_type": str(content_type),
-            }
-        )
-        async with gcp_pool.gcp_client() as gcp:
-            url = gcp.storage_client().get_signed_url(
-                bucket_name=bucket_name,
-                key=key,
-                content_disposition=content_disposition,
-                content_type=content_type,
-            )
-
-            async def generate_signed_url():
-                return url
-
-            return generate_signed_url()
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def generate_presigned_part_upload_url(
-        s: Span,
-        bucket_name: str,
-        bucket_key: str,
-        upload_id: str,
-        part_number: int,
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-                "idx": part_number,
-            }
-        )
-
-        async with gcp_pool.gcp_client() as gcp:
-            return await gcp.storage_client().get_signed_upload_url(
-                bucket_name=bucket_name,
-                key=bucket_key,
-                upload_id=upload_id,
-                part_number=part_number,
-            )
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def multipart_initiate_upload(
-        s: Span,
-        bucket_name: str,
-        bucket_key: str,
-        content_type: str,
-        acl: str = "storageAdmin",
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "key": bucket_key,
-                "content_type": content_type,
-                "acl": acl,
-            }
-        )
-        async with gcp_pool.gcp_client() as gcp:
-            return await gcp.storage_client().multipart_initiate_upload(
-                bucket_name, bucket_key, content_type
-            )
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def multipart_upload_part(
-        s: Span,
-        bucket_name: str,
-        bucket_key: str,
-        upload_id: str,
-        part_number: int,
-        data: bytes,
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-                "part_number": part_number,
-            }
-        )
-
-        async with gcp_pool.gcp_client() as gcp:
-            return await gcp.storage_client().multipart_upload_part(
-                bucket_name, bucket_key, upload_id, part_number, data
-            )
-
-    @staticmethod
-    @trace_function_with_span(tracer)
-    async def multipart_complete_upload(
-        s: Span,
-        bucket_name: str,
-        bucket_key: str,
-        upload_id: str,
-        parts: list[CompletedPartTypeDef],
-    ):
-        s.set_attributes(
-            {
-                "bucket_name": bucket_name,
-                "bucket_key": bucket_key,
-            }
-        )
-        async with gcp_pool.gcp_client() as gcp:
-            return await gcp.storage_client().multipart_complete_upload(
-                bucket_name, bucket_key, upload_id, parts
-            )
```

### Comparing `latch_cloud_clients-0.1.4/pyproject.toml` & `latch_cloud_clients-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-cloud-clients"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Taras Priadka <taras@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_cloud_clients"}]
 
 [tool.poetry.dependencies]
@@ -16,22 +16,24 @@
 types-aiobotocore = { extras = ["s3"], version = "^2.4.2" }
 google-auth = "^2.29.0"
 requests = "^2.31.0"
 google-cloud = "^0.34.0"
 google-cloud-storage = "^2.16.0"
 google-api-core = "^2.18.0"
 xmltodict = "^0.13.0"
+latch-aws = "^0.1.9"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 rich = "^13.2.0"
 ruff = "^0.0.269"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
+pytest-timeout = "^2.3.1"
 
 [tool.black]
 preview = true
 target-version = ["py311"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `latch_cloud_clients-0.1.4/PKG-INFO` & `latch_cloud_clients-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: latch-cloud-clients
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: CC0 1.0
 Author: Taras Priadka
 Author-email: taras@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiobotocore[s3] (>=2.4.2,<3.0.0)
 Requires-Dist: google-api-core (>=2.18.0,<3.0.0)
 Requires-Dist: google-auth (>=2.29.0,<3.0.0)
 Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
 Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
+Requires-Dist: latch-aws (>=0.1.9,<0.2.0)
 Requires-Dist: latch-data-validation (>=0.1.3,<0.2.0)
 Requires-Dist: latch-o11y (>=0.1.4,<0.2.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-aiobotocore[s3] (>=2.4.2,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
```


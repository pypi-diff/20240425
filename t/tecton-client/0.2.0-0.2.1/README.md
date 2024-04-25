# Comparing `tmp/tecton_client-0.2.0.tar.gz` & `tmp/tecton_client-0.2.1.tar.gz`

## Comparing `tecton_client-0.2.0.tar` & `tecton_client-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tecton_client-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 tecton_client-0.2.0/RELEASE.md
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/release-docs.yml
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/testing.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/make.bat
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/quickstart.rst
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/tecton_client.rst
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tecton_client-0.2.0/examples/example_async.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tecton_client-0.2.0/examples/example_sync.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/__about__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/__init__.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/__init__.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/async_tecton_client.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/data_types.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/tecton_client.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/utils.py
--rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_async_client.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_data_types.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_tecton_client.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_data/nested_sample_response.json
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_data/sample_response.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.gitignore
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 tecton_client-0.2.0/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 tecton_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 tecton_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tecton_client-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 tecton_client-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tecton_client-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 tecton_client-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tecton_client-0.2.1/docs/index.rst
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tecton_client-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 tecton_client-0.2.1/docs/quickstart.rst
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tecton_client-0.2.1/docs/tecton_client.rst
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 tecton_client-0.2.1/examples/example_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 tecton_client-0.2.1/examples/example_sync.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/__about__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/__init__.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/_internal/__init__.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/_internal/async_tecton_client.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/_internal/request_utils.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/_internal/response_utils.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/_internal/tecton_client.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tecton_client/_internal/utils.py
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tests/test_async_client.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tests/test_response_utils.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tests/test_tecton_client.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tests/test_data/nested_sample_response.json
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tests/test_data/sample_response.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 tecton_client-0.2.1/tests/test_data/slo_info_sample_response.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tecton_client-0.2.1/.gitignore
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 tecton_client-0.2.1/README.md
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 tecton_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 tecton_client-0.2.1/PKG-INFO
```

### Comparing `tecton_client-0.2.0/.pre-commit-config.yaml` & `tecton_client-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/CONTRIBUTING.md` & `tecton_client-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/RELEASE.md` & `tecton_client-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `tecton_client-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `tecton_client-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/.github/workflows/release-docs.yml` & `tecton_client-0.2.1/.github/workflows/release-docs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 name: publish docs to github pages
 
 on:
+  # Runs on pushes targeting the default branch
   release:
     types: [published]
+
+  # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
+# Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
+permissions:
+  contents: read
+  pages: write
+  id-token: write
+
+# Allow only one concurrent deployment, skipping runs queued between the run in-progress and latest queued.
+# However, do NOT cancel in-progress runs as we want to allow these production deployments to complete.
+concurrency:
+  group: "pages"
+  cancel-in-progress: false
+
 jobs:
   build-docs:
     name: Build the Docs
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
@@ -17,29 +32,37 @@
           pip install -e ".[docs]"
       - name: Install tecton_client
         run: |
           pip install .
       - name: Sphinx build
         run: |
           sphinx-build docs docs/build
-      - name: Upload artifact
-        uses: actions/upload-pages-artifact@v1
+      - name: upload artifacts
+        uses: actions/upload-artifact@v4
         with:
+          name: docs
           path: ./docs/build
+          if-no-files-found: error
 
   deploy-docs:
-      runs-on: ubuntu-latest
-      needs: build-docs
-
-      permissions:
-        pages: write
-        id-token: write
-
-      environment:
-        # environment created automatically by GitHub
-        name: github-pages
-        url: ${{ steps.deployment.outputs.page_url }}
-
-      steps:
-        - name: Deploy to GitHub Pages
-          id: deployment
-          uses: actions/deploy-pages@v2
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    runs-on: ubuntu-latest
+    needs: build-docs
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+      - name: Setup Pages
+        uses: actions/configure-pages@v5
+      - name: Download artifacts from build
+        uses: actions/download-artifact@v4
+        with:
+          name: docs
+          path: ./build
+      - name: Upload artifact
+        uses: actions/upload-pages-artifact@v3
+        with:
+          path: ./build
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v4
```

### Comparing `tecton_client-0.2.0/.github/workflows/release.yml` & `tecton_client-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/.github/workflows/testing.yml` & `tecton_client-0.2.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/docs/Makefile` & `tecton_client-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/docs/conf.py` & `tecton_client-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/docs/index.rst` & `tecton_client-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/docs/make.bat` & `tecton_client-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/docs/quickstart.rst` & `tecton_client-0.2.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/docs/tecton_client.rst` & `tecton_client-0.2.1/docs/tecton_client.rst`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/examples/example_async.py` & `tecton_client-0.2.1/examples/example_async.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from tecton_client import AsyncTectonClient, MetadataOptions
 
 my_url = "https://explore.tecton.ai/"
 workspace = "prod"
 my_api_key = os.environ.get("TECTON_API_KEY")
 
-
 async_client = AsyncTectonClient(url=my_url, api_key=my_api_key, default_workspace_name=workspace)
 
 
 async def call_api_ten_times():
     requests = [
         async_client.get_features(
             feature_service_name="fraud_detection_feature_service:v2",
@@ -21,9 +20,20 @@
         )
         for i in range(10)
     ]
     responses = await asyncio.gather(*requests)
     for resp in responses:
         print(resp.result.features)
 
+    # also call get_feature_service_metadata
+    requests = [
+        async_client.get_feature_service_metadata(
+            feature_service_name="fraud_detection_feature_service:v2",
+        )
+        for i in range(10)
+    ]
+    responses = await asyncio.gather(*requests)
+    for resp in responses:
+        print(resp)
+
 
 asyncio.run(call_api_ten_times())
```

### Comparing `tecton_client-0.2.0/examples/example_sync.py` & `tecton_client-0.2.1/examples/example_sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 client = TectonClient(url=my_url, default_workspace_name=workspace, api_key=my_api_key)
 
 resp = client.get_features(
     feature_service_name="fraud_detection_feature_service:v2",
     join_key_map={"user_id": "user_4407104885"},
     request_context_map={"amount": 500.00},
-    metadata_options=MetadataOptions(include_data_types=True),
+    metadata_options=MetadataOptions.all(),
 )
 
 print("A nicely formatted output")
 print(resp.get_features_dict())
 
 print("Full response: ")
 print(resp)
```

### Comparing `tecton_client-0.2.0/tecton_client/exceptions.py` & `tecton_client-0.2.1/tecton_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/tecton_client/_internal/async_tecton_client.py` & `tecton_client-0.2.1/tecton_client/_internal/async_tecton_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Dict, Optional, Union
 from urllib.parse import urljoin
 
 import httpx
 from httpx import HTTPStatusError
 
-from tecton_client._internal.data_types import (
+from tecton_client._internal.request_utils import MetadataOptions, RequestOptions
+from tecton_client._internal.response_utils import (
     GetFeatureServiceMetadataResponse,
     GetFeaturesResponse,
-    MetadataOptions,
-    RequestOptions,
 )
 from tecton_client._internal.utils import (
     build_get_feature_service_metadata_request,
     build_get_features_request,
     get_default_headers,
     validate_request_args,
 )
@@ -26,14 +25,15 @@
     (`pip install tecton`) and not this client library.
 
     Examples:
 
     .. code-block:: python
 
         import asyncio
+        from tecton_client import AsyncTectonClient, MetadataOptions
 
         async_client = AsyncTectonClient(
             url="http://explore.tecton.ai", api_key="my_key", default_workspace_name="prod"
         )
         asyncio.run(
             async_client.get_features(
                 feature_service_name="fraud_detection_feature_service:v2",
@@ -143,14 +143,14 @@
         validate_request_args(feature_service_name, workspace_name, self.default_workspace_name)
         if not workspace_name:
             workspace_name = self.default_workspace_name
         request_data = build_get_feature_service_metadata_request(
             feature_service_name=feature_service_name,
             workspace_name=workspace_name,
         )
-        resp = self._client.post(url=self._paths["get_feature_service_metadata"], json=request_data)
+        resp = await self._client.post(url=self._paths["get_feature_service_metadata"], json=request_data)
         try:
             resp.raise_for_status()
         except HTTPStatusError as exc:
             raise convert_exception(exc) from exc
 
         return GetFeatureServiceMetadataResponse.from_response(resp.json())
```

### Comparing `tecton_client-0.2.0/tecton_client/_internal/tecton_client.py` & `tecton_client-0.2.1/tecton_client/_internal/tecton_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any, Dict, Optional, Union
 from urllib.parse import urljoin
 
 import httpx
 from httpx import HTTPStatusError
 
-from tecton_client._internal.data_types import (
+from tecton_client._internal.request_utils import MetadataOptions, RequestOptions
+from tecton_client._internal.response_utils import (
     GetFeatureServiceMetadataResponse,
     GetFeaturesResponse,
-    MetadataOptions,
-    RequestOptions,
 )
 from tecton_client._internal.utils import (
     build_get_feature_service_metadata_request,
     build_get_features_request,
     get_default_headers,
     validate_request_args,
 )
@@ -24,14 +23,15 @@
 
     For feature development and interacting with the rest of your Tecton deployment, use the Tecton SDK
     (`pip install tecton`) and not this client library.
 
     Examples:
 
     .. code-block:: python
+        from tecton_client import TectonClient, MetadataOptions
 
         client = TectonClient(
             url="http://explore.tecton.ai", api_key="my_key", default_workspace_name="prod"
         )
         client.get_features(
             feature_service_name="fraud_detection_feature_service:v2",
             join_key_map={"user_id": "user_4407104885"},
```

### Comparing `tecton_client-0.2.0/tecton_client/_internal/utils.py` & `tecton_client-0.2.1/tecton_client/_internal/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
-from tecton_client.__about__ import __version__ as tecton_version
-from tecton_client._internal.data_types import MetadataOptions, RequestOptions
+from tecton_client.__about__ import __version__ as tecton_client_version
+from tecton_client._internal.request_utils import MetadataOptions, RequestOptions
 
 
 def get_default_headers(api_key):
     return httpx.Headers(
-        {"Authorization": "Tecton-key " + api_key, "User-Agent": "tecton-http-python-client " + tecton_version}
+        {"Authorization": "Tecton-key " + api_key, "User-Agent": "tecton-http-python-client " + tecton_client_version}
     )
 
 
 def build_get_features_request(
     feature_service_name: str,
     join_key_map: Optional[Dict[str, Optional[Union[int, str]]]] = None,
     request_context_map: Optional[Dict[str, Any]] = None,
```

### Comparing `tecton_client-0.2.0/tests/test_async_client.py` & `tecton_client-0.2.1/tests/test_async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
-from unittest import TestCase
-from unittest.mock import MagicMock, patch
+from unittest import IsolatedAsyncioTestCase
+from unittest.mock import AsyncMock, MagicMock, patch
 
 import httpx
 from httpx import Headers
-from pytest import mark
 
 from tecton_client import AsyncTectonClient, MetadataOptions, RequestOptions
 from tecton_client.exceptions import NotFoundError
 
 
-class TestTectonClient(TestCase):
+class TestTectonClient(IsolatedAsyncioTestCase):
     def mockPatch(self, *args, **kwargs):
         patcher = patch(*args, **kwargs)
         self.addCleanup(patcher.stop)
         return patcher.start()
 
     def setUp(self):
         _request_log = []
@@ -22,67 +21,64 @@
         def handler(request):
             _request_log.append(json.loads(request.content.decode("utf8")))
             return httpx.Response(200, json={"result": {"features": []}})
 
         self.mock_client = httpx.AsyncClient(transport=httpx.MockTransport(handler))
         self.mock_client._request_log = _request_log
 
-    @patch("tecton_client._internal.utils.tecton_version", "0.1.0test")
+    @patch("tecton_client._internal.utils.tecton_client_version", "0.1.0test")
     def test_client_construction(self):
         mock_httpx_constructor = self.mockPatch("httpx.AsyncClient", autospec=True)
         AsyncTectonClient(url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace")
         mock_httpx_constructor.assert_called_once_with(
             headers=Headers(
                 {"authorization": "Tecton-key fake-api-key", "user-agent": "tecton-http-python-client 0.1.0test"}
             )
         )
 
-    @patch("tecton_client._internal.utils.tecton_version", "0.1.0test")
+    @patch("tecton_client._internal.utils.tecton_client_version", "0.1.0test")
     def test_client_construction_custom_client(self):
         mock_httpx_constructor = self.mockPatch("httpx.AsyncClient", autospec=True)
         mock_client = MagicMock()
         mock_client.headers = {}
         AsyncTectonClient(
             url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=mock_client
         )
         mock_httpx_constructor.assert_not_called()
-        self.assertEquals(
+        self.assertEqual(
             mock_client.headers,
             {"authorization": "Tecton-key fake-api-key", "user-agent": "tecton-http-python-client 0.1.0test"},
         )
 
-    @mark.asyncio
     async def test_default_workspace_null(self):
         client = AsyncTectonClient(url="https://fake.tecton.ai", api_key="fake-api-key", client=self.mock_client)
 
         with self.assertRaisesRegexp(ValueError, "workspace_name not set"):
             await client.get_features(feature_service_name="fake-feature-service", join_key_map={"user_id": "id123"})
 
         await client.get_features(
             feature_service_name="fake-feature-service",
             join_key_map={"user_id": "id123"},
             workspace_name="override-workspace",
         )
         workspace = self.mock_client._request_log[0]["params"]["workspaceName"]
-        self.assertEquals(workspace, "override-workspace")
+        self.assertEqual(workspace, "override-workspace")
 
-    @mark.asyncio
     async def test_default_workspace(self):
         client = AsyncTectonClient(
             url="https://fake.tecton.ai",
             api_key="fake-api-key",
             client=self.mock_client,
             default_workspace_name="fake-workspace",
         )
 
         await client.get_features(feature_service_name="fake-feature-service", join_key_map={"user_id": "id123"})
         workspace = self.mock_client._request_log[0]["params"]["workspaceName"]
-        self.assertEquals(workspace, "fake-workspace")
+        self.assertEqual(workspace, "fake-workspace")
 
-    @mark.asyncio
     async def test_override_workspace(self):
         client = AsyncTectonClient(
             url="https://fake.tecton.ai",
             api_key="fake-api-key",
             client=self.mock_client,
             default_workspace_name="fake-workspace",
         )
@@ -90,40 +86,40 @@
         await client.get_features(
             feature_service_name="fake-feature-service",
             join_key_map={"user_id": "id123"},
             workspace_name="override-workspace",
         )
 
         workspace = self.mock_client._request_log[0]["params"]["workspaceName"]
-        self.assertEquals(workspace, "override-workspace")
+        self.assertEqual(workspace, "override-workspace")
 
-    @mark.asyncio
     async def test_get_features_encode(self):
         # using just magic_mock here in order to assert on client.post.assert_called_with
-        mock_http_client = MagicMock()
-        mock_http_client.post.return_value.json.return_value = {"result": {"features": []}}
+        mock_response = MagicMock()
+        mock_response.json.return_value = {"result": {"features": []}}
+        mock_http_client = MagicMock(post=AsyncMock())
+        mock_http_client.post.return_value = mock_response
         client = AsyncTectonClient(
             url="https://fake.tecton.ai",
             api_key="fake-api-key",
             default_workspace_name="workspace",
             client=mock_http_client,
         )
         await client.get_features(
             feature_service_name="fake-feature-service",
             join_key_map={"user_id": "id123"},
             metadata_options=MetadataOptions(include_effective_times=True, include_data_types=False),
             request_options=RequestOptions(read_from_cache=False),
         )
         mock_http_client.post.assert_called_with(
-            "https://fake.tecton.ai/api/v1/feature-service/get-features",
+            url="https://fake.tecton.ai/api/v1/feature-service/get-features",
             json={
                 "params": {
                     "workspaceName": "workspace",
                     "featureServiceName": "fake-feature-service",
-                    "featureServiceId": None,
                     "joinKeyMap": {"user_id": "id123"},
                     "requestContextMap": {},
                     "allowPartialResults": False,
                     "metadataOptions": {
                         "includeNames": True,
                         "includeDataTypes": False,
                         "includeEffectiveTimes": True,
@@ -131,23 +127,24 @@
                         "includeServingStatus": False,
                     },
                     "requestOptions": {"readFromCache": False, "writeToCache": True},
                 }
             },
         )
 
-    @mark.asycnio
     async def test_get_feature_service_metadata_encode(self):
         # using just magic_mock here in order to assert on client.post.assert_called_with
-        mock_http_client = MagicMock()
-        mock_http_client.post.return_value.json.return_value = {
+        mock_response = MagicMock()
+        mock_response.json.return_value = {
             "inputJoinKeys": [],
             "inputRequestContextKeys": [],
             "featureValues": [],
         }
+        mock_http_client = AsyncMock()
+        mock_http_client.post.return_value = mock_response
         client = AsyncTectonClient(
             url="https://fake.tecton.ai",
             api_key="fake-api-key",
             default_workspace_name="workspace",
             client=mock_http_client,
         )
         await client.get_feature_service_metadata(
@@ -159,28 +156,36 @@
                 "params": {
                     "workspaceName": "workspace",
                     "featureServiceName": "fake-feature-service",
                 }
             },
         )
 
-    @mark.asyncio
     async def test_get_features_decode(self):
-        test_client = httpx.Client(
+        test_client = httpx.AsyncClient(
             transport=httpx.MockTransport(lambda request: httpx.Response(200, json={"result": {"features": []}}))
         )
         client = AsyncTectonClient(
             url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=test_client
         )
         resp = await client.get_features(feature_service_name="fake-feature-service", join_key_map={"user_id": "id123"})
-        self.assertEquals(resp.result.features, [])
+        self.assertEqual(resp.result.features, [])
+
+    async def test_get_feature_service_metadata_decode(self):
+        test_client = httpx.AsyncClient(
+            transport=httpx.MockTransport(lambda request: httpx.Response(200, json={"featureValues": ["this"]}))
+        )
+        client = AsyncTectonClient(
+            url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=test_client
+        )
+        resp = await client.get_feature_service_metadata(feature_service_name="fake-feature-service")
+        self.assertEqual(resp.feature_values, ["this"])
 
-    @mark.asyncio
     async def test_raise_error(self):
-        test_client = httpx.Client(
+        test_client = httpx.AsyncClient(
             transport=httpx.MockTransport(lambda request: httpx.Response(404, json={"result": {"features": []}}))
         )
         client = AsyncTectonClient(
             url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=test_client
         )
         with self.assertRaises(NotFoundError):
             await client.get_features(feature_service_name="fake-feature-service", join_key_map={"user_id": "id123"})
```

### Comparing `tecton_client-0.2.0/tests/test_data_types.py` & `tecton_client-0.2.1/tests/test_response_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 import pathlib
 from unittest import TestCase
 
 from tecton_client import GetFeaturesResponse
+from tecton_client._internal.response_utils import SLOInfo
 
 TEST_DATA_DIR = pathlib.Path(__file__).parent.joinpath("test_data")
 
 
-class TestDataTypes(TestCase):
+class TestResponses(TestCase):
     def test_GetFeaturesResponse_from_dict(self):
         self.maxDiff = 10000
         file_1 = TEST_DATA_DIR.joinpath("sample_response.json")
         with open(file_1) as f:
             resp = json.load(f)
         resp = GetFeaturesResponse.from_response(resp)
-        self.assertEquals(
+        self.assertEqual(
             resp.result.features,
             [["0"], None, [55.5, 57.88, 58.96, 57.66, None, 55.98], ["0", "1", None, "3", "4", None]],
         )
         self.assertDictEqual(
             resp.metadata,
             {
                 "features": [
@@ -71,59 +72,85 @@
                 # Test null in nested array, null in top level array and empty array.
                 "schema.two_dimensional_array": [[123, None], None, []],
                 "schema.simple_struct": {"string_field": "fake-string", "int64_field": 12, "float64_field": 123},
                 "schema.dist_km": 100,
             },
         )
 
+    def test_GetFeaturesResponse_slo_info_null(self):
+        file_1 = TEST_DATA_DIR.joinpath("sample_response.json")
+        with open(file_1) as f:
+            resp = json.load(f)
+        resp = GetFeaturesResponse.from_response(resp)
+        self.assertIsNone(resp.slo_info)
+
+    def test_GetFeaturesResponse_slo_info(self):
+        file_1 = TEST_DATA_DIR.joinpath("slo_info_sample_response.json")
+        with open(file_1) as f:
+            resp = json.load(f)
+        resp = GetFeaturesResponse.from_response(resp)
+        self.assertEqual(
+            resp.slo_info,
+            SLOInfo(
+                slo_eligible=True,
+                slo_ineligibility_reasons=None,
+                slo_server_time_seconds=0.01,
+                server_time_seconds=0.02,
+                store_max_latency=0.03,
+                store_response_size_bytes=4096,
+            ),
+        )
+
+
+class TestGetFeatureValue(TestCase):
     def test_get_feature_value_simple_types(self):
-        self.assertEquals(GetFeaturesResponse._get_feature_value({"type": "string"}, "thing"), "thing")
-        self.assertEquals(GetFeaturesResponse._get_feature_value({"type": "string"}, "thing"), "thing")
-        self.assertEquals(GetFeaturesResponse._get_feature_value({"type": "int64"}, "1"), 1)
-        self.assertEquals(GetFeaturesResponse._get_feature_value({"type": "float64"}, 1), 1)
-        self.assertEquals(GetFeaturesResponse._get_feature_value({"type": "float64"}, "NaN"), "NaN")
+        self.assertEqual(GetFeaturesResponse._get_feature_value({"type": "string"}, "thing"), "thing")
+        self.assertEqual(GetFeaturesResponse._get_feature_value({"type": "string"}, "thing"), "thing")
+        self.assertEqual(GetFeaturesResponse._get_feature_value({"type": "int64"}, "1"), 1)
+        self.assertEqual(GetFeaturesResponse._get_feature_value({"type": "float64"}, 1), 1)
+        self.assertEqual(GetFeaturesResponse._get_feature_value({"type": "float64"}, "NaN"), "NaN")
 
     def test_get_feature_value_array(self):
-        self.assertEquals(
+        self.assertEqual(
             GetFeaturesResponse._get_feature_value({"type": "array", "elementType": {"type": "int64"}}, []), []
         )
-        self.assertEquals(
+        self.assertEqual(
             GetFeaturesResponse._get_feature_value({"type": "array", "elementType": {"type": "int64"}}, None), None
         )
-        self.assertEquals(
+        self.assertEqual(
             GetFeaturesResponse._get_feature_value(
                 {"type": "array", "elementType": {"type": "int64"}}, ["1", None, "2"]
             ),
             [1, None, 2],
         )
 
     def test_get_feature_value_nested_array(self):
-        self.assertEquals(
+        self.assertEqual(
             GetFeaturesResponse._get_feature_value(
                 {"type": "array", "elementType": {"type": "array", "elementType": {"type": "int64"}}},
                 [["1", "2", None], None, []],
             ),
             [[1, 2, None], None, []],
         )
 
     def test_get_feature_value_map(self):
-        self.assertEquals(
+        self.assertEqual(
             GetFeaturesResponse._get_feature_value(
                 {
                     "type": "map",
                     "keyType": {"type": "string"},
                     "valueType": {"type": "int64"},
                 },
                 {"key1": "1", "key2": None},
             ),
             {"key1": 1, "key2": None},
         )
 
     def test_get_feature_value_struct(self):
-        self.assertEquals(
+        self.assertEqual(
             GetFeaturesResponse._get_feature_value(
                 {
                     "type": "struct",
                     "fields": [
                         {"name": "string_field", "dataType": {"type": "string"}},
                         {"name": "int64_field", "dataType": {"type": "int64"}},
                         {"name": "float64_field", "dataType": {"type": "float64"}},
```

### Comparing `tecton_client-0.2.0/tests/test_tecton_client.py` & `tecton_client-0.2.1/tests/test_tecton_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,34 +21,34 @@
         def handler(request):
             _request_log.append(json.loads(request.content.decode("utf8")))
             return httpx.Response(200, json={"result": {"features": []}})
 
         self.mock_client = httpx.Client(transport=httpx.MockTransport(handler))
         self.mock_client._request_log = _request_log
 
-    @patch("tecton_client._internal.utils.tecton_version", "0.1.0test")
+    @patch("tecton_client._internal.utils.tecton_client_version", "0.1.0test")
     def test_client_construction(self):
         mock_httpx_constructor = self.mockPatch("httpx.Client", autospec=True)
         TectonClient(url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace")
         mock_httpx_constructor.assert_called_once_with(
             headers=Headers(
                 {"authorization": "Tecton-key fake-api-key", "user-agent": "tecton-http-python-client 0.1.0test"}
             )
         )
 
-    @patch("tecton_client._internal.utils.tecton_version", "0.1.0test")
+    @patch("tecton_client._internal.utils.tecton_client_version", "0.1.0test")
     def test_client_construction_custom_client(self):
         mock_httpx_constructor = self.mockPatch("httpx.Client", autospec=True)
         mock_client = MagicMock()
         mock_client.headers = {}
         TectonClient(
             url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=mock_client
         )
         mock_httpx_constructor.assert_not_called()
-        self.assertEquals(
+        self.assertEqual(
             mock_client.headers,
             {"authorization": "Tecton-key fake-api-key", "user-agent": "tecton-http-python-client 0.1.0test"},
         )
 
     def test_default_workspace_null(self):
         client = TectonClient(url="https://fake.tecton.ai", api_key="fake-api-key", client=self.mock_client)
 
@@ -57,27 +57,27 @@
 
         client.get_features(
             feature_service_name="fake-feature-service",
             join_key_map={"user_id": "id123"},
             workspace_name="override-workspace",
         )
         workspace = self.mock_client._request_log[0]["params"]["workspaceName"]
-        self.assertEquals(workspace, "override-workspace")
+        self.assertEqual(workspace, "override-workspace")
 
     def test_default_workspace(self):
         client = TectonClient(
             url="https://fake.tecton.ai",
             api_key="fake-api-key",
             client=self.mock_client,
             default_workspace_name="fake-workspace",
         )
 
         client.get_features(feature_service_name="fake-feature-service", join_key_map={"user_id": "id123"})
         workspace = self.mock_client._request_log[0]["params"]["workspaceName"]
-        self.assertEquals(workspace, "fake-workspace")
+        self.assertEqual(workspace, "fake-workspace")
 
     def test_override_workspace(self):
         client = TectonClient(
             url="https://fake.tecton.ai",
             api_key="fake-api-key",
             client=self.mock_client,
             default_workspace_name="fake-workspace",
@@ -86,15 +86,15 @@
         client.get_features(
             feature_service_name="fake-feature-service",
             join_key_map={"user_id": "id123"},
             workspace_name="override-workspace",
         )
 
         workspace = self.mock_client._request_log[0]["params"]["workspaceName"]
-        self.assertEquals(workspace, "override-workspace")
+        self.assertEqual(workspace, "override-workspace")
 
     def test_get_features_encode(self):
         # using just magic_mock here in order to assert on client.post.assert_called_with
         mock_http_client = MagicMock()
         mock_http_client.post.return_value.json.return_value = {"result": {"features": []}}
         client = TectonClient(
             url="https://fake.tecton.ai",
@@ -125,14 +125,51 @@
                         "includeServingStatus": False,
                     },
                     "requestOptions": {"readFromCache": False, "writeToCache": True},
                 }
             },
         )
 
+    def test_get_features_metadata_all(self):
+        # using just magic_mock here in order to assert on client.post.assert_called_with
+        mock_http_client = MagicMock()
+        mock_http_client.post.return_value.json.return_value = {"result": {"features": []}}
+        client = TectonClient(
+            url="https://fake.tecton.ai",
+            api_key="fake-api-key",
+            default_workspace_name="workspace",
+            client=mock_http_client,
+        )
+        client.get_features(
+            feature_service_name="fake-feature-service",
+            join_key_map={"user_id": "id123"},
+            metadata_options=MetadataOptions.all(),
+            request_options=RequestOptions(read_from_cache=False),
+        )
+        mock_http_client.post.assert_called_with(
+            "https://fake.tecton.ai/api/v1/feature-service/get-features",
+            json={
+                "params": {
+                    "workspaceName": "workspace",
+                    "featureServiceName": "fake-feature-service",
+                    "joinKeyMap": {"user_id": "id123"},
+                    "requestContextMap": {},
+                    "allowPartialResults": False,
+                    "metadataOptions": {
+                        "includeNames": True,
+                        "includeDataTypes": True,
+                        "includeEffectiveTimes": True,
+                        "includeSloInfo": True,
+                        "includeServingStatus": True,
+                    },
+                    "requestOptions": {"readFromCache": False, "writeToCache": True},
+                }
+            },
+        )
+
     def test_get_feature_service_metadata_encode(self):
         # using just magic_mock here in order to assert on client.post.assert_called_with
         mock_http_client = MagicMock()
         mock_http_client.post.return_value.json.return_value = {
             "inputJoinKeys": [],
             "inputRequestContextKeys": [],
             "featureValues": [],
@@ -160,15 +197,15 @@
         test_client = httpx.Client(
             transport=httpx.MockTransport(lambda request: httpx.Response(200, json={"result": {"features": []}}))
         )
         client = TectonClient(
             url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=test_client
         )
         resp = client.get_features(feature_service_name="fake-feature-service", join_key_map={"user_id": "id123"})
-        self.assertEquals(resp.result.features, [])
+        self.assertEqual(resp.result.features, [])
 
     def test_raise_error(self):
         test_client = httpx.Client(
             transport=httpx.MockTransport(lambda request: httpx.Response(404, json={"result": {"features": []}}))
         )
         client = TectonClient(
             url="https://fake.tecton.ai", api_key="fake-api-key", default_workspace_name="workspace", client=test_client
```

### Comparing `tecton_client-0.2.0/tests/test_data/nested_sample_response.json` & `tecton_client-0.2.1/tests/test_data/nested_sample_response.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/tests/test_data/sample_response.json` & `tecton_client-0.2.1/tests/test_data/sample_response.json`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/LICENSE.md` & `tecton_client-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.2.0/README.md` & `tecton_client-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Python Client Library for Tecton Online Feature Store
 
 A simple Python client for the Feature Server HTTP API that helps customers integrate with Tecton easily.
 
 
 ## Documentation
 
-* [Tecton Python Client API Reference](https://tecton-ai.github.io/tecton-http-client-python/html/index.html)
+* [Tecton Python Client API Reference](https://tecton-ai.github.io/tecton-http-client-python/index.html)
 
 * [Tecton Python Client Example Code](/examples)
 
 * [FeatureServer API Reference](https://docs.tecton.ai/rest-swagger/docs.html)
 
 * [Fetching Online Features](https://docs.tecton.ai/latest/examples/fetch-real-time-features.html)
```

### Comparing `tecton_client-0.2.0/pyproject.toml` & `tecton_client-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 license = "Apache-2.0"
 dynamic = ["version"]
 readme = "README.md"
 
 [project.optional-dependencies]
 dev = [
   "pytest>=6.2.5",
-  "pytest_httpx"
+  "pytest_httpx",
+  "pytest-asyncio"
 ]
 docs = [
   "alabaster==0.7.16",
   "Babel==2.14.0",
   "certifi==2024.2.2",
   "charset-normalizer==3.3.2",
   "docutils==0.20.1",
```

### Comparing `tecton_client-0.2.0/PKG-INFO` & `tecton_client-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: tecton-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python Client for the Tecton FeatureService API
 Project-URL: Source, https://github.com/tecton-ai/tecton-http-client-python
 Project-URL: Documentation, https://tecton-ai.github.io/tecton-http-client-python/html/index.html
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 Requires-Python: >=3.8
 Requires-Dist: httpx>=0.23.0
 Provides-Extra: dev
+Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: pytest-httpx; extra == 'dev'
 Requires-Dist: pytest>=6.2.5; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: alabaster==0.7.16; extra == 'docs'
 Requires-Dist: babel==2.14.0; extra == 'docs'
 Requires-Dist: certifi==2024.2.2; extra == 'docs'
 Requires-Dist: charset-normalizer==3.3.2; extra == 'docs'
@@ -38,15 +39,15 @@
 # Python Client Library for Tecton Online Feature Store
 
 A simple Python client for the Feature Server HTTP API that helps customers integrate with Tecton easily.
 
 
 ## Documentation
 
-* [Tecton Python Client API Reference](https://tecton-ai.github.io/tecton-http-client-python/html/index.html)
+* [Tecton Python Client API Reference](https://tecton-ai.github.io/tecton-http-client-python/index.html)
 
 * [Tecton Python Client Example Code](/examples)
 
 * [FeatureServer API Reference](https://docs.tecton.ai/rest-swagger/docs.html)
 
 * [Fetching Online Features](https://docs.tecton.ai/latest/examples/fetch-real-time-features.html)
```


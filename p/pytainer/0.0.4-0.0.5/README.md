# Comparing `tmp/pytainer-0.0.4.tar.gz` & `tmp/pytainer-0.0.5.tar.gz`

## Comparing `pytainer-0.0.4.tar` & `pytainer-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.4/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.4/requirements.txt
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pytainer-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytainer-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.4/pytainer/__about__.py
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 pytainer-0.0.4/pytainer/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pytainer-0.0.4/pytainer/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.4/pytainer/models/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pytainer-0.0.4/pytainer/models/gittypes.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 pytainer-0.0.4/pytainer/models/portainer.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pytainer-0.0.4/scripts/docker-compose.example.yml
--rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pytainer-0.0.4/scripts/run_portainer_ce.sh
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pytainer-0.0.4/tests/test_pytainer.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 pytainer-0.0.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pytainer-0.0.4/LICENSE
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.4/README.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytainer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pytainer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.5/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pytainer-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytainer-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.5/pytainer/__about__.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pytainer-0.0.5/pytainer/__init__.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 pytainer-0.0.5/pytainer/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.5/pytainer/models/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pytainer-0.0.5/pytainer/models/gittypes.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 pytainer-0.0.5/pytainer/models/portainer.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pytainer-0.0.5/scripts/docker-compose.example.yml
+-rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pytainer-0.0.5/scripts/run_portainer_ce.sh
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 pytainer-0.0.5/tests/test_pytainer.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 pytainer-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pytainer-0.0.5/LICENSE
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.5/README.md
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pytainer-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pytainer-0.0.5/PKG-INFO
```

### Comparing `pytainer-0.0.4/.github/workflows/publish.yml` & `pytainer-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.4/pytainer/__init__.py` & `pytainer-0.0.5/pytainer/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,78 +21,55 @@
     _base_url: str
     _headers: dict
     _api_token: str
     _requester: httpx.Client
 
     def __init__(
         self,
-        base_url: str | None,
+        base_url: str | None = None,
         api_token: str | None = None,
         username: str | None = None,
         password: str | None = None,
     ) -> None:
-        if not base_url:
-            self.base_url = os.getenv("PORTAINER_URL")
-        else:
-            self.base_url = base_url
-        if not api_token:
-            self.api_token = os.getenv("PORTAINER_API_TOKEN")
-        else:
-            self.api_token = api_token
+        self._base_url = base_url or os.getenv("PORTAINER_URL")
+        self._api_token = api_token or os.getenv("PORTAINER_API_TOKEN")
+        
+        if not self._api_token:
+            raise Exception("API token is required")
+        
+        if not self._base_url:
+            raise Exception("Base URL is required")
 
         self._headers = {}
         self._requester = httpx.Client()
 
         self.stacks = Stacks(self)
         self.auth = Auth(self)
         self.system = System(self)
-
-    @property
-    def headers(self) -> dict:
-        return self._headers
-
-    @headers.setter
-    def headers(self, headers: dict) -> None:
-        self._headers.update(headers)
-
-    @property
-    def api_token(self) -> str:
-        return self._api_token
-
-    @api_token.setter
-    def api_token(self, token: str) -> None:
-        self._api_token = token
-
+    
     @property
     def base_url(self) -> str:
         return self._base_url
 
-    @base_url.setter
-    def base_url(self, url: str) -> None:
-        self._base_url = url
-
-    @property
-    def requester(self) -> httpx.Client:
-        return self._requester
-
     def make_request(
         self,
         method: HttpMethod,
         url: str,
         params: dict | None = None,
         data: BaseModel | None = None,
     ) -> httpx.Response:
-        self.headers["X-API-Key"] = f"{self.api_token}"
+        
+        self._headers["X-API-Key"] = f"{self._api_token}"
 
         if data:
             data = data.model_dump_json()
-
-        return self._requester.request(
-            method, url, data=data, headers=self.headers, params=params
-        )
+        req = self._requester.request(
+            method, url, data=data, headers=self._headers, params=params
+        ).raise_for_status()
+        return req
 
 
 class APIResource:
     _client: Pytainer
 
     def __init__(self, client: Pytainer) -> None:
         self.client = client
@@ -204,68 +181,86 @@
 
 
 class Stacks(APIResource):
     _base_path = "/api/stacks"
     _client: Pytainer
 
     def list(self) -> List[portainer.Stack]:
-        """List stacks"""
+        """List stacks https://app.swaggerhub.com/apis/portainer/portainer-ce/2.19.4#/stacks/StackList"""
         req = self.client.make_request(
-            "GET", urljoin(self.client._base_url, self._base_path)
+            "GET", urljoin(self.client.base_url, self._base_path)
         )
-        print(req.json())
         return [portainer.Stack.model_validate(stack_item) for stack_item in req.json()]
 
     def update(
         self, stack_id: int, endpoint_id: int, data: portainer.UpdateSwarmStackPayload
     ) -> dict:
-        """Update a stack"""
-        req = self.client.make_request(
-            "PUT",
-            urljoin(self.client._base_url, f"{self._base_path}/{stack_id}"),
-            params={"endpointId": endpoint_id},
-            data=data,
-        )
-        return portainer.Stack.model_validate(req.json())
+        """Update a stack https://app.swaggerhub.com/apis/portainer/portainer-ce/2.19.4#/stacks/StackUpdate"""
+        try:
+            req = self.client.make_request(
+                HttpMethod.PUT,
+                urljoin(self.client.base_url, f"{self._base_path}/{stack_id}"),
+                params={"endpointId": endpoint_id},
+                data=data,
+            ).raise_for_status()
+            return portainer.Stack.model_validate(req.json())
+        except httpx.RequestError as e:
+            raise Exception(f"An error occurred while updating the stack: {e}")
 
     def get(self, stack_id: int) -> portainer.Stack:
-        """Get a stack"""
-        req = self.client.make_request(
-            "GET",
-            urljoin(self.client._base_url, f"{self._base_path}/{stack_id}"),
-        )
-        return portainer.Stack.model_validate(req.json())
+        """Get a stack https://app.swaggerhub.com/apis/portainer/portainer-ce/2.19.4#/stacks/StackInspect"""
+        try:
+            req = self.client.make_request(
+                HttpMethod.GET,
+                urljoin(self.client.base_url, f"{self._base_path}/{stack_id}"),
+            ).raise_for_status()
+            return portainer.Stack.model_validate(req.json())
+        except httpx.RequestError as e:
+            raise Exception(
+                f"An error occurred while getting the stack: {e}, {req.json()}"
+            )
 
     def get_file(self, stack_id: int) -> portainer.Stack:
-        """Get stack file"""
+        """Get stack file https://app.swaggerhub.com/apis/portainer/portainer-ce/2.19.4#/stacks/StackFileInspect"""
         req = self.client.make_request(
-            "GET",
-            urljoin(self.client._base_url, f"{self._base_path}/{stack_id}/file"),
+            HttpMethod.GET,
+            urljoin(self.client.base_url, f"{self._base_path}/{stack_id}/file"),
         )
         return portainer.StackFileResponse.model_validate(req.json())
 
+    def start(self, stack_id: int, endpoint_id: int) -> portainer.Stack:
+        """Start a stack https://app.swaggerhub.com/apis/portainer/portainer-ce/2.19.4#/stacks/StackStart"""
+        req = self.client.make_request(
+            HttpMethod.POST,
+            urljoin(self.client.base_url, f"{self._base_path}/{stack_id}/start"), params={"endpointId": endpoint_id}
+        )
+        return portainer.Stack.model_validate(req.json())
+    
+    def stop(self, stack_id: int, endpoint_id: int) -> portainer.Stack:
+        """Stop a stack https://app.swaggerhub.com/apis/portainer/portainer-ce/2.19.4#/stacks/StackStop"""
+        req = self.client.make_request(
+            HttpMethod.POST,
+            urljoin(self.client.base_url, f"{self._base_path}/{stack_id}/stop"), params={"endpointId": endpoint_id}
+        )
+        return portainer.Stack.model_validate(req.json())
 
 class Status(APIResource):
     pass
 
 
 class System(APIResource):
     def info(self) -> portainer.SystemInfoResponse:
-        resource_path = "api/system/info"
-        request_url = urljoin(self.client.base_url, resource_path)
-        info_req = self.client.make_request(HttpMethod.GET, request_url)
-        info_resp = portainer.SystemInfoResponse.model_validate(info_req.json())
-        return info_resp
+        """Get system info"""
+        info_req = self.client.make_request(HttpMethod.GET, urljoin(self.client.base_url, "api/system/info"))
+        return portainer.SystemInfoResponse.model_validate(info_req.json())
 
     def version(self) -> portainer.SystemVersionResponse:
-        resource_path = "api/system/version"
-        request_url = urljoin(self.client.base_url, resource_path)
-        version_req = self.client.make_request(HttpMethod.GET, request_url)
-        version_resp = portainer.SystemInfoResponse.model_validate(version_req.json())
-        return version_resp
+        """Get Portainer version"""
+        info_req = self.client.make_request(HttpMethod.GET, urljoin(self.client.base_url, "api/system/version"))
+        return portainer.SystemVersionResponse.model_validate(info_req.json())
 
 
 class Tags(APIResource):
     pass
 
 
 class Team_memberships(APIResource):
```

### Comparing `pytainer-0.0.4/pytainer/cli.py` & `pytainer-0.0.5/pytainer/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 import typer
 import os
 from typing import Annotated, List, Optional
 from pytainer import Pytainer
-from pytainer.models.portainer import UpdateSwarmStackPayload, Pair
+from pytainer.models.portainer import UpdateSwarmStackPayload, Pair, StackFileResponse
 from rich import print
 
 app = typer.Typer()
-system_app = typer.Typer()
-stack_app = typer.Typer()
+system_app = typer.Typer(help="System commands")
+stacks_app = typer.Typer(help="Stacks control commands")
 
 app.add_typer(system_app, name="system")
-app.add_typer(stack_app, name="stack")
+app.add_typer(stacks_app, name="stacks")
 
-client = Pytainer(
-    base_url=os.getenv("PORTAINER_URL"), api_token=os.getenv("PORTAINER_API_TOKEN")
-)
+client = Pytainer()
 
 
 @system_app.command("info")
 def info():
     print(client.system.info())
 
 
 @system_app.command("version")
 def version():
     print(client.system.version())
 
 
-@stack_app.command("list")
+@stacks_app.command("list")
 def list_stack():
     print(client.stacks.list())
 
 
-@stack_app.command("get")
+@stacks_app.command("get")
 def get_stack(
     stack_id: Annotated[int, typer.Argument(...)],
 ):
     print(client.stacks.get(stack_id=stack_id))
 
 
-@stack_app.command("update")
+@stacks_app.command("update")
 def update_stack(
     stack_id: Annotated[int, typer.Argument(...)],
-    env: Annotated[Optional[List[str]], typer.Option()] = None,
+    env: Annotated[Optional[List[str]], typer.Option("--env")] = None,
     prune: Annotated[bool, typer.Option("--prune")] = False,
     pull_image: Annotated[bool, typer.Option("--pull")] = False,
 ):
     parsed_env = []
     if env:
         for item in env:
             key, value = item.split("=")
@@ -73,14 +71,35 @@
             stackFileContent=current_stack_file.StackFileContent,
         )
         response = client.stacks.update(
             stack_id=stack_id, endpoint_id=current_stack.EndpointId, data=data
         )
         return response
 
+@stacks_app.command("start")
+def satrt_stack(
+    stack_id: Annotated[int, typer.Argument(...)],
+    endpoint_id: Annotated[int, typer.Option("--endpoint")] = None,
+):  
+    if not endpoint_id:
+        endpoint_id = client.stacks.get(stack_id=stack_id).EndpointId
+    response = client.stacks.start(stack_id=stack_id, endpoint_id=endpoint_id)    
+    return response
+
+@stacks_app.command("stop")
+def satrt_stack(
+    stack_id: Annotated[int, typer.Argument(...)],
+    endpoint_id: Annotated[int, typer.Option("--endpoint")] = None,
+):  
+    if not endpoint_id:
+        endpoint_id = client.stacks.get(stack_id=stack_id).EndpointId
+
+    response = client.stacks.stop(stack_id=stack_id, endpoint_id=endpoint_id)    
+    return response
+
 
 def main():
     app()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pytainer-0.0.4/tests/test_pytainer.py` & `pytainer-0.0.5/tests/test_pytainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import httpx
 from pytest_httpx import HTTPXMock
 
 from pytainer import Pytainer
-from pytainer.models.portainer import AuthAuthenticateResponse, SystemInfoResponse
+from pytainer.models.portainer import AuthAuthenticateResponse, SystemInfoResponse, SystemVersionResponse, SystemBuildInfo
 
 
 def test_portainer_init():
     portainer = Pytainer(
         base_url="https://portainer.test/", api_token="debug-auth-token"
     )
-    assert portainer.base_url == "https://portainer.test/"
-    assert portainer.headers == {}
-    assert portainer.api_token == "debug-auth-token"
-    assert isinstance(portainer.requester, httpx.Client)
+    assert portainer._base_url == "https://portainer.test/"
+    assert portainer._headers == {}
+    assert portainer._api_token == "debug-auth-token"
+    assert isinstance(portainer._requester, httpx.Client)
 
 
 def test_auth_auth(httpx_mock: HTTPXMock):
     jwt = "debug-auth-token"
     httpx_mock.add_response(
         method="POST",
         url="https://portainer.test/api/auth",
@@ -42,7 +42,49 @@
         url="https://portainer.test/api/system/info",
         json=SystemInfoResponse(agents=0, edgeAgents=0, platform="str").model_dump(),
     )
 
     with httpx.Client() as client:
         resp = portainer.system.info()
         assert isinstance(resp, SystemInfoResponse)
+
+def test_system_version(httpx_mock: HTTPXMock):
+    portainer = Pytainer(
+        base_url="https://portainer.test/", api_token="debug-auth-token"
+    )
+    httpx_mock.add_response(
+        method="GET",
+        url="https://portainer.test/api/system/version",
+        json=SystemVersionResponse(
+            LatestVersion="0.0.0",
+            UpdateAvailable=False,
+            Build=SystemBuildInfo(
+                BuildNumber="0.0.0",
+                GoVersion="0.0.0",
+                ImageTag="0.0.0",
+                NodejsVersion="0.0.0",
+                WebpackVersion="0.0.0",
+                YarnVersion="0.0.0",
+            ),
+            DatabaseVersion="0.0.0",
+            ServerVersion="0.0.0",
+        ).model_dump(),
+    )
+
+    with httpx.Client() as client:
+        resp = portainer.system.version()
+        assert isinstance(resp, SystemVersionResponse)
+
+def test_stacks_list(httpx_mock: HTTPXMock):
+    portainer = Pytainer(
+        base_url="https://portainer.test/", api_token="debug-auth-token"
+    )
+    httpx_mock.add_response(
+        method="GET",
+        url="https://portainer.test/api/stacks",
+        json=[],
+    )
+
+    with httpx.Client() as client:
+        resp = portainer.stacks.list()
+        assert isinstance(resp, list)
+        assert len(resp) == 0
```

### Comparing `pytainer-0.0.4/.gitignore` & `pytainer-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.4/LICENSE` & `pytainer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.4/pyproject.toml` & `pytainer-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pytainer"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Krzysztof Myjak"},
 ]
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
@@ -22,16 +22,14 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
-    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
-    "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "httpx",
     "pydantic",
     "typer >= 0.12.3",
     "pytest-httpx",
     "pytest-asyncio"
```

### Comparing `pytainer-0.0.4/PKG-INFO` & `pytainer-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytainer
-Version: 0.0.4
+Version: 0.0.5
 Author: Krzysztof Myjak
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -13,16 +13,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Requires-Python: >=3.9
 Requires-Dist: httpx
 Requires-Dist: pydantic
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytest-httpx
 Requires-Dist: typer>=0.12.3
 Description-Content-Type: text/markdown
```


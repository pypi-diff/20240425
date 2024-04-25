# Comparing `tmp/synapse_token_authenticator-0.4.2.tar.gz` & `tmp/synapse_token_authenticator-0.4.5.tar.gz`

## Comparing `synapse_token_authenticator-0.4.2.tar` & `synapse_token_authenticator-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/CODEOWNERS
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/cliff.toml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/.github/workflows/main.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/.github/workflows/python.yml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/synapse_token_authenticator/__init__.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/synapse_token_authenticator/config.py
--rw-r--r--   0        0        0     9982 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/synapse_token_authenticator/token_authenticator.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/synapse_token_authenticator/utils.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/tests/test_jwt.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/tests/test_oidc.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/.gitignore
--rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/LICENSE
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/README.md
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/CHANGELOG.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/CODEOWNERS
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/cliff.toml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/workflows/python.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/__init__.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/config.py
+-rw-r--r--   0        0        0    10012 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/token_authenticator.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/utils.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/server.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_jwt.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_oidc.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/unittest.py
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/utils.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_utils/html_parsers.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_utils/logging_setup.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.gitignore
+-rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/README.md
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/PKG-INFO
```

### Comparing `synapse_token_authenticator-0.4.2/CHANGELOG.md` & `synapse_token_authenticator-0.4.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.4.5] - 2024-04-25
+
+### Continuous Integration Pipeline
+
+- Bump pypi publish action
+
+## [0.4.4] - 2024-04-24
+
+### Bug Fixes
+
+- Basic auth utf8
+
+## [0.4.3] - 2024-04-08
+
+### Features
+
+- Refactor http calls to ModuleApi
+
 ## [0.4.2] - 2024-01-31
 
 ### Bug Fixes
 
 - Fix proxy notation
 
 ## [0.4.1] - 2024-01-31
```

### Comparing `synapse_token_authenticator-0.4.2/cliff.toml` & `synapse_token_authenticator-0.4.5/cliff.toml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.2/.github/workflows/publish.yml` & `synapse_token_authenticator-0.4.5/.github/workflows/publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip 
         pip install hatch
     - name: Build package
       run: hatch build
     - name: Publish package distributions to PyPI
-      uses: pypa/gh-action-pypi-publish@c12cc61414480c03e10ea76e2a0a1a17d6c764e2
+      uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
```

### Comparing `synapse_token_authenticator-0.4.2/.github/workflows/python.yml` & `synapse_token_authenticator-0.4.5/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.2/synapse_token_authenticator/config.py` & `synapse_token_authenticator-0.4.5/synapse_token_authenticator/config.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.2/synapse_token_authenticator/token_authenticator.py` & `synapse_token_authenticator-0.4.5/synapse_token_authenticator/token_authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,72 +1,70 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2024 Famedly
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
-import re
-from typing import Awaitable, Callable, Optional, Tuple
-import logging
-from jwcrypto import jwt, jwk
-from jwcrypto.common import JWException, json_decode
-import json
 import base64
-import requests
-from requests.auth import HTTPBasicAuth
+import json
+import logging
+import re
+from collections.abc import Awaitable
+from typing import Callable, Optional
 from urllib.parse import urljoin
 
 import synapse
+from jwcrypto import jwk, jwt
+from jwcrypto.common import JWException, json_decode
+from synapse.api.errors import HttpResponseException
 from synapse.module_api import ModuleApi
 from synapse.types import UserID
-
 from twisted.web import resource
 
 from synapse_token_authenticator.config import TokenAuthenticatorConfig
-from synapse_token_authenticator.utils import OpenIDProviderMetadata
+from synapse_token_authenticator.utils import get_oidp_metadata, basic_auth
 
 logger = logging.getLogger(__name__)
 
 
-class TokenAuthenticator(object):
+class TokenAuthenticator:
     __version__ = "0.0.0"
 
-    def __init__(self, config: dict, account_handler: ModuleApi):
-        self.api = account_handler
+    def __init__(self, config: dict, api: ModuleApi):
+        self.api = api
 
         auth_checkers = {}
 
         self.config: TokenAuthenticatorConfig = config
         if (jwt := getattr(self.config, "jwt", None)) is not None:
             if jwt.secret:
                 k = {
                     "k": base64.urlsafe_b64encode(jwt.secret.encode("utf-8")).decode(
                         "utf-8"
                     ),
                     "kty": "oct",
                 }
                 self.key = jwk.JWK(**k)
             else:
-                with open(jwt.keyfile, "r") as f:
+                with open(jwt.keyfile) as f:
                     self.key = jwk.JWK.from_pem(f.read())
             auth_checkers[("com.famedly.login.token", ("token",))] = self.check_jwt_auth
 
         if (oidc := getattr(self.config, "oidc", None)) is not None:
-            auth_checkers[
-                ("com.famedly.login.token.oidc", ("token",))
-            ] = self.check_oidc_auth
+            auth_checkers[("com.famedly.login.token.oidc", ("token",))] = (
+                self.check_oidc_auth
+            )
 
             self.api.register_web_resource(
                 "/_famedly/login/com.famedly.login.token.oidc",
                 self.LoginMetadataResource(oidc),
             )
 
         self.api.register_password_auth_provider_callbacks(auth_checkers=auth_checkers)
@@ -91,15 +89,15 @@
                     "project-id": self.project_id,
                 }
             ).encode("utf-8")
 
     async def check_jwt_auth(
         self, username: str, login_type: str, login_dict: "synapse.module_api.JsonDict"
     ) -> Optional[
-        Tuple[
+        tuple[
             str,
             Optional[Callable[["synapse.module_api.LoginResponse"], Awaitable[None]]],
         ]
     ]:
         logger.info("Receiving auth request")
         if login_type != "com.famedly.login.token":
             logger.info("Wrong login type")
@@ -117,18 +115,18 @@
             token = jwt.JWT(
                 jwt=token,
                 key=self.key,
                 check_claims=check_claims,
                 algs=[self.config.jwt.algorithm],
             )
         except ValueError as e:
-            logger.info("Unrecognized token", e)
+            logger.info("Unrecognized token %s", e)
             return None
         except JWException as e:
-            logger.info("Invalid token", e)
+            logger.info("Invalid token %s", e)
             return None
         payload = json_decode(token.claims)
         if "sub" not in payload:
             logger.info("Missing user_id field")
             return None
         token_user_id_or_localpart = payload["sub"]
         if not isinstance(token_user_id_or_localpart, str):
@@ -147,15 +145,15 @@
                 "[0-9a-f]{8}-[0-9a-f]{4}-[0-5][0-9a-f]{3}-[089ab][0-9a-f]{3}-[0-9a-f]{12}$",
                 user_id.localpart,
             )
         ):
             logger.info("user_id does not end with a UUID even though in chatbox mode")
             return None
 
-        if not user_id.domain == self.api.server_name:
+        if user_id.domain != self.api.server_name:
             logger.info("user_id isn't for our homeserver")
             return
 
         if user_id_str != token_user_id_str:
             logger.info("Non-matching user")
             return None
 
@@ -183,45 +181,46 @@
 
         logger.info("All done and valid, logging in!")
         return (user_id_str, None)
 
     async def check_oidc_auth(
         self, username: str, login_type: str, login_dict: "synapse.module_api.JsonDict"
     ) -> Optional[
-        Tuple[
+        tuple[
             str,
             Optional[Callable[["synapse.module_api.LoginResponse"], Awaitable[None]]],
         ]
     ]:
         logger.info("Receiving auth request")
         if login_type != "com.famedly.login.token.oidc":
             logger.info("Wrong login type")
             return None
         if "token" not in login_dict:
             logger.info("Missing token")
             return None
         token = login_dict["token"]
 
         oidc = self.config.oidc
-        oidc_metadata = OpenIDProviderMetadata(oidc.issuer)
+        oidc_metadata = await get_oidp_metadata(oidc.issuer, self.api.http_client)
 
         # Further validation using token introspection
         data = {"token": token, "token_type_hint": "access_token", "scope": "openid"}
-        auth = HTTPBasicAuth(oidc.client_id, oidc.client_secret)
-        response = requests.post(
-            oidc_metadata.introspection_endpoint,
-            data=data,
-            auth=auth,
-            proxies={"http": "", "https": ""},
-        )
-        if response.status_code == 401:
-            logger.info("User's access token is invalid")
-            return None
 
-        introspection_resp = response.json()
+        try:
+            introspection_resp = await self.api.http_client.post_json_get_json(
+                oidc_metadata.introspection_endpoint,
+                data,
+                headers=basic_auth(oidc.client_id, oidc.client_secret),
+            )
+        except HttpResponseException as e:
+            if e.code == 401:
+                logger.info("User's access token is invalid")
+                return None
+            else:
+                raise e
 
         if not introspection_resp["active"]:
             logger.info("User is not active")
             return None
 
         allowed_roles = ["User", "OrgAdmin"]
```

### Comparing `synapse_token_authenticator-0.4.2/LICENSE` & `synapse_token_authenticator-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.2/README.md` & `synapse_token_authenticator-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
   "token": "<jwt here>"
 }
 ```
 
 ### OIDC Authentication
 
 First, the user needs to obtain an Access token and an ID token from the IDP:
-```json
+```http
 POST https://idp.example.org/oauth/v2/token
 
 ```
 
 Next, the client needs to use these tokens and construct a payload to the login endpoint:
 
 ```jsonc
```

### Comparing `synapse_token_authenticator-0.4.2/pyproject.toml` & `synapse_token_authenticator-0.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synapse-token-authenticator"
 description = 'Synapse authentication module which allows for authenticating and registering using JWTs'
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 license = "AGPL-3.0-only"
 keywords = []
 authors = [
   { name = "Sorunome", email = "mail@sorunome.de" },
   { name = "Amanda Graven", email = "amanda@graven.dev" },
   { name = "Jan Christian Grünhage", email = "jan.christian@gruenhage.xyz" },
 ]
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["jwcrypto", "twisted"]
-version = "0.4.2"
+version = "0.4.5"
 
 [project.urls]
 Documentation = "https://github.com/famedly/synapse-token-authenticator"
 Issues = "https://github.com/famedly/synapse-token-authenticator/issues"
 Source = "https://github.com/famedly/synapse-token-authenticator"
 
 [tool.hatch.envs.default]
```

### Comparing `synapse_token_authenticator-0.4.2/PKG-INFO` & `synapse_token_authenticator-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: synapse-token-authenticator
-Version: 0.4.2
+Version: 0.4.5
 Summary: Synapse authentication module which allows for authenticating and registering using JWTs
 Project-URL: Documentation, https://github.com/famedly/synapse-token-authenticator
 Project-URL: Issues, https://github.com/famedly/synapse-token-authenticator/issues
 Project-URL: Source, https://github.com/famedly/synapse-token-authenticator
 Author-email: Sorunome <mail@sorunome.de>, Amanda Graven <amanda@graven.dev>, Jan Christian Grünhage <jan.christian@gruenhage.xyz>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Requires-Dist: jwcrypto
 Requires-Dist: twisted
 Description-Content-Type: text/markdown
 
 # Synapse Token Authenticator
 
 [![PyPI - Version](https://img.shields.io/pypi/v/synapse-token-authenticator.svg)](https://pypi.org/project/synapse-token-authenticator)
@@ -95,15 +95,15 @@
   "token": "<jwt here>"
 }
 ```
 
 ### OIDC Authentication
 
 First, the user needs to obtain an Access token and an ID token from the IDP:
-```json
+```http
 POST https://idp.example.org/oauth/v2/token
 
 ```
 
 Next, the client needs to use these tokens and construct a payload to the login endpoint:
 
 ```jsonc
```


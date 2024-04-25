# Comparing `tmp/flask_jwt_oidc-0.3.0.tar.gz` & `tmp/flask_jwt_oidc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask_jwt_oidc-0.3.0.tar", last modified: Wed Feb 17 06:08:32 2021, max compression
+gzip compressed data, was "flask_jwt_oidc-0.5.0.tar", max compression
```

## Comparing `flask_jwt_oidc-0.3.0.tar` & `flask_jwt_oidc-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,7 @@
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.630857 flask_jwt_oidc-0.3.0/
--rw-r--r--   0 thor       (501) staff       (20)     1400 2021-02-17 06:08:32.631010 flask_jwt_oidc-0.3.0/PKG-INFO
--rw-r--r--   0 thor       (501) staff       (20)     3837 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/README.md
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.621264 flask_jwt_oidc-0.3.0/examples/
--rw-r--r--   0 thor       (501) staff       (20)        0 2021-02-17 05:48:41.000000 flask_jwt_oidc-0.3.0/examples/__init__.py
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.622384 flask_jwt_oidc-0.3.0/examples/flask_app/
--rw-r--r--   0 thor       (501) staff       (20)        0 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/examples/flask_app/__init__.py
--rw-r--r--   0 thor       (501) staff       (20)     4182 2021-02-17 05:52:23.000000 flask_jwt_oidc-0.3.0/examples/flask_app/app.py
--rw-r--r--   0 thor       (501) staff       (20)     4013 2021-02-17 05:52:23.000000 flask_jwt_oidc-0.3.0/examples/flask_app/config.py
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.623918 flask_jwt_oidc-0.3.0/examples/flask_app/tests/
--rw-r--r--   0 thor       (501) staff       (20)        0 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/examples/flask_app/tests/__init__.py
--rw-r--r--   0 thor       (501) staff       (20)      646 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/examples/flask_app/tests/conftest.py
--rw-r--r--   0 thor       (501) staff       (20)     4303 2021-02-17 05:52:23.000000 flask_jwt_oidc-0.3.0/examples/flask_app/tests/test_flask_app.py
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.625522 flask_jwt_oidc-0.3.0/flask_jwt_oidc/
--rw-r--r--   0 thor       (501) staff       (20)     1739 2021-02-17 05:48:41.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc/__init__.py
--rw-r--r--   0 thor       (501) staff       (20)      939 2021-02-17 05:48:41.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc/exceptions.py
--rw-r--r--   0 thor       (501) staff       (20)    15481 2021-02-17 05:52:23.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc/jwt_manager.py
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.630579 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/
--rw-r--r--   0 thor       (501) staff       (20)     1400 2021-02-17 06:08:32.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/PKG-INFO
--rw-r--r--   0 thor       (501) staff       (20)      711 2021-02-17 06:08:32.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 thor       (501) staff       (20)        1 2021-02-17 06:08:32.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 thor       (501) staff       (20)        1 2021-01-06 04:57:25.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/not-zip-safe
--rw-r--r--   0 thor       (501) staff       (20)       31 2021-02-17 06:08:32.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/requires.txt
--rw-r--r--   0 thor       (501) staff       (20)       30 2021-02-17 06:08:32.000000 flask_jwt_oidc-0.3.0/flask_jwt_oidc.egg-info/top_level.txt
--rw-r--r--   0 thor       (501) staff       (20)     1197 2021-02-17 06:08:32.631843 flask_jwt_oidc-0.3.0/setup.cfg
--rw-r--r--   0 thor       (501) staff       (20)     2637 2021-02-17 06:08:18.000000 flask_jwt_oidc-0.3.0/setup.py
-drwxr-xr-x   0 thor       (501) staff       (20)        0 2021-02-17 06:08:32.628071 flask_jwt_oidc-0.3.0/tests/
--rw-r--r--   0 thor       (501) staff       (20)        0 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/tests/__init__.py
--rw-r--r--   0 thor       (501) staff       (20)     3875 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/tests/conftest.py
--rw-r--r--   0 thor       (501) staff       (20)     2000 2021-02-17 05:52:23.000000 flask_jwt_oidc-0.3.0/tests/test_cookie_protected.py
--rw-r--r--   0 thor       (501) staff       (20)     2006 2021-02-17 05:48:41.000000 flask_jwt_oidc-0.3.0/tests/test_protected.py
--rw-r--r--   0 thor       (501) staff       (20)      314 2019-02-03 07:04:47.000000 flask_jwt_oidc-0.3.0/tests/test_unprotected.py
+-rw-r--r--   0        0        0     1695 2024-04-25 05:49:07.962393 flask_jwt_oidc-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3734 2024-04-25 05:49:53.011595 flask_jwt_oidc-0.5.0/README.md
+-rw-r--r--   0        0        0      736 2024-04-25 05:57:19.718975 flask_jwt_oidc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1739 2024-04-22 19:57:59.613632 flask_jwt_oidc-0.5.0/src/flask_jwt_oidc/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-22 19:57:59.613705 flask_jwt_oidc-0.5.0/src/flask_jwt_oidc/exceptions.py
+-rw-r--r--   0        0        0    15530 2024-04-22 19:57:59.613830 flask_jwt_oidc-0.5.0/src/flask_jwt_oidc/jwt_manager.py
+-rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 flask_jwt_oidc-0.5.0/PKG-INFO
```

### Comparing `flask_jwt_oidc-0.3.0/README.md` & `flask_jwt_oidc-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -108,16 +108,12 @@
                            "You provided a valid JWT token")
 
 
 if __name__ == "__main__":
     app.run()
 
 ```
-## Thanks
-The following folks have provided help, feedback, PRs, etc:
-- Jamie Lennox
-- James Hollinger
 
 ## TODO
 - add tests
 - add more examples
 - add tests for the OIDC service providers listed above
```

### Comparing `flask_jwt_oidc-0.3.0/flask_jwt_oidc/__init__.py` & `flask_jwt_oidc-0.5.0/src/flask_jwt_oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.3.0/flask_jwt_oidc/exceptions.py` & `flask_jwt_oidc-0.5.0/src/flask_jwt_oidc/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.3.0/flask_jwt_oidc/jwt_manager.py` & `flask_jwt_oidc-0.5.0/src/flask_jwt_oidc/jwt_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 """
 
 import json
 import ssl  # pylint: disable=unused-import # noqa: F401; for local hacks
 from functools import wraps
 
 from cachelib import SimpleCache
-from flask import _request_ctx_stack, current_app, g, jsonify, request
+from flask import current_app, g, jsonify, request
+from flask.globals import request_ctx
 from jose import jwt
 from six.moves.urllib.request import urlopen
 
 from .exceptions import AuthError
 
 
 class JwtManager:  # pylint: disable=too-many-instance-attributes
     """Manages the JWT verification and JWKS key lookup."""
 
-    ALGORITHMS = ['RS256']
+    ALGORITHMS = 'RS256'
 
     def __init__(self, app=None):
         """Initialize the JWTManager instance."""
         # These are all set in the init_app function, but are listed here for easy reference
         self.app = app
         self.well_known_config = None
         self.well_known_obj_cache = None
@@ -95,16 +96,17 @@
                 app.logger.error(
                     'Attempting to run JWT Manager with no local key assigned')
                 raise Exception(
                     'Attempting to run JWT Manager with no local key assigned')
 
         else:
 
-            self.algorithms = [app.config.get(
-                'JWT_OIDC_ALGORITHMS', JwtManager.ALGORITHMS)]
+            self.algorithms = app.config.get(
+                'JWT_OIDC_ALGORITHMS', JwtManager.ALGORITHMS).replace(' ', '')\
+                .split(',')
 
             # If the WELL_KNOWN_CONFIG is set, then go fetch the JWKS & ISSUER
             self.well_known_config = app.config.get(
                 'JWT_OIDC_WELL_KNOWN_CONFIG', None)
             if self.well_known_config:
                 # try to get the jwks & issuer from the well known config
                 # jurl = urlopen(url=self.well_known_config, context=ssl.SSLContext()) # for gangster testing
@@ -326,15 +328,15 @@
             payload = jwt.decode(
                 token,
                 rsa_key,
                 algorithms=self.algorithms,
                 audience=self.audience,
                 issuer=self.issuer
             )
-            _request_ctx_stack.top.current_user = g.jwt_oidc_token_info = payload
+            request_ctx.current_user = g.jwt_oidc_token_info = payload
         except jwt.ExpiredSignatureError as sig:
             raise AuthError({'code': 'token_expired',
                              'description': 'token has expired'}, 401) from sig
         except jwt.JWTClaimsError as jwe:
             raise AuthError({'code': 'invalid_claims',
                              'description':
                                  'incorrect claims,'
```


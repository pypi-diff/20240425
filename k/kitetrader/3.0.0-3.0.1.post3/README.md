# Comparing `tmp/kitetrader-3.0.0.tar.gz` & `tmp/kitetrader-3.0.1.post3.tar.gz`

## Comparing `kitetrader-3.0.0.tar` & `kitetrader-3.0.1.post3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 kitetrader-3.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kitetrader-3.0.0/src/__init__.py
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 kitetrader-3.0.0/src/kitetrader/Kite.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 kitetrader-3.0.0/src/kitetrader/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kitetrader-3.0.0/tests/Dockerfile
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 kitetrader-3.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kitetrader-3.0.0/LICENSE
--rw-r--r--   0        0        0    12984 2020-02-02 00:00:00.000000 kitetrader-3.0.0/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 kitetrader-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    13696 2020-02-02 00:00:00.000000 kitetrader-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/src/__init__.py
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/src/kitetrader/Kite.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/src/kitetrader/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/tests/Dockerfile
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/LICENSE
+-rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/README.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/pyproject.toml
+-rw-r--r--   0        0        0    14250 2020-02-02 00:00:00.000000 kitetrader-3.0.1.post3/PKG-INFO
```

### Comparing `kitetrader-3.0.0/.github/workflows/python-publish.yml` & `kitetrader-3.0.1.post3/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
           build
           --user
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
       - name: Store the distribution packages
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -38,15 +38,15 @@
       name: pypi
       url: https://pypi.org/p/kitetrader # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write # IMPORTANT: mandatory for trusted publishing
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -59,20 +59,20 @@
 
     permissions:
       contents: write # IMPORTANT: mandatory for making GitHub Releases
       id-token: write # IMPORTANT: mandatory for sigstore
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
       - name: Sign the dists with Sigstore
-        uses: sigstore/gh-action-sigstore-python@v1.2.3
+        uses: sigstore/gh-action-sigstore-python@v2.1.1
         with:
           inputs: >-
             ./dist/*.tar.gz
             ./dist/*.whl
       - name: Create GitHub Release
         env:
           GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `kitetrader-3.0.0/src/kitetrader/Kite.py` & `kitetrader-3.0.1.post3/src/kitetrader/Kite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Collection
+from collections.abc import Callable, Collection
 from typing import Optional, Union, Any
 from requests import Session
 from requests.exceptions import ReadTimeout
 from urllib3.util import Retry
 from requests.adapters import HTTPAdapter
 from pathlib import Path
 from mthrottle import Throttle
@@ -109,15 +109,15 @@
     cookies = None
     config = None
 
     def __init__(
         self,
         user_id: Optional[str] = None,
         password: Optional[str] = None,
-        twofa: Optional[str] = None,
+        twofa: Union[str, Callable, None] = None,
         enctoken: Optional[str] = None,
         access_token: Optional[str] = None,
         api_key: Optional[str] = None,
         api_secret: Optional[str] = None,
         request_token: Optional[str] = None,
         logger: Optional[logging.Logger] = None,
     ):
@@ -258,15 +258,15 @@
 
         raise ConnectionError(f"{hint} | {code}: {r.reason}")
 
     def _authorize(
         self,
         user_id: Optional[str] = None,
         password: Optional[str] = None,
-        twofa: Optional[str] = None,
+        twofa: Union[str, Callable, None] = None,
         api_key: Optional[str] = None,
         request_token: Optional[str] = None,
         secret: Optional[str] = None,
     ):
         """Authenthicate the user"""
 
         login_url = "https://kite.zerodha.com"
@@ -292,40 +292,52 @@
             ).json()
 
             self.access_token = response["access_token"]
             self.log.info("KiteConnect login success")
             return self._set_access_token(api_key, self.access_token)
 
         # WEB LOGIN
-        if not user_id:
-            user_id = input("Enter User id\n> ")
+        try:
+            if user_id is None:
+                user_id = input("Enter User id\n> ")
 
-        if not password:
-            password = input("Enter Password\n> ")
+            if password is None:
+                password = input("Enter Password\n> ")
+        except KeyboardInterrupt:
+            self.close()
+            exit("\nUser exit")
 
         response = self._req(
             f"{login_url}/api/login",
             "POST",
             payload=dict(user_id=user_id, password=password),
             hint="WEB_LOGIN",
         ).json()
 
         request_id = response["data"]["request_id"]
         twofa_type = response["data"]["twofa_type"]
 
-        if not twofa:
-            twofa = input(f"Please enter {twofa_type} code\n> ")
+        if callable(twofa):
+            otp = twofa()
+        elif isinstance(twofa, str):
+            otp = twofa
+        else:
+            try:
+                otp = input(f"Please enter {twofa_type} code\n> ")
+            except KeyboardInterrupt:
+                self.close()
+                exit("\nUser exit")
 
         response = self._req(
             f"{login_url}/api/twofa",
             "POST",
             payload=dict(
                 user_id=user_id,
                 request_id=request_id,
-                twofa_value=twofa,
+                twofa_value=otp,
                 twofa_type=twofa_type,
                 skip_session="",
             ),
             hint="TwoFA",
         )
 
         self.enctoken = response.cookies["enctoken"]
```

### Comparing `kitetrader-3.0.0/.gitignore` & `kitetrader-3.0.1.post3/.gitignore`

 * *Files identical despite different names*

### Comparing `kitetrader-3.0.0/LICENSE` & `kitetrader-3.0.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `kitetrader-3.0.0/README.md` & `kitetrader-3.0.1.post3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -338,14 +338,33 @@
 }
 
 max_penalty_count = 15
 
 th = Throttle(throttle_config, max_penalty_count)
 ```
 
+### Logging
+
+Kite-Trader uses the logging module. If no logger is defined, it uses a default logger, set to `INFO`. You can define your own logger and pass it to Kite during initialization.
+
+A helper function is also provided, so you can change the log level easily
+
+```python
+from kitetrader import Kite, configure_default_logger
+import logging
+
+logger = configure_default_logger(__name__)
+
+# set level to WARNING and above, default is INFO
+logger.setLevel(logging.WARNING)
+
+with Kite(logger=logger) as kite:
+    data = kite.quote("NSE:TCS")
+```
+
 ### Class and Method signature
 
 ```python
 class Kite(builtins.object)
  |  Kite(enctoken: Optional[str] = None)
  |  
  |  Unofficial implementation of Zerodha Kite api
```

### Comparing `kitetrader-3.0.0/pyproject.toml` & `kitetrader-3.0.1.post3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kitetrader"
-version = "3.0.0"
+version = "3.0.1-3"
 authors = [
   { name="Benny Thadikaran" },
 ]
 description = "Unofficial Python Client for Zerodha Kite"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kitetrader-3.0.0/PKG-INFO` & `kitetrader-3.0.1.post3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitetrader
-Version: 3.0.0
+Version: 3.0.1.post3
 Summary: Unofficial Python Client for Zerodha Kite
 Project-URL: Homepage, https://github.com/BennyThadikaran/Kite-Trader
 Project-URL: Bug Tracker, https://github.com/BennyThadikaran/Kite-Trader/issues
 Author: Benny Thadikaran
 License-File: LICENSE
 Keywords: algo-trading,historical-data,intraday-data,kiteconnect,stock-data,stock-market,zerodha,zerodha-kite
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -355,14 +355,33 @@
 }
 
 max_penalty_count = 15
 
 th = Throttle(throttle_config, max_penalty_count)
 ```
 
+### Logging
+
+Kite-Trader uses the logging module. If no logger is defined, it uses a default logger, set to `INFO`. You can define your own logger and pass it to Kite during initialization.
+
+A helper function is also provided, so you can change the log level easily
+
+```python
+from kitetrader import Kite, configure_default_logger
+import logging
+
+logger = configure_default_logger(__name__)
+
+# set level to WARNING and above, default is INFO
+logger.setLevel(logging.WARNING)
+
+with Kite(logger=logger) as kite:
+    data = kite.quote("NSE:TCS")
+```
+
 ### Class and Method signature
 
 ```python
 class Kite(builtins.object)
  |  Kite(enctoken: Optional[str] = None)
  |  
  |  Unofficial implementation of Zerodha Kite api
```


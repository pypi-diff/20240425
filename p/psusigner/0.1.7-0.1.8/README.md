# Comparing `tmp/psusigner-0.1.7.tar.gz` & `tmp/psusigner-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psusigner-0.1.7.tar", max compression
+gzip compressed data, was "psusigner-0.1.8.tar", max compression
```

## Comparing `psusigner-0.1.7.tar` & `psusigner-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1472 2023-07-15 10:42:39.330263 psusigner-0.1.7/README.md
--rw-r--r--   0        0        0       70 2023-07-14 08:53:52.900150 psusigner-0.1.7/psusigner/__init__.py
--rw-r--r--   0        0        0       44 2023-07-14 07:28:25.442201 psusigner-0.1.7/psusigner/exception.py
--rw-r--r--   0        0        0     9342 2023-07-14 13:37:18.397375 psusigner-0.1.7/psusigner/psucms.py
--rw-r--r--   0        0        0     2473 2023-08-18 15:01:12.291775 psusigner-0.1.7/psusigner/psuhsm.py
--rw-r--r--   0        0        0     3977 2023-08-11 06:18:47.535962 psusigner-0.1.7/psusigner/signers.py
--rw-r--r--   0        0        0      403 2023-08-18 15:03:05.274710 psusigner-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 psusigner-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1472 2023-07-15 10:42:39.330263 psusigner-0.1.8/README.md
+-rw-r--r--   0        0        0       70 2023-07-14 08:53:52.900150 psusigner-0.1.8/psusigner/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-14 07:28:25.442201 psusigner-0.1.8/psusigner/exception.py
+-rw-r--r--   0        0        0     9342 2023-07-14 13:37:18.397375 psusigner-0.1.8/psusigner/psucms.py
+-rw-r--r--   0        0        0     2519 2024-04-25 13:55:52.962705 psusigner-0.1.8/psusigner/psuhsm.py
+-rw-r--r--   0        0        0     3977 2023-08-11 06:18:47.535962 psusigner-0.1.8/psusigner/signers.py
+-rw-r--r--   0        0        0      403 2024-04-25 13:56:17.255350 psusigner-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 psusigner-0.1.8/PKG-INFO
```

### Comparing `psusigner-0.1.7/README.md` & `psusigner-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `psusigner-0.1.7/psusigner/psucms.py` & `psusigner-0.1.8/psusigner/psucms.py`

 * *Files identical despite different names*

### Comparing `psusigner-0.1.7/psusigner/psuhsm.py` & `psusigner-0.1.8/psusigner/psuhsm.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 
 from endesive import hsm, pdf, signer
 
 from . import exception
 
 
 class PSUHSM(hsm.BaseHSM):
-    def __init__(self, code, secret, agent_key, api_url=None):
+    def __init__(self, code, secret, agent_key, api_url=None, timeout=120):
         self.api_url = "https://ds.psu.ac.th/api/v1"
         if api_url:
             self.api_url = api_url
 
         self.sign_api_url = f"{self.api_url}/sign/withPdfSignature"
         self.log_api_url = f"{self.api_url}/sign/logs"
 
         self.code = code
         self.secret = secret
         self.agent_key = agent_key
         self.sign_parameters = {}
+        self.sign_timeout = timeout
 
     def set_sign_parameters(self, **kwargs):
         self.sign_parameters = kwargs
 
     def certificate(self):
         return None, None
 
@@ -40,17 +41,15 @@
     def sign(self, keyid, data, mech):
         headers = self.get_headers()
         payload = self.get_payload(data)
 
         # print("headers:", headers)
         # print("payload:", payload)
         response = requests.post(
-            self.sign_api_url,
-            json=payload,
-            headers=headers,
+            self.sign_api_url, json=payload, headers=headers, timeout=self.timeout
         )
 
         if response.status_code != 200:
             raise exception.PSUSignException(response.json())
 
         json_data = response.json()
         status_code = json_data.get("statusCode")
```

### Comparing `psusigner-0.1.7/psusigner/signers.py` & `psusigner-0.1.8/psusigner/signers.py`

 * *Files identical despite different names*

### Comparing `psusigner-0.1.7/PKG-INFO` & `psusigner-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psusigner
-Version: 0.1.7
+Version: 0.1.8
 Summary: PSU Signer
 Author: Thanathip Limna
 Author-email: thanathip.l@coe.psu.ac.th
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: endesive (>=2.0.16,<3.0.0)
```


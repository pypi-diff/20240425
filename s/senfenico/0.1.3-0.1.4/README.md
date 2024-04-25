# Comparing `tmp/senfenico-0.1.3.tar.gz` & `tmp/senfenico-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senfenico-0.1.3.tar", last modified: Wed Apr 24 04:52:14 2024, max compression
+gzip compressed data, was "senfenico-0.1.4.tar", last modified: Thu Apr 25 17:02:43 2024, max compression
```

## Comparing `senfenico-0.1.3.tar` & `senfenico-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 04:52:14.310872 senfenico-0.1.3/
--rw-rw-rw-   0        0        0     1189 2024-04-24 04:52:14.265879 senfenico-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-04-22 18:36:03.000000 senfenico-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 04:52:14.231202 senfenico-0.1.3/senfenico/
--rw-rw-rw-   0        0        0      187 2024-04-19 22:01:48.000000 senfenico-0.1.3/senfenico/__init__.py
--rw-rw-rw-   0        0        0     1541 2024-04-24 03:10:19.000000 senfenico-0.1.3/senfenico/_balance.py
--rw-rw-rw-   0        0        0     5926 2024-04-24 03:40:26.000000 senfenico-0.1.3/senfenico/_charge.py
--rw-rw-rw-   0        0        0     3590 2024-04-24 04:43:45.000000 senfenico-0.1.3/senfenico/_checkout.py
--rw-rw-rw-   0        0        0     3699 2024-04-24 03:10:53.000000 senfenico-0.1.3/senfenico/_settlement.py
--rw-rw-rw-   0        0        0     1034 2024-04-24 03:33:35.000000 senfenico-0.1.3/senfenico/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 04:52:14.263884 senfenico-0.1.3/senfenico.egg-info/
--rw-rw-rw-   0        0        0     1189 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 04:52:14.310872 senfenico-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      900 2024-04-24 04:45:43.000000 senfenico-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:02:43.861956 senfenico-0.1.4/
+-rw-rw-rw-   0        0        0     1189 2024-04-25 17:02:43.858807 senfenico-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-22 18:36:03.000000 senfenico-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 17:02:43.830502 senfenico-0.1.4/senfenico/
+-rw-rw-rw-   0        0        0      187 2024-04-19 22:01:48.000000 senfenico-0.1.4/senfenico/__init__.py
+-rw-rw-rw-   0        0        0     1541 2024-04-24 03:10:19.000000 senfenico-0.1.4/senfenico/_balance.py
+-rw-rw-rw-   0        0        0     5926 2024-04-24 03:40:26.000000 senfenico-0.1.4/senfenico/_charge.py
+-rw-rw-rw-   0        0        0     3590 2024-04-24 04:43:45.000000 senfenico-0.1.4/senfenico/_checkout.py
+-rw-rw-rw-   0        0        0     3719 2024-04-25 16:55:53.000000 senfenico-0.1.4/senfenico/_settlement.py
+-rw-rw-rw-   0        0        0     1034 2024-04-24 03:33:35.000000 senfenico-0.1.4/senfenico/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:02:43.856805 senfenico-0.1.4/senfenico.egg-info/
+-rw-rw-rw-   0        0        0     1189 2024-04-25 17:02:43.000000 senfenico-0.1.4/senfenico.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-25 17:02:43.000000 senfenico-0.1.4/senfenico.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 17:02:43.000000 senfenico-0.1.4/senfenico.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 17:02:43.000000 senfenico-0.1.4/senfenico.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 17:02:43.000000 senfenico-0.1.4/senfenico.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 17:02:43.861956 senfenico-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-04-25 17:02:26.000000 senfenico-0.1.4/setup.py
```

### Comparing `senfenico-0.1.3/PKG-INFO` & `senfenico-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senfenico
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python bindings for the Senfenico API
 Home-page: https://github.com/senfenico/senfenico-python
 Author: Senfenico
 Author-email: contact@senfenico.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/senfenico/senfenico-python/issues
 Project-URL: Documentation, https://docs.senfenico.com/en/
```

### Comparing `senfenico-0.1.3/README.md` & `senfenico-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.3/senfenico/_balance.py` & `senfenico-0.1.4/senfenico/_balance.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.3/senfenico/_charge.py` & `senfenico-0.1.4/senfenico/_charge.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.3/senfenico/_checkout.py` & `senfenico-0.1.4/senfenico/_checkout.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.3/senfenico/_settlement.py` & `senfenico-0.1.4/senfenico/_settlement.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Union, List, Optional
 from senfenico.utils import SenfenicoJSONEncoder
 
 @dataclass
 class SettlementData:
     reference: str
     amount: int
-    payout_fees: float
+    settlement_fees: float
     currency: str
     status: str
     live_mode: bool
     created_at: str
     updated_at: str
     account_type: str
     iban: str
@@ -62,15 +62,15 @@
 
 class Settlement:
 
     @classmethod
     def create(cls, amount: int) -> SenfenicoObject:
         from senfenico import api_key
         
-        url = "https://api.senfenico.com/v1/payment/payouts/"
+        url = "https://api.senfenico.com/v1/payment/settlements/"
 
         payload = json.dumps({
             "amount": amount
         })
         
         headers = {
             'Content-Type': 'application/json',
@@ -82,15 +82,15 @@
         settlement = SenfenicoObject.from_dict(response.json())
         return settlement
     
 
     @classmethod
     def fetch(cls, settlement_reference) -> SenfenicoObject:
         from senfenico import api_key
-        url = f"https://api.senfenico.com/v1/payment/payouts/{settlement_reference}"
+        url = f"https://api.senfenico.com/v1/payment/settlements/{settlement_reference}"
 
         payload = {}
         headers = {
             'Accept': 'application/json',
             'X-API-KEY': api_key
         }
 
@@ -98,15 +98,15 @@
         fetched_charge = SenfenicoObject.from_dict(response.json())
         return fetched_charge
 
 
     @classmethod
     def list(cls) -> SenfenicoObject:
         from senfenico import api_key
-        url = "https://api.senfenico.com/v1/payment/payouts"
+        url = "https://api.senfenico.com/v1/payment/settlements"
 
         payload = {}
         headers = {
             'Accept': 'application/json',
             'X-API-KEY': api_key
         }
 
@@ -114,15 +114,15 @@
         charge_list = SenfenicoObject.from_dict(response.json())
         return charge_list
     
 
     @classmethod
     def cancel(cls, settlement_reference) -> SenfenicoObject:
         from senfenico import api_key
-        url = f"https://api.senfenico.com/v1/payment/payouts/{settlement_reference}/cancel/"
+        url = f"https://api.senfenico.com/v1/payment/settlements/{settlement_reference}/cancel/"
 
         payload = {}
         headers = {
             'Accept': 'application/json',
             'X-API-KEY': api_key
         }
```

### Comparing `senfenico-0.1.3/senfenico/utils.py` & `senfenico-0.1.4/senfenico/utils.py`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.3/senfenico.egg-info/PKG-INFO` & `senfenico-0.1.4/senfenico.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senfenico
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python bindings for the Senfenico API
 Home-page: https://github.com/senfenico/senfenico-python
 Author: Senfenico
 Author-email: contact@senfenico.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/senfenico/senfenico-python/issues
 Project-URL: Documentation, https://docs.senfenico.com/en/
```

### Comparing `senfenico-0.1.3/setup.py` & `senfenico-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='senfenico',
-    version='0.1.3',
+    version='0.1.4',
 
     description="Python bindings for the Senfenico API",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Senfenico",
     author_email="contact@senfenico.com",
     url="https://github.com/senfenico/senfenico-python",
```


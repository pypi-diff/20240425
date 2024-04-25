# Comparing `tmp/python_mpesa_koros-0.1.8.tar.gz` & `tmp/python_mpesa_koros-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_mpesa_koros-0.1.8.tar", last modified: Thu Apr 25 07:14:36 2024, max compression
+gzip compressed data, was "python_mpesa_koros-0.1.9.tar", last modified: Thu Apr 25 07:38:20 2024, max compression
```

## Comparing `python_mpesa_koros-0.1.8.tar` & `python_mpesa_koros-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 07:14:36.109940 python_mpesa_koros-0.1.8/
--rw-rw-rw-   0        0        0      437 2024-04-25 07:14:36.106962 python_mpesa_koros-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 07:14:36.051039 python_mpesa_koros-0.1.8/python_mpesa_koros/
--rw-rw-rw-   0        0        0      266 2024-01-17 12:05:33.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/__ init __.py
--rw-rw-rw-   0        0        0      856 2024-04-22 09:35:08.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/access_token.py
--rw-rw-rw-   0        0        0     1456 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/b2c_response_test_data.json
--rw-rw-rw-   0        0        0     3147 2024-04-22 09:58:04.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/business_to_customer.py
--rw-rw-rw-   0        0        0     1955 2024-04-22 09:37:27.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/customer_to_business.py
--rw-rw-rw-   0        0        0     3574 2024-04-22 12:18:39.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query.py
--rw-rw-rw-   0        0        0     1101 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query_response_test_data.json
--rw-rw-rw-   0        0        0     1116 2024-04-22 09:48:46.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:14:36.103957 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 07:14:36.109940 python_mpesa_koros-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-04-25 07:13:04.000000 python_mpesa_koros-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:38:20.823426 python_mpesa_koros-0.1.9/
+-rw-rw-rw-   0        0        0      437 2024-04-25 07:38:20.821431 python_mpesa_koros-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 07:38:20.783115 python_mpesa_koros-0.1.9/python_mpesa_koros/
+-rw-rw-rw-   0        0        0      266 2024-01-17 12:05:33.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/__ init __.py
+-rw-rw-rw-   0        0        0      856 2024-04-22 09:35:08.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/access_token.py
+-rw-rw-rw-   0        0        0     1456 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/b2c_response_test_data.json
+-rw-rw-rw-   0        0        0     3149 2024-04-25 07:37:50.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/business_to_customer.py
+-rw-rw-rw-   0        0        0     1956 2024-04-25 07:36:44.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/customer_to_business.py
+-rw-rw-rw-   0        0        0     3576 2024-04-25 07:37:31.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query.py
+-rw-rw-rw-   0        0        0     1101 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query_response_test_data.json
+-rw-rw-rw-   0        0        0     1116 2024-04-22 09:48:46.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:38:20.819438 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:38:20.823426 python_mpesa_koros-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-04-25 07:38:12.000000 python_mpesa_koros-0.1.9/setup.py
```

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/access_token.py` & `python_mpesa_koros-0.1.9/python_mpesa_koros/access_token.py`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/b2c_response_test_data.json` & `python_mpesa_koros-0.1.9/python_mpesa_koros/b2c_response_test_data.json`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/business_to_customer.py` & `python_mpesa_koros-0.1.9/python_mpesa_koros/business_to_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import os
 from dotenv import load_dotenv
-from access_token import AccessToken
-from utils import generate_security_credential
+from .access_token import AccessToken
+from .utils import generate_security_credential
 
 class BusinessToCustomer:
 	def __init__(self):
 		if os.getenv('MPESA_ENV') == "1":
 			self.business_to_customer_url=os.getenv('MPESA_LIVE_B2C_URL')
 			self.initiator=os.getenv('MPESA_LIVE_INITIATOR')
 			self.party_a=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_PARTY_A')
```

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/customer_to_business.py` & `python_mpesa_koros-0.1.9/python_mpesa_koros/customer_to_business.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import datetime
 import requests
 import os
 
 from dotenv import load_dotenv
-from access_token import AccessToken
+from .access_token import AccessToken
 load_dotenv()
 
 
 class CustomerToBusiness:	
 	def stk_push(self,amount, phone,bill_reference,transaction_description =""):
 		if transaction_description == "":
 			transaction_description = "Payment REquest for Bill Reference "+bill_reference
```

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query.py` & `python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import os
 from dotenv import load_dotenv
-from access_token import AccessToken
+from .access_token import AccessToken
 load_dotenv()
-from utils import generate_security_credential
+from .utils import generate_security_credential
 
 class TransactionQuery:
 	def __init__(self):
 		if os.getenv('MPESA_ENV') == "1":
 			self.trans_status_url=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_URL')
 			self.initiator=os.getenv('MPESA_LIVE_INITIATOR')
 			self.party_a=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_PARTY_A')
```

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query_response_test_data.json` & `python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query_response_test_data.json`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros/utils.py` & `python_mpesa_koros-0.1.9/python_mpesa_koros/utils.py`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/SOURCES.txt` & `python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.8/setup.py` & `python_mpesa_koros-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='python_mpesa_koros',
-    version='0.1.8',
+    version='0.1.9',
     author='Kevin Ongulu',
     author_email='kevinongulu@gmail.com',
     description='A python package for connecting to MPESA APIs',
     #packages=find_packages(),
     packages = ['python_mpesa_koros'], 
     classifiers=[
         'Programming Language :: Python :: 3',
```


# Comparing `tmp/python_mpesa_koros-0.1.7.tar.gz` & `tmp/python_mpesa_koros-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_mpesa_koros-0.1.7.tar", last modified: Wed Jan 17 12:39:32 2024, max compression
+gzip compressed data, was "python_mpesa_koros-0.1.8.tar", last modified: Thu Apr 25 07:14:36 2024, max compression
```

## Comparing `python_mpesa_koros-0.1.7.tar` & `python_mpesa_koros-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 12:39:32.892004 python_mpesa_koros-0.1.7/
--rw-rw-rw-   0        0        0      437 2024-01-17 12:39:32.889013 python_mpesa_koros-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-17 12:39:32.851113 python_mpesa_koros-0.1.7/python_mpesa_koros/
--rw-rw-rw-   0        0        0      266 2024-01-17 12:05:33.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/__ init __.py
--rw-rw-rw-   0        0        0      854 2024-01-15 11:23:21.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/access_token.py
--rw-rw-rw-   0        0        0     1456 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/b2c_response_test_data.json
--rw-rw-rw-   0        0        0     3140 2024-01-17 12:38:03.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/business_to_customer.py
--rw-rw-rw-   0        0        0     1953 2024-01-17 12:16:41.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/customer_to_business.py
--rw-rw-rw-   0        0        0     3574 2024-01-17 12:38:20.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/transaction_query.py
--rw-rw-rw-   0        0        0     1101 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/transaction_query_response_test_data.json
--rw-rw-rw-   0        0        0     1011 2024-01-17 12:37:40.000000 python_mpesa_koros-0.1.7/python_mpesa_koros/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-17 12:39:32.886020 python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/
--rw-rw-rw-   0        0        0      437 2024-01-17 12:39:32.000000 python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2024-01-17 12:39:32.000000 python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 12:39:32.000000 python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-01-17 12:39:32.000000 python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-01-17 12:39:32.000000 python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-17 12:39:32.893001 python_mpesa_koros-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-01-17 12:39:30.000000 python_mpesa_koros-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:14:36.109940 python_mpesa_koros-0.1.8/
+-rw-rw-rw-   0        0        0      437 2024-04-25 07:14:36.106962 python_mpesa_koros-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 07:14:36.051039 python_mpesa_koros-0.1.8/python_mpesa_koros/
+-rw-rw-rw-   0        0        0      266 2024-01-17 12:05:33.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/__ init __.py
+-rw-rw-rw-   0        0        0      856 2024-04-22 09:35:08.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/access_token.py
+-rw-rw-rw-   0        0        0     1456 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/b2c_response_test_data.json
+-rw-rw-rw-   0        0        0     3147 2024-04-22 09:58:04.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/business_to_customer.py
+-rw-rw-rw-   0        0        0     1955 2024-04-22 09:37:27.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/customer_to_business.py
+-rw-rw-rw-   0        0        0     3574 2024-04-22 12:18:39.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query.py
+-rw-rw-rw-   0        0        0     1101 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query_response_test_data.json
+-rw-rw-rw-   0        0        0     1116 2024-04-22 09:48:46.000000 python_mpesa_koros-0.1.8/python_mpesa_koros/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:14:36.103957 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-25 07:14:35.000000 python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:14:36.109940 python_mpesa_koros-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-04-25 07:13:04.000000 python_mpesa_koros-0.1.8/setup.py
```

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/access_token.py` & `python_mpesa_koros-0.1.8/python_mpesa_koros/access_token.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import os
 from dotenv import load_dotenv
 load_dotenv()
 
 class AccessToken:
 	def __init__(self):
-		if os.getenv('MPESA_ENV') == 1:
+		if os.getenv('MPESA_ENV') == "1":
 			self.consumer_key=os.getenv('MPESA_LIVE_CONSUMER_KEY')
 			self.consumer_secret=os.getenv('MPESA_LIVE_CONSUMER_SECRET')
 			self.token_url=os.getenv('MPESA_LIVE_TOKEN_URL')
 		else:
 			self.consumer_key=os.getenv('MPESA_TEST_CONSUMER_KEY')
 			self.consumer_secret=os.getenv('MPESA_TEST_CONSUMER_SECRET')
 			self.token_url=os.getenv('MPESA_TEST_TOKEN_URL')
```

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/b2c_response_test_data.json` & `python_mpesa_koros-0.1.8/python_mpesa_koros/b2c_response_test_data.json`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/business_to_customer.py` & `python_mpesa_koros-0.1.8/python_mpesa_koros/business_to_customer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 import os
 from dotenv import load_dotenv
-from .access_token import AccessToken
-from .utils import generate_security_credential
+from access_token import AccessToken
+from utils import generate_security_credential
 
 class BusinessToCustomer:
 	def __init__(self):
-		if os.getenv('MPESA_ENV') == 1:
+		if os.getenv('MPESA_ENV') == "1":
 			self.business_to_customer_url=os.getenv('MPESA_LIVE_B2C_URL')
 			self.initiator=os.getenv('MPESA_LIVE_INITIATOR')
 			self.party_a=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_PARTY_A')
 			self.party_b=os.getenv('MPESA_LIVE_B2C_PARTY_B')
 			self.result_url=os.getenv('MPESA_LIVE_B2C_RESULT_URL')
 			self.queue_timeout_url=os.getenv('MPESA_LIVE_B2C_QUEUE_TIMEOUT_URL')
 			self.command_id=os.getenv('MPESA_LIVE_B2C_COMMAND_ID')
@@ -50,18 +50,18 @@
 		    "CommandID": self.command_id,
 		    "PartyA": self.party_a,
 		    "PartyB": phone_number,
 		    "Amount": amount,
 		    "ResultURL": self.result_url,
 		    "QueueTimeOutURL": self.queue_timeout_url,
 		    "Remarks": remarks,
-		    "Occassion": "",
+		    "Occassion": occasion,
 		}
 
-		r = requests.get(self.business_to_customer_url, json=payload, headers=headers)
+		r = requests.post(self.business_to_customer_url, json=payload, headers=headers)
 		json_response = r.json()
 		print(json_response)
 		return json_response
 
 	def extract_response_details(self, data):
 		receiver=data['Result']['ResultParameters']['ResultParameter'][4]['Value']
 		split_receiver = receiver.split('-')
```

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/customer_to_business.py` & `python_mpesa_koros-0.1.8/python_mpesa_koros/customer_to_business.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import base64
 import datetime
 import requests
 import os
 
 from dotenv import load_dotenv
-from .access_token import AccessToken
+from access_token import AccessToken
 load_dotenv()
 
 
 class CustomerToBusiness:	
 	def stk_push(self,amount, phone,bill_reference,transaction_description =""):
 		if transaction_description == "":
 			transaction_description = "Payment REquest for Bill Reference "+bill_reference
 		time = datetime.datetime.now()
 		timestamp = time.strftime('%Y%m%d%H%M%S')
-		if os.getenv('MPESA_ENV') == 1:
+		if os.getenv('MPESA_ENV_1') == "1":
 			api_url = os.getenv('MPESA_LIVE_CUSTOMER_TO_BUSINESS_URL')
 			data = os.getenv('MPESA_LIVE_BUSINESS_SHORTCODE') + os.getenv('MPESA_LIVE_PASSKEY') + timestamp
 			callback_url = os.getenv('MPESA_LIVE_CALLBACK_URL')
 			busines_shortcode = os.getenv('MPESA_LIVE_BUSINESS_SHORTCODE')
 		else:
 			api_url = os.getenv('MPESA_TEST_CUSTOMER_TO_BUSINESS_URL')
 			data = os.getenv('MPESA_TEST_BUSINESS_SHORTCODE') + os.getenv('MPESA_TEST_PASSKEY') + timestamp
 			callback_url = os.getenv('MPESA_TEST_CALLBACK_URL')
 			busines_shortcode = os.getenv('MPESA_TEST_BUSINESS_SHORTCODE')
 		encoded_string = base64.b64encode(data.encode())
 		password = encoded_string.decode('utf-8')
 		token = AccessToken()
 		access_token=token.get_access_token()
-		headers = { "Authorization": "Bearer %s" % access_token }
+		headers = {"Authorization": "Bearer %s" % access_token }
 		request = {
             "BusinessShortCode": busines_shortcode,
             "Password": password,
             "Timestamp": timestamp,
             "TransactionType": "CustomerPayBillOnline",
             "Amount": amount,
             "PartyA": phone,
```

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/transaction_query.py` & `python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import requests
 import os
 from dotenv import load_dotenv
-from .access_token import AccessToken
+from access_token import AccessToken
 load_dotenv()
-from .utils import generate_security_credential
+from utils import generate_security_credential
 
 class TransactionQuery:
 	def __init__(self):
-		if os.getenv('MPESA_ENV') == 1:
+		if os.getenv('MPESA_ENV') == "1":
 			self.trans_status_url=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_URL')
 			self.initiator=os.getenv('MPESA_LIVE_INITIATOR')
 			self.party_a=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_PARTY_A')
 			self.result_url=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_RESULT_URL')
 			self.queue_timeout_url=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_QUEUE_TIMEOUT_URL')
 			self.remarks=os.getenv('MPESA_LIVE_TRANSACTION_QUERY_REMARKS')
 			self.password=os.getenv('MPESA_LIVE_PASSWORD')
```

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/transaction_query_response_test_data.json` & `python_mpesa_koros-0.1.8/python_mpesa_koros/transaction_query_response_test_data.json`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros/utils.py` & `python_mpesa_koros-0.1.8/python_mpesa_koros/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_v1_5
 import base64
 import os
 
 
 def generate_security_credential(initiator_password) -> str:
-    if os.getenv('MPESA_ENV') == 1:
-        path='./certs/ProductCertificate.cer'
+    current_dir = os.path.dirname(__file__)
+    if os.getenv('MPESA_ENV') == "1":
+        path=os.path.join(current_dir, 'certs', 'ProductionCertificate.cer')
     else:
-        path='./certs/SandboxCertificate.cer'
+        path=os.path.join(current_dir, 'certs', 'SandboxCertificate.cer')
     """
     Generates security credentials for C2B, B2C, B2B, REVERSAL and Transaction status post requests.
     :param inititator_password: Password for the organization initiating the transaction, provided by safaricom.
     :return: string representing the security credential
     """
     bytearray_password = bytearray(initiator_password.encode('utf-8'))
     with open(path, "rb") as f:
```

### Comparing `python_mpesa_koros-0.1.7/python_mpesa_koros.egg-info/SOURCES.txt` & `python_mpesa_koros-0.1.8/python_mpesa_koros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.7/setup.py` & `python_mpesa_koros-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='python_mpesa_koros',
-    version='0.1.7',
+    version='0.1.8',
     author='Kevin Ongulu',
     author_email='kevinongulu@gmail.com',
     description='A python package for connecting to MPESA APIs',
     #packages=find_packages(),
     packages = ['python_mpesa_koros'], 
     classifiers=[
         'Programming Language :: Python :: 3',
```


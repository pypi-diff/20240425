# Comparing `tmp/python_mpesa_koros-0.1.9.tar.gz` & `tmp/python_mpesa_koros-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_mpesa_koros-0.1.9.tar", last modified: Thu Apr 25 07:38:20 2024, max compression
+gzip compressed data, was "python_mpesa_koros-2.0.0.tar", last modified: Thu Apr 25 11:34:51 2024, max compression
```

## Comparing `python_mpesa_koros-0.1.9.tar` & `python_mpesa_koros-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 07:38:20.823426 python_mpesa_koros-0.1.9/
--rw-rw-rw-   0        0        0      437 2024-04-25 07:38:20.821431 python_mpesa_koros-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 07:38:20.783115 python_mpesa_koros-0.1.9/python_mpesa_koros/
--rw-rw-rw-   0        0        0      266 2024-01-17 12:05:33.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/__ init __.py
--rw-rw-rw-   0        0        0      856 2024-04-22 09:35:08.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/access_token.py
--rw-rw-rw-   0        0        0     1456 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/b2c_response_test_data.json
--rw-rw-rw-   0        0        0     3149 2024-04-25 07:37:50.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/business_to_customer.py
--rw-rw-rw-   0        0        0     1956 2024-04-25 07:36:44.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/customer_to_business.py
--rw-rw-rw-   0        0        0     3576 2024-04-25 07:37:31.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query.py
--rw-rw-rw-   0        0        0     1101 2023-01-06 08:58:57.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query_response_test_data.json
--rw-rw-rw-   0        0        0     1116 2024-04-22 09:48:46.000000 python_mpesa_koros-0.1.9/python_mpesa_koros/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:38:20.819438 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-25 07:38:20.000000 python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 07:38:20.823426 python_mpesa_koros-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-04-25 07:38:12.000000 python_mpesa_koros-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:34:51.431149 python_mpesa_koros-2.0.0/
+-rw-rw-rw-   0        0        0      437 2024-04-25 11:34:51.427158 python_mpesa_koros-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 11:34:51.367313 python_mpesa_koros-2.0.0/python_mpesa_koros/
+-rw-rw-rw-   0        0        0      266 2024-01-17 12:05:33.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/__ init __.py
+-rw-rw-rw-   0        0        0      858 2024-04-25 11:33:23.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/access_token.py
+-rw-rw-rw-   0        0        0     1456 2023-01-06 08:58:57.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/b2c_response_test_data.json
+-rw-rw-rw-   0        0        0     3151 2024-04-25 11:33:40.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/business_to_customer.py
+-rw-rw-rw-   0        0        0     1958 2024-04-25 11:32:18.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/customer_to_business.py
+-rw-rw-rw-   0        0        0     3578 2024-04-25 11:33:54.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/transaction_query.py
+-rw-rw-rw-   0        0        0     1101 2023-01-06 08:58:57.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/transaction_query_response_test_data.json
+-rw-rw-rw-   0        0        0     1116 2024-04-22 09:48:46.000000 python_mpesa_koros-2.0.0/python_mpesa_koros/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:34:51.425165 python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-25 11:34:51.000000 python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-04-25 11:34:51.000000 python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 11:34:51.000000 python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-25 11:34:51.000000 python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-25 11:34:51.000000 python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 11:34:51.431149 python_mpesa_koros-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-04-25 11:34:15.000000 python_mpesa_koros-2.0.0/setup.py
```

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/access_token.py` & `python_mpesa_koros-2.0.0/python_mpesa_koros/access_token.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 			self.token_url=os.getenv('MPESA_TEST_TOKEN_URL')
 
 	def get_access_token(self):
 		access_token=None
 		r = requests.get(self.token_url, auth=requests.auth.HTTPBasicAuth(self.consumer_key, self.consumer_secret))
 		status_code=r.status_code
 		json_response = r.json()
-		print(json_response)
+		# print(json_response)
 		if 'access_token' in json_response:
 			access_token = json_response['access_token']
 		return access_token
```

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/b2c_response_test_data.json` & `python_mpesa_koros-2.0.0/python_mpesa_koros/b2c_response_test_data.json`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/business_to_customer.py` & `python_mpesa_koros-2.0.0/python_mpesa_koros/business_to_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		    "QueueTimeOutURL": self.queue_timeout_url,
 		    "Remarks": remarks,
 		    "Occassion": occasion,
 		}
 
 		r = requests.post(self.business_to_customer_url, json=payload, headers=headers)
 		json_response = r.json()
-		print(json_response)
+		# print(json_response)
 		return json_response
 
 	def extract_response_details(self, data):
 		receiver=data['Result']['ResultParameters']['ResultParameter'][4]['Value']
 		split_receiver = receiver.split('-')
 		phone = split_receiver[0]
 		name = split_receiver[1]
```

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/customer_to_business.py` & `python_mpesa_koros-2.0.0/python_mpesa_koros/customer_to_business.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
             "PhoneNumber": phone,
             "CallBackURL": callback_url,
             "AccountReference": bill_reference,
             "TransactionDesc": transaction_description
         }
 		response = requests.post(api_url, json = request, headers=headers)
 		json_response = response.json()
-		print(json_response)
+		# print(json_response)
 		return (json_response)
```

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query.py` & `python_mpesa_koros-2.0.0/python_mpesa_koros/transaction_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 		    "QueueTimeOutURL": self.queue_timeout_url,
 		    "Remarks": remarks,
 		    "Occassion": occassion,
 		 }
 
 		r = requests.post(self.trans_status_url, json=payload, headers=headers)
 		json_response = r.json()
-		print(json_response)
+		# print(json_response)
 		return json_response
 
 	def extract_response_details(self, data):
 		sender=data['Result']['ResultParameters']['ResultParameter'][1]['Value']
 		split_sender = sender.split('-')
 		phone = split_sender[0]
 		name = split_sender[1]
```

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/transaction_query_response_test_data.json` & `python_mpesa_koros-2.0.0/python_mpesa_koros/transaction_query_response_test_data.json`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros/utils.py` & `python_mpesa_koros-2.0.0/python_mpesa_koros/utils.py`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.9/python_mpesa_koros.egg-info/SOURCES.txt` & `python_mpesa_koros-2.0.0/python_mpesa_koros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_mpesa_koros-0.1.9/setup.py` & `python_mpesa_koros-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='python_mpesa_koros',
-    version='0.1.9',
+    version='2.0.0',
     author='Kevin Ongulu',
     author_email='kevinongulu@gmail.com',
     description='A python package for connecting to MPESA APIs',
     #packages=find_packages(),
     packages = ['python_mpesa_koros'], 
     classifiers=[
         'Programming Language :: Python :: 3',
```


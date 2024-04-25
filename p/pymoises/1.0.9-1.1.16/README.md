# Comparing `tmp/pymoises-1.0.9.tar.gz` & `tmp/pymoises-1.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoises-1.0.9.tar", last modified: Thu Dec  7 00:31:56 2023, max compression
+gzip compressed data, was "pymoises-1.1.16.tar", last modified: Thu Apr 25 18:02:53 2024, max compression
```

## Comparing `pymoises-1.0.9.tar` & `pymoises-1.1.16.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.585068 pymoises-1.0.9/
--rw-rw-rw-   0        0        0      187 2023-12-07 00:31:56.584064 pymoises-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-12-06 15:35:18.000000 pymoises-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.523066 pymoises-1.0.9/pymoises/
--rw-rw-rw-   0        0        0     5226 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/Transactions.py
--rw-rw-rw-   0        0        0      135 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/bussinesUnits.py
--rw-rw-rw-   0        0        0    10329 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/customer.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.553068 pymoises-1.0.9/pymoises/dto/
--rw-rw-rw-   0        0        0       43 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.555068 pymoises-1.0.9/pymoises/dto/input/
--rw-rw-rw-   0        0        0       52 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.562067 pymoises-1.0.9/pymoises/dto/input/customer/
--rw-rw-rw-   0        0        0       86 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/customer/__init__.py
--rw-rw-rw-   0        0        0      530 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
--rw-rw-rw-   0        0        0     1570 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/customer/createLead_input_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.565067 pymoises-1.0.9/pymoises/dto/input/transaction/
--rw-rw-rw-   0        0        0       43 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/transaction/__init__.py
--rw-rw-rw-   0        0        0      524 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/input/transaction/create_transaction_input_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.567066 pymoises-1.0.9/pymoises/dto/output/
--rw-rw-rw-   0        0        0       51 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.575068 pymoises-1.0.9/pymoises/dto/output/customer/
--rw-rw-rw-   0        0        0      108 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/__init__.py
--rw-rw-rw-   0        0        0      758 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/createLead_output_dto.py
--rw-rw-rw-   0        0        0     1351 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/customer_output_dto.py
--rw-rw-rw-   0        0        0      930 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/customer/moveLead_output_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.578066 pymoises-1.0.9/pymoises/dto/output/psps/
--rw-rw-rw-   0        0        0        0 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/psps/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/psps/get_info_psp_output_dto.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.582074 pymoises-1.0.9/pymoises/dto/output/transaction/
--rw-rw-rw-   0        0        0       37 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/transaction/__init__.py
--rw-rw-rw-   0        0        0      552 2023-12-06 15:35:18.000000 pymoises-1.0.9/pymoises/dto/output/transaction/transaction_output_dto.py
--rw-rw-rw-   0        0        0     3626 2023-12-07 00:19:28.000000 pymoises-1.0.9/pymoises/psps.py
-drwxrwxrwx   0        0        0        0 2023-12-07 00:31:56.551067 pymoises-1.0.9/pymoises.egg-info/
--rw-rw-rw-   0        0        0      187 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-07 00:31:56.000000 pymoises-1.0.9/pymoises.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-07 00:31:56.585068 pymoises-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-12-07 00:31:37.000000 pymoises-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.643278 pymoises-1.1.16/
+-rw-rw-rw-   0        0        0      171 2024-04-25 18:02:53.642279 pymoises-1.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-25 16:50:13.000000 pymoises-1.1.16/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.604279 pymoises-1.1.16/pymoises/
+-rw-rw-rw-   0        0        0     5226 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/Transactions.py
+-rw-rw-rw-   0        0        0      135 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/__init__.py
+-rw-rw-rw-   0        0        0     1705 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/bussinesUnits.py
+-rw-rw-rw-   0        0        0    10573 2024-04-25 18:02:18.000000 pymoises-1.1.16/pymoises/customer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.619279 pymoises-1.1.16/pymoises/dto/
+-rw-rw-rw-   0        0        0       43 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.621278 pymoises-1.1.16/pymoises/dto/input/
+-rw-rw-rw-   0        0        0       52 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.625277 pymoises-1.1.16/pymoises/dto/input/customer/
+-rw-rw-rw-   0        0        0       86 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/customer/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+-rw-rw-rw-   0        0        0     1570 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/customer/createLead_input_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.627277 pymoises-1.1.16/pymoises/dto/input/transaction/
+-rw-rw-rw-   0        0        0       43 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/transaction/__init__.py
+-rw-rw-rw-   0        0        0      524 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/transaction/create_transaction_input_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.628279 pymoises-1.1.16/pymoises/dto/output/
+-rw-rw-rw-   0        0        0       51 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.634281 pymoises-1.1.16/pymoises/dto/output/customer/
+-rw-rw-rw-   0        0        0      108 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/__init__.py
+-rw-rw-rw-   0        0        0      758 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/createLead_output_dto.py
+-rw-rw-rw-   0        0        0     1351 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/customer_output_dto.py
+-rw-rw-rw-   0        0        0      930 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/moveLead_output_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.636277 pymoises-1.1.16/pymoises/dto/output/psps/
+-rw-rw-rw-   0        0        0        0 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/psps/__init__.py
+-rw-rw-rw-   0        0        0     1602 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/psps/get_info_psp_output_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.639278 pymoises-1.1.16/pymoises/dto/output/transaction/
+-rw-rw-rw-   0        0        0       37 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/transaction/__init__.py
+-rw-rw-rw-   0        0        0      552 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/transaction/transaction_output_dto.py
+-rw-rw-rw-   0        0        0     7122 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/psps.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.641278 pymoises-1.1.16/pymoises.egg-info/
+-rw-rw-rw-   0        0        0      171 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:02:53.644278 pymoises-1.1.16/setup.cfg
+-rw-rw-rw-   0        0        0      559 2024-04-25 18:02:44.000000 pymoises-1.1.16/setup.py
```

### Comparing `pymoises-1.0.9/pymoises/Transactions.py` & `pymoises-1.1.16/pymoises/Transactions.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/bussinesUnits.py` & `pymoises-1.1.16/pymoises/bussinesUnits.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/customer.py` & `pymoises-1.1.16/pymoises/customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import requests
 import logging
+import re
 
 from .dto import (
     check_email_phone_input_schema,
     get_customer_output_schema,
     move_lead_output_schema, 
     create_lead_input_schema,
     create_customer_output_schema
 )
 
+def clean_strings(string):
+
+    clean_specials = re.sub(r'[^\w\s]', '', string)
+    
+    return clean_specials.title()
+
 class Customers:
     def check_customer_by_email_phone(request: check_email_phone_input_schema) -> get_customer_output_schema:
         """
         Check if exist a customer in moises whit the email and phone.
 
         Params:
             check_email_phone_input_schema : 
@@ -102,20 +109,22 @@
 
             respone : get_customer_output_schema = {}
             respone['success'] = True
             respone['message'] = "Customer info"
             respone['payload'] = {}
             respone['payload']['tpid'] = moisesResponse['data']['tpId']
             respone['payload']['crmId'] = moisesResponse['data']['crmId']
-            respone['payload']['firstName'] = moisesResponse['data']['firstName']
-            respone['payload']['lastName'] = moisesResponse['data']['lastName']
+            respone['payload']['firstName'] = clean_strings(moisesResponse['data']['firstName'])
+            respone['payload']['lastName'] = clean_strings(moisesResponse['data']['lastName'])
             respone['payload']['phoneCode'] = moisesResponse['data']['phoneCode']
             respone['payload']['phoneNumber'] = moisesResponse['data']['phoneNumber']
             respone['payload']['country'] = moisesResponse['data']['country']
             respone['payload']['BussinessUnit'] = moisesResponse['data']['idCrmBusinessUnit']
+            respone['payload']['email'] = moisesResponse['data']['email']
+
 
             return respone
     
         except Exception as Err:
             respone : get_customer_output_schema = {}
             respone['success'] = False
             respone['message'] = str(Err)
```

### Comparing `pymoises-1.0.9/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py` & `pymoises-1.1.16/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/input/customer/createLead_input_dto.py` & `pymoises-1.1.16/pymoises/dto/input/customer/createLead_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/input/transaction/create_transaction_input_dto.py` & `pymoises-1.1.16/pymoises/dto/input/transaction/create_transaction_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/output/customer/createLead_output_dto.py` & `pymoises-1.1.16/pymoises/dto/output/customer/createLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/output/customer/customer_output_dto.py` & `pymoises-1.1.16/pymoises/dto/output/customer/customer_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/output/customer/moveLead_output_dto.py` & `pymoises-1.1.16/pymoises/dto/output/customer/moveLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/output/psps/get_info_psp_output_dto.py` & `pymoises-1.1.16/pymoises/dto/output/psps/get_info_psp_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises/dto/output/transaction/transaction_output_dto.py` & `pymoises-1.1.16/pymoises/dto/output/transaction/transaction_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/pymoises.egg-info/SOURCES.txt` & `pymoises-1.1.16/pymoises.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.9/setup.py` & `pymoises-1.1.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pymoises",
-    version="1.0.9",
+    version="1.1.16",
     description="Callings from moises endpoints...",
     author="Platimex",
     packages=[
         "pymoises", 
         "pymoises.dto", 
         "pymoises.dto.input", 
         "pymoises.dto.input.customer",
```


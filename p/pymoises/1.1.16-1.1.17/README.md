# Comparing `tmp/pymoises-1.1.16.tar.gz` & `tmp/pymoises-1.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoises-1.1.16.tar", last modified: Thu Apr 25 18:02:53 2024, max compression
+gzip compressed data, was "pymoises-1.1.17.tar", last modified: Thu Apr 25 18:19:31 2024, max compression
```

## Comparing `pymoises-1.1.16.tar` & `pymoises-1.1.17.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.643278 pymoises-1.1.16/
--rw-rw-rw-   0        0        0      171 2024-04-25 18:02:53.642279 pymoises-1.1.16/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-04-25 16:50:13.000000 pymoises-1.1.16/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.604279 pymoises-1.1.16/pymoises/
--rw-rw-rw-   0        0        0     5226 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/Transactions.py
--rw-rw-rw-   0        0        0      135 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/__init__.py
--rw-rw-rw-   0        0        0     1705 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/bussinesUnits.py
--rw-rw-rw-   0        0        0    10573 2024-04-25 18:02:18.000000 pymoises-1.1.16/pymoises/customer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.619279 pymoises-1.1.16/pymoises/dto/
--rw-rw-rw-   0        0        0       43 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.621278 pymoises-1.1.16/pymoises/dto/input/
--rw-rw-rw-   0        0        0       52 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.625277 pymoises-1.1.16/pymoises/dto/input/customer/
--rw-rw-rw-   0        0        0       86 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/customer/__init__.py
--rw-rw-rw-   0        0        0      530 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
--rw-rw-rw-   0        0        0     1570 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/customer/createLead_input_dto.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.627277 pymoises-1.1.16/pymoises/dto/input/transaction/
--rw-rw-rw-   0        0        0       43 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/transaction/__init__.py
--rw-rw-rw-   0        0        0      524 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/input/transaction/create_transaction_input_dto.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.628279 pymoises-1.1.16/pymoises/dto/output/
--rw-rw-rw-   0        0        0       51 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.634281 pymoises-1.1.16/pymoises/dto/output/customer/
--rw-rw-rw-   0        0        0      108 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/__init__.py
--rw-rw-rw-   0        0        0      758 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/createLead_output_dto.py
--rw-rw-rw-   0        0        0     1351 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/customer_output_dto.py
--rw-rw-rw-   0        0        0      930 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/customer/moveLead_output_dto.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.636277 pymoises-1.1.16/pymoises/dto/output/psps/
--rw-rw-rw-   0        0        0        0 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/psps/__init__.py
--rw-rw-rw-   0        0        0     1602 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/psps/get_info_psp_output_dto.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.639278 pymoises-1.1.16/pymoises/dto/output/transaction/
--rw-rw-rw-   0        0        0       37 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/transaction/__init__.py
--rw-rw-rw-   0        0        0      552 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/dto/output/transaction/transaction_output_dto.py
--rw-rw-rw-   0        0        0     7122 2024-04-25 16:50:13.000000 pymoises-1.1.16/pymoises/psps.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:02:53.641278 pymoises-1.1.16/pymoises.egg-info/
--rw-rw-rw-   0        0        0      171 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 18:02:53.000000 pymoises-1.1.16/pymoises.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 18:02:53.644278 pymoises-1.1.16/setup.cfg
--rw-rw-rw-   0        0        0      559 2024-04-25 18:02:44.000000 pymoises-1.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.900051 pymoises-1.1.17/
+-rw-rw-rw-   0        0        0      171 2024-04-25 18:19:31.898052 pymoises-1.1.17/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-25 16:50:13.000000 pymoises-1.1.17/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.860052 pymoises-1.1.17/pymoises/
+-rw-rw-rw-   0        0        0     5226 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/Transactions.py
+-rw-rw-rw-   0        0        0      135 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/__init__.py
+-rw-rw-rw-   0        0        0     1705 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/bussinesUnits.py
+-rw-rw-rw-   0        0        0    10573 2024-04-25 18:19:07.000000 pymoises-1.1.17/pymoises/customer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.875052 pymoises-1.1.17/pymoises/dto/
+-rw-rw-rw-   0        0        0       43 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.877052 pymoises-1.1.17/pymoises/dto/input/
+-rw-rw-rw-   0        0        0       52 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/input/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.881051 pymoises-1.1.17/pymoises/dto/input/customer/
+-rw-rw-rw-   0        0        0       86 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/input/customer/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+-rw-rw-rw-   0        0        0     1570 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/input/customer/createLead_input_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.884051 pymoises-1.1.17/pymoises/dto/input/transaction/
+-rw-rw-rw-   0        0        0       43 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/input/transaction/__init__.py
+-rw-rw-rw-   0        0        0      524 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/input/transaction/create_transaction_input_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.885052 pymoises-1.1.17/pymoises/dto/output/
+-rw-rw-rw-   0        0        0       51 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.890052 pymoises-1.1.17/pymoises/dto/output/customer/
+-rw-rw-rw-   0        0        0      108 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/customer/__init__.py
+-rw-rw-rw-   0        0        0      758 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/customer/createLead_output_dto.py
+-rw-rw-rw-   0        0        0     1351 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/customer/customer_output_dto.py
+-rw-rw-rw-   0        0        0      930 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/customer/moveLead_output_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.893052 pymoises-1.1.17/pymoises/dto/output/psps/
+-rw-rw-rw-   0        0        0        0 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/psps/__init__.py
+-rw-rw-rw-   0        0        0     1602 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/psps/get_info_psp_output_dto.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.895052 pymoises-1.1.17/pymoises/dto/output/transaction/
+-rw-rw-rw-   0        0        0       37 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/transaction/__init__.py
+-rw-rw-rw-   0        0        0      552 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/dto/output/transaction/transaction_output_dto.py
+-rw-rw-rw-   0        0        0     7122 2024-04-25 16:50:13.000000 pymoises-1.1.17/pymoises/psps.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:19:31.897051 pymoises-1.1.17/pymoises.egg-info/
+-rw-rw-rw-   0        0        0      171 2024-04-25 18:19:31.000000 pymoises-1.1.17/pymoises.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-25 18:19:31.000000 pymoises-1.1.17/pymoises.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:19:31.000000 pymoises-1.1.17/pymoises.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-25 18:19:31.000000 pymoises-1.1.17/pymoises.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 18:19:31.000000 pymoises-1.1.17/pymoises.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:19:31.900051 pymoises-1.1.17/setup.cfg
+-rw-rw-rw-   0        0        0      559 2024-04-25 18:19:16.000000 pymoises-1.1.17/setup.py
```

### Comparing `pymoises-1.1.16/pymoises/Transactions.py` & `pymoises-1.1.17/pymoises/Transactions.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/bussinesUnits.py` & `pymoises-1.1.17/pymoises/bussinesUnits.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/customer.py` & `pymoises-1.1.17/pymoises/customer.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py` & `pymoises-1.1.17/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/input/customer/createLead_input_dto.py` & `pymoises-1.1.17/pymoises/dto/input/customer/createLead_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/input/transaction/create_transaction_input_dto.py` & `pymoises-1.1.17/pymoises/dto/input/transaction/create_transaction_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/output/customer/createLead_output_dto.py` & `pymoises-1.1.17/pymoises/dto/output/customer/createLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/output/customer/customer_output_dto.py` & `pymoises-1.1.17/pymoises/dto/output/customer/customer_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/output/customer/moveLead_output_dto.py` & `pymoises-1.1.17/pymoises/dto/output/customer/moveLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/output/psps/get_info_psp_output_dto.py` & `pymoises-1.1.17/pymoises/dto/output/psps/get_info_psp_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/dto/output/transaction/transaction_output_dto.py` & `pymoises-1.1.17/pymoises/dto/output/transaction/transaction_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises/psps.py` & `pymoises-1.1.17/pymoises/psps.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/pymoises.egg-info/SOURCES.txt` & `pymoises-1.1.17/pymoises.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymoises-1.1.16/setup.py` & `pymoises-1.1.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pymoises",
-    version="1.1.16",
+    version="1.1.17",
     description="Callings from moises endpoints...",
     author="Platimex",
     packages=[
         "pymoises", 
         "pymoises.dto", 
         "pymoises.dto.input", 
         "pymoises.dto.input.customer",
```


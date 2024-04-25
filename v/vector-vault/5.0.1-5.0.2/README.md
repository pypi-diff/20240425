# Comparing `tmp/vector_vault-5.0.1.tar.gz` & `tmp/vector_vault-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-5.0.1.tar", last modified: Mon Apr 22 19:14:41 2024, max compression
+gzip compressed data, was "vector_vault-5.0.2.tar", last modified: Thu Apr 25 14:48:51 2024, max compression
```

## Comparing `vector_vault-5.0.1.tar` & `vector_vault-5.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-22 19:14:41.296893 vector_vault-5.0.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-5.0.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-22 19:14:41.296757 vector_vault-5.0.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-5.0.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-22 19:14:41.296930 vector_vault-5.0.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-22 19:13:43.000000 vector_vault-5.0.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-22 19:14:41.294511 vector_vault-5.0.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-22 19:14:41.000000 vector_vault-5.0.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-22 19:14:41.000000 vector_vault-5.0.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-22 19:14:41.000000 vector_vault-5.0.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-22 19:14:41.000000 vector_vault-5.0.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-22 19:14:41.000000 vector_vault-5.0.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-22 19:14:41.296580 vector_vault-5.0.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-5.0.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-5.0.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-5.0.1/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6312 2024-04-22 19:13:35.000000 vector_vault-5.0.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1932 2024-04-19 03:28:12.000000 vector_vault-5.0.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-5.0.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-5.0.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    22962 2024-04-12 07:29:05.000000 vector_vault-5.0.1/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62412 2024-04-18 17:21:28.000000 vector_vault-5.0.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-5.0.1/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-5.0.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-25 14:48:51.518530 vector_vault-5.0.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-5.0.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-25 14:48:51.518367 vector_vault-5.0.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-5.0.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-25 14:48:51.518568 vector_vault-5.0.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-25 14:48:42.000000 vector_vault-5.0.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-25 14:48:51.514993 vector_vault-5.0.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-25 14:48:51.000000 vector_vault-5.0.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-25 14:48:51.000000 vector_vault-5.0.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-25 14:48:51.000000 vector_vault-5.0.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-25 14:48:51.000000 vector_vault-5.0.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-25 14:48:51.000000 vector_vault-5.0.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-25 14:48:51.518084 vector_vault-5.0.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-5.0.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16780 2024-04-25 14:48:35.000000 vector_vault-5.0.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-5.0.2/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6312 2024-04-22 19:13:35.000000 vector_vault-5.0.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1932 2024-04-19 03:28:12.000000 vector_vault-5.0.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-5.0.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-5.0.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    22962 2024-04-12 07:29:05.000000 vector_vault-5.0.2/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62412 2024-04-18 17:21:28.000000 vector_vault-5.0.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-5.0.2/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-5.0.2/vectorvault/wrap.py
```

### Comparing `vector_vault-5.0.1/LICENSE` & `vector_vault-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/PKG-INFO` & `vector_vault-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 5.0.1
+Version: 5.0.2
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-5.0.1/README.md` & `vector_vault-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/setup.py` & `vector_vault-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="5.0.1",
+    version="5.0.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-5.0.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-5.0.2/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 5.0.1
+Version: 5.0.2
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-5.0.1/vectorvault/ai.py` & `vector_vault-5.0.2/vectorvault/ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
         self.verbose = verbose
         self.timeout = timeout
         self.model_token_limits = {
         'gpt-3.5-turbo': 16000,
         'gpt-3.5-turbo-0125': 16000,
         'gpt-3.5-turbo-16k': 16000,
         'gpt-4': 8000,
-        'gpt-4-32k': 32000,
-        'gpt-4-32k-0613': 32000,
         'gpt-4-1106-preview': 128000,
         'gpt-4-turbo': 128000,
         'gpt-4-turbo-preview': 128000,
         'gpt-4-0125-preview': 128000,
     }
         
         self.main_prompt_with_context = """Use the following Context to answer the Question at the end.
```

### Comparing `vector_vault-5.0.1/vectorvault/cloud_api.py` & `vector_vault-5.0.2/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/cloudmanager.py` & `vector_vault-5.0.2/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/creds.py` & `vector_vault-5.0.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/download.py` & `vector_vault-5.0.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/itemize.py` & `vector_vault-5.0.2/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/tools_gpt.py` & `vector_vault-5.0.2/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/vault.py` & `vector_vault-5.0.2/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-5.0.1/vectorvault/vecreq.py` & `vector_vault-5.0.2/vectorvault/vecreq.py`

 * *Files identical despite different names*


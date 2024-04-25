# Comparing `tmp/aes_python-1.5.3.tar.gz` & `tmp/aes_python-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aes_python-1.5.3.tar", last modified: Thu Apr 25 07:24:34 2024, max compression
+gzip compressed data, was "aes_python-1.5.4.tar", last modified: Thu Apr 25 07:44:58 2024, max compression
```

## Comparing `aes_python-1.5.3.tar` & `aes_python-1.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.117026 aes_python-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 07:24:29.000000 aes_python-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 07:24:34.117026 aes_python-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-25 07:24:29.000000 aes_python-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-25 07:24:30.000000 aes_python-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 07:24:34.117026 aes_python-1.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.109026 aes_python-1.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.113026 aes_python-1.5.3/src/AES_Python/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 07:24:30.000000 aes_python-1.5.3/src/AES_Python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-04-25 07:24:30.000000 aes_python-1.5.3/src/AES_Python/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.113026 aes_python-1.5.3/src/AES_Python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.113026 aes_python-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_file_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_file_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)    48027 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_key_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:44:58.364984 aes_python-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 07:44:54.000000 aes_python-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 07:44:58.364984 aes_python-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-25 07:44:54.000000 aes_python-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-25 07:44:54.000000 aes_python-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 07:44:58.364984 aes_python-1.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:44:58.360983 aes_python-1.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:44:58.360983 aes_python-1.5.4/src/AES_Python/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 07:44:54.000000 aes_python-1.5.4/src/AES_Python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-04-25 07:44:54.000000 aes_python-1.5.4/src/AES_Python/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:44:58.364984 aes_python-1.5.4/src/AES_Python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 07:44:58.000000 aes_python-1.5.4/src/AES_Python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 07:44:58.000000 aes_python-1.5.4/src/AES_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:44:58.000000 aes_python-1.5.4/src/AES_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 07:44:58.000000 aes_python-1.5.4/src/AES_Python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 07:44:58.000000 aes_python-1.5.4/src/AES_Python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:44:58.364984 aes_python-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 07:44:54.000000 aes_python-1.5.4/tests/test_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 07:44:54.000000 aes_python-1.5.4/tests/test_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-25 07:44:54.000000 aes_python-1.5.4/tests/test_file_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-25 07:44:54.000000 aes_python-1.5.4/tests/test_file_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48027 2024-04-25 07:44:54.000000 aes_python-1.5.4/tests/test_key_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-25 07:44:54.000000 aes_python-1.5.4/tests/test_methods.py
```

### Comparing `aes_python-1.5.3/LICENSE` & `aes_python-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/PKG-INFO` & `aes_python-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AES_Python
-Version: 1.5.3
+Version: 1.5.4
 Summary: AES (Advanced Encryption Standard) implementation in Python-3
 Author-email: Gabriel Lindeblad <Gabriel.Lindeblad@icloud.com>
 Project-URL: Homepage, https://github.com/Glindeb/AES-Python
 Project-URL: Repository, https://github.com/Glindeb/AES-Python
 Project-URL: Documentation, https://github.com/Glindeb/AES-Python
 Keywords: AES,AES-Python,Advanced Encryption Standard,encryption,cryptography
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aes_python-1.5.3/README.md` & `aes_python-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/pyproject.toml` & `aes_python-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AES_Python"
-version = "v1.5.3"
+version = "v1.5.4"
 description = "AES (Advanced Encryption Standard) implementation in Python-3"
 readme = "README.md"
 authors = [{name = "Gabriel Lindeblad", email = "Gabriel.Lindeblad@icloud.com"}]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Education",
```

### Comparing `aes_python-1.5.3/src/AES_Python/main.py` & `aes_python-1.5.4/src/AES_Python/main.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/src/AES_Python.egg-info/PKG-INFO` & `aes_python-1.5.4/src/AES_Python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AES_Python
-Version: 1.5.3
+Version: 1.5.4
 Summary: AES (Advanced Encryption Standard) implementation in Python-3
 Author-email: Gabriel Lindeblad <Gabriel.Lindeblad@icloud.com>
 Project-URL: Homepage, https://github.com/Glindeb/AES-Python
 Project-URL: Repository, https://github.com/Glindeb/AES-Python
 Project-URL: Documentation, https://github.com/Glindeb/AES-Python
 Keywords: AES,AES-Python,Advanced Encryption Standard,encryption,cryptography
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aes_python-1.5.3/tests/test_dec.py` & `aes_python-1.5.4/tests/test_dec.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/tests/test_enc.py` & `aes_python-1.5.4/tests/test_enc.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/tests/test_file_dec.py` & `aes_python-1.5.4/tests/test_file_dec.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/tests/test_file_enc.py` & `aes_python-1.5.4/tests/test_file_enc.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/tests/test_key_expansion.py` & `aes_python-1.5.4/tests/test_key_expansion.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.3/tests/test_methods.py` & `aes_python-1.5.4/tests/test_methods.py`

 * *Files identical despite different names*


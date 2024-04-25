# Comparing `tmp/aes_python-1.5.2.tar.gz` & `tmp/aes_python-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aes_python-1.5.2.tar", last modified: Sun Apr 21 21:40:03 2024, max compression
+gzip compressed data, was "aes_python-1.5.3.tar", last modified: Thu Apr 25 07:24:34 2024, max compression
```

## Comparing `aes_python-1.5.2.tar` & `aes_python-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:40:03.873472 aes_python-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-21 21:39:59.000000 aes_python-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-21 21:40:03.873472 aes_python-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-21 21:39:59.000000 aes_python-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-21 21:40:00.000000 aes_python-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 21:40:03.873472 aes_python-1.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:40:03.869472 aes_python-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:40:03.873472 aes_python-1.5.2/src/AES_Python/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-21 21:40:00.000000 aes_python-1.5.2/src/AES_Python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15613 2024-04-21 21:40:00.000000 aes_python-1.5.2/src/AES_Python/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:40:03.873472 aes_python-1.5.2/src/AES_Python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-21 21:40:03.000000 aes_python-1.5.2/src/AES_Python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-21 21:40:03.000000 aes_python-1.5.2/src/AES_Python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:40:03.000000 aes_python-1.5.2/src/AES_Python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-21 21:40:03.000000 aes_python-1.5.2/src/AES_Python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 21:40:03.000000 aes_python-1.5.2/src/AES_Python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:40:03.873472 aes_python-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-21 21:40:00.000000 aes_python-1.5.2/tests/test_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-21 21:40:00.000000 aes_python-1.5.2/tests/test_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-21 21:40:00.000000 aes_python-1.5.2/tests/test_file_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-21 21:40:00.000000 aes_python-1.5.2/tests/test_file_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)    48027 2024-04-21 21:40:00.000000 aes_python-1.5.2/tests/test_key_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-21 21:40:00.000000 aes_python-1.5.2/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.117026 aes_python-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 07:24:29.000000 aes_python-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 07:24:34.117026 aes_python-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-25 07:24:29.000000 aes_python-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-25 07:24:30.000000 aes_python-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 07:24:34.117026 aes_python-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.109026 aes_python-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.113026 aes_python-1.5.3/src/AES_Python/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 07:24:30.000000 aes_python-1.5.3/src/AES_Python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-04-25 07:24:30.000000 aes_python-1.5.3/src/AES_Python/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.113026 aes_python-1.5.3/src/AES_Python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 07:24:34.000000 aes_python-1.5.3/src/AES_Python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:24:34.113026 aes_python-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_file_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_file_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48027 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_key_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-25 07:24:30.000000 aes_python-1.5.3/tests/test_methods.py
```

### Comparing `aes_python-1.5.2/LICENSE` & `aes_python-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.2/PKG-INFO` & `aes_python-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AES_Python
-Version: 1.5.2
+Version: 1.5.3
 Summary: AES (Advanced Encryption Standard) implementation in Python-3
 Author-email: Gabriel Lindeblad <Gabriel.Lindeblad@icloud.com>
 Project-URL: Homepage, https://github.com/Glindeb/AES-Python
 Project-URL: Repository, https://github.com/Glindeb/AES-Python
 Project-URL: Documentation, https://github.com/Glindeb/AES-Python
 Keywords: AES,AES-Python,Advanced Encryption Standard,encryption,cryptography
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aes_python-1.5.2/README.md` & `aes_python-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.2/pyproject.toml` & `aes_python-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AES_Python"
-version = "v1.5.2"
+version = "v1.5.3"
 description = "AES (Advanced Encryption Standard) implementation in Python-3"
 readme = "README.md"
 authors = [{name = "Gabriel Lindeblad", email = "Gabriel.Lindeblad@icloud.com"}]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Education",
```

### Comparing `aes_python-1.5.2/src/AES_Python.egg-info/PKG-INFO` & `aes_python-1.5.3/src/AES_Python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AES_Python
-Version: 1.5.2
+Version: 1.5.3
 Summary: AES (Advanced Encryption Standard) implementation in Python-3
 Author-email: Gabriel Lindeblad <Gabriel.Lindeblad@icloud.com>
 Project-URL: Homepage, https://github.com/Glindeb/AES-Python
 Project-URL: Repository, https://github.com/Glindeb/AES-Python
 Project-URL: Documentation, https://github.com/Glindeb/AES-Python
 Keywords: AES,AES-Python,Advanced Encryption Standard,encryption,cryptography
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aes_python-1.5.2/tests/test_enc.py` & `aes_python-1.5.3/tests/test_dec.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,44 +2,67 @@
 import numpy as np
 from numpy.typing import NDArray
 from AES_Python import AES
 
 
 @pytest.mark.parametrize("data,key,expected", [
     # 128 bit
-    ("6bc1bee22e409f96e93d7e117393172a", "2b7e151628aed2a6abf7158809cf4f3c", "3ad77bb40d7a3660a89ecaf32466ef97"),
-    ("ae2d8a571e03ac9c9eb76fac45af8e51", "2b7e151628aed2a6abf7158809cf4f3c", "f5d3d58503b9699de785895a96fdbaaf"),
-    ("30c81c46a35ce411e5fbc1191a0a52ef", "2b7e151628aed2a6abf7158809cf4f3c", "43b1cd7f598ece23881b00e3ed030688"),
-    ("f69f2445df4f9b17ad2b417be66c3710", "2b7e151628aed2a6abf7158809cf4f3c", "7b0c785e27e8ad3f8223207104725dd4"),
+    ("3ad77bb40d7a3660a89ecaf32466ef97", "2b7e151628aed2a6abf7158809cf4f3c", "6bc1bee22e409f96e93d7e117393172a"),
+    ("f5d3d58503b9699de785895a96fdbaaf", "2b7e151628aed2a6abf7158809cf4f3c", "ae2d8a571e03ac9c9eb76fac45af8e51"),
+    ("43b1cd7f598ece23881b00e3ed030688", "2b7e151628aed2a6abf7158809cf4f3c", "30c81c46a35ce411e5fbc1191a0a52ef"),
+    ("7b0c785e27e8ad3f8223207104725dd4", "2b7e151628aed2a6abf7158809cf4f3c", "f69f2445df4f9b17ad2b417be66c3710"),
     # 192 bit
-    ("6bc1bee22e409f96e93d7e117393172a", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
-     "bd334f1d6e45f25ff712a214571fa5cc"),
-    ("ae2d8a571e03ac9c9eb76fac45af8e51", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
-     "974104846d0ad3ad7734ecb3ecee4eef"),
-    ("30c81c46a35ce411e5fbc1191a0a52ef", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
-     "ef7afd2270e2e60adce0ba2face6444e"),
-    ("f69f2445df4f9b17ad2b417be66c3710", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
-     "9a4b41ba738d6c72fb16691603c18e0e"),
+    ("bd334f1d6e45f25ff712a214571fa5cc", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
+     "6bc1bee22e409f96e93d7e117393172a"),
+    ("974104846d0ad3ad7734ecb3ecee4eef", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
+     "ae2d8a571e03ac9c9eb76fac45af8e51"),
+    ("ef7afd2270e2e60adce0ba2face6444e", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
+     "30c81c46a35ce411e5fbc1191a0a52ef"),
+    ("9a4b41ba738d6c72fb16691603c18e0e", "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b",
+     "f69f2445df4f9b17ad2b417be66c3710"),
     # 256 bit
-    ("6bc1bee22e409f96e93d7e117393172a", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
-     "f3eed1bdb5d2a03c064b5a7e3db181f8"),
-    ("ae2d8a571e03ac9c9eb76fac45af8e51", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
-     "591ccb10d410ed26dc5ba74a31362870"),
-    ("30c81c46a35ce411e5fbc1191a0a52ef", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
-     "b6ed21b99ca6f4f9f153e7b1beafed1d"),
-    ("f69f2445df4f9b17ad2b417be66c3710", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
-     "23304b7a39f9f3ff067d8d8f9e24ecc7"),
+    ("f3eed1bdb5d2a03c064b5a7e3db181f8", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
+     "6bc1bee22e409f96e93d7e117393172a"),
+    ("591ccb10d410ed26dc5ba74a31362870", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
+     "ae2d8a571e03ac9c9eb76fac45af8e51"),
+    ("b6ed21b99ca6f4f9f153e7b1beafed1d", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
+     "30c81c46a35ce411e5fbc1191a0a52ef"),
+    ("23304b7a39f9f3ff067d8d8f9e24ecc7", "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4",
+     "f69f2445df4f9b17ad2b417be66c3710"),
 ])
-def test_enc_schedule(data, key: str, expected: str) -> None:
+def test_dec_schedule(data, key: str, expected: str) -> None:
     # Formats input data
     data = np.frombuffer(bytes.fromhex(data), dtype=np.uint8).reshape(4, 4)
 
     # Creates round keys
     round_keys: NDArray[np.uint8] = AES.key_expand(key)
 
     # Runs decryption
-    result: NDArray[np.uint8] = AES()._AES__enc_schedule(data, round_keys)  # type: ignore
+    result: NDArray[np.uint8] = AES()._AES__dec_schedule(data, round_keys)  # type: ignore
 
     result_formatted = result.astype(np.uint8).tobytes().hex()
 
     # Evaluates result
     assert result_formatted == expected
+
+
+@pytest.mark.parametrize("data,key,expected", [
+    # 128 bit
+    (b'|\xc2\x94\x18\xc3\x8f\x1c\xc3\xb0\xc3\xaf\xc2\xa0\xc3\xbf\xc2\xa4\xc2\xbb\xc3\xa9\xc3\x98\xc2\x8am\xc2\xa4',
+     "2b7e151628aed2a6abf7158809cf4f3c", '1234567890'),
+    (b'(>\xc2\xa4JH\xc3\x97\x18\xc2\xa2\xc3\x81\xc3\xb7\xc2\xb7\xc3\xa3\xc2\xbbKJ\xc3\xb8',
+     "2b7e151628aed2a6abf7158809cf4f3c", '1234567890123456'),
+    # 192 bit
+    (b'K\xc2\x9d\xc3\xa5\xc3\xa9l8&\xc3\x9alO\xc2\xbb\xc3\x83\xc3\xb2\xc3\x83*\xc3\xb2',
+     "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b", '1234567890'),
+    (b'\xc3\xb9\x01\xc3\x97\xc3\xa8\xc3\x9c\xc3\xb7\\\xc3\x80\xc3\x88\xc2\xa1*>t\xc2\xabA\xc3\x98',
+     "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b", '1234567890123456'),
+    # 256 bit
+    (b'2 ?\xc3\xabm\xc3\xb5o\xc3\x82\xc2\x8b\xc2\x90\xc2\x80\xc2\x84 D\xc3\x84\xc2\x95',
+     "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", '1234567890'),
+    (b"\xc2\x8cc'\xc3\x88d\xc2\x82\xc2\xb3\xc2\x8cj\xc3\x92\\\xc2\xaa\xc2\x96\xc3\xb1\xc3\xbfi",
+     "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", '1234567890123456')
+])
+def test_enc_ecb(data, key, expected):
+    aes = AES(key=key)
+
+    assert aes.dec(data_string=data.decode("utf-8")) == expected
```

### Comparing `aes_python-1.5.2/tests/test_file_dec.py` & `aes_python-1.5.3/tests/test_file_dec.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
      "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b", "tmp4.txt", b'1234567890123456'),
     # 256 bit
     (b'2 ?\xebm\xf5o\xc2\x8b\x90\x80\x84 D\xc4\x95\x89\x18\n\xeb\xac\xde\xa7P>Ei\xbc|\x9c\xfa\xf2',
      "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp5.txt", b'1234567890'),
     (b"\x8cc'\xc8d\x82\xb3\x8cj\xd2\\\xaa\x96\xf1\xffi\xe5h\xf6\x81\x94\xcfv\xd6\x17ML\xc0C\x10\xa8T",
      "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp6.txt", b'1234567890123456')
 ])
-def test_dec_ecb(data, key, file_name, expected):
+def test_file_dec_ecb(data, key, file_name, expected):
     with open(f"{file_name}.enc", "wb") as file:
         file.write(data)
 
     ecb = AES(key=key, running_mode="ECB")
     ecb.dec(file_path=file_name)
 
     with open(file_name, "rb") as file:
@@ -56,15 +56,15 @@
      "8e73b0f7da0e6452c810f32b809079e562f8ead2522c6b7b", "tmp4.txt", "000102030405060708090a0b0c0d0e0f", b'1234567890123456'),
     # 256 bit
     (b'\x9dT\xb7B\x19e\xb8q\xc95\xfa\x80L\x88.9)`\xef\xc2\x10\x9a\x95\x90U\xe0\x0f N\x80\xba\xb3',
      "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp5.txt", "000102030405060708090a0b0c0d0e0f", b'1234567890'),
     (b'a\xfdIRQ\xf8\xf1D\xcc\xbf\x89\xc8\xd6\xec\x01;pNAT\xedT\xd9Tp-_\xbbr\xd3\xb5\x11',
      "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp6.txt", "000102030405060708090a0b0c0d0e0f", b'1234567890123456')
 ])
-def test_dec_cbc(data, key, file_name, iv, expected):
+def test_file_dec_cbc(data, key, file_name, iv, expected):
     with open(f"{file_name}.enc", "wb") as file:
         file.write(data)
 
     cbc = AES(key=key, running_mode="CBC")
     cbc.dec(file_path=file_name)
 
     with open(file_name, "rb") as file:
```

### Comparing `aes_python-1.5.2/tests/test_file_enc.py` & `aes_python-1.5.3/tests/test_file_enc.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
      b'\xf9\x01\xd7\xe8\xdc\xf7\\\xc0\xc8\xa1*>t\xabA\xd8"E-\x8eI\xa8\xa5\x93\x9fs!\xce\xeamQK'),
     # 256 bit
     (b'1234567890', "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp4.txt",
      b'2 ?\xebm\xf5o\xc2\x8b\x90\x80\x84 D\xc4\x95\x89\x18\n\xeb\xac\xde\xa7P>Ei\xbc|\x9c\xfa\xf2'),
     (b'1234567890123456', "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp5.txt",
      b"\x8cc'\xc8d\x82\xb3\x8cj\xd2\\\xaa\x96\xf1\xffi\xe5h\xf6\x81\x94\xcfv\xd6\x17ML\xc0C\x10\xa8T")
 ])
-def test_enc_ecb(data, key, file_name, expected):
+def test_file_enc_ecb(data, key, file_name, expected):
     with open(file_name, "wb") as file:
         file.write(data)
 
     ecb = AES(key=key, running_mode="ECB")
     ecb.enc(file_path=file_name)
 
     with open(f"{file_name}.enc", "rb") as file:
@@ -56,15 +56,15 @@
     (b'1234567890', "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp4.txt",
      "000102030405060708090a0b0c0d0e0f",
      b'\x9dT\xb7B\x19e\xb8q\xc95\xfa\x80L\x88.9)`\xef\xc2\x10\x9a\x95\x90U\xe0\x0f N\x80\xba\xb3'),
     (b'1234567890123456', "603deb1015ca71be2b73aef0857d77811f352c073b6108d72d9810a30914dff4", "tmp5.txt",
      "000102030405060708090a0b0c0d0e0f",
      b'a\xfdIRQ\xf8\xf1D\xcc\xbf\x89\xc8\xd6\xec\x01;pNAT\xedT\xd9Tp-_\xbbr\xd3\xb5\x11')
 ])
-def test_enc_cbc(data, key, file_name, iv, expected):
+def test_file_enc_cbc(data, key, file_name, iv, expected):
     with open(file_name, "wb") as file:
         file.write(data)
 
     cbc = AES(key=key, running_mode="CBC", iv=iv)
     cbc.enc(file_path=file_name)
 
     with open(f"{file_name}.enc", "rb") as file:
```

### Comparing `aes_python-1.5.2/tests/test_key_expansion.py` & `aes_python-1.5.3/tests/test_key_expansion.py`

 * *Files identical despite different names*

### Comparing `aes_python-1.5.2/tests/test_methods.py` & `aes_python-1.5.3/tests/test_methods.py`

 * *Files identical despite different names*


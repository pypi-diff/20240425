# Comparing `tmp/cefi-4.6.7.tar.gz` & `tmp/cefi-4.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.6.7.tar", max compression
+gzip compressed data, was "cefi-4.6.8.tar", max compression
```

## Comparing `cefi-4.6.7.tar` & `cefi-4.6.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-24 04:10:13.202661 cefi-4.6.7/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-24 04:10:13.202661 cefi-4.6.7/README.md
--rw-r--r--   0        0        0       87 2024-04-24 04:10:51.870606 cefi-4.6.7/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/__init__.py
--rw-r--r--   0        0        0    11153 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9015 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8160 2024-04-24 04:10:13.202661 cefi-4.6.7/cefi/main.py
--rw-r--r--   0        0        0     3776 2024-04-24 04:10:51.870606 cefi-4.6.7/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-25 11:29:12.616399 cefi-4.6.8/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-25 11:29:12.616399 cefi-4.6.8/README.md
+-rw-r--r--   0        0        0       87 2024-04-25 11:29:51.880327 cefi-4.6.8/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    11153 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9015 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8160 2024-04-25 11:29:12.616399 cefi-4.6.8/cefi/main.py
+-rw-r--r--   0        0        0     3778 2024-04-25 11:29:51.880327 cefi-4.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.8/PKG-INFO
```

### Comparing `cefi-4.6.7/LICENSE` & `cefi-4.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/README.md` & `cefi-4.6.8/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/default_settings.toml` & `cefi-4.6.8/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/handler/capitalcom.py` & `cefi-4.6.8/cefi/handler/capitalcom.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/handler/ccxt.py` & `cefi-4.6.8/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/handler/client.py` & `cefi-4.6.8/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/handler/ctrader.py` & `cefi-4.6.8/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/handler/ib_sync.py` & `cefi-4.6.8/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/cefi/main.py` & `cefi-4.6.8/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.7/pyproject.toml` & `cefi-4.6.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.6.7"
+version = "4.6.8"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -29,15 +29,15 @@
 ccxt = "^4.2.80"
 ib_insync = "0.9.86"
 capitalcom-python = "0.2.3"
 
 [ tool.poetry.group.dev.dependencies]
 python-semantic-release = ">=8.0.8"
 ruff = "^0.4.0"
-black = "24.4.0"
+black = "24.4.1"
 pre-commit = "^3.3.1"
 
 [tool.ruff]
 exclude = [
   ".github/*",
   "docs/*",
 ]
@@ -166,27 +166,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.6.7/PKG-INFO` & `cefi-4.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.6.7
+Version: 4.6.8
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.6.7 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.6.8 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```


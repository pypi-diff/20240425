# Comparing `tmp/bedrock_bot-1.2.2.tar.gz` & `tmp/bedrock_bot-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.2.2.tar", max compression
+gzip compressed data, was "bedrock_bot-1.2.3.tar", max compression
```

## Comparing `bedrock_bot-1.2.2.tar` & `bedrock_bot-1.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/README.md
--rw-r--r--   0        0        0      120 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     4018 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/cli.py
--rw-r--r--   0        0        0      143 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/__init__.py
--rw-r--r--   0        0        0     2146 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/base_model.py
--rw-r--r--   0        0        0     1476 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/claude.py
--rw-r--r--   0        0        0     1149 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/models/mistral.py
--rw-r--r--   0        0        0      175 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/bedrock_bot/util.py
--rw-r--r--   0        0        0      470 2024-04-25 06:16:52.279923 bedrock_bot-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-25 06:21:57.072927 bedrock_bot-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-25 06:21:57.072927 bedrock_bot-1.2.3/README.md
+-rw-r--r--   0        0        0      120 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     4018 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/cli.py
+-rw-r--r--   0        0        0      143 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/models/__init__.py
+-rw-r--r--   0        0        0     2146 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/models/base_model.py
+-rw-r--r--   0        0        0     1476 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/models/claude.py
+-rw-r--r--   0        0        0     1149 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/models/mistral.py
+-rw-r--r--   0        0        0      175 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/bedrock_bot/util.py
+-rw-r--r--   0        0        0      470 2024-04-25 06:21:57.076927 bedrock_bot-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.2.3/PKG-INFO
```

### Comparing `bedrock_bot-1.2.2/LICENSE` & `bedrock_bot-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.2/README.md` & `bedrock_bot-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.2/bedrock_bot/cli.py` & `bedrock_bot-1.2.3/bedrock_bot/cli.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.2/bedrock_bot/models/base_model.py` & `bedrock_bot-1.2.3/bedrock_bot/models/base_model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.2/bedrock_bot/models/claude.py` & `bedrock_bot-1.2.3/bedrock_bot/models/claude.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.2/bedrock_bot/models/mistral.py` & `bedrock_bot-1.2.3/bedrock_bot/models/mistral.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.2.2/PKG-INFO` & `bedrock_bot-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.2.2
+Version: 1.2.3
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


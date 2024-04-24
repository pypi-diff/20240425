# Comparing `tmp/langchain_upstage-0.1.0rc0.tar.gz` & `tmp/langchain_upstage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.0rc0.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.1.tar", max compression
```

## Comparing `langchain_upstage-0.1.0rc0.tar` & `langchain_upstage-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0      979 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/README.md
--rw-r--r--   0        0        0      161 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9097 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/langchain_upstage/py.typed
--rw-r--r--   0        0        0     2661 2024-04-17 23:34:06.806451 langchain_upstage-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 langchain_upstage-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/LICENSE
+-rw-r--r--   0        0        0      979 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/README.md
+-rw-r--r--   0        0        0      496 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9097 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0     6430 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/layout_analysis.py
+-rw-r--r--   0        0        0    12390 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/layout_analysis_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     3328 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/langchain_upstage/tools/groundedness_check.py
+-rw-r--r--   0        0        0     2727 2024-04-24 22:19:03.820376 langchain_upstage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.1/PKG-INFO
```

### Comparing `langchain_upstage-0.1.0rc0/LICENSE` & `langchain_upstage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0rc0/README.md` & `langchain_upstage-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0rc0/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.1/langchain_upstage/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0rc0/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.1/langchain_upstage/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.0rc0/pyproject.toml` & `langchain_upstage-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "langchain-upstage"
-version = "0.1.0rc0"
+version = "0.1.1"
 description = "An integration package connecting Upstage and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/upstage"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.44"
 langchain-openai = "^0.1.3"
+pymupdf = "^1.24.1"
+requests = "^2.31.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
@@ -46,14 +48,15 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
+types-requests = ">=2.31.0"
 langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
```

### Comparing `langchain_upstage-0.1.0rc0/PKG-INFO` & `langchain_upstage-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.0rc0
+Version: 0.1.1
 Summary: An integration package connecting Upstage and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1.44,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
+Requires-Dist: pymupdf (>=1.24.1,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/upstage
 Description-Content-Type: text/markdown
 
 # langchain-upstage
 
 This package contains the LangChain integrations for [Upstage](https://upstage.ai) through their [APIs](https://developers.upstage.ai/docs/getting-started/models).
```


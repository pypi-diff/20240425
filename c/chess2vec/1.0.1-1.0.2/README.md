# Comparing `tmp/chess2vec-1.0.1.tar.gz` & `tmp/chess2vec-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-1.0.1.tar", max compression
+gzip compressed data, was "chess2vec-1.0.2.tar", max compression
```

## Comparing `chess2vec-1.0.1.tar` & `chess2vec-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-25 07:29:21.231350 chess2vec-1.0.1/README.md
--rw-r--r--   0        0        0     1014 2024-04-25 09:51:13.652560 chess2vec-1.0.1/chess2vec/__init__.py
--rw-r--r--   0        0        0      582 2024-04-25 09:51:13.749229 chess2vec-1.0.1/chess2vec/pgn.py
--rw-r--r--   0        0        0     1415 2024-04-25 09:51:13.752562 chess2vec-1.0.1/chess2vec/utils.py
--rw-r--r--   0        0        0      374 2024-04-25 09:53:04.504727 chess2vec-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 chess2vec-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 07:29:21.231350 chess2vec-1.0.2/README.md
+-rw-r--r--   0        0        0     1014 2024-04-25 09:51:13.652560 chess2vec-1.0.2/chess2vec/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-25 09:51:13.749229 chess2vec-1.0.2/chess2vec/pgn.py
+-rw-r--r--   0        0        0     1415 2024-04-25 09:51:13.752562 chess2vec-1.0.2/chess2vec/utils.py
+-rw-r--r--   0        0        0      356 2024-04-25 09:53:32.691942 chess2vec-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 chess2vec-1.0.2/PKG-INFO
```

### Comparing `chess2vec-1.0.1/chess2vec/__init__.py` & `chess2vec-1.0.2/chess2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-1.0.1/chess2vec/pgn.py` & `chess2vec-1.0.2/chess2vec/pgn.py`

 * *Files identical despite different names*

### Comparing `chess2vec-1.0.1/chess2vec/utils.py` & `chess2vec-1.0.2/chess2vec/utils.py`

 * *Files identical despite different names*

### Comparing `chess2vec-1.0.1/PKG-INFO` & `chess2vec-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chess (>=1.10.0,<2.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
-Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```


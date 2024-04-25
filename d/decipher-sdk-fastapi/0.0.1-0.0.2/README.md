# Comparing `tmp/decipher_sdk_fastapi-0.0.1.tar.gz` & `tmp/decipher_sdk_fastapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decipher_sdk_fastapi-0.0.1.tar", last modified: Thu Apr 25 00:31:09 2024, max compression
+gzip compressed data, was "decipher_sdk_fastapi-0.0.2.tar", last modified: Thu Apr 25 19:53:23 2024, max compression
```

## Comparing `decipher_sdk_fastapi-0.0.1.tar` & `decipher_sdk_fastapi-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 00:31:08.998938 decipher_sdk_fastapi-0.0.1/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      369 2024-04-25 00:31:08.998801 decipher_sdk_fastapi-0.0.1/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      128 2024-04-14 18:27:12.000000 decipher_sdk_fastapi-0.0.1/README.md
--rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-04-25 00:31:08.999031 decipher_sdk_fastapi-0.0.1/setup.cfg
--rw-r--r--   0 mrosenfield   (501) staff       (20)      509 2024-04-25 00:30:57.000000 decipher_sdk_fastapi-0.0.1/setup.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 00:31:08.995078 decipher_sdk_fastapi-0.0.1/src/
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 00:31:08.997388 decipher_sdk_fastapi-0.0.1/src/decipher_sdk/
--rw-r--r--   0 mrosenfield   (501) staff       (20)       45 2024-04-14 18:23:34.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk/__init__.py
--rw-r--r--   0 mrosenfield   (501) staff       (20)     8205 2024-04-25 00:23:56.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk/decipher_sdk.py
-drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 00:31:08.998529 decipher_sdk_fastapi-0.0.1/src/decipher_sdk_fastapi.egg-info/
--rw-r--r--   0 mrosenfield   (501) staff       (20)      369 2024-04-25 00:31:08.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 mrosenfield   (501) staff       (20)      319 2024-04-25 00:31:08.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-04-25 00:31:08.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       17 2024-04-25 00:31:08.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk_fastapi.egg-info/requires.txt
--rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-04-25 00:31:08.000000 decipher_sdk_fastapi-0.0.1/src/decipher_sdk_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:53:23.555048 decipher_sdk_fastapi-0.0.2/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      369 2024-04-25 19:53:23.554938 decipher_sdk_fastapi-0.0.2/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      128 2024-04-14 18:27:12.000000 decipher_sdk_fastapi-0.0.2/README.md
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       38 2024-04-25 19:53:23.555089 decipher_sdk_fastapi-0.0.2/setup.cfg
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      509 2024-04-25 19:53:17.000000 decipher_sdk_fastapi-0.0.2/setup.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:53:23.553124 decipher_sdk_fastapi-0.0.2/src/
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:53:23.553918 decipher_sdk_fastapi-0.0.2/src/decipher_sdk/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       45 2024-04-14 18:23:34.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk/__init__.py
+-rw-r--r--   0 mrosenfield   (501) staff       (20)     8205 2024-04-25 00:42:11.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk/decipher_sdk.py
+drwxr-xr-x   0 mrosenfield   (501) staff       (20)        0 2024-04-25 19:53:23.554784 decipher_sdk_fastapi-0.0.2/src/decipher_sdk_fastapi.egg-info/
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      369 2024-04-25 19:53:23.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 mrosenfield   (501) staff       (20)      319 2024-04-25 19:53:23.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)        1 2024-04-25 19:53:23.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       17 2024-04-25 19:53:23.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk_fastapi.egg-info/requires.txt
+-rw-r--r--   0 mrosenfield   (501) staff       (20)       13 2024-04-25 19:53:23.000000 decipher_sdk_fastapi-0.0.2/src/decipher_sdk_fastapi.egg-info/top_level.txt
```

### Comparing `decipher_sdk_fastapi-0.0.1/src/decipher_sdk/decipher_sdk.py` & `decipher_sdk_fastapi-0.0.2/src/decipher_sdk/decipher_sdk.py`

 * *Files identical despite different names*


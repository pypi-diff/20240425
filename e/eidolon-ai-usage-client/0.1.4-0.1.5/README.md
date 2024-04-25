# Comparing `tmp/eidolon_ai_usage_client-0.1.4.tar.gz` & `tmp/eidolon_ai_usage_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_usage_client-0.1.4.tar", max compression
+gzip compressed data, was "eidolon_ai_usage_client-0.1.5.tar", max compression
```

## Comparing `eidolon_ai_usage_client-0.1.4.tar` & `eidolon_ai_usage_client-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-25 15:57:51.723375 eidolon_ai_usage_client-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-25 15:57:51.723375 eidolon_ai_usage_client-0.1.4/eidolon_ai_usage_client/__init__.py
--rw-r--r--   0        0        0     1723 2024-04-25 15:57:51.723375 eidolon_ai_usage_client-0.1.4/eidolon_ai_usage_client/client.py
--rw-r--r--   0        0        0      460 2024-04-25 15:57:51.723375 eidolon_ai_usage_client-0.1.4/eidolon_ai_usage_client/models.py
--rw-r--r--   0        0        0      501 2024-04-25 15:58:54.659883 eidolon_ai_usage_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 eidolon_ai_usage_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 16:01:55.314192 eidolon_ai_usage_client-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 16:01:55.314192 eidolon_ai_usage_client-0.1.5/eidolon_ai_usage_client/__init__.py
+-rw-r--r--   0        0        0     1723 2024-04-25 16:01:55.314192 eidolon_ai_usage_client-0.1.5/eidolon_ai_usage_client/client.py
+-rw-r--r--   0        0        0      460 2024-04-25 16:01:55.314192 eidolon_ai_usage_client-0.1.5/eidolon_ai_usage_client/models.py
+-rw-r--r--   0        0        0      501 2024-04-25 16:03:08.610720 eidolon_ai_usage_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 eidolon_ai_usage_client-0.1.5/PKG-INFO
```

### Comparing `eidolon_ai_usage_client-0.1.4/eidolon_ai_usage_client/client.py` & `eidolon_ai_usage_client-0.1.5/eidolon_ai_usage_client/client.py`

 * *Files identical despite different names*


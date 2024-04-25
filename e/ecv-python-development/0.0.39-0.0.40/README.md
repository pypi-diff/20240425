# Comparing `tmp/ecv-python-development-0.0.39.tar.gz` & `tmp/ecv-python-development-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecv-python-development-0.0.39.tar", last modified: Thu Apr 25 06:29:40 2024, max compression
+gzip compressed data, was "ecv-python-development-0.0.40.tar", last modified: Thu Apr 25 06:42:22 2024, max compression
```

## Comparing `ecv-python-development-0.0.39.tar` & `ecv-python-development-0.0.40.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/LICENSE
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/MANIFEST.in
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/README.md
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/events_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/events_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/events_module/base.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/handler.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/logger.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/response.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3536 2024-04-25 06:28:50.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/validator.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/aws_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/cognito_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/kms_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/lambda_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/s3_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/ses_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/sns_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/sqs_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/ssm_service.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/database/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.39/ecv_python_development/database/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/database/_pynamodb/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.39/ecv_python_development/database/_pynamodb/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.39/ecv_python_development/database/_pynamodb/base.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5748 2024-04-24 16:48:01.000000 ecv-python-development-0.0.39/ecv_python_development/database/base_model.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/database/py.typed
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1196 2024-04-24 12:18:58.000000 ecv-python-development-0.0.39/ecv_python_development/database/test.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/helpers/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/helpers/datetime/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/datetime/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/datetime/standard.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development/helpers/debugger/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/debugger/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1835 2024-04-24 18:23:53.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/debugger/debugging.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/ecv_python_development/helpers/files/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/files/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/files/file.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/ecv_python_development/helpers/formatter/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/formatter/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/formatter/formatter.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/formatter/regex.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/ecv_python_development/helpers/http/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/http/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/http/requests.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/ecv_python_development/helpers/strings/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/strings/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/strings/passwords.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/helpers/strings/uuid.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.39/ecv_python_development/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:29:40.042140 ecv-python-development-0.0.39/ecv_python_development.egg-info/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 06:29:39.000000 ecv-python-development-0.0.39/ecv_python_development.egg-info/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-25 06:29:39.000000 ecv-python-development-0.0.39/ecv_python_development.egg-info/SOURCES.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-25 06:29:39.000000 ecv-python-development-0.0.39/ecv_python_development.egg-info/dependency_links.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-25 06:29:39.000000 ecv-python-development-0.0.39/ecv_python_development.egg-info/requires.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-25 06:29:39.000000 ecv-python-development-0.0.39/ecv_python_development.egg-info/top_level.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-25 06:29:40.052140 ecv-python-development-0.0.39/setup.cfg
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-25 06:29:36.000000 ecv-python-development-0.0.39/setup.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/LICENSE
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/MANIFEST.in
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/README.md
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.772094 ecv-python-development-0.0.40/ecv_python_development/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.772094 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.772094 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/events_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/events_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/events_module/base.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.772094 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/handler.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/logger.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/response.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3630 2024-04-25 06:41:56.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/validator.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/aws_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/cognito_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/kms_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/lambda_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/s3_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/ses_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/sns_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/sqs_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/ssm_service.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/database/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.40/ecv_python_development/database/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/database/_pynamodb/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.40/ecv_python_development/database/_pynamodb/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.40/ecv_python_development/database/_pynamodb/base.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5748 2024-04-24 16:48:01.000000 ecv-python-development-0.0.40/ecv_python_development/database/base_model.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/database/py.typed
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1196 2024-04-24 12:18:58.000000 ecv-python-development-0.0.40/ecv_python_development/database/test.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/datetime/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/datetime/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/datetime/standard.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/debugger/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/debugger/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1835 2024-04-24 18:23:53.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/debugger/debugging.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/files/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/files/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/files/file.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/formatter/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/formatter/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/formatter/formatter.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/formatter/regex.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/http/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/http/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/http/requests.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/ecv_python_development/helpers/strings/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/strings/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/strings/passwords.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/helpers/strings/uuid.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.40/ecv_python_development/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 06:42:22.772094 ecv-python-development-0.0.40/ecv_python_development.egg-info/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 06:42:22.000000 ecv-python-development-0.0.40/ecv_python_development.egg-info/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-25 06:42:22.000000 ecv-python-development-0.0.40/ecv_python_development.egg-info/SOURCES.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-25 06:42:22.000000 ecv-python-development-0.0.40/ecv_python_development.egg-info/dependency_links.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-25 06:42:22.000000 ecv-python-development-0.0.40/ecv_python_development.egg-info/requires.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-25 06:42:22.000000 ecv-python-development-0.0.40/ecv_python_development.egg-info/top_level.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-25 06:42:22.782094 ecv-python-development-0.0.40/setup.cfg
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-25 06:42:21.000000 ecv-python-development-0.0.40/setup.py
```

### Comparing `ecv-python-development-0.0.39/LICENSE` & `ecv-python-development-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/PKG-INFO` & `ecv-python-development-0.0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.39
+Version: 0.0.40
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/events_module/base.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/events_module/base.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/__init__.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/handler.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/handler.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/response.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/response.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/lambda_module/validator.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/lambda_module/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,17 @@
     if event["queryStringParameters"]:
         body = {**body, **event["queryStringParameters"]}
     if event["pathParameters"]:
         body = {**body, **event["pathParameters"]}
 
     log("UNVALIDATED_BODY", data=body)
     result = _validate_data(body, model_class=model)
-    log("VALIDATION_RESULT", data=result)
 
     if not isinstance(result, BaseModel):
-        return {
+        request_validation_exception_response = {
             "body": json.dumps(
                 {
                     "error": {
                         "code": RequestValidationException.ERROR_CODE,
                         "message": RequestValidationException.ERROR_MESSAGE,
                         "error_details": _construct_validation_error_message(result),
                     }
@@ -69,14 +68,17 @@
                 "Content-Type": "application/json",
                 "Access-Control-Allow-Origin": "*",
                 "Access-Control-Allow-Header": "*",
             },
             "status_code": RequestValidationException.STATUS_CODE,
         }
 
+        log("REQUEST_VALIDATION_EXCEPTION", data=request_validation_exception_response)
+        return
+
     app.validated_body = result.model_dump()
 
     response = handler(event, context)
     print("LAMBDA_HANDLER_RESPONSE: ", response)
 
     return response
 
@@ -97,15 +99,15 @@
         validated_data = model_class.model_validate(data)
         return validated_data
     except ValidationError as e:
         errors: dict[Any, Any] = {}
         for error in e.errors():
             errors[error["loc"][0]] = error["msg"]
 
-        log("VALIDATION ERRORS", data=errors)
+        print("VALIDATION_ERRORS: ", errors)
         return errors
 
 
 def _construct_validation_error_message(
     validated_data: dict[Any, Any]
 ) -> list[dict[str, Any]]:
     error_message_list: list[dict[Any, Any]] = []
```

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/aws_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/aws_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/cognito_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/cognito_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/dynamodb_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/eventbridge_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/kms_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/kms_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/lambda_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/s3_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/s3_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/ses_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/ses_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/sns_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/sns_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/sqs_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/aws_cloud_native/services/ssm_service.py` & `ecv-python-development-0.0.40/ecv_python_development/aws_cloud_native/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/database/base_model.py` & `ecv-python-development-0.0.40/ecv_python_development/database/base_model.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/database/test.py` & `ecv-python-development-0.0.40/ecv_python_development/database/test.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/helpers/datetime/standard.py` & `ecv-python-development-0.0.40/ecv_python_development/helpers/datetime/standard.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/helpers/debugger/debugging.py` & `ecv-python-development-0.0.40/ecv_python_development/helpers/debugger/debugging.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/helpers/formatter/__init__.py` & `ecv-python-development-0.0.40/ecv_python_development/helpers/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/helpers/formatter/formatter.py` & `ecv-python-development-0.0.40/ecv_python_development/helpers/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/helpers/http/requests.py` & `ecv-python-development-0.0.40/ecv_python_development/helpers/http/requests.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development/helpers/strings/passwords.py` & `ecv-python-development-0.0.40/ecv_python_development/helpers/strings/passwords.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development.egg-info/PKG-INFO` & `ecv-python-development-0.0.40/ecv_python_development.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.39
+Version: 0.0.40
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `ecv-python-development-0.0.39/ecv_python_development.egg-info/SOURCES.txt` & `ecv-python-development-0.0.40/ecv_python_development.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/ecv_python_development.egg-info/requires.txt` & `ecv-python-development-0.0.40/ecv_python_development.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.39/setup.py` & `ecv-python-development-0.0.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="ecv-python-development",
-    version="0.0.39",
+    version="0.0.40",
     author="Warren Ezra Bruce Jaudian",
     author_email="warren.jaudian@ecloudvalley.com",
     packages=find_packages(),
     description="ECV Python Development Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development",
```


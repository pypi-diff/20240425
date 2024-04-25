# Comparing `tmp/ecv-python-development-0.0.50.tar.gz` & `tmp/ecv-python-development-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecv-python-development-0.0.50.tar", last modified: Thu Apr 25 14:36:45 2024, max compression
+gzip compressed data, was "ecv-python-development-0.0.51.tar", last modified: Thu Apr 25 17:28:59 2024, max compression
```

## Comparing `ecv-python-development-0.0.50.tar` & `ecv-python-development-0.0.51.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/LICENSE
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/MANIFEST.in
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/README.md
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.180357 ecv-python-development-0.0.50/ecv_python_development/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.180357 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.180357 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/events_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/events_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/events_module/base.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.190357 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/handler.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/logger.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/response.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3907 2024-04-25 14:36:02.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/validator.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.190357 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/aws_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/cognito_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/kms_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/lambda_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/s3_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/ses_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/sns_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/sqs_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/ssm_service.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.190357 ecv-python-development-0.0.50/ecv_python_development/database/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.50/ecv_python_development/database/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.190357 ecv-python-development-0.0.50/ecv_python_development/database/_pynamodb/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.50/ecv_python_development/database/_pynamodb/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.50/ecv_python_development/database/_pynamodb/base.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5300 2024-04-25 14:35:08.000000 ecv-python-development-0.0.50/ecv_python_development/database/base_model.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/database/py.typed
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1714 2024-04-25 14:35:24.000000 ecv-python-development-0.0.50/ecv_python_development/database/test.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.190357 ecv-python-development-0.0.50/ecv_python_development/helpers/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/ecv_python_development/helpers/datetime/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/datetime/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/datetime/standard.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/ecv_python_development/helpers/debugger/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/debugger/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1835 2024-04-24 18:23:53.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/debugger/debugging.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/ecv_python_development/helpers/files/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/files/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/files/file.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/ecv_python_development/helpers/formatter/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/formatter/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/formatter/formatter.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/formatter/regex.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/ecv_python_development/helpers/http/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/http/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/http/requests.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/ecv_python_development/helpers/strings/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/strings/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/strings/passwords.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/helpers/strings/uuid.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.50/ecv_python_development/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 14:36:45.180357 ecv-python-development-0.0.50/ecv_python_development.egg-info/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 14:36:44.000000 ecv-python-development-0.0.50/ecv_python_development.egg-info/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-25 14:36:44.000000 ecv-python-development-0.0.50/ecv_python_development.egg-info/SOURCES.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-25 14:36:44.000000 ecv-python-development-0.0.50/ecv_python_development.egg-info/dependency_links.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-25 14:36:44.000000 ecv-python-development-0.0.50/ecv_python_development.egg-info/requires.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-25 14:36:44.000000 ecv-python-development-0.0.50/ecv_python_development.egg-info/top_level.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-25 14:36:45.200357 ecv-python-development-0.0.50/setup.cfg
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-25 14:36:12.000000 ecv-python-development-0.0.50/setup.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.379727 ecv-python-development-0.0.51/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/LICENSE
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/MANIFEST.in
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 17:28:59.379727 ecv-python-development-0.0.51/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/README.md
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.359727 ecv-python-development-0.0.51/ecv_python_development/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.359727 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.359727 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/events_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/events_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/events_module/base.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.359727 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/handler.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/logger.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/response.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3894 2024-04-25 17:21:52.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/validator.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/aws_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/cognito_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/kms_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/lambda_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/s3_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/ses_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/sns_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/sqs_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/ssm_service.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/database/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.51/ecv_python_development/database/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/database/_pynamodb/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.51/ecv_python_development/database/_pynamodb/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.51/ecv_python_development/database/_pynamodb/base.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5645 2024-04-25 17:25:56.000000 ecv-python-development-0.0.51/ecv_python_development/database/base_model.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/database/py.typed
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1664 2024-04-25 17:28:13.000000 ecv-python-development-0.0.51/ecv_python_development/database/test.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/helpers/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/helpers/datetime/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/datetime/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/datetime/standard.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/helpers/debugger/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/debugger/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1835 2024-04-24 18:23:53.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/debugger/debugging.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/helpers/files/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/files/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/files/file.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.369727 ecv-python-development-0.0.51/ecv_python_development/helpers/formatter/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/formatter/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/formatter/formatter.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/formatter/regex.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.379727 ecv-python-development-0.0.51/ecv_python_development/helpers/http/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/http/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/http/requests.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.379727 ecv-python-development-0.0.51/ecv_python_development/helpers/strings/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/strings/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/strings/passwords.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/helpers/strings/uuid.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.51/ecv_python_development/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-25 17:28:59.359727 ecv-python-development-0.0.51/ecv_python_development.egg-info/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-25 17:28:59.000000 ecv-python-development-0.0.51/ecv_python_development.egg-info/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-25 17:28:59.000000 ecv-python-development-0.0.51/ecv_python_development.egg-info/SOURCES.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-25 17:28:59.000000 ecv-python-development-0.0.51/ecv_python_development.egg-info/dependency_links.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-25 17:28:59.000000 ecv-python-development-0.0.51/ecv_python_development.egg-info/requires.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-25 17:28:59.000000 ecv-python-development-0.0.51/ecv_python_development.egg-info/top_level.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-25 17:28:59.379727 ecv-python-development-0.0.51/setup.cfg
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-25 17:28:54.000000 ecv-python-development-0.0.51/setup.py
```

### Comparing `ecv-python-development-0.0.50/LICENSE` & `ecv-python-development-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/PKG-INFO` & `ecv-python-development-0.0.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.50
+Version: 0.0.51
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/events_module/base.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/events_module/base.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/__init__.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/handler.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/handler.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/response.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/response.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/lambda_module/validator.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/lambda_module/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         print(
             "REQUEST_VALIDATION_EXCEPTION_RESPONSE: ",
             request_validation_exception_response,
         )
         return request_validation_exception_response
 
-    app.validated_body = result.model_dump(by_alias=True)
+    app.validated_body = result.model_dump()
 
     response = handler(event, context)
     print("LAMBDA_HANDLER_RESPONSE: ", response)
 
     return response
```

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/aws_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/aws_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/cognito_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/cognito_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/dynamodb_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/eventbridge_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/kms_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/kms_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/lambda_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/s3_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/s3_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/ses_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/ses_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/sns_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/sns_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/sqs_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/aws_cloud_native/services/ssm_service.py` & `ecv-python-development-0.0.51/ecv_python_development/aws_cloud_native/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/database/base_model.py` & `ecv-python-development-0.0.51/ecv_python_development/database/base_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 from __future__ import annotations
 
 import os
 from typing import Any, Callable, ClassVar, List, Literal, Optional, Pattern
 
+from _pynamodb.base import (
+    PYDANTIC_PYNAMO_MAPPING,
+    PynamoDBBaseModel,
+    PynamoDBModel,
+    UnicodeAttribute,
+)
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import (
     Field,
     PrivateAttr,
     StrictBool,
     StrictFloat,
     StrictInt,
     StrictStr,
     create_model,
 )
 
-from ._pynamodb.base import (
-    PYDANTIC_PYNAMO_MAPPING,
-    PynamoDBBaseModel,
-    PynamoDBModel,
-    UnicodeAttribute,
-)
-
 """
 check full documentation for fields at: https://docs.pydantic.dev/latest/concepts/fields/
 
 """
 
 
 def field(
     default: Optional[str] = None,
     default_factory: Optional[Callable[..., Any]] = None,
-    alias: Optional[str] = None,
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
     gt: Optional[float] = None,
     ge: Optional[float] = None,
     lt: Optional[float] = None,
     le: Optional[float] = None,
     title: Optional[str] = None,
     description: Optional[str] = None,
-    validation_alias: Optional[str] = None,
-    serialization_alias: Optional[str] = None,
     examples: Optional[List[Any]] = None,
     frozen: Optional[bool] = False,
     exclude: Optional[bool] = False,
     pattern: Optional[Pattern[str]] = None,
+    db_field: Optional[str] = None,
     is_hash_key: Optional[bool] = False,
     is_range_key: Optional[bool] = False,
     metadata: Optional[dict] = None,
 ) -> Any:
 
     json_extra_schema = {}
 
+    if db_field is not None:
+        json_extra_schema["db_field"] = db_field
+
     if is_hash_key == True:
         json_extra_schema["__hash_key__"] = True
     elif is_range_key == True:
         json_extra_schema["__range_key__"] = True
 
     if metadata is not None:
         json_extra_schema = {**json_extra_schema, **metadata}
 
     parameters = {
         key: value
         for key, value in locals().items()
         if value is not None
-        and key not in ["parameters", "is_hash_key", "is_range_key"]
+        and key not in ["parameters", "is_hash_key", "is_range_key", "db_field"]
     }
 
     """
     These are the parameters I find to be extremely useful.
     
     I limited the parameters to this for easier readability. 
     
@@ -113,25 +113,33 @@
             raise Exception("Other database not yet supported")
 
     @classmethod
     def set_pynamodb_model(cls, table_name: str):
         attributes: dict = {}
 
         for field_name, field_info in cls.model_fields.items():
-
             metadata = field_info.json_schema_extra["json_extra_schema"]
             if "__hash_key__" in metadata or "__range_key__" in metadata:
                 if metadata.get("__hash_key__", False):
-                    attributes[field_name] = UnicodeAttribute(hash_key=True)
+                    attributes[field_name] = UnicodeAttribute(
+                        hash_key=True,
+                        attr_name=metadata.get("db_field", field_name),
+                    )
                 else:
-                    attributes[field_name] = UnicodeAttribute(range_key=True)
+                    attributes[field_name] = UnicodeAttribute(
+                        range_key=True,
+                        attr_name=metadata.get("db_field", field_name),
+                    )
             else:
                 attributes[field_name] = PYDANTIC_PYNAMO_MAPPING.get(
                     field_info.annotation, UnicodeAttribute
-                )(null=field_info.exclude)
+                )(
+                    null=field_info.exclude,
+                    attr_name=metadata.get("db_field", field_name),
+                )
 
         model_name = f"{cls.__name__}PynamoDBModel"
         PynamoDBModel = type(model_name, (PynamoDBBaseModel,), attributes)
         PynamoDBModel.Meta.table_name = table_name
 
         cls.database_model = PynamoDBModel
```

### Comparing `ecv-python-development-0.0.50/ecv_python_development/database/test.py` & `ecv-python-development-0.0.51/ecv_python_development/database/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from base_model import BaseModel, field
 
 
 class UserModel(BaseModel):
-    username: str = field(min_length=1, is_hash_key=True)
+    username: str = field(min_length=1, is_hash_key=True, db_field="PK")
     email: str = field(min_length=1, is_range_key=True)
     datetime: str = field(pattern=r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
-    test_frozen: str = field(default="", alias="test_frozen", frozen=True)
-    new_field: str = field(validation_alias="check", serialization_alias="serial")
+    test_frozen: str = field(default="", frozen=True)
+    check: str = field(db_field="NAH")
     updated_by: str = field(exclude=True)
 
 
 class TestExclude(BaseModel):
     test_exclude: str
```

### Comparing `ecv-python-development-0.0.50/ecv_python_development/helpers/datetime/standard.py` & `ecv-python-development-0.0.51/ecv_python_development/helpers/datetime/standard.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/helpers/debugger/debugging.py` & `ecv-python-development-0.0.51/ecv_python_development/helpers/debugger/debugging.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/helpers/formatter/__init__.py` & `ecv-python-development-0.0.51/ecv_python_development/helpers/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/helpers/formatter/formatter.py` & `ecv-python-development-0.0.51/ecv_python_development/helpers/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/helpers/http/requests.py` & `ecv-python-development-0.0.51/ecv_python_development/helpers/http/requests.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development/helpers/strings/passwords.py` & `ecv-python-development-0.0.51/ecv_python_development/helpers/strings/passwords.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development.egg-info/PKG-INFO` & `ecv-python-development-0.0.51/ecv_python_development.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.50
+Version: 0.0.51
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `ecv-python-development-0.0.50/ecv_python_development.egg-info/SOURCES.txt` & `ecv-python-development-0.0.51/ecv_python_development.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/ecv_python_development.egg-info/requires.txt` & `ecv-python-development-0.0.51/ecv_python_development.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.50/setup.py` & `ecv-python-development-0.0.51/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="ecv-python-development",
-    version="0.0.50",
+    version="0.0.51",
     author="Warren Ezra Bruce Jaudian",
     author_email="warren.jaudian@ecloudvalley.com",
     packages=find_packages(),
     description="ECV Python Development Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development",
```


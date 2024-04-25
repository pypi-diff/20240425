# Comparing `tmp/pilot-platform-common-0.7.3.tar.gz` & `tmp/pilot-platform-common-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.7.3.tar", last modified: Wed Apr 24 14:07:32 2024, max compression
+gzip compressed data, was "pilot-platform-common-0.7.4.tar", last modified: Thu Apr 25 20:32:32 2024, max compression
```

## Comparing `pilot-platform-common-0.7.3.tar` & `pilot-platform-common-0.7.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/geid/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/jwt_handler_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/project/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/services/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/services/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/vault/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/fixtures/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/tests/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/test_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/test_permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/jwt_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/services/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/fixtures/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/tests/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/test_permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.7.3/PKG-INFO` & `pilot-platform-common-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.7.3
+Version: 0.7.4
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.7.3/README.md` & `pilot-platform-common-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/__init__.py` & `pilot-platform-common-0.7.4/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/geid/geid_client.py` & `pilot-platform-common-0.7.4/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-0.7.4/common/jwt_handler/JWTHandler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/jwt_handler/models.py` & `pilot-platform-common-0.7.4/common/jwt_handler/models.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/logging/formatter.py` & `pilot-platform-common-0.7.4/common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/logging/logging.py` & `pilot-platform-common-0.7.4/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/models/config_center_policy.py` & `pilot-platform-common-0.7.4/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-0.7.4/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-0.7.4/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/permissions/exceptions.py` & `pilot-platform-common-0.7.4/common/permissions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/permissions/permissions.py` & `pilot-platform-common-0.7.4/common/permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/permissions/permissions_manager.py` & `pilot-platform-common-0.7.4/common/permissions/permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/permissions/schemas.py` & `pilot-platform-common-0.7.4/common/permissions/schemas.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/project/project_client.py` & `pilot-platform-common-0.7.4/common/project/project_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,17 @@
         description=None,
         is_discoverable=None,
         tags_all=None,
         code_any=None,
         created_at_start=None,
         created_at_end=None,
         favourite_by=None,
+        guacamole: bool = False,
+        superset: bool = False,
+        jupyterhub: bool = False,
     ):
         data = {
             'page': page,
             'page_size': page_size,
             'sort_by': order_by,
             'sort_order': order_type,
             'name': name,
@@ -127,17 +130,20 @@
             'description': description,
             'is_discoverable': is_discoverable,
             'tags_all': tags_all,
             'code_any': code_any,
             'created_at_start': created_at_start,
             'created_at_end': created_at_end,
             'favourite_by': favourite_by,
+            'guacamole': guacamole,
+            'superset': superset,
+            'jupyterhub': jupyterhub,
         }
         # remove blank items
-        data = {k: v for k, v in data.items() if v is not None}
+        data = {k: v for k, v in data.items() if v not in [None, False]}
 
         async with httpx.AsyncClient() as client:
             response = await client.get(self.base_url + '/v1/projects/', params=data)
         if response.status_code == 404:
             raise ProjectNotFoundException
         elif response.status_code != 200:
             raise ProjectException(status_code=response.status_code, error_msg=response.json())
```

### Comparing `pilot-platform-common-0.7.3/common/project/project_exceptions.py` & `pilot-platform-common-0.7.4/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/services/auth_client.py` & `pilot-platform-common-0.7.4/common/services/auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/common/vault/vault_client.py` & `pilot-platform-common-0.7.4/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-0.7.4/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.7.3
+Version: 0.7.4
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.7.3/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-0.7.4/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/pyproject.toml` & `pilot-platform-common-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common"
-version = "0.7.3"
+version = "0.7.4"
 description = ""
 authors = ["Indoc Systems"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = ">=0.19.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
```

### Comparing `pilot-platform-common-0.7.3/setup.py` & `pilot-platform-common-0.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.7.3',
+    version='0.7.4',
     author='Indoc Systems',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pilot-platform-common-0.7.3/tests/conftest.py` & `pilot-platform-common-0.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/fixtures/metadata.py` & `pilot-platform-common-0.7.4/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/permissions/test_auth_client.py` & `pilot-platform-common-0.7.4/tests/permissions/test_auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/permissions/test_permissions.py` & `pilot-platform-common-0.7.4/tests/permissions/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/permissions/test_permissions_manager.py` & `pilot-platform-common-0.7.4/tests/permissions/test_permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/test_formatter.py` & `pilot-platform-common-0.7.4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/test_geid_client.py` & `pilot-platform-common-0.7.4/tests/test_geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/test_jwt_handler.py` & `pilot-platform-common-0.7.4/tests/test_jwt_handler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/test_logging.py` & `pilot-platform-common-0.7.4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.3/tests/test_project_client.py` & `pilot-platform-common-0.7.4/tests/test_project_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,7 +153,26 @@
         name=PROJECT_DATA['name'],
         code=PROJECT_DATA['code'],
         description=PROJECT_DATA['description'],
         tags_all=PROJECT_DATA['tags'],
     )
     assert result['result'][0].name == PROJECT_DATA['name']
     assert result['total'] == 1
+
+
+def test_project_search_200_with_workbench_filters(redis, httpx_mock):
+    result = {
+        'result': [PROJECT_DATA],
+        'total': 1,
+    }
+    url = PROJECT_URL + ('/v1/projects/?guacamole=true&superset=true&jupyterhub=true')
+    httpx_mock.add_response(
+        method='GET',
+        url=url,
+        json=result,
+        status_code=200,
+    )
+
+    project_client = ProjectClient(PROJECT_URL, redis.url, enable_cache=False)
+    result = project_client.search(guacamole=True, superset=True, jupyterhub=True)
+    assert result['result'][0].name == PROJECT_DATA['name']
+    assert result['total'] == 1
```

### Comparing `pilot-platform-common-0.7.3/tests/test_vault_client.py` & `pilot-platform-common-0.7.4/tests/test_vault_client.py`

 * *Files identical despite different names*


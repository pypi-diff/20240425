# Comparing `tmp/pricecypher-sdk-2.0.0.dev2.tar.gz` & `tmp/pricecypher_sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pricecypher-sdk-2.0.0.dev2.tar", last modified: Thu Sep 28 15:14:05 2023, max compression
+gzip compressed data, was "pricecypher_sdk-2.1.0.tar", last modified: Thu Apr 25 11:28:05 2024, max compression
```

## Comparing `pricecypher-sdk-2.0.0.dev2.tar` & `pricecypher_sdk-2.1.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.327973 pricecypher-sdk-2.0.0.dev2/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.206740 pricecypher-sdk-2.0.0.dev2/.github/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.210115 pricecypher-sdk-2.0.0.dev2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      968 2022-03-25 10:57:36.000000 pricecypher-sdk-2.0.0.dev2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      595 2022-03-25 10:57:36.000000 pricecypher-sdk-2.0.0.dev2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1129 2022-03-25 10:57:36.000000 pricecypher-sdk-2.0.0.dev2/.github/pull_request_template.md
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.221670 pricecypher-sdk-2.0.0.dev2/.idea/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      176 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/.idea/.gitignore
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.223724 pricecypher-sdk-2.0.0.dev2/.idea/inspectionProfiles/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      174 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      180 2023-09-28 15:13:35.000000 pricecypher-sdk-2.0.0.dev2/.idea/misc.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      296 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/.idea/modules.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      504 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/.idea/pricecypher_python_api.iml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      508 2023-09-28 15:13:35.000000 pricecypher-sdk-2.0.0.dev2/.idea/pricecypher_python_sdk.iml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      180 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/.idea/vcs.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1407 2023-09-28 15:14:04.000000 pricecypher-sdk-2.0.0.dev2/ChangeLog
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1080 2022-03-25 10:57:36.000000 pricecypher-sdk-2.0.0.dev2/LICENSE
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      900 2023-09-28 15:14:05.325931 pricecypher-sdk-2.0.0.dev2/PKG-INFO
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3241 2023-09-28 11:29:21.000000 pricecypher-sdk-2.0.0.dev2/README.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      110 2023-09-28 15:13:32.000000 pricecypher-sdk-2.0.0.dev2/pyproject.toml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      121 2023-09-28 15:13:32.000000 pricecypher-sdk-2.0.0.dev2/requirements.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      781 2023-09-28 15:14:05.330670 pricecypher-sdk-2.0.0.dev2/setup.cfg
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      104 2023-09-28 15:13:32.000000 pricecypher-sdk-2.0.0.dev2/setup.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.182109 pricecypher-sdk-2.0.0.dev2/src/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.240574 pricecypher-sdk-2.0.0.dev2/src/pricecypher/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      170 2023-09-28 15:13:32.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.256502 pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      103 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      666 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/base_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1202 2022-09-30 14:31:36.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/scope_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1154 2022-09-30 14:31:36.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/scope_value_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2337 2023-08-22 09:53:07.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/config_sections.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.261913 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1240 2023-09-28 15:13:33.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/QualityTestScript.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1824 2023-09-28 15:13:33.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/ScopeScript.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2448 2023-09-28 15:13:33.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/Script.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      161 2022-10-07 15:03:39.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.267872 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/dataclasses/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3054 2022-11-02 15:42:11.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/dataclasses/TestResult.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       26 2022-10-07 15:34:17.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/dataclasses/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.273483 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/enums/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      119 2022-10-07 14:52:35.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/enums/TestStatus.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       35 2022-10-07 15:03:58.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/enums/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    17213 2023-09-28 11:29:21.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/datasets.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.278580 pricecypher-sdk-2.0.0.dev2/src/pricecypher/encoders/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      572 2022-10-20 11:57:22.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/encoders/JsonEncoder.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       48 2022-10-20 11:55:13.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/encoders/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.294509 pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      107 2023-08-22 09:53:07.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      808 2022-09-30 14:31:36.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/base_endpoint.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2156 2023-08-22 09:53:08.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/config.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     5245 2023-09-28 11:29:21.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/datasets.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1517 2023-09-28 11:29:21.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/users.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      509 2022-09-30 14:31:36.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/exceptions.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.307597 pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      238 2023-08-22 09:53:08.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1355 2023-08-22 09:53:08.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/config.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3493 2023-08-22 09:53:08.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/datasets.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      843 2022-07-29 09:08:07.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/namespaced_schema.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      667 2023-08-22 09:53:08.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/users.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    12425 2023-09-28 11:29:21.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher/rest.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.319902 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      900 2023-09-28 15:14:04.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1878 2023-09-28 15:14:05.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2023-09-28 15:14:04.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       50 2023-09-28 15:14:04.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/entry_points.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2023-09-28 15:14:04.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/not-zip-safe
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       47 2023-09-28 15:14:05.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/pbr.json
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      145 2023-09-28 15:14:05.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/requires.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       12 2023-09-28 15:14:05.000000 pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2023-09-28 15:14:05.324910 pricecypher-sdk-2.0.0.dev2/tests/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        0 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/tests/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    25448 2022-05-17 11:22:56.000000 pricecypher-sdk-2.0.0.dev2/tests/test_rest.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.987990 pricecypher_sdk-2.1.0/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.719811 pricecypher_sdk-2.1.0/.github/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.727433 pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      968 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      595 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1129 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.791678 pricecypher_sdk-2.1.0/.idea/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      176 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/.idea/.gitignore
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.796941 pricecypher_sdk-2.1.0/.idea/inspectionProfiles/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      174 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      283 2024-04-25 08:49:40.000000 pricecypher_sdk-2.1.0/.idea/misc.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      519 2024-04-25 08:39:04.000000 pricecypher_sdk-2.1.0/.idea/modules.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      504 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/.idea/pricecypher_python_api.iml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      603 2024-04-25 08:49:40.000000 pricecypher_sdk-2.1.0/.idea/pricecypher_python_sdk.iml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      167 2024-04-25 08:39:04.000000 pricecypher_sdk-2.1.0/.idea/vcs.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1544 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/ChangeLog
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1080 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.0/LICENSE
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      895 2024-04-25 11:28:05.987613 pricecypher_sdk-2.1.0/PKG-INFO
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3241 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.0/README.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      110 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/pyproject.toml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      121 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/requirements.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      781 2024-04-25 11:28:05.992354 pricecypher_sdk-2.1.0/setup.cfg
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      104 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/setup.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.707491 pricecypher_sdk-2.1.0/src/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.819284 pricecypher_sdk-2.1.0/src/pricecypher/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      298 2024-04-25 09:35:27.000000 pricecypher_sdk-2.1.0/src/pricecypher/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.840663 pricecypher_sdk-2.1.0/src/pricecypher/collections/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      666 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/src/pricecypher/collections/base_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1179 2024-04-25 09:37:26.000000 pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1131 2024-04-25 09:38:50.000000 pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_value_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2337 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.0/src/pricecypher/config_sections.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.862416 pricecypher_sdk-2.1.0/src/pricecypher/contracts/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1240 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/QualityTestScript.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1824 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/ScopeScript.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2448 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/Script.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      161 2022-10-07 15:03:39.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.872661 pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3054 2022-11-02 15:42:11.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/TestResult.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       26 2022-10-07 15:34:17.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.880055 pricecypher_sdk-2.1.0/src/pricecypher/contracts/enums/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      119 2022-10-07 14:52:35.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/enums/TestStatus.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       35 2022-10-07 15:03:58.000000 pricecypher_sdk-2.1.0/src/pricecypher/contracts/enums/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    17731 2024-04-25 10:19:01.000000 pricecypher_sdk-2.1.0/src/pricecypher/datasets.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.887802 pricecypher_sdk-2.1.0/src/pricecypher/encoders/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      572 2022-10-20 11:57:22.000000 pricecypher_sdk-2.1.0/src/pricecypher/encoders/JsonEncoder.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       48 2022-10-20 11:55:13.000000 pricecypher_sdk-2.1.0/src/pricecypher/encoders/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.919247 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      107 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      808 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/base_endpoint.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2156 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/config.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     5245 2024-04-25 08:28:14.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/datasets.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1517 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.0/src/pricecypher/endpoints/users.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      509 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.0/src/pricecypher/exceptions.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.949211 pricecypher_sdk-2.1.0/src/pricecypher/models/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      238 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1355 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/config.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3493 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/datasets.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      843 2022-07-29 09:08:07.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/namespaced_schema.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      667 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.0/src/pricecypher/models/users.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    12425 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.0/src/pricecypher/rest.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.985868 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      895 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1838 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       50 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2023-09-28 15:14:04.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       47 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/pbr.json
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      145 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/requires.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       12 2024-04-25 11:28:05.000000 pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-04-25 11:28:05.984225 pricecypher_sdk-2.1.0/tests/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        0 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/tests/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    25448 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.0/tests/test_rest.py
```

### Comparing `pricecypher-sdk-2.0.0.dev2/.github/ISSUE_TEMPLATE/bug_report.md` & `pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/.github/ISSUE_TEMPLATE/feature_request.md` & `pricecypher_sdk-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/.github/pull_request_template.md` & `pricecypher_sdk-2.1.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/ChangeLog` & `pricecypher_sdk-2.1.0/ChangeLog`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 CHANGES
 =======
 
-* BREAKING CHANGE: Update Script contracts to take \`get\_bearer\_token\` function argument instead of static \`bearer\_token\`
+v2.1.0
+------
+
+* Release v2.1.0 to master (#34)
+* Add dataset environment parameter to \`get\_transactions\` (#33)
+
+v2.0.0
+------
+
+* BREAKING CHANGE: Update Script contracts to take \`get\_bearer\_token\` function argument instead of static \`bearer\_token\` (#31)
 
 v1.0.1
 ------
 
 * HOTFIX - Use \`pbr\` for building and include \`\_\_version\_\_\` property in top-level module (#29)
 
 v1.0.0
```

### Comparing `pricecypher-sdk-2.0.0.dev2/LICENSE` & `pricecypher_sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/PKG-INFO` & `pricecypher_sdk-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pricecypher-sdk
-Version: 2.0.0.dev2
+Version: 2.1.0
 Summary: Python wrapper around the different PriceCypher APIs
 Home-page: https://github.com/marketredesign/pricecypher_python_sdk
 Author: Deloitte Consulting B.V.
 Project-URL: Bug Tracker, https://github.com/marketredesign/pricecypher_python_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pricecypher-sdk-2.0.0.dev2/README.md` & `pricecypher_sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/setup.cfg` & `pricecypher_sdk-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/base_collection.py` & `pricecypher_sdk-2.1.0/src/pricecypher/collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/scope_collection.py` & `pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pricecypher.collections.base_collection import BaseCollection
+from .base_collection import BaseCollection
 from pricecypher.models import Scope
 
 
 class ScopeCollection(BaseCollection):
     _type = Scope
 
     def __repr__(self):
```

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/collections/scope_value_collection.py` & `pricecypher_sdk-2.1.0/src/pricecypher/collections/scope_value_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pricecypher.collections.base_collection import BaseCollection
+from .base_collection import BaseCollection
 from pricecypher.models import ScopeValue
 
 
 class ScopeValueCollection(BaseCollection):
     _type = ScopeValue
 
     def __repr__(self):
```

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/config_sections.py` & `pricecypher_sdk-2.1.0/src/pricecypher/config_sections.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/QualityTestScript.py` & `pricecypher_sdk-2.1.0/src/pricecypher/contracts/QualityTestScript.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/ScopeScript.py` & `pricecypher_sdk-2.1.0/src/pricecypher/contracts/ScopeScript.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/Script.py` & `pricecypher_sdk-2.1.0/src/pricecypher/contracts/Script.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/contracts/dataclasses/TestResult.py` & `pricecypher_sdk-2.1.0/src/pricecypher/contracts/dataclasses/TestResult.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/datasets.py` & `pricecypher_sdk-2.1.0/src/pricecypher/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
-
 from pandas import DataFrame
 
-from pricecypher.collections import ScopeCollection, ScopeValueCollection
 from pricecypher.endpoints import DatasetsEndpoint, UsersEndpoint
+from .collections.scope_collection import ScopeCollection
+from .collections.scope_value_collection import ScopeValueCollection
 
 
 class Datasets(object):
     """
     Datasets API. Exposes all available operations on datasets, like fetching the available datasets, listing
     the scopes within a dataset, retrieving transactions within a dataset, etc.
 
@@ -142,20 +142,24 @@
         columns,
         start_date_time=None,
         end_date_time=None,
         bc_id='all',
         filters=[],
         intake_status=None,
         filter_transaction_ids=None,
+        dataset_environment=None,
     ):
         """
         Display a listing of transactions as a dataframe. The transactions can be grouped or not, using the aggregate
         parameter. The desired columns, as well as filters and aggregation methods, can be specified.
 
         :param int dataset_id: Dataset to retrieve transactions for.
+        :param param dataset_environment: Key specifying the "environment" of the underlying data intake to query. 
+            Use `None` (the default) to query transactions from the latest intake, regardless of the associated 
+            environment with that intake.
         :param bool aggregate: If true, the transactions will be grouped on all categorical columns that have no
             aggregation method specified.
         :param list columns: Desired columns in the resulting dataframe. Each column must be a dict. Each column must
             have a `representation`, `scope_id`, or `name_dataset` specified. The following properties are optional.
                 `filter`: value or list of values the resulting transactions should be filtered on.
                 `aggregate`: aggregation method that should be used for this column. When aggregating and no
                     aggregation method is specified, the method that is used is determined by the underlying dataset
@@ -225,14 +229,18 @@
             raise ValueError('start_date_time should be an instance of datetime.')
 
         if isinstance(end_date_time, datetime):
             request_data['end_date_time'] = end_date_time
         elif end_date_time is not None:
             raise ValueError('end_date_time should be an instance of datetime.')
 
+        # Attach the dataset environment if specified
+        if dataset_environment is not None:
+            request_data['environment'] = dataset_environment
+
         # Fetch transactions from the dataset service.
         transactions = DatasetsEndpoint(self._bearer, dataset_id, dss_base, self._rest_options) \
             .business_cell(bc_id) \
             .transactions() \
             .index(request_data)
 
         # Map transactions to dicts based on the provided column keys and convert to pandas dataframe.
```

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/encoders/JsonEncoder.py` & `pricecypher_sdk-2.1.0/src/pricecypher/encoders/JsonEncoder.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/base_endpoint.py` & `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/config.py` & `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/config.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/datasets.py` & `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/endpoints/users.py` & `pricecypher_sdk-2.1.0/src/pricecypher/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/config.py` & `pricecypher_sdk-2.1.0/src/pricecypher/models/config.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/datasets.py` & `pricecypher_sdk-2.1.0/src/pricecypher/models/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/namespaced_schema.py` & `pricecypher_sdk-2.1.0/src/pricecypher/models/namespaced_schema.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/models/users.py` & `pricecypher_sdk-2.1.0/src/pricecypher/models/users.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher/rest.py` & `pricecypher_sdk-2.1.0/src/pricecypher/rest.py`

 * *Files identical despite different names*

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/PKG-INFO` & `pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pricecypher-sdk
-Version: 2.0.0.dev2
+Version: 2.1.0
 Summary: Python wrapper around the different PriceCypher APIs
 Home-page: https://github.com/marketredesign/pricecypher_python_sdk
 Author: Deloitte Consulting B.V.
 Project-URL: Bug Tracker, https://github.com/marketredesign/pricecypher_python_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pricecypher-sdk-2.0.0.dev2/src/pricecypher_sdk.egg-info/SOURCES.txt` & `pricecypher_sdk-2.1.0/src/pricecypher_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 .idea/vcs.xml
 .idea/inspectionProfiles/profiles_settings.xml
 src/pricecypher/__init__.py
 src/pricecypher/config_sections.py
 src/pricecypher/datasets.py
 src/pricecypher/exceptions.py
 src/pricecypher/rest.py
-src/pricecypher/collections/__init__.py
 src/pricecypher/collections/base_collection.py
 src/pricecypher/collections/scope_collection.py
 src/pricecypher/collections/scope_value_collection.py
 src/pricecypher/contracts/QualityTestScript.py
 src/pricecypher/contracts/ScopeScript.py
 src/pricecypher/contracts/Script.py
 src/pricecypher/contracts/__init__.py
```

### Comparing `pricecypher-sdk-2.0.0.dev2/tests/test_rest.py` & `pricecypher_sdk-2.1.0/tests/test_rest.py`

 * *Files identical despite different names*


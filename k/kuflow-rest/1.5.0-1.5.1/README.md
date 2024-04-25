# Comparing `tmp/kuflow_rest-1.5.0.tar.gz` & `tmp/kuflow_rest-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_rest-1.5.0.tar", max compression
+gzip compressed data, was "kuflow_rest-1.5.1.tar", max compression
```

## Comparing `kuflow_rest-1.5.0.tar` & `kuflow_rest-1.5.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      875 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/README.md
--rw-r--r--   0        0        0        6 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/VERSION
--rw-r--r--   0        0        0     1367 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/kuflow_rest/__init__.py
--rw-r--r--   0        0        0     1907 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/kuflow_rest/_generated/__init__.py
--rw-r--r--   0        0        0      599 2024-04-09 11:50:13.765090 kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7095 2024-04-09 11:50:13.769091 kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
--rw-r--r--   0        0        0     2282 2024-04-09 11:50:13.877092 kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
--rw-r--r--   0        0        0      732 2024-04-09 11:50:13.897092 kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0    57988 2024-04-09 11:50:13.857092 kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
--rw-r--r--   0        0        0      178 2024-04-09 11:50:13.877092 kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0        0        0     8790 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/kuflow_rest/_generated/_client.py
--rw-r--r--   0        0        0     3928 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/kuflow_rest/_generated/_configuration.py
--rw-r--r--   0        0        0      675 2024-04-09 11:44:28.825042 kuflow_rest-1.5.0/kuflow_rest/_generated/_patch.py
--rw-r--r--   0        0        0    78871 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/_serialization.py
--rw-r--r--   0        0        0     1517 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/_version.py
--rw-r--r--   0        0        0     1854 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/__init__.py
--rw-r--r--   0        0        0     8964 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/_client.py
--rw-r--r--   0        0        0     3971 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/_configuration.py
--rw-r--r--   0        0        0      675 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/_patch.py
--rw-r--r--   0        0        0     2289 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/__init__.py
--rw-r--r--   0        0        0     7515 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py
--rw-r--r--   0        0        0      675 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_patch.py
--rw-r--r--   0        0        0     8610 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_principal_operations.py
--rw-r--r--   0        0        0    47079 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_process_operations.py
--rw-r--r--   0        0        0    13498 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_robot_operations.py
--rw-r--r--   0        0        0    64995 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_task_operations.py
--rw-r--r--   0        0        0     8534 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_tenant_user_operations.py
--rw-r--r--   0        0        0     7717 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_worker_operations.py
--rw-r--r--   0        0        0     6679 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/models/__init__.py
--rw-r--r--   0        0        0     4177 2024-04-09 11:50:13.841091 kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4324 2024-04-09 11:50:13.873092 kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
--rw-r--r--   0        0        0    92161 2024-04-09 11:50:13.849091 kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0      739 2024-04-09 11:50:13.877092 kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     4714 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/models/_enums.py
--rw-r--r--   0        0        0   107550 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/models/_models.py
--rw-r--r--   0        0        0      675 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/models/_patch.py
--rw-r--r--   0        0        0     2289 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__init__.py
--rw-r--r--   0        0        0      948 2024-04-09 11:50:13.877092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5588 2024-04-09 11:50:13.877092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0      743 2024-04-09 11:50:13.897092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
--rw-r--r--   0        0        0     7219 2024-04-09 11:50:13.881092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0    36368 2024-04-09 11:50:13.889092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0    10742 2024-04-09 11:50:13.897092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_robot_operations.cpython-38.pyc
--rw-r--r--   0        0        0    51494 2024-04-09 11:50:13.893092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     7253 2024-04-09 11:50:13.881092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_tenant_user_operations.cpython-38.pyc
--rw-r--r--   0        0        0     5779 2024-04-09 11:50:13.897092 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_worker_operations.cpython-38.pyc
--rw-r--r--   0        0        0     8109 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_authentication_operations.py
--rw-r--r--   0        0        0      675 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_patch.py
--rw-r--r--   0        0        0    10642 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_principal_operations.py
--rw-r--r--   0        0        0    56895 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_process_operations.py
--rw-r--r--   0        0        0    17153 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_robot_operations.py
--rw-r--r--   0        0        0    79296 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_task_operations.py
--rw-r--r--   0        0        0    10587 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_tenant_user_operations.py
--rw-r--r--   0        0        0     8311 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_worker_operations.py
--rw-r--r--   0        0        0       26 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_generated/py.typed
--rw-r--r--   0        0        0     9544 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/_kuflow_rest_client.py
--rw-r--r--   0        0        0     5686 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/models/__init__.py
--rw-r--r--   0        0        0     3560 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3994 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0     3986 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/models/_models.py
--rw-r--r--   0        0        0     1674 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/__init__.py
--rw-r--r--   0        0        0      679 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1677 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
--rw-r--r--   0        0        0     3656 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
--rw-r--r--   0        0        0    12284 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
--rw-r--r--   0        0        0     3328 2024-04-09 11:50:13.901092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_robot_operations.cpython-38.pyc
--rw-r--r--   0        0        0    16229 2024-04-09 11:50:13.905092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
--rw-r--r--   0        0        0     3464 2024-04-09 11:50:13.905092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_tenant_user_operations.cpython-38.pyc
--rw-r--r--   0        0        0     1819 2024-04-09 11:50:13.905092 kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_worker_operations.cpython-38.pyc
--rw-r--r--   0        0        0     2330 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_authentication_operations.py
--rw-r--r--   0        0        0     4463 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_principal_operations.py
--rw-r--r--   0        0        0    12882 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_process_operations.py
--rw-r--r--   0        0        0     4071 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_robot_operations.py
--rw-r--r--   0        0        0    17487 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_task_operations.py
--rw-r--r--   0        0        0     4421 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_tenant_user_operations.py
--rw-r--r--   0        0        0     2452 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/operations/_worker_operations.py
--rw-r--r--   0        0        0     2112 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/__init__.py
--rw-r--r--   0        0        0     1002 2024-04-09 11:50:13.905092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    10671 2024-04-09 11:50:13.905092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_process_page_item_utils.cpython-38.pyc
--rw-r--r--   0        0        0     9750 2024-04-09 11:50:13.909092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_process_save_element_command_utils.cpython-38.pyc
--rw-r--r--   0        0        0    22940 2024-04-09 11:50:13.909092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_process_utils.cpython-38.pyc
--rw-r--r--   0        0        0    15041 2024-04-09 11:50:13.913092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_page_item_utils.cpython-38.pyc
--rw-r--r--   0        0        0    13819 2024-04-09 11:50:13.917092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_save_element_command_utils.cpython-38.pyc
--rw-r--r--   0        0        0    14250 2024-04-09 11:50:13.917092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_save_json_forms_value_data_utils.cpython-38.pyc
--rw-r--r--   0        0        0    26632 2024-04-09 11:50:13.917092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_utils.cpython-38.pyc
--rw-r--r--   0        0        0    13712 2024-04-09 11:50:13.921092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_tenant_user_utils.cpython-38.pyc
--rw-r--r--   0        0        0    15450 2024-04-09 11:50:13.909092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/element_values.cpython-38.pyc
--rw-r--r--   0        0        0    17794 2024-04-09 11:50:13.913092 kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/json_forms.cpython-38.pyc
--rw-r--r--   0        0        0    13419 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_process_page_item_utils.py
--rw-r--r--   0        0        0    11819 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_process_save_element_command_utils.py
--rw-r--r--   0        0        0    25012 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_process_utils.py
--rw-r--r--   0        0        0    18454 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_task_page_item_utils.py
--rw-r--r--   0        0        0    16414 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_task_save_element_command_utils.py
--rw-r--r--   0        0        0    15395 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_task_save_json_forms_value_data_utils.py
--rw-r--r--   0        0        0    29410 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_task_utils.py
--rw-r--r--   0        0        0    14671 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/_tenant_user_utils.py
--rw-r--r--   0        0        0    18912 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/element_values.py
--rw-r--r--   0        0        0    23944 2024-04-09 11:44:28.829042 kuflow_rest-1.5.0/kuflow_rest/utils/json_forms.py
--rw-r--r--   0        0        0      880 2024-04-09 11:50:36.277349 kuflow_rest-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-1.5.0/setup.py
--rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      875 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/README.md
+-rw-r--r--   0        0        0        6 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/VERSION
+-rw-r--r--   0        0        0     1367 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/__init__.py
+-rw-r--r--   0        0        0     1907 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/__init__.py
+-rw-r--r--   0        0        0      599 2024-04-25 11:56:36.100035 kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7095 2024-04-25 11:56:36.100035 kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc
+-rw-r--r--   0        0        0     2282 2024-04-25 11:56:36.208036 kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2024-04-25 11:56:36.228036 kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0    57988 2024-04-25 11:56:36.188036 kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc
+-rw-r--r--   0        0        0      178 2024-04-25 11:56:36.208036 kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0        0        0     8790 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/_client.py
+-rw-r--r--   0        0        0     3928 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/_configuration.py
+-rw-r--r--   0        0        0      675 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/_patch.py
+-rw-r--r--   0        0        0    78871 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/_serialization.py
+-rw-r--r--   0        0        0     1517 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/_version.py
+-rw-r--r--   0        0        0     1854 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/__init__.py
+-rw-r--r--   0        0        0     8964 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/_client.py
+-rw-r--r--   0        0        0     3971 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/_configuration.py
+-rw-r--r--   0        0        0      675 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/_patch.py
+-rw-r--r--   0        0        0     2289 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/__init__.py
+-rw-r--r--   0        0        0     7515 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      675 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_patch.py
+-rw-r--r--   0        0        0     8610 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_principal_operations.py
+-rw-r--r--   0        0        0    47079 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_process_operations.py
+-rw-r--r--   0        0        0    13498 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_robot_operations.py
+-rw-r--r--   0        0        0    64995 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_task_operations.py
+-rw-r--r--   0        0        0     8534 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_tenant_user_operations.py
+-rw-r--r--   0        0        0     7717 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_worker_operations.py
+-rw-r--r--   0        0        0     6679 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/models/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-25 11:56:36.172036 kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4324 2024-04-25 11:56:36.204036 kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc
+-rw-r--r--   0        0        0    92161 2024-04-25 11:56:36.180036 kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0      739 2024-04-25 11:56:36.204036 kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     4714 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/models/_enums.py
+-rw-r--r--   0        0        0   107550 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/models/_models.py
+-rw-r--r--   0        0        0      675 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/models/_patch.py
+-rw-r--r--   0        0        0     2289 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__init__.py
+-rw-r--r--   0        0        0      948 2024-04-25 11:56:36.208036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5588 2024-04-25 11:56:36.208036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0      743 2024-04-25 11:56:36.228036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc
+-rw-r--r--   0        0        0     7219 2024-04-25 11:56:36.212036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    36368 2024-04-25 11:56:36.220036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    10742 2024-04-25 11:56:36.228036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_robot_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    51494 2024-04-25 11:56:36.224036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     7253 2024-04-25 11:56:36.212036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_tenant_user_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     5779 2024-04-25 11:56:36.228036 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_worker_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     8109 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_authentication_operations.py
+-rw-r--r--   0        0        0      675 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_patch.py
+-rw-r--r--   0        0        0    10642 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_principal_operations.py
+-rw-r--r--   0        0        0    56895 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_process_operations.py
+-rw-r--r--   0        0        0    17153 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_robot_operations.py
+-rw-r--r--   0        0        0    79296 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_task_operations.py
+-rw-r--r--   0        0        0    10587 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_tenant_user_operations.py
+-rw-r--r--   0        0        0     8311 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_worker_operations.py
+-rw-r--r--   0        0        0       26 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_generated/py.typed
+-rw-r--r--   0        0        0     9544 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/_kuflow_rest_client.py
+-rw-r--r--   0        0        0     5686 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/models/__init__.py
+-rw-r--r--   0        0        0     3560 2024-04-25 11:56:36.232036 kuflow_rest-1.5.1/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3994 2024-04-25 11:56:36.232036 kuflow_rest-1.5.1/kuflow_rest/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0     3986 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/models/_models.py
+-rw-r--r--   0        0        0     1674 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/operations/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-25 11:56:36.232036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1677 2024-04-25 11:56:36.232036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3656 2024-04-25 11:56:36.232036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    12388 2024-04-25 11:56:36.232036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3328 2024-04-25 11:56:36.236036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_robot_operations.cpython-38.pyc
+-rw-r--r--   0        0        0    16229 2024-04-25 11:56:36.236036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     3464 2024-04-25 11:56:36.236036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_tenant_user_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     1819 2024-04-25 11:56:36.236036 kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_worker_operations.cpython-38.pyc
+-rw-r--r--   0        0        0     2330 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/operations/_authentication_operations.py
+-rw-r--r--   0        0        0     4463 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/operations/_principal_operations.py
+-rw-r--r--   0        0        0    13081 2024-04-25 11:49:37.321017 kuflow_rest-1.5.1/kuflow_rest/operations/_process_operations.py
+-rw-r--r--   0        0        0     4071 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/operations/_robot_operations.py
+-rw-r--r--   0        0        0    17487 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/operations/_task_operations.py
+-rw-r--r--   0        0        0     4421 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/operations/_tenant_user_operations.py
+-rw-r--r--   0        0        0     2452 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/operations/_worker_operations.py
+-rw-r--r--   0        0        0     2112 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2024-04-25 11:56:36.236036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10671 2024-04-25 11:56:36.236036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_process_page_item_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     9750 2024-04-25 11:56:36.240036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_process_save_element_command_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    22279 2024-04-25 11:56:36.240036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_process_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    15041 2024-04-25 11:56:36.244036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_page_item_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13819 2024-04-25 11:56:36.248036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_save_element_command_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14250 2024-04-25 11:56:36.248036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_save_json_forms_value_data_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    26632 2024-04-25 11:56:36.248036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13712 2024-04-25 11:56:36.252036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_tenant_user_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    15450 2024-04-25 11:56:36.240036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/element_values.cpython-38.pyc
+-rw-r--r--   0        0        0    17794 2024-04-25 11:56:36.244036 kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/json_forms.cpython-38.pyc
+-rw-r--r--   0        0        0    13419 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_process_page_item_utils.py
+-rw-r--r--   0        0        0    11819 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_process_save_element_command_utils.py
+-rw-r--r--   0        0        0    24356 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_process_utils.py
+-rw-r--r--   0        0        0    18454 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_task_page_item_utils.py
+-rw-r--r--   0        0        0    16414 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_task_save_element_command_utils.py
+-rw-r--r--   0        0        0    15395 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_task_save_json_forms_value_data_utils.py
+-rw-r--r--   0        0        0    29410 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_task_utils.py
+-rw-r--r--   0        0        0    14671 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/_tenant_user_utils.py
+-rw-r--r--   0        0        0    18912 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/element_values.py
+-rw-r--r--   0        0        0    23944 2024-04-25 11:49:37.325017 kuflow_rest-1.5.1/kuflow_rest/utils/json_forms.py
+-rw-r--r--   0        0        0      880 2024-04-25 11:56:56.584179 kuflow_rest-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 kuflow_rest-1.5.1/setup.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 kuflow_rest-1.5.1/PKG-INFO
```

### Comparing `kuflow_rest-1.5.0/README.md` & `kuflow_rest-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 #
 
 from ._generated._serialization import Deserializer, Model, Serializer
 from ._kuflow_rest_client import KuBotTokenCredential, KuFlowRestClient
 
 
 __all__ = ["Deserializer", "KuBotTokenCredential", "KuFlowRestClient", "Model", "Serializer"]
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 1907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 7307 0000  U........*.fs...
+00000000: 550d 0d0a 0000 0000 5143 2a66 7307 0000  U.......QC*fs...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6503 5a04 7a18 6400 6403  m.Z...e.Z.z.d.d.
 00000050: 6c05 6d06 5a07 0100 6400 6404 6c05 5400  l.m.Z...d.d.l.T.
 00000060: 5700 6e18 0400 6508 6b0a 724c 0100 0100  W.n...e.k.rL....
 00000070: 0100 6700 5a07 5900 6e02 5800 6400 6405  ..g.Z.Y.n.X.d.d.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_client.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 8790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 5622 0000  U........*.fV"..
+00000000: 550d 0d0a 0000 0000 5143 2a66 5622 0000  U.......QC*fV"..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6406 6407 6c0c 6d0d 5a0e 0100 6406  ..d.d.l.m.Z...d.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_configuration.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 3928 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 580f 0000  U........*.fX...
+00000000: 550d 0d0a 0000 0000 5143 2a66 580f 0000  U.......QC*fX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6403 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6502 7238 6400 6405 6c07  m.Z...e.r8d.d.l.
 00000060: 6d08 5a08 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 8302 5a09 6408 5300 2909 e900 0000 0029  ..Z.d.S.)......)
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 675 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 a302 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 a302 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/__pycache__/_serialization.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 78871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 1734 0100  U........*.f.4..
+00000000: 550d 0d0a 0000 0000 5143 2a66 1734 0100  U.......QC*f.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9602 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6402 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 5a05 6400 6402 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6400 6402 6c09  d.l.m.Z...d.d.l.
 00000070: 5a09 6400 6402 6c0a 5a0a 6400 6402 6c0b  Z.d.d.l.Z.d.d.l.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/_client.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/_configuration.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/_patch.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/_serialization.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/_version.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # --------------------------------------------------------------------------
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 #
 # --------------------------------------------------------------------------
 
-VERSION = "1.5.0"
+VERSION = "1.5.1"
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/_client.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/_configuration.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/_patch.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_authentication_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_patch.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_principal_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_process_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_robot_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_robot_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_task_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_tenant_user_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_tenant_user_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/aio/operations/_worker_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/aio/operations/_worker_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 6679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 171a 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 171a 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0049 0000 0040 0000 0073 4004 0000 6400  .I...@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c00 6d05 5a05 0100 6400 6406 6c00  d.l.m.Z...d.d.l.
 00000070: 6d06 5a06 0100 6400 6407 6c00 6d07 5a07  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/_enums.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 4714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 6a12 0000  U........*.fj...
+00000000: 550d 0d0a 0000 0000 5143 2a66 6a12 0000  U.......QC*fj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6601 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 6501 6503 6405 8d05 5a05 4700 6406  e.e.e.d...Z.G.d.
 00000060: 6407 8400 6407 6504 6501 6503 6405 8d05  d...d.e.e.e.d...
 00000070: 5a06 4700 6408 6409 8400 6409 6504 6501  Z.G.d.d...d.e.e.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 107550 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 1ea4 0100  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 1ea4 0100  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3004 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6403 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6506 7244 6403 6405 6c08 6d0a 5a0b  ..e.rDd.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 6509 6a0c  ..G.d.d...d.e.j.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 675 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 a302 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 a302 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
@@ -27,21 +27,21 @@
 000001a0: 6820 7573 696e 6720 7468 6520 7465 6368  h using the tech
 000001b0: 6e69 7175 6573 2064 6573 6372 6962 6564  niques described
 000001c0: 2069 6e0a 2020 2020 6874 7470 733a 2f2f   in.    https://
 000001d0: 616b 612e 6d73 2f61 7a73 646b 2f70 7974  aka.ms/azsdk/pyt
 000001e0: 686f 6e2f 6470 636f 6465 6765 6e2f 7079  hon/dpcodegen/py
 000001f0: 7468 6f6e 2f63 7573 746f 6d69 7a65 0a20  thon/customize. 
 00000200: 2020 204e a900 7204 0000 0072 0400 0000     N..r....r....
-00000210: 7204 0000 00fa 4b2f 776f 726b 2f6b 7566  r.....K/work/kuf
+00000210: 7204 0000 00fa 4f2f 776f 726b 2f6b 7566  r.....O/work/kuf
 00000220: 6c6f 772d 7364 6b2d 7079 7468 6f6e 2f6b  low-sdk-python/k
 00000230: 7566 6c6f 772d 7265 7374 2f6b 7566 6c6f  uflow-rest/kuflo
 00000240: 775f 7265 7374 2f5f 6765 6e65 7261 7465  w_rest/_generate
-00000250: 642f 6d6f 6465 6c73 2f5f 7061 7463 682e  d/models/_patch.
-00000260: 7079 da09 7061 7463 685f 7364 6b0f 0000  py..patch_sdk...
-00000270: 0073 0200 0000 0001 7206 0000 004e 2907  .s......r....N).
-00000280: da07 5f5f 646f 635f 5fda 0674 7970 696e  ..__doc__..typin
-00000290: 6772 0200 0000 7203 0000 00da 0373 7472  gr....r......str
-000002a0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-000002b0: 5f72 0600 0000 7204 0000 0072 0400 0000  _r....r....r....
-000002c0: 7204 0000 0072 0500 0000 da08 3c6d 6f64  r....r......<mod
-000002d0: 756c 653e 0500 0000 7306 0000 0006 050c  ule>....s.......
-000002e0: 0210 03                                  ...
+00000250: 642f 6f70 6572 6174 696f 6e73 2f5f 7061  d/operations/_pa
+00000260: 7463 682e 7079 da09 7061 7463 685f 7364  tch.py..patch_sd
+00000270: 6b0f 0000 0073 0200 0000 0001 7206 0000  k....s......r...
+00000280: 004e 2907 da07 5f5f 646f 635f 5fda 0674  .N)...__doc__..t
+00000290: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
+000002a0: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
+000002b0: 6f6e 735f 5f72 0600 0000 7204 0000 0072  ons__r....r....r
+000002c0: 0400 0000 7204 0000 0072 0500 0000 da08  ....r....r......
+000002d0: 3c6d 6f64 756c 653e 0500 0000 7306 0000  <module>....s...
+000002e0: 0006 050c 0210 03                        .......
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/_enums.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/_enums.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/_models.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/models/_patch.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 2289 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 f108 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 f108 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 8109 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 ad1f 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 ad1f 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6404 6c0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  d.l.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_patch.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/models/__pycache__/_patch.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 675 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 a302 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 a302 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6700 5a03 6502 6504 1900 6505 6403 3c00  g.Z.e.e...e.d.<.
 00000050: 6404 6405 8400 5a06 6406 5300 2907 7a7b  d.d...Z.d.S.).z{
 00000060: 4375 7374 6f6d 697a 6520 6765 6e65 7261  Customize genera
 00000070: 7465 6420 636f 6465 2068 6572 652e 0a0a  ted code here...
@@ -27,21 +27,21 @@
 000001a0: 6820 7573 696e 6720 7468 6520 7465 6368  h using the tech
 000001b0: 6e69 7175 6573 2064 6573 6372 6962 6564  niques described
 000001c0: 2069 6e0a 2020 2020 6874 7470 733a 2f2f   in.    https://
 000001d0: 616b 612e 6d73 2f61 7a73 646b 2f70 7974  aka.ms/azsdk/pyt
 000001e0: 686f 6e2f 6470 636f 6465 6765 6e2f 7079  hon/dpcodegen/py
 000001f0: 7468 6f6e 2f63 7573 746f 6d69 7a65 0a20  thon/customize. 
 00000200: 2020 204e a900 7204 0000 0072 0400 0000     N..r....r....
-00000210: 7204 0000 00fa 4f2f 776f 726b 2f6b 7566  r.....O/work/kuf
+00000210: 7204 0000 00fa 4b2f 776f 726b 2f6b 7566  r.....K/work/kuf
 00000220: 6c6f 772d 7364 6b2d 7079 7468 6f6e 2f6b  low-sdk-python/k
 00000230: 7566 6c6f 772d 7265 7374 2f6b 7566 6c6f  uflow-rest/kuflo
 00000240: 775f 7265 7374 2f5f 6765 6e65 7261 7465  w_rest/_generate
-00000250: 642f 6f70 6572 6174 696f 6e73 2f5f 7061  d/operations/_pa
-00000260: 7463 682e 7079 da09 7061 7463 685f 7364  tch.py..patch_sd
-00000270: 6b0f 0000 0073 0200 0000 0001 7206 0000  k....s......r...
-00000280: 004e 2907 da07 5f5f 646f 635f 5fda 0674  .N)...__doc__..t
-00000290: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
-000002a0: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-000002b0: 6f6e 735f 5f72 0600 0000 7204 0000 0072  ons__r....r....r
-000002c0: 0400 0000 7204 0000 0072 0500 0000 da08  ....r....r......
-000002d0: 3c6d 6f64 756c 653e 0500 0000 7306 0000  <module>....s...
-000002e0: 0006 050c 0210 03                        .......
+00000250: 642f 6d6f 6465 6c73 2f5f 7061 7463 682e  d/models/_patch.
+00000260: 7079 da09 7061 7463 685f 7364 6b0f 0000  py..patch_sdk...
+00000270: 0073 0200 0000 0001 7206 0000 004e 2907  .s......r....N).
+00000280: da07 5f5f 646f 635f 5fda 0674 7970 696e  ..__doc__..typin
+00000290: 6772 0200 0000 7203 0000 00da 0373 7472  gr....r......str
+000002a0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+000002b0: 5f72 0600 0000 7204 0000 0072 0400 0000  _r....r....r....
+000002c0: 7204 0000 0072 0500 0000 da08 3c6d 6f64  r....r......<mod
+000002d0: 756c 653e 0500 0000 7306 0000 0006 050c  ule>....s.......
+000002e0: 0210 03                                  ...
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 10642 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 9229 0000  U........*.f.)..
+00000000: 550d 0d0a 0000 0000 5143 2a66 9229 0000  U.......QC*f.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6403 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 0100 6400  m.Z.m.Z.m.Z...d.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 56895 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 3fde 0000  U........*.f?...
+00000000: 550d 0d0a 0000 0000 5143 2a66 3fde 0000  U.......QC*f?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 3602 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 0100 6400 6404 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_robot_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_robot_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 17153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 0143 0000  U........*.f.C..
+00000000: 550d 0d0a 0000 0000 5143 2a66 0143 0000  U.......QC*f.C..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 b201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6403 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 79296 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 c035 0100  U........*.f.5..
+00000000: 550d 0d0a 0000 0000 5143 2a66 c035 0100  U.......QC*f.5..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 cc02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 0100 6400 6404 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_tenant_user_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_tenant_user_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 10587 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 5b29 0000  U........*.f[)..
+00000000: 550d 0d0a 0000 0000 5143 2a66 5b29 0000  U.......QC*f[)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 6601 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 6400 6404 6c10  m.Z.m.Z...d.d.l.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/__pycache__/_worker_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/__pycache__/_worker_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 8311 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 7720 0000  U........*.fw ..
+00000000: 550d 0d0a 0000 0000 5143 2a66 7720 0000  U.......QC*fw ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6404 6c0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  d.l.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_authentication_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_patch.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_principal_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_process_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_process_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_robot_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_robot_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_task_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_tenant_user_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_tenant_user_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_generated/operations/_worker_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/_generated/operations/_worker_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/_kuflow_rest_client.py` & `kuflow_rest-1.5.1/kuflow_rest/_kuflow_rest_client.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/models/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 5686 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 3616 0000  U........*.f6...
+00000000: 550d 0d0a 0000 0000 5143 2a66 3616 0000  U.......QC*f6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 004f 0000 0040 0000 0073 1602 0000 6400  .O...@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/models/__pycache__/_models.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 3986 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 920f 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 920f 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 4700 6406 6407 8400  ..d...Z.G.d.d...
 00000060: 6407 8302 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
 00000070: 8302 5a07 4700 640a 640b 8400 640b 8302  ..Z.G.d.d...d...
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/models/_models.py` & `kuflow_rest-1.5.1/kuflow_rest/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 1674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 8a06 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 8a06 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_authentication_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 2330 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 1a09 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 1a09 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6402 6404 6c02 6d05 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 8302 5a07  ..G.d.d...d...Z.
 00000060: 6407 5300 2908 e900 0000 0029 01da 0341  d.S.)......)...A
 00000070: 6e79 e902 0000 0029 01da 104b 7546 6c6f  ny.....)...KuFlo
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_principal_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 4463 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 6f11 0000  U........*.fo...
+00000000: 550d 0d0a 0000 0000 5143 2a66 6f11 0000  U.......QC*fo...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d08 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a0a 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 04da 0341 6e79 da04  )......)...Any..
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_process_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 12882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 5232 0000  U........*.fR2..
+00000000: 550d 0d0a 0000 0000 5143 2a66 1933 0000  U.......QC*f.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6402  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c07 6d08 5a09 0100 6402 6404 6c0a  d.l.m.Z...d.d.l.
 00000060: 6d0b 5a0c 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 8302 5a0d 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
@@ -551,218 +551,225 @@
 00002260: 6f63 6573 735f 7361 7665 5f75 7365 725f  ocess_save_user_
 00002270: 6163 7469 6f6e 5f76 616c 7565 5f64 6f63  action_value_doc
 00002280: 756d 656e 747a 1061 7070 6c69 6361 7469  umentz.applicati
 00002290: 6f6e 2f6a 736f 6e29 0172 2e00 0000 2905  on/json).r....).
 000022a0: 721e 0000 0072 2100 0000 722e 0000 0072  r....r!...r....r
 000022b0: 1700 0000 7218 0000 0063 0300 0000 0000  ....r....c......
 000022c0: 0000 0100 0000 0500 0000 0600 0000 4b00  ..............K.
-000022d0: 0000 7314 0000 007c 006a 006a 01a0 027c  ..s....|.j.j...|
-000022e0: 017c 027c 037c 04a1 0453 0029 0161 b902  .|.|.|...S.).a..
-000022f0: 0000 5361 7665 204a 534f 4e20 6461 7461  ..Save JSON data
-00002300: 2e0a 0a20 2020 2020 2020 2041 6c6c 6f77  ...        Allow
-00002310: 2074 6f20 7361 7665 2061 204a 534f 4e20   to save a JSON 
-00002320: 7661 6c69 6461 7469 6e67 2074 6861 7420  validating that 
-00002330: 7468 6520 6461 7461 2066 6f6c 6c6f 7720  the data follow 
-00002340: 7468 6520 7265 6c61 7465 6420 7363 6865  the related sche
-00002350: 6d61 2e20 4966 2074 6865 2064 6174 6120  ma. If the data 
-00002360: 6973 0a20 2020 2020 2020 2069 6e76 616c  is.        inval
-00002370: 6964 2c20 7468 656e 0a20 2020 2020 2020  id, then.       
-00002380: 2074 6865 206a 736f 6e20 666f 726d 2069   the json form i
-00002390: 7320 6d61 726b 6564 2061 7320 696e 7661  s marked as inva
-000023a0: 6c69 642e 0a0a 2020 2020 2020 2020 3a70  lid...        :p
-000023b0: 6172 616d 2069 643a 2054 6865 2072 6573  aram id: The res
-000023c0: 6f75 7263 6520 4944 2e20 5265 7175 6972  ource ID. Requir
-000023d0: 6564 2e0a 2020 2020 2020 2020 3a74 7970  ed..        :typ
-000023e0: 6520 6964 3a20 7374 720a 2020 2020 2020  e id: str.      
-000023f0: 2020 3a70 6172 616d 2063 6f6d 6d61 6e64    :param command
-00002400: 3a20 436f 6d6d 616e 6420 746f 2073 6176  : Command to sav
-00002410: 6520 7468 6520 4a53 4f4e 2076 616c 7565  e the JSON value
-00002420: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
-00002430: 2020 2020 3a74 7970 6520 636f 6d6d 616e      :type comman
-00002440: 643a 207e 6b75 666c 6f77 2e72 6573 742e  d: ~kuflow.rest.
-00002450: 6d6f 6465 6c73 2e50 726f 6365 7373 5361  models.ProcessSa
-00002460: 7665 456e 7469 7479 4461 7461 436f 6d6d  veEntityDataComm
-00002470: 616e 640a 2020 2020 2020 2020 3a6b 6579  and.        :key
-00002480: 776f 7264 2063 6f6e 7465 6e74 5f74 7970  word content_typ
-00002490: 653a 2042 6f64 7920 5061 7261 6d65 7465  e: Body Paramete
-000024a0: 7220 636f 6e74 656e 742d 7479 7065 2e20  r content-type. 
-000024b0: 436f 6e74 656e 7420 7479 7065 2070 6172  Content type par
-000024c0: 616d 6574 6572 2066 6f72 204a 534f 4e20  ameter for JSON 
-000024d0: 626f 6479 2e0a 2020 2020 2020 2020 2044  body..         D
-000024e0: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
-000024f0: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
-00002500: 6e22 2e0a 2020 2020 2020 2020 3a74 7970  n"..        :typ
-00002510: 6520 636f 6e74 656e 745f 7479 7065 3a20  e content_type: 
-00002520: 7374 720a 2020 2020 2020 2020 3a72 6574  str.        :ret
-00002530: 7572 6e3a 2050 726f 6365 7373 0a20 2020  urn: Process.   
-00002540: 2020 2020 203a 7274 7970 653a 207e 6b75       :rtype: ~ku
-00002550: 666c 6f77 2e72 6573 742e 6d6f 6465 6c73  flow.rest.models
-00002560: 2e50 726f 6365 7373 0a20 2020 2020 2020  .Process.       
-00002570: 203a 7261 6973 6573 207e 617a 7572 652e   :raises ~azure.
-00002580: 636f 7265 2e65 7863 6570 7469 6f6e 732e  core.exceptions.
-00002590: 4874 7470 5265 7370 6f6e 7365 4572 726f  HttpResponseErro
-000025a0: 723a 0a20 2020 2020 2020 2029 0372 0d00  r:.        ).r..
-000025b0: 0000 721b 0000 00da 2061 6374 696f 6e73  ..r..... actions
-000025c0: 5f70 726f 6365 7373 5f73 6176 655f 656e  _process_save_en
-000025d0: 7469 7479 5f64 6174 6129 0572 0e00 0000  tity_data).r....
-000025e0: 721e 0000 0072 2100 0000 722e 0000 0072  r....r!...r....r
-000025f0: 1700 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00002600: 0000 0072 2f00 0000 f800 0000 7302 0000  ...r/.......s...
-00002610: 0000 197a 3250 726f 6365 7373 4f70 6572  ...z2ProcessOper
-00002620: 6174 696f 6e73 2e61 6374 696f 6e73 5f70  ations.actions_p
-00002630: 726f 6365 7373 5f73 6176 655f 656e 7469  rocess_save_enti
-00002640: 7479 5f64 6174 6129 0772 1e00 0000 7229  ty_data).r....r)
-00002650: 0000 0072 2a00 0000 722b 0000 00da 0b73  ...r*...r+.....s
-00002660: 6368 656d 615f 7061 7468 7217 0000 0072  chema_pathr....r
-00002670: 1800 0000 6303 0000 0000 0000 0003 0000  ....c...........
-00002680: 0007 0000 0008 0000 004b 0000 0073 1800  .........K...s..
-00002690: 0000 7c00 6a00 6a01 a002 7c01 7c02 7c03  ..|.j.j...|.|.|.
-000026a0: 7c04 7c05 7c06 a106 5300 2901 6144 0300  |.|.|...S.).aD..
-000026b0: 0053 6176 6520 616e 2065 6e74 6974 7920  .Save an entity 
-000026c0: 7661 6c75 6520 646f 6375 6d65 6e74 2e0a  value document..
-000026d0: 0a20 2020 2020 2020 2053 6176 6520 6120  .        Save a 
-000026e0: 646f 6375 6d65 6e74 2069 6e20 7468 6520  document in the 
-000026f0: 7072 6f63 6573 7320 746f 206c 6174 6572  process to later
-00002700: 2062 6520 6c69 6e6b 6564 2069 6e74 6f20   be linked into 
-00002710: 7468 6520 4a53 4f4e 2064 6174 612e 0a0a  the JSON data...
-00002720: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00002730: 643a 2054 6865 2072 6573 6f75 7263 6520  d: The resource 
-00002740: 4944 2e20 5265 7175 6972 6564 2e0a 2020  ID. Required..  
-00002750: 2020 2020 2020 3a74 7970 6520 6964 3a20        :type id: 
-00002760: 7374 720a 2020 2020 2020 2020 3a70 6172  str.        :par
-00002770: 616d 2066 696c 653a 2044 6f63 756d 656e  am file: Documen
-00002780: 7420 746f 2073 6176 652e 2052 6571 7569  t to save. Requi
-00002790: 7265 642e 0a20 2020 2020 2020 203a 7479  red..        :ty
-000027a0: 7065 2066 696c 653a 2049 4f5b 6279 7465  pe file: IO[byte
-000027b0: 735d 0a20 2020 2020 2020 203a 6b65 7977  s].        :keyw
-000027c0: 6f72 6420 6669 6c65 5f63 6f6e 7465 6e74  ord file_content
-000027d0: 5f74 7970 653a 2044 6f63 756d 656e 7420  _type: Document 
-000027e0: 636f 6e74 656e 7420 7479 7065 2e20 5265  content type. Re
-000027f0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-00002800: 3a74 7970 6520 6669 6c65 5f63 6f6e 7465  :type file_conte
-00002810: 6e74 5f74 7970 653a 2073 7472 0a20 2020  nt_type: str.   
-00002820: 2020 2020 203a 6b65 7977 6f72 6420 6669       :keyword fi
-00002830: 6c65 5f6e 616d 653a 2044 6f63 756d 656e  le_name: Documen
-00002840: 7420 6e61 6d65 2e20 5265 7175 6972 6564  t name. Required
-00002850: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00002860: 6669 6c65 5f6e 616d 653a 2073 7472 0a20  file_name: str. 
-00002870: 2020 2020 2020 203a 6b65 7977 6f72 6420         :keyword 
-00002880: 7363 6865 6d61 5f70 6174 683a 204a 534f  schema_path: JSO
-00002890: 4e20 5363 6865 6d61 2070 6174 6820 7265  N Schema path re
-000028a0: 6c61 7465 6420 746f 2074 6865 2064 6f63  lated to the doc
-000028b0: 756d 656e 742e 2054 6865 2075 706c 6f61  ument. The uploa
-000028c0: 6465 6420 646f 6375 6d65 6e74 2077 696c  ded document wil
-000028d0: 6c20 6265 0a20 2020 2020 2020 2020 7661  l be.         va
-000028e0: 6c69 6461 7465 6420 6279 2074 6865 2070  lidated by the p
-000028f0: 6173 7365 6420 7363 6865 6d61 2070 6174  assed schema pat
-00002900: 682e 2052 6571 7569 7265 642e 0a20 2020  h. Required..   
-00002910: 2020 2020 203a 7479 7065 2073 6368 656d       :type schem
-00002920: 615f 7061 7468 3a20 7374 720a 2020 2020  a_path: str.    
-00002930: 2020 2020 3a72 6574 7572 6e3a 2050 726f      :return: Pro
-00002940: 6365 7373 5361 7665 456e 7469 7479 446f  cessSaveEntityDo
-00002950: 6375 6d65 6e74 5265 7370 6f6e 7365 436f  cumentResponseCo
-00002960: 6d6d 616e 640a 2020 2020 2020 2020 3a72  mmand.        :r
-00002970: 7479 7065 3a20 7e6b 7566 6c6f 772e 7265  type: ~kuflow.re
-00002980: 7374 2e6d 6f64 656c 732e 5072 6f63 6573  st.models.Proces
-00002990: 7353 6176 6545 6e74 6974 7944 6f63 756d  sSaveEntityDocum
-000029a0: 656e 7452 6573 706f 6e73 6543 6f6d 6d61  entResponseComma
-000029b0: 6e64 0a20 2020 2020 2020 203a 7261 6973  nd.        :rais
-000029c0: 6573 207e 617a 7572 652e 636f 7265 2e65  es ~azure.core.e
-000029d0: 7863 6570 7469 6f6e 732e 4874 7470 5265  xceptions.HttpRe
-000029e0: 7370 6f6e 7365 4572 726f 723a 0a20 2020  sponseError:.   
-000029f0: 2020 2020 2029 0372 0d00 0000 721b 0000       ).r....r...
-00002a00: 00da 2461 6374 696f 6e73 5f70 726f 6365  ..$actions_proce
-00002a10: 7373 5f73 6176 655f 656e 7469 7479 5f64  ss_save_entity_d
-00002a20: 6f63 756d 656e 7429 0772 0e00 0000 721e  ocument).r....r.
-00002a30: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00002a40: 0000 7230 0000 0072 1700 0000 720f 0000  ..r0...r....r...
-00002a50: 0072 0f00 0000 7210 0000 0072 3100 0000  .r....r....r1...
-00002a60: 1301 0000 7310 0000 0000 1608 0102 0002  ....s...........
-00002a70: 0002 0002 0002 0002 ff7a 3650 726f 6365  .........z6Proce
-00002a80: 7373 4f70 6572 6174 696f 6e73 2e61 6374  ssOperations.act
-00002a90: 696f 6e73 5f70 726f 6365 7373 5f73 6176  ions_process_sav
-00002aa0: 655f 656e 7469 7479 5f64 6f63 756d 656e  e_entity_documen
-00002ab0: 7429 0472 1e00 0000 da0c 646f 6375 6d65  t).r......docume
-00002ac0: 6e74 5f75 7269 7217 0000 0072 1800 0000  nt_urir....r....
-00002ad0: 6302 0000 0000 0000 0001 0000 0004 0000  c...............
-00002ae0: 0005 0000 004b 0000 0073 1200 0000 7c00  .....K...s....|.
-00002af0: 6a00 6a01 a002 7c01 7c02 7c03 a103 5300  j.j...|.|.|...S.
-00002b00: 2901 617f 0100 0044 6f77 6e6c 6f61 6420  ).a....Download 
-00002b10: 646f 6375 6d65 6e74 2e0a 0a20 2020 2020  document...     
-00002b20: 2020 2047 6976 656e 2061 2070 726f 6365     Given a proce
-00002b30: 7373 2061 6e64 2061 2064 6f63 756d 656e  ss and a documen
-00002b40: 7455 7269 2c20 646f 776e 6c6f 6164 2061  tUri, download a
-00002b50: 2064 6f63 756d 656e 742e 0a0a 2020 2020   document...    
-00002b60: 2020 2020 3a70 6172 616d 2069 643a 2054      :param id: T
-00002b70: 6865 2072 6573 6f75 7263 6520 4944 2e20  he resource ID. 
-00002b80: 5265 7175 6972 6564 2e0a 2020 2020 2020  Required..      
-00002b90: 2020 3a74 7970 6520 6964 3a20 7374 720a    :type id: str.
-00002ba0: 2020 2020 2020 2020 3a6b 6579 776f 7264          :keyword
-00002bb0: 2064 6f63 756d 656e 745f 7572 693a 2044   document_uri: D
-00002bc0: 6f63 756d 656e 7420 5552 4920 746f 2064  ocument URI to d
-00002bd0: 6f77 6e6c 6f61 642e 2052 6571 7569 7265  ownload. Require
-00002be0: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
-00002bf0: 2064 6f63 756d 656e 745f 7572 693a 2073   document_uri: s
-00002c00: 7472 0a20 2020 2020 2020 203a 7265 7475  tr.        :retu
-00002c10: 726e 3a20 4974 6572 6174 6f72 5b62 7974  rn: Iterator[byt
-00002c20: 6573 5d0a 2020 2020 2020 2020 3a72 7479  es].        :rty
-00002c30: 7065 3a20 4974 6572 6174 6f72 5b62 7974  pe: Iterator[byt
-00002c40: 6573 5d0a 2020 2020 2020 2020 3a72 6169  es].        :rai
-00002c50: 7365 7320 7e61 7a75 7265 2e63 6f72 652e  ses ~azure.core.
-00002c60: 6578 6365 7074 696f 6e73 2e48 7474 7052  exceptions.HttpR
-00002c70: 6573 706f 6e73 6545 7272 6f72 3a0a 2020  esponseError:.  
-00002c80: 2020 2020 2020 2903 720d 0000 0072 1b00        ).r....r..
-00002c90: 0000 da28 6163 7469 6f6e 735f 7072 6f63  ...(actions_proc
-00002ca0: 6573 735f 646f 776e 6c6f 6164 5f65 6e74  ess_download_ent
-00002cb0: 6974 795f 646f 6375 6d65 6e74 2904 720e  ity_document).r.
-00002cc0: 0000 0072 1e00 0000 7232 0000 0072 1700  ...r....r2...r..
-00002cd0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00002ce0: 0072 3300 0000 2d01 0000 7302 0000 0000  .r3...-...s.....
-00002cf0: 0d7a 3a50 726f 6365 7373 4f70 6572 6174  .z:ProcessOperat
-00002d00: 696f 6e73 2e61 6374 696f 6e73 5f70 726f  ions.actions_pro
-00002d10: 6365 7373 5f64 6f77 6e6c 6f61 645f 656e  cess_download_en
-00002d20: 7469 7479 5f64 6f63 756d 656e 7429 0472  tity_document).r
-00002d30: 1200 0000 7201 0000 004e 4e29 25da 085f  ....r....NN)%.._
-00002d40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00002d50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00002d60: 5fda 075f 5f64 6f63 5f5f da19 4b75 466c  _..__doc__..KuFl
-00002d70: 6f77 5265 7374 436c 6965 6e74 4765 6e65  owRestClientGene
-00002d80: 7261 7465 6472 1100 0000 da03 696e 7472  ratedr......intr
-00002d90: 0600 0000 7207 0000 0072 1a00 0000 7205  ....r....r....r.
-00002da0: 0000 0072 0300 0000 da07 5f6d 6f64 656c  ...r......_model
-00002db0: 73da 0b50 726f 6365 7373 5061 6765 721c  s..ProcessPager.
-00002dc0: 0000 00da 0750 726f 6365 7373 721d 0000  .....Processr...
-00002dd0: 0072 1f00 0000 da1d 5072 6f63 6573 7343  .r......ProcessC
-00002de0: 6861 6e67 6549 6e69 7469 6174 6f72 436f  hangeInitiatorCo
-00002df0: 6d6d 616e 6472 2300 0000 da19 5072 6f63  mmandr#.....Proc
-00002e00: 6573 7353 6176 6545 6c65 6d65 6e74 436f  essSaveElementCo
-00002e10: 6d6d 616e 6472 2500 0000 da1b 5072 6f63  mmandr%.....Proc
-00002e20: 6573 7344 656c 6574 6545 6c65 6d65 6e74  essDeleteElement
-00002e30: 436f 6d6d 616e 6472 2600 0000 7227 0000  Commandr&...r'..
-00002e40: 0072 2800 0000 5a08 446f 6375 6d65 6e74  .r(...Z.Document
-00002e50: 5a29 5072 6f63 6573 7353 6176 6555 7365  Z)ProcessSaveUse
-00002e60: 7241 6374 696f 6e56 616c 7565 446f 6375  rActionValueDocu
-00002e70: 6d65 6e74 436f 6d6d 616e 6472 2d00 0000  mentCommandr-...
-00002e80: da1c 5072 6f63 6573 7353 6176 6545 6e74  ..ProcessSaveEnt
-00002e90: 6974 7944 6174 6143 6f6d 6d61 6e64 722f  ityDataCommandr/
-00002ea0: 0000 0072 0200 0000 da05 6279 7465 73da  ...r......bytes.
-00002eb0: 2850 726f 6365 7373 5361 7665 456e 7469  (ProcessSaveEnti
-00002ec0: 7479 446f 6375 6d65 6e74 5265 7370 6f6e  tyDocumentRespon
-00002ed0: 7365 436f 6d6d 616e 6472 3100 0000 7204  seCommandr1...r.
-00002ee0: 0000 0072 3300 0000 720f 0000 0072 0f00  ...r3...r....r..
-00002ef0: 0000 720f 0000 0072 1000 0000 720b 0000  ..r....r....r...
-00002f00: 001f 0000 0073 7000 0000 0801 0409 0e05  .....sp.........
-00002f10: 0001 0001 0001 00fb 0202 0201 0201 1201  ................
-00002f20: 1201 0201 04f9 0c29 1619 140e 0200 0400  .......)........
-00002f30: 0201 04fe 0c16 0200 0400 0201 04fe 0c18  ................
-00002f40: 0200 0400 0201 04fe 0c13 140f 1413 0201  ................
-00002f50: 0401 0401 0201 08fa 0c23 02fb 0402 0201  .........#......
-00002f60: 0402 0201 0201 04f9 0c1c 0200 0600 0200  ................
-00002f70: 0200 0200 0201 04fe 0c1a 720b 0000 004e  ..........r....N
-00002f80: 290e da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
-00002f90: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
-00002fa0: 0000 0072 0700 0000 da00 7209 0000 0072  ...r......r....r
-00002fb0: 3a00 0000 da0a 5f67 656e 6572 6174 6564  :....._generated
-00002fc0: 720a 0000 0072 3800 0000 720b 0000 0072  r....r8...r....r
-00002fd0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00002fe0: 0000 00da 083c 6d6f 6475 6c65 3e19 0000  .....<module>...
-00002ff0: 0073 0600 0000 2002 0c01 0c03            .s.... .....
+000022d0: 0000 731c 0000 007c 006a 006a 016a 0266  ..s....|.j.j.j.f
+000022e0: 007c 017c 027c 0364 019c 037c 0497 028e  .|.|.|.d...|....
+000022f0: 0153 0029 0261 b902 0000 5361 7665 204a  .S.).a....Save J
+00002300: 534f 4e20 6461 7461 2e0a 0a20 2020 2020  SON data...     
+00002310: 2020 2041 6c6c 6f77 2074 6f20 7361 7665     Allow to save
+00002320: 2061 204a 534f 4e20 7661 6c69 6461 7469   a JSON validati
+00002330: 6e67 2074 6861 7420 7468 6520 6461 7461  ng that the data
+00002340: 2066 6f6c 6c6f 7720 7468 6520 7265 6c61   follow the rela
+00002350: 7465 6420 7363 6865 6d61 2e20 4966 2074  ted schema. If t
+00002360: 6865 2064 6174 6120 6973 0a20 2020 2020  he data is.     
+00002370: 2020 2069 6e76 616c 6964 2c20 7468 656e     invalid, then
+00002380: 0a20 2020 2020 2020 2074 6865 206a 736f  .        the jso
+00002390: 6e20 666f 726d 2069 7320 6d61 726b 6564  n form is marked
+000023a0: 2061 7320 696e 7661 6c69 642e 0a0a 2020   as invalid...  
+000023b0: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
+000023c0: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
+000023d0: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
+000023e0: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
+000023f0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+00002400: 2063 6f6d 6d61 6e64 3a20 436f 6d6d 616e   command: Comman
+00002410: 6420 746f 2073 6176 6520 7468 6520 4a53  d to save the JS
+00002420: 4f4e 2076 616c 7565 2e20 5265 7175 6972  ON value. Requir
+00002430: 6564 2e0a 2020 2020 2020 2020 3a74 7970  ed..        :typ
+00002440: 6520 636f 6d6d 616e 643a 207e 6b75 666c  e command: ~kufl
+00002450: 6f77 2e72 6573 742e 6d6f 6465 6c73 2e50  ow.rest.models.P
+00002460: 726f 6365 7373 5361 7665 456e 7469 7479  rocessSaveEntity
+00002470: 4461 7461 436f 6d6d 616e 640a 2020 2020  DataCommand.    
+00002480: 2020 2020 3a6b 6579 776f 7264 2063 6f6e      :keyword con
+00002490: 7465 6e74 5f74 7970 653a 2042 6f64 7920  tent_type: Body 
+000024a0: 5061 7261 6d65 7465 7220 636f 6e74 656e  Parameter conten
+000024b0: 742d 7479 7065 2e20 436f 6e74 656e 7420  t-type. Content 
+000024c0: 7479 7065 2070 6172 616d 6574 6572 2066  type parameter f
+000024d0: 6f72 204a 534f 4e20 626f 6479 2e0a 2020  or JSON body..  
+000024e0: 2020 2020 2020 2044 6566 6175 6c74 2076         Default v
+000024f0: 616c 7565 2069 7320 2261 7070 6c69 6361  alue is "applica
+00002500: 7469 6f6e 2f6a 736f 6e22 2e0a 2020 2020  tion/json"..    
+00002510: 2020 2020 3a74 7970 6520 636f 6e74 656e      :type conten
+00002520: 745f 7479 7065 3a20 7374 720a 2020 2020  t_type: str.    
+00002530: 2020 2020 3a72 6574 7572 6e3a 2050 726f      :return: Pro
+00002540: 6365 7373 0a20 2020 2020 2020 203a 7274  cess.        :rt
+00002550: 7970 653a 207e 6b75 666c 6f77 2e72 6573  ype: ~kuflow.res
+00002560: 742e 6d6f 6465 6c73 2e50 726f 6365 7373  t.models.Process
+00002570: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+00002580: 207e 617a 7572 652e 636f 7265 2e65 7863   ~azure.core.exc
+00002590: 6570 7469 6f6e 732e 4874 7470 5265 7370  eptions.HttpResp
+000025a0: 6f6e 7365 4572 726f 723a 0a20 2020 2020  onseError:.     
+000025b0: 2020 2029 0372 1e00 0000 7221 0000 0072     ).r....r!...r
+000025c0: 2e00 0000 2903 720d 0000 0072 1b00 0000  ....).r....r....
+000025d0: da20 6163 7469 6f6e 735f 7072 6f63 6573  . actions_proces
+000025e0: 735f 7361 7665 5f65 6e74 6974 795f 6461  s_save_entity_da
+000025f0: 7461 2905 720e 0000 0072 1e00 0000 7221  ta).r....r....r!
+00002600: 0000 0072 2e00 0000 7217 0000 0072 0f00  ...r....r....r..
+00002610: 0000 720f 0000 0072 1000 0000 722f 0000  ..r....r....r/..
+00002620: 00f8 0000 0073 0e00 0000 0019 0a01 0200  .....s..........
+00002630: 0200 02ff 0401 02ff 7a32 5072 6f63 6573  ........z2Proces
+00002640: 734f 7065 7261 7469 6f6e 732e 6163 7469  sOperations.acti
+00002650: 6f6e 735f 7072 6f63 6573 735f 7361 7665  ons_process_save
+00002660: 5f65 6e74 6974 795f 6461 7461 2907 721e  _entity_data).r.
+00002670: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00002680: 0000 da0b 7363 6865 6d61 5f70 6174 6872  ....schema_pathr
+00002690: 1700 0000 7218 0000 0063 0300 0000 0000  ....r....c......
+000026a0: 0000 0300 0000 0700 0000 0800 0000 4b00  ..............K.
+000026b0: 0000 7320 0000 007c 006a 006a 016a 0266  ..s ...|.j.j.j.f
+000026c0: 007c 017c 027c 037c 047c 0564 019c 057c  .|.|.|.|.|.d...|
+000026d0: 0697 028e 0153 0029 0261 4403 0000 5361  .....S.).aD...Sa
+000026e0: 7665 2061 6e20 656e 7469 7479 2076 616c  ve an entity val
+000026f0: 7565 2064 6f63 756d 656e 742e 0a0a 2020  ue document...  
+00002700: 2020 2020 2020 5361 7665 2061 2064 6f63        Save a doc
+00002710: 756d 656e 7420 696e 2074 6865 2070 726f  ument in the pro
+00002720: 6365 7373 2074 6f20 6c61 7465 7220 6265  cess to later be
+00002730: 206c 696e 6b65 6420 696e 746f 2074 6865   linked into the
+00002740: 204a 534f 4e20 6461 7461 2e0a 0a20 2020   JSON data...   
+00002750: 2020 2020 203a 7061 7261 6d20 6964 3a20       :param id: 
+00002760: 5468 6520 7265 736f 7572 6365 2049 442e  The resource ID.
+00002770: 2052 6571 7569 7265 642e 0a20 2020 2020   Required..     
+00002780: 2020 203a 7479 7065 2069 643a 2073 7472     :type id: str
+00002790: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000027a0: 6669 6c65 3a20 446f 6375 6d65 6e74 2074  file: Document t
+000027b0: 6f20 7361 7665 2e20 5265 7175 6972 6564  o save. Required
+000027c0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+000027d0: 6669 6c65 3a20 494f 5b62 7974 6573 5d0a  file: IO[bytes].
+000027e0: 2020 2020 2020 2020 3a6b 6579 776f 7264          :keyword
+000027f0: 2066 696c 655f 636f 6e74 656e 745f 7479   file_content_ty
+00002800: 7065 3a20 446f 6375 6d65 6e74 2063 6f6e  pe: Document con
+00002810: 7465 6e74 2074 7970 652e 2052 6571 7569  tent type. Requi
+00002820: 7265 642e 0a20 2020 2020 2020 203a 7479  red..        :ty
+00002830: 7065 2066 696c 655f 636f 6e74 656e 745f  pe file_content_
+00002840: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+00002850: 2020 3a6b 6579 776f 7264 2066 696c 655f    :keyword file_
+00002860: 6e61 6d65 3a20 446f 6375 6d65 6e74 206e  name: Document n
+00002870: 616d 652e 2052 6571 7569 7265 642e 0a20  ame. Required.. 
+00002880: 2020 2020 2020 203a 7479 7065 2066 696c         :type fil
+00002890: 655f 6e61 6d65 3a20 7374 720a 2020 2020  e_name: str.    
+000028a0: 2020 2020 3a6b 6579 776f 7264 2073 6368      :keyword sch
+000028b0: 656d 615f 7061 7468 3a20 4a53 4f4e 2053  ema_path: JSON S
+000028c0: 6368 656d 6120 7061 7468 2072 656c 6174  chema path relat
+000028d0: 6564 2074 6f20 7468 6520 646f 6375 6d65  ed to the docume
+000028e0: 6e74 2e20 5468 6520 7570 6c6f 6164 6564  nt. The uploaded
+000028f0: 2064 6f63 756d 656e 7420 7769 6c6c 2062   document will b
+00002900: 650a 2020 2020 2020 2020 2076 616c 6964  e.         valid
+00002910: 6174 6564 2062 7920 7468 6520 7061 7373  ated by the pass
+00002920: 6564 2073 6368 656d 6120 7061 7468 2e20  ed schema path. 
+00002930: 5265 7175 6972 6564 2e0a 2020 2020 2020  Required..      
+00002940: 2020 3a74 7970 6520 7363 6865 6d61 5f70    :type schema_p
+00002950: 6174 683a 2073 7472 0a20 2020 2020 2020  ath: str.       
+00002960: 203a 7265 7475 726e 3a20 5072 6f63 6573   :return: Proces
+00002970: 7353 6176 6545 6e74 6974 7944 6f63 756d  sSaveEntityDocum
+00002980: 656e 7452 6573 706f 6e73 6543 6f6d 6d61  entResponseComma
+00002990: 6e64 0a20 2020 2020 2020 203a 7274 7970  nd.        :rtyp
+000029a0: 653a 207e 6b75 666c 6f77 2e72 6573 742e  e: ~kuflow.rest.
+000029b0: 6d6f 6465 6c73 2e50 726f 6365 7373 5361  models.ProcessSa
+000029c0: 7665 456e 7469 7479 446f 6375 6d65 6e74  veEntityDocument
+000029d0: 5265 7370 6f6e 7365 436f 6d6d 616e 640a  ResponseCommand.
+000029e0: 2020 2020 2020 2020 3a72 6169 7365 7320          :raises 
+000029f0: 7e61 7a75 7265 2e63 6f72 652e 6578 6365  ~azure.core.exce
+00002a00: 7074 696f 6e73 2e48 7474 7052 6573 706f  ptions.HttpRespo
+00002a10: 6e73 6545 7272 6f72 3a0a 2020 2020 2020  nseError:.      
+00002a20: 2020 2905 721e 0000 0072 2900 0000 722a    ).r....r)...r*
+00002a30: 0000 0072 2b00 0000 7230 0000 0029 0372  ...r+...r0...).r
+00002a40: 0d00 0000 721b 0000 00da 2461 6374 696f  ....r.....$actio
+00002a50: 6e73 5f70 726f 6365 7373 5f73 6176 655f  ns_process_save_
+00002a60: 656e 7469 7479 5f64 6f63 756d 656e 7429  entity_document)
+00002a70: 0772 0e00 0000 721e 0000 0072 2900 0000  .r....r....r)...
+00002a80: 722a 0000 0072 2b00 0000 7230 0000 0072  r*...r+...r0...r
+00002a90: 1700 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00002aa0: 0000 0072 3100 0000 1501 0000 7312 0000  ...r1.......s...
+00002ab0: 0000 160a 0102 0102 0102 0102 0102 fb04  ................
+00002ac0: 0602 fa7a 3650 726f 6365 7373 4f70 6572  ...z6ProcessOper
+00002ad0: 6174 696f 6e73 2e61 6374 696f 6e73 5f70  ations.actions_p
+00002ae0: 726f 6365 7373 5f73 6176 655f 656e 7469  rocess_save_enti
+00002af0: 7479 5f64 6f63 756d 656e 7429 0472 1e00  ty_document).r..
+00002b00: 0000 da0c 646f 6375 6d65 6e74 5f75 7269  ....document_uri
+00002b10: 7217 0000 0072 1800 0000 6302 0000 0000  r....r....c.....
+00002b20: 0000 0001 0000 0004 0000 0005 0000 004b  ...............K
+00002b30: 0000 0073 1a00 0000 7c00 6a00 6a01 6a02  ...s....|.j.j.j.
+00002b40: 6600 7c01 7c02 6401 9c02 7c03 9702 8e01  f.|.|.d...|.....
+00002b50: 5300 2902 617f 0100 0044 6f77 6e6c 6f61  S.).a....Downloa
+00002b60: 6420 646f 6375 6d65 6e74 2e0a 0a20 2020  d document...   
+00002b70: 2020 2020 2047 6976 656e 2061 2070 726f       Given a pro
+00002b80: 6365 7373 2061 6e64 2061 2064 6f63 756d  cess and a docum
+00002b90: 656e 7455 7269 2c20 646f 776e 6c6f 6164  entUri, download
+00002ba0: 2061 2064 6f63 756d 656e 742e 0a0a 2020   a document...  
+00002bb0: 2020 2020 2020 3a70 6172 616d 2069 643a        :param id:
+00002bc0: 2054 6865 2072 6573 6f75 7263 6520 4944   The resource ID
+00002bd0: 2e20 5265 7175 6972 6564 2e0a 2020 2020  . Required..    
+00002be0: 2020 2020 3a74 7970 6520 6964 3a20 7374      :type id: st
+00002bf0: 720a 2020 2020 2020 2020 3a6b 6579 776f  r.        :keywo
+00002c00: 7264 2064 6f63 756d 656e 745f 7572 693a  rd document_uri:
+00002c10: 2044 6f63 756d 656e 7420 5552 4920 746f   Document URI to
+00002c20: 2064 6f77 6e6c 6f61 642e 2052 6571 7569   download. Requi
+00002c30: 7265 642e 0a20 2020 2020 2020 203a 7479  red..        :ty
+00002c40: 7065 2064 6f63 756d 656e 745f 7572 693a  pe document_uri:
+00002c50: 2073 7472 0a20 2020 2020 2020 203a 7265   str.        :re
+00002c60: 7475 726e 3a20 4974 6572 6174 6f72 5b62  turn: Iterator[b
+00002c70: 7974 6573 5d0a 2020 2020 2020 2020 3a72  ytes].        :r
+00002c80: 7479 7065 3a20 4974 6572 6174 6f72 5b62  type: Iterator[b
+00002c90: 7974 6573 5d0a 2020 2020 2020 2020 3a72  ytes].        :r
+00002ca0: 6169 7365 7320 7e61 7a75 7265 2e63 6f72  aises ~azure.cor
+00002cb0: 652e 6578 6365 7074 696f 6e73 2e48 7474  e.exceptions.Htt
+00002cc0: 7052 6573 706f 6e73 6545 7272 6f72 3a0a  pResponseError:.
+00002cd0: 2020 2020 2020 2020 2902 721e 0000 0072          ).r....r
+00002ce0: 3200 0000 2903 720d 0000 0072 1b00 0000  2...).r....r....
+00002cf0: da28 6163 7469 6f6e 735f 7072 6f63 6573  .(actions_proces
+00002d00: 735f 646f 776e 6c6f 6164 5f65 6e74 6974  s_download_entit
+00002d10: 795f 646f 6375 6d65 6e74 2904 720e 0000  y_document).r...
+00002d20: 0072 1e00 0000 7232 0000 0072 1700 0000  .r....r2...r....
+00002d30: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00002d40: 3300 0000 3401 0000 730c 0000 0000 0d0a  3...4...s.......
+00002d50: 0102 0002 ff04 0102 ff7a 3a50 726f 6365  .........z:Proce
+00002d60: 7373 4f70 6572 6174 696f 6e73 2e61 6374  ssOperations.act
+00002d70: 696f 6e73 5f70 726f 6365 7373 5f64 6f77  ions_process_dow
+00002d80: 6e6c 6f61 645f 656e 7469 7479 5f64 6f63  nload_entity_doc
+00002d90: 756d 656e 7429 0472 1200 0000 7201 0000  ument).r....r...
+00002da0: 004e 4e29 25da 085f 5f6e 616d 655f 5fda  .NN)%..__name__.
+00002db0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00002dc0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00002dd0: 5f5f da19 4b75 466c 6f77 5265 7374 436c  __..KuFlowRestCl
+00002de0: 6965 6e74 4765 6e65 7261 7465 6472 1100  ientGeneratedr..
+00002df0: 0000 da03 696e 7472 0600 0000 7207 0000  ....intr....r...
+00002e00: 0072 1a00 0000 7205 0000 0072 0300 0000  .r....r....r....
+00002e10: da07 5f6d 6f64 656c 73da 0b50 726f 6365  .._models..Proce
+00002e20: 7373 5061 6765 721c 0000 00da 0750 726f  ssPager......Pro
+00002e30: 6365 7373 721d 0000 0072 1f00 0000 da1d  cessr....r......
+00002e40: 5072 6f63 6573 7343 6861 6e67 6549 6e69  ProcessChangeIni
+00002e50: 7469 6174 6f72 436f 6d6d 616e 6472 2300  tiatorCommandr#.
+00002e60: 0000 da19 5072 6f63 6573 7353 6176 6545  ....ProcessSaveE
+00002e70: 6c65 6d65 6e74 436f 6d6d 616e 6472 2500  lementCommandr%.
+00002e80: 0000 da1b 5072 6f63 6573 7344 656c 6574  ....ProcessDelet
+00002e90: 6545 6c65 6d65 6e74 436f 6d6d 616e 6472  eElementCommandr
+00002ea0: 2600 0000 7227 0000 0072 2800 0000 5a08  &...r'...r(...Z.
+00002eb0: 446f 6375 6d65 6e74 5a29 5072 6f63 6573  DocumentZ)Proces
+00002ec0: 7353 6176 6555 7365 7241 6374 696f 6e56  sSaveUserActionV
+00002ed0: 616c 7565 446f 6375 6d65 6e74 436f 6d6d  alueDocumentComm
+00002ee0: 616e 6472 2d00 0000 da1c 5072 6f63 6573  andr-.....Proces
+00002ef0: 7353 6176 6545 6e74 6974 7944 6174 6143  sSaveEntityDataC
+00002f00: 6f6d 6d61 6e64 722f 0000 0072 0200 0000  ommandr/...r....
+00002f10: da05 6279 7465 73da 2850 726f 6365 7373  ..bytes.(Process
+00002f20: 5361 7665 456e 7469 7479 446f 6375 6d65  SaveEntityDocume
+00002f30: 6e74 5265 7370 6f6e 7365 436f 6d6d 616e  ntResponseComman
+00002f40: 6472 3100 0000 7204 0000 0072 3300 0000  dr1...r....r3...
+00002f50: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00002f60: 1000 0000 720b 0000 001f 0000 0073 7000  ....r........sp.
+00002f70: 0000 0801 0409 0e05 0001 0001 0001 00fb  ................
+00002f80: 0202 0201 0201 1201 1201 0201 04f9 0c29  ...............)
+00002f90: 1619 140e 0200 0400 0201 04fe 0c16 0200  ................
+00002fa0: 0400 0201 04fe 0c18 0200 0400 0201 04fe  ................
+00002fb0: 0c13 140f 1413 0201 0401 0401 0201 08fa  ................
+00002fc0: 0c23 02fb 0402 0201 0402 0201 0201 04f9  .#..............
+00002fd0: 0c1e 0200 0600 0200 0200 0200 0201 04fe  ................
+00002fe0: 0c1f 720b 0000 004e 290e da06 7479 7069  ..r....N)...typi
+00002ff0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
+00003000: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00003010: da00 7209 0000 0072 3a00 0000 da0a 5f67  ..r....r:....._g
+00003020: 656e 6572 6174 6564 720a 0000 0072 3800  eneratedr....r8.
+00003030: 0000 720b 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00003040: 0072 0f00 0000 7210 0000 00da 083c 6d6f  .r....r......<mo
+00003050: 6475 6c65 3e19 0000 0073 0600 0000 2002  dule>....s.... .
+00003060: 0c01 0c03                                ....
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_robot_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_robot_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 4071 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 e70f 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 e70f 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d08 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a0a 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 04da 0341 6e79 da04  )......)...Any..
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_task_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 17487 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 4f44 0000  U........*.fOD..
+00000000: 550d 0d0a 0000 0000 5143 2a66 4f44 0000  U.......QC*fOD..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6402 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6402 6404 6c09 6d0a 5a0b  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a0c  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 05da 0341  d.S.)......)...A
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_tenant_user_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_tenant_user_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 4421 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 4511 0000  U........*.fE...
+00000000: 550d 0d0a 0000 0000 5143 2a66 4511 0000  U.......QC*fE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d08 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a0a 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 04da 0341 6e79 da04  )......)...Any..
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/__pycache__/_worker_operations.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/operations/__pycache__/_worker_operations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 2452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 9409 0000  U........*.f....
+00000000: 550d 0d0a 0000 0000 5143 2a66 9409 0000  U.......QC*f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6402 6404 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 8302 5a08  ..G.d.d...d...Z.
 00000060: 6407 5300 2908 e900 0000 0029 01da 0341  d.S.)......)...A
 00000070: 6e79 e902 0000 0029 01da 066d 6f64 656c  ny.....)...model
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_authentication_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_authentication_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_principal_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_principal_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_process_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_process_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,17 @@
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :type content_type: str
         :return: Process
         :rtype: ~kuflow.rest.models.Process
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self._kuflow_client.process.actions_process_save_entity_data(id, command, content_type, kwargs)
+        return self._kuflow_client.process.actions_process_save_entity_data(
+            id=id, command=command, content_type=content_type, **kwargs
+        )
 
     def actions_process_save_entity_document(
         self, id: str, file: IO[bytes], *, file_content_type: str, file_name: str, schema_path: str, **kwargs: Any
     ) -> _models.ProcessSaveEntityDocumentResponseCommand:
         """Save an entity value document.
 
         Save a document in the process to later be linked into the JSON data.
@@ -291,15 +293,20 @@
          validated by the passed schema path. Required.
         :type schema_path: str
         :return: ProcessSaveEntityDocumentResponseCommand
         :rtype: ~kuflow.rest.models.ProcessSaveEntityDocumentResponseCommand
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return self._kuflow_client.process.actions_process_save_entity_document(
-            id, file, file_content_type, file_name, schema_path, kwargs
+            id=id,
+            file=file,
+            file_content_type=file_content_type,
+            file_name=file_name,
+            schema_path=schema_path,
+            **kwargs,
         )
 
     def actions_process_download_entity_document(self, id: str, *, document_uri: str, **kwargs: Any) -> Iterator[bytes]:
         """Download document.
 
         Given a process and a documentUri, download a document.
 
@@ -307,8 +314,10 @@
         :type id: str
         :keyword document_uri: Document URI to download. Required.
         :type document_uri: str
         :return: Iterator[bytes]
         :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        return self._kuflow_client.process.actions_process_download_entity_document(id, document_uri, kwargs)
+        return self._kuflow_client.process.actions_process_download_entity_document(
+            id=id, document_uri=document_uri, **kwargs
+        )
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_robot_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_robot_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_task_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_task_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_tenant_user_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_tenant_user_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/operations/_worker_operations.py` & `kuflow_rest-1.5.1/kuflow_rest/operations/_worker_operations.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__init__.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 4008 0000  U........*.f@...
+00000000: 550d 0d0a 0000 0000 5143 2a66 4008 0000  U.......QC*f@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_process_page_item_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_process_page_item_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 13419 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 6b34 0000  U........*.fk4..
+00000000: 550d 0d0a 0000 0000 5143 2a66 6b34 0000  U.......QC*fk4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_process_save_element_command_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_process_save_element_command_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 11819 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 2b2e 0000  U........*.f+...
+00000000: 550d 0d0a 0000 0000 5143 2a66 2b2e 0000  U.......QC*f+...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_process_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_process_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 25012 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 b461 0000  U........*.f.a..
+00000000: 550d 0d0a 0000 0000 5143 2a66 245f 0000  U.......QC*f$_..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
+00000020: 0004 0000 0040 0000 0073 2a01 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 6d00 5a00 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6403 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6406 6407 6c0e  m.Z.m.Z...d.d.l.
 00000080: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
 00000090: 6d13 5a13 6d14 5a14 6d15 5a15 6d16 5a16  m.Z.m.Z.m.Z.m.Z.
@@ -12,1423 +12,1382 @@
 000000b0: 6d1b 5a1b 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e  m.Z.m.Z.m.Z.m.Z.
 000000c0: 6d1f 5a1f 6d20 5a20 6d21 5a21 6d22 5a22  m.Z.m Z m!Z!m"Z"
 000000d0: 0100 6406 6408 6c23 6d24 5a24 6d25 5a25  ..d.d.l#m$Z$m%Z%
 000000e0: 6d26 5a26 6d27 5a27 6d28 5a28 6d29 5a29  m&Z&m'Z'm(Z(m)Z)
 000000f0: 6d2a 5a2a 6d2b 5a2b 6d2c 5a2c 6d2d 5a2d  m*Z*m+Z+m,Z,m-Z-
 00000100: 6d2e 5a2e 6d2f 5a2f 6d30 5a30 6d31 5a31  m.Z.m/Z/m0Z0m1Z1
 00000110: 6d32 5a32 6d33 5a33 6d34 5a34 6d35 5a35  m2Z2m3Z3m4Z4m5Z5
-00000120: 6d36 5a36 6d37 5a37 6d38 5a38 0100 4700  m6Z6m7Z7m8Z8..G.
-00000130: 6409 640a 8400 640a 8302 5a39 4700 640b  d.d...d...Z9G.d.
-00000140: 640c 8400 640c 6511 8303 5a3a 4700 640d  d...d.e...Z:G.d.
-00000150: 640e 8400 640e 6524 8303 5a3b 640f 5300  d...d.e$..Z;d.S.
-00000160: 2910 e900 0000 0029 02da 0464 6174 65da  )......)...date.
-00000170: 0864 6174 6574 696d 6529 04da 0341 6e79  .datetime)...Any
-00000180: da04 4469 6374 da04 4c69 7374 da08 4f70  ..Dict..List..Op
-00000190: 7469 6f6e 616c e902 0000 0029 01da 1350  tional.....)...P
-000001a0: 726f 6365 7373 456c 656d 656e 7456 616c  rocessElementVal
-000001b0: 7565 2904 da0d 4a73 6f6e 466f 726d 7346  ue)...JsonFormsF
-000001c0: 696c 65da 124a 736f 6e46 6f72 6d73 5072  ile..JsonFormsPr
-000001d0: 696e 6369 7061 6cda 0e4a 736f 6e46 6f72  incipal..JsonFor
-000001e0: 6d73 5661 6c75 65da 0750 726f 6365 7373  msValue..Process
-000001f0: e901 0000 0029 14da 1645 6c65 6d65 6e74  .....)...Element
-00000200: 5661 6c75 6553 696d 706c 6554 7970 65da  ValueSimpleType.
-00000210: 1145 6c65 6d65 6e74 5661 6c75 6555 6e69  .ElementValueUni
-00000220: 6f6e da1b 5072 6f63 6573 7345 6c65 6d65  on..ProcessEleme
-00000230: 6e74 5661 6c75 6541 6363 6573 736f 72da  ntValueAccessor.
-00000240: 1161 6464 5f65 6c65 6d65 6e74 5f76 616c  .add_element_val
-00000250: 7565 da16 6164 645f 656c 656d 656e 745f  ue..add_element_
-00000260: 7661 6c75 655f 6c69 7374 da1a 6669 6e64  value_list..find
-00000270: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f61  _element_value_a
-00000280: 735f 6461 7465 da1b 6669 6e64 5f65 6c65  s_date..find_ele
-00000290: 6d65 6e74 5f76 616c 7565 5f61 735f 666c  ment_value_as_fl
-000002a0: 6f61 74da 1966 696e 645f 656c 656d 656e  oat..find_elemen
-000002b0: 745f 7661 6c75 655f 6173 5f73 7472 da19  t_value_as_str..
-000002c0: 6765 745f 656c 656d 656e 745f 7661 6c75  get_element_valu
-000002d0: 655f 6173 5f64 6174 65da 1e67 6574 5f65  e_as_date..get_e
-000002e0: 6c65 6d65 6e74 5f76 616c 7565 5f61 735f  lement_value_as_
-000002f0: 6461 7465 5f6c 6973 74da 1a67 6574 5f65  date_list..get_e
-00000300: 6c65 6d65 6e74 5f76 616c 7565 5f61 735f  lement_value_as_
-00000310: 666c 6f61 74da 1f67 6574 5f65 6c65 6d65  float..get_eleme
-00000320: 6e74 5f76 616c 7565 5f61 735f 666c 6f61  nt_value_as_floa
-00000330: 745f 6c69 7374 da18 6765 745f 656c 656d  t_list..get_elem
-00000340: 656e 745f 7661 6c75 655f 6173 5f73 7472  ent_value_as_str
-00000350: da1d 6765 745f 656c 656d 656e 745f 7661  ..get_element_va
-00000360: 6c75 655f 6173 5f73 7472 5f6c 6973 74da  lue_as_str_list.
-00000370: 1767 6574 5f65 6c65 6d65 6e74 5f76 616c  .get_element_val
-00000380: 7565 5f76 616c 6964 da1a 6765 745f 656c  ue_valid..get_el
-00000390: 656d 656e 745f 7661 6c75 655f 7661 6c69  ement_value_vali
-000003a0: 645f 6174 da11 7365 745f 656c 656d 656e  d_at..set_elemen
-000003b0: 745f 7661 6c75 65da 1673 6574 5f65 6c65  t_value..set_ele
-000003c0: 6d65 6e74 5f76 616c 7565 5f6c 6973 74da  ment_value_list.
-000003d0: 1773 6574 5f65 6c65 6d65 6e74 5f76 616c  .set_element_val
-000003e0: 7565 5f76 616c 6964 da1a 7365 745f 656c  ue_valid..set_el
-000003f0: 656d 656e 745f 7661 6c75 655f 7661 6c69  ement_value_vali
-00000400: 645f 6174 2915 da14 4a73 6f6e 466f 726d  d_at)...JsonForm
-00000410: 4461 7461 4163 6365 7373 6f72 da13 4a73  DataAccessor..Js
-00000420: 6f6e 466f 726d 7353 696d 706c 6554 7970  onFormsSimpleTyp
-00000430: 65da 2066 696e 645f 6a73 6f6e 5f66 6f72  e. find_json_for
-00000440: 6d73 5f70 726f 7065 7274 795f 6173 5f64  ms_property_as_d
-00000450: 6174 65da 2466 696e 645f 6a73 6f6e 5f66  ate.$find_json_f
-00000460: 6f72 6d73 5f70 726f 7065 7274 795f 6173  orms_property_as
-00000470: 5f64 6174 6574 696d 65da 2066 696e 645f  _datetime. find_
-00000480: 6a73 6f6e 5f66 6f72 6d73 5f70 726f 7065  json_forms_prope
-00000490: 7274 795f 6173 5f64 6963 74da 2166 696e  rty_as_dict.!fin
-000004a0: 645f 6a73 6f6e 5f66 6f72 6d73 5f70 726f  d_json_forms_pro
-000004b0: 7065 7274 795f 6173 5f66 6c6f 6174 da1f  perty_as_float..
-000004c0: 6669 6e64 5f6a 736f 6e5f 666f 726d 735f  find_json_forms_
-000004d0: 7072 6f70 6572 7479 5f61 735f 696e 74da  property_as_int.
-000004e0: 2b66 696e 645f 6a73 6f6e 5f66 6f72 6d73  +find_json_forms
-000004f0: 5f70 726f 7065 7274 795f 6173 5f6a 736f  _property_as_jso
-00000500: 6e5f 666f 726d 735f 6669 6c65 da30 6669  n_forms_file.0fi
-00000510: 6e64 5f6a 736f 6e5f 666f 726d 735f 7072  nd_json_forms_pr
-00000520: 6f70 6572 7479 5f61 735f 6a73 6f6e 5f66  operty_as_json_f
-00000530: 6f72 6d73 5f70 7269 6e63 6970 616c da20  orms_principal. 
-00000540: 6669 6e64 5f6a 736f 6e5f 666f 726d 735f  find_json_forms_
-00000550: 7072 6f70 6572 7479 5f61 735f 6c69 7374  property_as_list
-00000560: da1f 6669 6e64 5f6a 736f 6e5f 666f 726d  ..find_json_form
-00000570: 735f 7072 6f70 6572 7479 5f61 735f 7374  s_property_as_st
-00000580: 72da 1f67 6574 5f6a 736f 6e5f 666f 726d  r..get_json_form
-00000590: 735f 7072 6f70 6572 7479 5f61 735f 6461  s_property_as_da
-000005a0: 7465 da23 6765 745f 6a73 6f6e 5f66 6f72  te.#get_json_for
-000005b0: 6d73 5f70 726f 7065 7274 795f 6173 5f64  ms_property_as_d
-000005c0: 6174 6574 696d 65da 1f67 6574 5f6a 736f  atetime..get_jso
-000005d0: 6e5f 666f 726d 735f 7072 6f70 6572 7479  n_forms_property
-000005e0: 5f61 735f 6469 6374 da20 6765 745f 6a73  _as_dict. get_js
-000005f0: 6f6e 5f66 6f72 6d73 5f70 726f 7065 7274  on_forms_propert
-00000600: 795f 6173 5f66 6c6f 6174 da1e 6765 745f  y_as_float..get_
-00000610: 6a73 6f6e 5f66 6f72 6d73 5f70 726f 7065  json_forms_prope
-00000620: 7274 795f 6173 5f69 6e74 da2a 6765 745f  rty_as_int.*get_
-00000630: 6a73 6f6e 5f66 6f72 6d73 5f70 726f 7065  json_forms_prope
-00000640: 7274 795f 6173 5f6a 736f 6e5f 666f 726d  rty_as_json_form
-00000650: 735f 6669 6c65 da2f 6765 745f 6a73 6f6e  s_file./get_json
-00000660: 5f66 6f72 6d73 5f70 726f 7065 7274 795f  _forms_property_
-00000670: 6173 5f6a 736f 6e5f 666f 726d 735f 7072  as_json_forms_pr
-00000680: 696e 6369 7061 6cda 1f67 6574 5f6a 736f  incipal..get_jso
-00000690: 6e5f 666f 726d 735f 7072 6f70 6572 7479  n_forms_property
-000006a0: 5f61 735f 6c69 7374 da1e 6765 745f 6a73  _as_list..get_js
-000006b0: 6f6e 5f66 6f72 6d73 5f70 726f 7065 7274  on_forms_propert
-000006c0: 795f 6173 5f73 7472 da1a 7570 6461 7465  y_as_str..update
-000006d0: 5f6a 736f 6e5f 666f 726d 735f 7072 6f70  _json_forms_prop
-000006e0: 6572 7479 6300 0000 0000 0000 0000 0000  ertyc...........
-000006f0: 0000 0000 0007 0000 0040 0000 0073 9a03  .........@...s..
-00000700: 0000 6500 5a01 6400 5a02 6503 6504 6505  ..e.Z.d.Z.e.e.e.
-00000710: 6506 6401 9c03 6402 6403 8404 8301 5a07  e.d...d.d.....Z.
-00000720: 6503 6504 6505 6508 6506 6404 9c04 6405  e.e.e.e.e.d...d.
-00000730: 6406 8404 8301 5a09 6503 6504 6505 650a  d.....Z.e.e.e.e.
-00000740: 6506 1900 6504 6407 9c04 6408 6409 8404  e...e.d...d.d...
-00000750: 8301 5a0b 6503 6504 6505 650a 6506 1900  ..Z.e.e.e.e.e...
-00000760: 6508 6504 640a 9c05 640b 640c 8404 8301  e.e.d...d.d.....
-00000770: 5a0c 6503 6452 6504 6505 650a 650d 1900  Z.e.dRe.e.e.e...
-00000780: 6504 640e 9c04 640f 6410 8405 8301 5a0e  e.d...d.d.....Z.
-00000790: 6503 6453 6504 6505 650a 650f 650d 1900  e.dSe.e.e.e.e...
-000007a0: 1900 6504 6411 9c04 6412 6413 8405 8301  ..e.d...d.d.....
-000007b0: 5a10 6503 6454 6504 6505 650a 650d 1900  Z.e.dTe.e.e.e...
-000007c0: 6504 640e 9c04 6414 6415 8405 8301 5a11  e.d...d.d.....Z.
-000007d0: 6503 6455 6504 6505 650a 650f 650d 1900  e.dUe.e.e.e.e...
-000007e0: 1900 6504 6411 9c04 6416 6417 8405 8301  ..e.d...d.d.....
-000007f0: 5a12 6503 6504 6505 6505 6401 9c03 6418  Z.e.e.e.e.d...d.
-00000800: 6419 8404 8301 5a13 6503 6504 6505 650a  d.....Z.e.e.e.e.
-00000810: 6505 1900 6401 9c03 641a 641b 8404 8301  e...d...d.d.....
-00000820: 5a14 6503 6504 6505 650f 6505 1900 6401  Z.e.e.e.e.e...d.
-00000830: 9c03 641c 641d 8404 8301 5a15 6503 6504  ..d.d.....Z.e.e.
-00000840: 6505 6516 6401 9c03 641e 641f 8404 8301  e.e.d...d.d.....
-00000850: 5a17 6503 6504 6505 6516 6401 9c03 6420  Z.e.e.e.e.d...d 
-00000860: 6421 8404 8301 5a18 6503 6504 6505 650f  d!....Z.e.e.e.e.
-00000870: 6516 1900 6401 9c03 6422 6423 8404 8301  e...d...d"d#....
-00000880: 5a19 6503 6504 6505 651a 6401 9c03 6424  Z.e.e.e.e.d...d$
-00000890: 6425 8404 8301 5a1b 6503 6504 6505 650a  d%....Z.e.e.e.e.
-000008a0: 651a 1900 6401 9c03 6426 6427 8404 8301  e...d...d&d'....
-000008b0: 5a1c 6503 6504 6505 650f 651a 1900 6401  Z.e.e.e.e.e...d.
-000008c0: 9c03 6428 6429 8404 8301 5a1d 6503 6504  ..d(d)....Z.e.e.
-000008d0: 6505 6505 642a 9c03 642b 642c 8404 8301  e.e.d*..d+d,....
-000008e0: 5a1e 6503 6504 6505 650a 6505 1900 642a  Z.e.e.e.e.e...d*
-000008f0: 9c03 642d 642e 8404 8301 5a1f 6503 6504  ..d-d.....Z.e.e.
-00000900: 6505 6508 642a 9c03 642f 6430 8404 8301  e.e.d*..d/d0....
-00000910: 5a20 6503 6504 6505 650a 6508 1900 642a  Z e.e.e.e.e...d*
-00000920: 9c03 6431 6432 8404 8301 5a21 6503 6504  ..d1d2....Z!e.e.
-00000930: 6505 6516 642a 9c03 6433 6434 8404 8301  e.e.d*..d3d4....
-00000940: 5a22 6503 6504 6505 650a 6516 1900 642a  Z"e.e.e.e.e...d*
-00000950: 9c03 6435 6436 8404 8301 5a23 6503 6504  ..d5d6....Z#e.e.
-00000960: 6505 651a 642a 9c03 6437 6438 8404 8301  e.e.d*..d7d8....
-00000970: 5a24 6503 6504 6505 650a 651a 1900 642a  Z$e.e.e.e.e...d*
-00000980: 9c03 6439 643a 8404 8301 5a25 6503 6504  ..d9d:....Z%e.e.
-00000990: 6505 6526 642a 9c03 643b 643c 8404 8301  e.e&d*..d;d<....
-000009a0: 5a27 6503 6504 6505 650a 6526 1900 642a  Z'e.e.e.e.e&..d*
-000009b0: 9c03 643d 643e 8404 8301 5a28 6503 6504  ..d=d>....Z(e.e.
-000009c0: 6505 6529 642a 9c03 643f 6440 8404 8301  e.e)d*..d?d@....
-000009d0: 5a2a 6503 6504 6505 650a 6529 1900 642a  Z*e.e.e.e.e)..d*
-000009e0: 9c03 6441 6442 8404 8301 5a2b 6503 6504  ..dAdB....Z+e.e.
-000009f0: 6505 652c 642a 9c03 6443 6444 8404 8301  e.e,d*..dCdD....
-00000a00: 5a2d 6503 6504 6505 650a 652c 1900 642a  Z-e.e.e.e.e,..d*
-00000a10: 9c03 6445 6446 8404 8301 5a2e 6503 6504  ..dEdF....Z.e.e.
-00000a20: 6505 652f 642a 9c03 6447 6448 8404 8301  e.e/d*..dGdH....
-00000a30: 5a30 6503 6504 6505 650a 652f 1900 642a  Z0e.e.e.e.e/..d*
-00000a40: 9c03 6449 644a 8404 8301 5a31 6503 6504  ..dIdJ....Z1e.e.
-00000a50: 6505 6532 642a 9c03 644b 644c 8404 8301  e.e2d*..dKdL....
-00000a60: 5a33 6503 6504 6505 650a 6532 1900 642a  Z3e.e.e.e.e2..d*
-00000a70: 9c03 644d 644e 8404 8301 5a34 6503 6504  ..dMdN....Z4e.e.
-00000a80: 6505 650a 6535 1900 640d 644f 9c04 6450  e.e.e5..d.dO..dP
-00000a90: 6451 8404 8301 5a36 640d 5300 2956 da0c  dQ....Z6d.S.)V..
-00000aa0: 5072 6f63 6573 7355 7469 6c73 2903 da07  ProcessUtils)...
-00000ab0: 7072 6f63 6573 73da 1765 6c65 6d65 6e74  process..element
-00000ac0: 5f64 6566 696e 6974 696f 6e5f 636f 6465  _definition_code
-00000ad0: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
-00000ae0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000af0: 0073 0e00 0000 7400 7401 7c00 7c01 8302  .s....t.t.|.|...
-00000b00: 8301 5300 2901 610b 0100 000a 2020 2020  ..S.).a.....    
-00000b10: 2020 2020 4368 6563 6b20 6966 2061 6c6c      Check if all
-00000b20: 2072 656c 6174 6564 2076 616c 6964 2076   related valid v
-00000b30: 616c 7565 7320 6172 6520 5452 5545 2e0a  alues are TRUE..
-00000b40: 0a20 2020 2020 2020 2041 7267 756d 656e  .        Argumen
-00000b50: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00000b60: 7072 6f63 6573 733a 2054 6865 2070 726f  process: The pro
-00000b70: 6365 7373 2e0a 2020 2020 2020 2020 2020  cess..          
-00000b80: 2020 656c 656d 656e 745f 6465 6669 6e69    element_defini
-00000b90: 7469 6f6e 5f63 6f64 653a 2045 6c65 6d65  tion_code: Eleme
-00000ba0: 6e74 2044 6566 696e 6974 696f 6e20 436f  nt Definition Co
-00000bb0: 6465 2e0a 0a20 2020 2020 2020 2052 6574  de...        Ret
-00000bc0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00000bd0: 2020 5472 7565 2069 6620 616c 6c20 7265    True if all re
-00000be0: 6c61 7465 6420 7661 6c69 6420 7661 6c75  lated valid valu
-00000bf0: 6573 2061 7265 2054 5255 452c 206f 7468  es are TRUE, oth
-00000c00: 6572 7769 7365 2046 616c 7365 2e0a 2020  erwise False..  
-00000c10: 2020 2020 2020 2902 721d 0000 00da 1b43        ).r......C
-00000c20: 7572 7265 6e74 456c 656d 656e 7456 616c  urrentElementVal
-00000c30: 7565 4163 6365 7373 6f72 a902 7239 0000  ueAccessor..r9..
-00000c40: 0072 3a00 0000 a900 723e 0000 00fa 472f  .r:.....r>....G/
-00000c50: 776f 726b 2f6b 7566 6c6f 772d 7364 6b2d  work/kuflow-sdk-
-00000c60: 7079 7468 6f6e 2f6b 7566 6c6f 772d 7265  python/kuflow-re
-00000c70: 7374 2f6b 7566 6c6f 775f 7265 7374 2f75  st/kuflow_rest/u
-00000c80: 7469 6c73 2f5f 7072 6f63 6573 735f 7574  tils/_process_ut
-00000c90: 696c 732e 7079 721d 0000 004e 0000 0073  ils.pyr....N...s
-00000ca0: 0200 0000 000c 7a24 5072 6f63 6573 7355  ......z$ProcessU
-00000cb0: 7469 6c73 2e67 6574 5f65 6c65 6d65 6e74  tils.get_element
-00000cc0: 5f76 616c 7565 5f76 616c 6964 2904 7239  _value_valid).r9
-00000cd0: 0000 0072 3a00 0000 da05 696e 6465 7872  ...r:.....indexr
-00000ce0: 3b00 0000 6303 0000 0000 0000 0000 0000  ;...c...........
-00000cf0: 0003 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00000d00: 0000 7400 7401 7c00 7c01 8302 7c02 8302  ..t.t.|.|...|...
-00000d10: 5300 2901 614a 0100 000a 2020 2020 2020  S.).aJ....      
-00000d20: 2020 4368 6563 6b20 6966 2074 6865 2072    Check if the r
-00000d30: 6571 7565 7374 6564 2076 616c 6964 2076  equested valid v
-00000d40: 616c 7565 2061 7420 7468 6520 6769 7665  alue at the give
-00000d50: 6e20 696e 6465 7820 6973 2054 5255 452e  n index is TRUE.
-00000d60: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
-00000d70: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
-00000d80: 2070 726f 6365 7373 3a20 5468 6520 7072   process: The pr
-00000d90: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
-00000da0: 2020 2065 6c65 6d65 6e74 5f64 6566 696e     element_defin
-00000db0: 6974 696f 6e5f 636f 6465 3a20 5468 6520  ition_code: The 
-00000dc0: 656c 656d 656e 7420 6465 6669 6e69 7469  element definiti
-00000dd0: 6f6e 2063 6f64 652e 0a20 2020 2020 2020  on code..       
-00000de0: 2020 2020 2069 6e64 6578 3a20 5468 6520       index: The 
-00000df0: 656c 656d 656e 7420 7661 6c75 6520 696e  element value in
-00000e00: 6465 782e 0a0a 2020 2020 2020 2020 5265  dex...        Re
-00000e10: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00000e20: 2020 2054 6865 2072 6571 7565 7374 6564     The requested
-00000e30: 2076 616c 6964 2076 616c 7565 2069 6620   valid value if 
-00000e40: 6974 2065 7869 7374 732c 206f 7468 6572  it exists, other
-00000e50: 7769 7365 204e 6f6e 652e 0a20 2020 2020  wise None..     
-00000e60: 2020 2029 0272 1e00 0000 723c 0000 0029     ).r....r<...)
-00000e70: 0372 3900 0000 723a 0000 0072 4000 0000  .r9...r:...r@...
-00000e80: 723e 0000 0072 3e00 0000 723f 0000 0072  r>...r>...r?...r
-00000e90: 1e00 0000 5c00 0000 7302 0000 0000 117a  ....\...s......z
-00000ea0: 2750 726f 6365 7373 5574 696c 732e 6765  'ProcessUtils.ge
-00000eb0: 745f 656c 656d 656e 745f 7661 6c75 655f  t_element_value_
-00000ec0: 7661 6c69 645f 6174 2904 7239 0000 0072  valid_at).r9...r
-00000ed0: 3a00 0000 da05 7661 6c69 6472 3b00 0000  :.....validr;...
-00000ee0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000ef0: 0004 0000 0043 0000 0073 1400 0000 7400  .....C...s....t.
-00000f00: 7401 7c00 7c01 8302 7c02 8302 0100 7c00  t.|.|...|.....|.
-00000f10: 5300 2901 610b 0100 000a 2020 2020 2020  S.).a.....      
-00000f20: 2020 5365 7420 7468 6520 7661 6c69 6420    Set the valid 
-00000f30: 7661 6c75 6520 666f 7220 616c 6c20 656c  value for all el
-00000f40: 656d 656e 7420 7661 6c75 6573 2e0a 0a20  ement values... 
-00000f50: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-00000f60: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00000f70: 6f63 6573 733a 2054 6865 2070 726f 6365  ocess: The proce
-00000f80: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
-00000f90: 656c 656d 656e 745f 6465 6669 6e69 7469  element_definiti
-00000fa0: 6f6e 5f63 6f64 653a 2054 6865 2065 6c65  on_code: The ele
-00000fb0: 6d65 6e74 2064 6566 696e 6974 696f 6e20  ment definition 
-00000fc0: 636f 6465 2e0a 2020 2020 2020 2020 2020  code..          
-00000fd0: 2020 7661 6c69 643a 2054 6865 2076 616c    valid: The val
-00000fe0: 6964 2076 616c 7565 2e0a 0a20 2020 2020  id value...     
-00000ff0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00001000: 2020 2020 2020 2020 5468 6520 7061 7373          The pass
-00001010: 6564 2070 726f 6365 7373 2e0a 2020 2020  ed process..    
-00001020: 2020 2020 2902 7221 0000 0072 3c00 0000      ).r!...r<...
-00001030: 2903 7239 0000 0072 3a00 0000 7241 0000  ).r9...r:...rA..
-00001040: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
-00001050: 7221 0000 006f 0000 0073 0400 0000 000d  r!...o...s......
-00001060: 1002 7a24 5072 6f63 6573 7355 7469 6c73  ..z$ProcessUtils
-00001070: 2e73 6574 5f65 6c65 6d65 6e74 5f76 616c  .set_element_val
-00001080: 7565 5f76 616c 6964 2905 7239 0000 0072  ue_valid).r9...r
-00001090: 3a00 0000 7241 0000 0072 4000 0000 723b  :...rA...r@...r;
-000010a0: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
-000010b0: 0400 0000 0400 0000 4300 0000 7316 0000  ........C...s...
-000010c0: 0074 0074 017c 007c 0183 027c 027c 0383  .t.t.|.|...|.|..
-000010d0: 0301 007c 0053 0029 0161 3f01 0000 0a20  ...|.S.).a?.... 
-000010e0: 2020 2020 2020 2053 6574 2074 6865 2076         Set the v
-000010f0: 616c 6964 2076 616c 7565 2066 6f72 2074  alid value for t
-00001100: 6865 2073 656c 6563 7465 6420 656c 656d  he selected elem
-00001110: 656e 7420 7661 6c75 652e 0a0a 2020 2020  ent value...    
-00001120: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
-00001130: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-00001140: 7373 3a20 5468 6520 7072 6f63 6573 732e  ss: The process.
-00001150: 0a20 2020 2020 2020 2020 2020 2065 6c65  .            ele
-00001160: 6d65 6e74 5f64 6566 696e 6974 696f 6e5f  ment_definition_
-00001170: 636f 6465 3a20 5468 6520 656c 656d 656e  code: The elemen
-00001180: 7420 6465 6669 6e69 7469 6f6e 2063 6f64  t definition cod
-00001190: 652e 0a20 2020 2020 2020 2020 2020 2076  e..            v
-000011a0: 616c 6964 3a20 5468 6520 7661 6c69 6420  alid: The valid 
-000011b0: 7661 6c75 652e 0a20 2020 2020 2020 2020  value..         
-000011c0: 2020 2069 6e64 6578 3a20 5468 6520 656c     index: The el
-000011d0: 656d 656e 7420 7661 6c75 6520 696e 6465  ement value inde
-000011e0: 782e 0a0a 2020 2020 2020 2020 5265 7475  x...        Retu
-000011f0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00001200: 2054 6865 2070 6173 7365 6420 7072 6f63   The passed proc
-00001210: 6573 732e 0a20 2020 2020 2020 2029 0272  ess..        ).r
-00001220: 2200 0000 723c 0000 0029 0472 3900 0000  "...r<...).r9...
-00001230: 723a 0000 0072 4100 0000 7240 0000 0072  r:...rA...r@...r
-00001240: 3e00 0000 723e 0000 0072 3f00 0000 7222  >...r>...r?...r"
-00001250: 0000 0080 0000 0073 0400 0000 0013 1202  .......s........
-00001260: 7a27 5072 6f63 6573 7355 7469 6c73 2e73  z'ProcessUtils.s
-00001270: 6574 5f65 6c65 6d65 6e74 5f76 616c 7565  et_element_value
-00001280: 5f76 616c 6964 5f61 744e 2904 7239 0000  _valid_atN).r9..
-00001290: 0072 3a00 0000 da0d 656c 656d 656e 745f  .r:.....element_
-000012a0: 7661 6c75 6572 3b00 0000 6303 0000 0000  valuer;...c.....
-000012b0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-000012c0: 0000 0073 1400 0000 7400 7401 7c00 7c01  ...s....t.t.|.|.
-000012d0: 8302 7c02 8302 0100 7c00 5300 2901 6135  ..|.....|.S.).a5
-000012e0: 0100 000a 2020 2020 2020 2020 5365 7420  ....        Set 
-000012f0: 616e 2065 6c65 6d65 6e74 2076 616c 7565  an element value
-00001300: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
-00001310: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
-00001320: 2020 7072 6f63 6573 733a 2054 6865 2070    process: The p
-00001330: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
-00001340: 2020 2020 656c 656d 656e 745f 6465 6669      element_defi
-00001350: 6e69 7469 6f6e 5f63 6f64 653a 2054 6865  nition_code: The
-00001360: 2065 6c65 6d65 6e74 2064 6566 696e 6974   element definit
-00001370: 696f 6e20 636f 6465 2e0a 2020 2020 2020  ion code..      
-00001380: 2020 2020 2020 656c 656d 656e 745f 7661        element_va
-00001390: 6c75 653a 2054 6865 2065 6c65 6d65 6e74  lue: The element
-000013a0: 2076 616c 7565 2e20 4966 2074 6865 2076   value. If the v
-000013b0: 616c 7565 2069 7320 4e6f 6e65 2c20 616c  alue is None, al
-000013c0: 6c20 6375 7272 656e 7420 7661 6c75 6573  l current values
-000013d0: 2061 7265 2072 656d 6f76 6564 2e0a 0a20   are removed... 
-000013e0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000013f0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001400: 7061 7373 6564 2070 726f 6365 7373 2e0a  passed process..
-00001410: 2020 2020 2020 2020 2902 721f 0000 0072          ).r....r
-00001420: 3c00 0000 a903 7239 0000 0072 3a00 0000  <.....r9...r:...
-00001430: 7242 0000 0072 3e00 0000 723e 0000 0072  rB...r>...r>...r
-00001440: 3f00 0000 721f 0000 0097 0000 0073 0400  ?...r........s..
-00001450: 0000 0011 1002 7a1e 5072 6f63 6573 7355  ......z.ProcessU
-00001460: 7469 6c73 2e73 6574 5f65 6c65 6d65 6e74  tils.set_element
-00001470: 5f76 616c 7565 2904 7239 0000 0072 3a00  _value).r9...r:.
-00001480: 0000 da0e 656c 656d 656e 745f 7661 6c75  ....element_valu
-00001490: 6573 723b 0000 0063 0300 0000 0000 0000  esr;...c........
-000014a0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-000014b0: 7314 0000 0074 0074 017c 007c 0183 027c  s....t.t.|.|...|
-000014c0: 0283 0201 007c 0053 0029 0161 3f01 0000  .....|.S.).a?...
-000014d0: 0a20 2020 2020 2020 2053 6574 2061 6e20  .        Set an 
-000014e0: 656c 656d 656e 7420 7661 6c75 652e 0a0a  element value...
-000014f0: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-00001500: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-00001510: 726f 6365 7373 3a20 5468 6520 7072 6f63  rocess: The proc
-00001520: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
-00001530: 2065 6c65 6d65 6e74 5f64 6566 696e 6974   element_definit
-00001540: 696f 6e5f 636f 6465 3a20 5468 6520 656c  ion_code: The el
-00001550: 656d 656e 7420 6465 6669 6e69 7469 6f6e  ement definition
-00001560: 2063 6f64 652e 0a20 2020 2020 2020 2020   code..         
-00001570: 2020 2065 6c65 6d65 6e74 5f76 616c 7565     element_value
-00001580: 733a 2054 6865 2065 6c65 6d65 6e74 2076  s: The element v
-00001590: 616c 7565 2e20 4966 2074 6865 2076 616c  alue. If the val
-000015a0: 7565 2069 7320 4e6f 6e65 206f 7220 656d  ue is None or em
-000015b0: 7074 792c 2061 6c6c 2063 7572 7265 6e74  pty, all current
-000015c0: 2076 616c 7565 7320 6172 6520 7265 6d6f   values are remo
-000015d0: 7665 642e 0a0a 2020 2020 2020 2020 5265  ved...        Re
-000015e0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000015f0: 2020 2054 6865 2070 6173 7365 6420 7072     The passed pr
-00001600: 6f63 6573 732e 0a20 2020 2020 2020 2029  ocess..        )
-00001610: 0272 2000 0000 723c 0000 00a9 0372 3900  .r ...r<.....r9.
-00001620: 0000 723a 0000 0072 4400 0000 723e 0000  ..r:...rD...r>..
-00001630: 0072 3e00 0000 723f 0000 0072 2000 0000  .r>...r?...r ...
-00001640: ac00 0000 730a 0000 0000 1102 0108 0102  ....s...........
-00001650: fe04 057a 2350 726f 6365 7373 5574 696c  ...z#ProcessUtil
-00001660: 732e 7365 745f 656c 656d 656e 745f 7661  s.set_element_va
-00001670: 6c75 655f 6c69 7374 6303 0000 0000 0000  lue_listc.......
-00001680: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00001690: 0073 1400 0000 7400 7401 7c00 7c01 8302  .s....t.t.|.|...
-000016a0: 7c02 8302 0100 7c00 5300 2901 6135 0100  |.....|.S.).a5..
-000016b0: 000a 2020 2020 2020 2020 4164 6420 616e  ..        Add an
-000016c0: 2065 6c65 6d65 6e74 2076 616c 7565 2e0a   element value..
-000016d0: 0a20 2020 2020 2020 2041 7267 756d 656e  .        Argumen
-000016e0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-000016f0: 7072 6f63 6573 733a 2054 6865 2070 726f  process: The pro
-00001700: 6365 7373 2e0a 2020 2020 2020 2020 2020  cess..          
-00001710: 2020 656c 656d 656e 745f 6465 6669 6e69    element_defini
-00001720: 7469 6f6e 5f63 6f64 653a 2054 6865 2065  tion_code: The e
-00001730: 6c65 6d65 6e74 2064 6566 696e 6974 696f  lement definitio
-00001740: 6e20 636f 6465 2e0a 2020 2020 2020 2020  n code..        
-00001750: 2020 2020 656c 656d 656e 745f 7661 6c75      element_valu
-00001760: 653a 2054 6865 2065 6c65 6d65 6e74 2076  e: The element v
-00001770: 616c 7565 2e20 4966 2074 6865 2076 616c  alue. If the val
-00001780: 7565 2069 7320 4e6f 6e65 2c20 616c 6c20  ue is None, all 
-00001790: 6375 7272 656e 7420 7661 6c75 6573 2061  current values a
-000017a0: 7265 2072 656d 6f76 6564 2e0a 0a20 2020  re removed...   
-000017b0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-000017c0: 2020 2020 2020 2020 2020 5468 6520 7061            The pa
-000017d0: 7373 6564 2070 726f 6365 7373 2e0a 2020  ssed process..  
-000017e0: 2020 2020 2020 2902 7212 0000 0072 3c00        ).r....r<.
-000017f0: 0000 7243 0000 0072 3e00 0000 723e 0000  ..rC...r>...r>..
-00001800: 0072 3f00 0000 7212 0000 00c4 0000 0073  .r?...r........s
-00001810: 0400 0000 0011 1002 7a1e 5072 6f63 6573  ........z.Proces
-00001820: 7355 7469 6c73 2e61 6464 5f65 6c65 6d65  sUtils.add_eleme
-00001830: 6e74 5f76 616c 7565 6303 0000 0000 0000  nt_valuec.......
-00001840: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00001850: 0073 1400 0000 7400 7401 7c00 7c01 8302  .s....t.t.|.|...
-00001860: 7c02 8302 0100 7c00 5300 2901 614c 0100  |.....|.S.).aL..
-00001870: 000a 2020 2020 2020 2020 4164 6420 656c  ..        Add el
-00001880: 656d 656e 7420 7661 6c75 6573 2e0a 0a20  ement values... 
-00001890: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-000018a0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-000018b0: 6f63 6573 733a 2054 6865 2070 726f 6365  ocess: The proce
-000018c0: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
-000018d0: 656c 656d 656e 745f 6465 6669 6e69 7469  element_definiti
-000018e0: 6f6e 5f63 6f64 653a 2054 6865 2065 6c65  on_code: The ele
-000018f0: 6d65 6e74 2064 6566 696e 6974 696f 6e20  ment definition 
-00001900: 636f 6465 2e0a 2020 2020 2020 2020 2020  code..          
-00001910: 2020 656c 656d 656e 745f 7661 6c75 6573    element_values
-00001920: 3a20 5468 6520 656c 656d 656e 7420 7661  : The element va
-00001930: 6c75 6573 2e20 4966 2074 6865 2076 616c  lues. If the val
-00001940: 7565 7320 6973 204e 6f6e 6520 6f72 2065  ues is None or e
-00001950: 6d70 7479 2c20 616c 6c20 6375 7272 656e  mpty, all curren
-00001960: 7420 7661 6c75 6573 2061 7265 2072 656d  t values are rem
-00001970: 6f76 6564 2e0a 0a20 2020 2020 2020 2052  oved...        R
-00001980: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00001990: 2020 2020 5468 6520 7061 7373 6564 206d      The passed m
-000019a0: 6f64 656c 2072 656c 6174 6564 206f 626a  odel related obj
-000019b0: 6563 742e 0a20 2020 2020 2020 2029 0272  ect..        ).r
-000019c0: 1300 0000 723c 0000 0072 4500 0000 723e  ....r<...rE...r>
-000019d0: 0000 0072 3e00 0000 723f 0000 0072 1300  ...r>...r?...r..
-000019e0: 0000 d900 0000 730a 0000 0000 1102 0108  ......s.........
-000019f0: 0102 fe04 057a 2350 726f 6365 7373 5574  .....z#ProcessUt
-00001a00: 696c 732e 6164 645f 656c 656d 656e 745f  ils.add_element_
-00001a10: 7661 6c75 655f 6c69 7374 6302 0000 0000  value_listc.....
-00001a20: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00001a30: 0000 0073 0e00 0000 7400 7401 7c00 7c01  ...s....t.t.|.|.
-00001a40: 8302 8301 5300 2901 7adc 0a20 2020 2020  ....S.).z..     
-00001a50: 2020 2047 6574 2061 6e20 656c 656d 656e     Get an elemen
-00001a60: 7420 6173 2061 2073 7472 2e0a 0a20 2020  t as a str...   
-00001a70: 2020 2020 2041 7267 756d 656e 7473 3a0a       Arguments:.
-00001a80: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00001a90: 6573 733a 2054 6865 2070 726f 6365 7373  ess: The process
-00001aa0: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00001ab0: 656d 656e 745f 6465 6669 6e69 7469 6f6e  ement_definition
-00001ac0: 5f63 6f64 653a 2054 6865 2065 6c65 6d65  _code: The eleme
-00001ad0: 6e74 2064 6566 696e 6974 696f 6e20 636f  nt definition co
-00001ae0: 6465 2e0a 0a20 2020 2020 2020 2052 6574  de...        Ret
-00001af0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00001b00: 2020 5468 6520 656c 656d 656e 7420 7661    The element va
-00001b10: 6c75 6520 6173 2061 2073 7472 2e0a 2020  lue as a str..  
-00001b20: 2020 2020 2020 2902 721b 0000 0072 3c00        ).r....r<.
-00001b30: 0000 723d 0000 0072 3e00 0000 723e 0000  ..r=...r>...r>..
-00001b40: 0072 3f00 0000 721b 0000 00f1 0000 0073  .r?...r........s
-00001b50: 0200 0000 000c 7a25 5072 6f63 6573 7355  ......z%ProcessU
-00001b60: 7469 6c73 2e67 6574 5f65 6c65 6d65 6e74  tils.get_element
-00001b70: 5f76 616c 7565 5f61 735f 7374 7263 0200  _value_as_strc..
-00001b80: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001b90: 0000 4300 0000 730e 0000 0074 0074 017c  ..C...s....t.t.|
-00001ba0: 007c 0183 0283 0153 0029 017a e30a 2020  .|.....S.).z..  
-00001bb0: 2020 2020 2020 5472 7920 746f 2067 6574        Try to get
-00001bc0: 2061 6e20 656c 656d 656e 7420 6173 2061   an element as a
-00001bd0: 2073 7472 2e0a 0a20 2020 2020 2020 2041   str...        A
-00001be0: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-00001bf0: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
-00001c00: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
-00001c10: 2020 2020 2020 2020 656c 656d 656e 745f          element_
-00001c20: 6465 6669 6e69 7469 6f6e 5f63 6f64 653a  definition_code:
-00001c30: 2054 6865 2065 6c65 6d65 6e74 2064 6566   The element def
-00001c40: 696e 6974 696f 6e20 636f 6465 2e0a 0a20  inition code... 
-00001c50: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00001c60: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001c70: 656c 656d 656e 7420 7661 6c75 6520 6173  element value as
-00001c80: 2061 2073 7472 2e0a 2020 2020 2020 2020   a str..        
-00001c90: 2902 7216 0000 0072 3c00 0000 723d 0000  ).r....r<...r=..
-00001ca0: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
-00001cb0: 7216 0000 00ff 0000 0073 0200 0000 000c  r........s......
-00001cc0: 7a26 5072 6f63 6573 7355 7469 6c73 2e66  z&ProcessUtils.f
-00001cd0: 696e 645f 656c 656d 656e 745f 7661 6c75  ind_element_valu
-00001ce0: 655f 6173 5f73 7472 6302 0000 0000 0000  e_as_strc.......
-00001cf0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00001d00: 0073 0e00 0000 7400 7401 7c00 7c01 8302  .s....t.t.|.|...
-00001d10: 8301 5300 2901 7aee 0a20 2020 2020 2020  ..S.).z..       
-00001d20: 2054 7279 2074 6f20 6765 7420 616e 2065   Try to get an e
-00001d30: 6c65 6d65 6e74 2061 7320 6120 7374 7220  lement as a str 
-00001d40: 6c69 7374 2e0a 0a20 2020 2020 2020 2041  list...        A
-00001d50: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-00001d60: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
-00001d70: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
-00001d80: 2020 2020 2020 2020 656c 656d 656e 745f          element_
-00001d90: 6465 6669 6e69 7469 6f6e 5f63 6f64 653a  definition_code:
-00001da0: 2054 6865 2065 6c65 6d65 6e74 2064 6566   The element def
-00001db0: 696e 6974 696f 6e20 636f 6465 2e0a 0a20  inition code... 
-00001dc0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00001dd0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001de0: 656c 656d 656e 7420 7661 6c75 6573 2061  element values a
-00001df0: 7320 6120 7374 7220 6c69 7374 2e0a 2020  s a str list..  
-00001e00: 2020 2020 2020 2902 721c 0000 0072 3c00        ).r....r<.
-00001e10: 0000 723d 0000 0072 3e00 0000 723e 0000  ..r=...r>...r>..
-00001e20: 0072 3f00 0000 721c 0000 000d 0100 0073  .r?...r........s
-00001e30: 0200 0000 000c 7a2a 5072 6f63 6573 7355  ......z*ProcessU
-00001e40: 7469 6c73 2e67 6574 5f65 6c65 6d65 6e74  tils.get_element
-00001e50: 5f76 616c 7565 5f61 735f 7374 725f 6c69  _value_as_str_li
-00001e60: 7374 6302 0000 0000 0000 0000 0000 0002  stc.............
-00001e70: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
-00001e80: 7400 7401 7c00 7c01 8302 8301 5300 2901  t.t.|.|.....S.).
-00001e90: 7ae0 0a20 2020 2020 2020 2047 6574 2061  z..        Get a
-00001ea0: 6e20 656c 656d 656e 7420 6173 2061 2066  n element as a f
-00001eb0: 6c6f 6174 2e0a 0a20 2020 2020 2020 2041  loat...        A
-00001ec0: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-00001ed0: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
-00001ee0: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
-00001ef0: 2020 2020 2020 2020 656c 656d 656e 745f          element_
-00001f00: 6465 6669 6e69 7469 6f6e 5f63 6f64 653a  definition_code:
-00001f10: 2054 6865 2065 6c65 6d65 6e74 2064 6566   The element def
-00001f20: 696e 6974 696f 6e20 636f 6465 2e0a 0a20  inition code... 
-00001f30: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00001f40: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001f50: 656c 656d 656e 7420 7661 6c75 6520 6173  element value as
-00001f60: 2061 2066 6c6f 6174 2e0a 2020 2020 2020   a float..      
-00001f70: 2020 2902 7219 0000 0072 3c00 0000 723d    ).r....r<...r=
-00001f80: 0000 0072 3e00 0000 723e 0000 0072 3f00  ...r>...r>...r?.
-00001f90: 0000 7219 0000 001b 0100 0073 0200 0000  ..r........s....
-00001fa0: 000c 7a27 5072 6f63 6573 7355 7469 6c73  ..z'ProcessUtils
-00001fb0: 2e67 6574 5f65 6c65 6d65 6e74 5f76 616c  .get_element_val
-00001fc0: 7565 5f61 735f 666c 6f61 7463 0200 0000  ue_as_floatc....
-00001fd0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001fe0: 4300 0000 730e 0000 0074 0074 017c 007c  C...s....t.t.|.|
-00001ff0: 0183 0283 0153 0029 017a e70a 2020 2020  .....S.).z..    
-00002000: 2020 2020 5472 7920 746f 2067 6574 2061      Try to get a
-00002010: 6e20 656c 656d 656e 7420 6173 2061 2066  n element as a f
-00002020: 6c6f 6174 2e0a 0a20 2020 2020 2020 2041  loat...        A
-00002030: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-00002040: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
-00002050: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
-00002060: 2020 2020 2020 2020 656c 656d 656e 745f          element_
-00002070: 6465 6669 6e69 7469 6f6e 5f63 6f64 653a  definition_code:
-00002080: 2054 6865 2065 6c65 6d65 6e74 2064 6566   The element def
-00002090: 696e 6974 696f 6e20 636f 6465 2e0a 0a20  inition code... 
-000020a0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000020b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000020c0: 656c 656d 656e 7420 7661 6c75 6520 6173  element value as
-000020d0: 2061 2066 6c6f 6174 2e0a 2020 2020 2020   a float..      
-000020e0: 2020 2902 7215 0000 0072 3c00 0000 723d    ).r....r<...r=
-000020f0: 0000 0072 3e00 0000 723e 0000 0072 3f00  ...r>...r>...r?.
-00002100: 0000 7215 0000 0029 0100 0073 0200 0000  ..r....)...s....
-00002110: 000c 7a28 5072 6f63 6573 7355 7469 6c73  ..z(ProcessUtils
-00002120: 2e66 696e 645f 656c 656d 656e 745f 7661  .find_element_va
-00002130: 6c75 655f 6173 5f66 6c6f 6174 6302 0000  lue_as_floatc...
-00002140: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00002150: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
-00002160: 7c01 8302 8301 5300 2901 7ae7 0a20 2020  |.....S.).z..   
-00002170: 2020 2020 2047 6574 2061 6c6c 2065 6c65       Get all ele
-00002180: 6d65 6e74 7320 6173 2061 2066 6c6f 6174  ments as a float
-00002190: 206c 6973 742e 0a0a 2020 2020 2020 2020   list...        
-000021a0: 4172 6775 6d65 6e74 733a 0a20 2020 2020  Arguments:.     
-000021b0: 2020 2020 2020 2070 726f 6365 7373 3a20         process: 
-000021c0: 5468 6520 7072 6f63 6573 732e 0a20 2020  The process..   
-000021d0: 2020 2020 2020 2020 2065 6c65 6d65 6e74           element
-000021e0: 5f64 6566 696e 6974 696f 6e5f 636f 6465  _definition_code
-000021f0: 3a20 5468 6520 656c 656d 656e 7420 6465  : The element de
-00002200: 6669 6e69 7469 6f6e 2063 6f64 652e 0a0a  finition code...
-00002210: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00002220: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00002230: 2065 6c65 6d65 6e74 2076 616c 7565 2061   element value a
-00002240: 7320 6120 666c 6f61 742e 0a20 2020 2020  s a float..     
-00002250: 2020 2029 0272 1a00 0000 723c 0000 0072     ).r....r<...r
-00002260: 3d00 0000 723e 0000 0072 3e00 0000 723f  =...r>...r>...r?
-00002270: 0000 0072 1a00 0000 3701 0000 7302 0000  ...r....7...s...
-00002280: 0000 0c7a 2c50 726f 6365 7373 5574 696c  ...z,ProcessUtil
-00002290: 732e 6765 745f 656c 656d 656e 745f 7661  s.get_element_va
-000022a0: 6c75 655f 6173 5f66 6c6f 6174 5f6c 6973  lue_as_float_lis
-000022b0: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
-000022c0: 0000 0400 0000 4300 0000 730e 0000 0074  ......C...s....t
-000022d0: 0074 017c 007c 0183 0283 0153 0029 017a  .t.|.|.....S.).z
-000022e0: de0a 2020 2020 2020 2020 4765 7420 616e  ..        Get an
-000022f0: 2065 6c65 6d65 6e74 2061 7320 6120 6461   element as a da
-00002300: 7465 2e0a 0a20 2020 2020 2020 2041 7267  te...        Arg
-00002310: 756d 656e 7473 3a0a 2020 2020 2020 2020  uments:.        
-00002320: 2020 2020 7072 6f63 6573 733a 2054 6865      process: The
-00002330: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
-00002340: 2020 2020 2020 656c 656d 656e 745f 6465        element_de
-00002350: 6669 6e69 7469 6f6e 5f63 6f64 653a 2054  finition_code: T
-00002360: 6865 2065 6c65 6d65 6e74 2064 6566 696e  he element defin
-00002370: 6974 696f 6e20 636f 6465 2e0a 0a20 2020  ition code...   
-00002380: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00002390: 2020 2020 2020 2020 2020 5468 6520 656c            The el
-000023a0: 656d 656e 7420 7661 6c75 6520 6173 2061  ement value as a
-000023b0: 2064 6174 652e 0a20 2020 2020 2020 2029   date..        )
-000023c0: 0272 1700 0000 723c 0000 0072 3d00 0000  .r....r<...r=...
-000023d0: 723e 0000 0072 3e00 0000 723f 0000 0072  r>...r>...r?...r
-000023e0: 1700 0000 4501 0000 7302 0000 0000 0c7a  ....E...s......z
-000023f0: 2650 726f 6365 7373 5574 696c 732e 6765  &ProcessUtils.ge
-00002400: 745f 656c 656d 656e 745f 7661 6c75 655f  t_element_value_
-00002410: 6173 5f64 6174 6563 0200 0000 0000 0000  as_datec........
-00002420: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00002430: 730e 0000 0074 0074 017c 007c 0183 0283  s....t.t.|.|....
-00002440: 0153 0029 017a e60a 2020 2020 2020 2020  .S.).z..        
-00002450: 5472 7920 746f 2067 6574 2020 616e 2065  Try to get  an e
-00002460: 6c65 6d65 6e74 2061 7320 6120 6461 7465  lement as a date
-00002470: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
-00002480: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
-00002490: 2020 7072 6f63 6573 733a 2054 6865 2070    process: The p
-000024a0: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
-000024b0: 2020 2020 656c 656d 656e 745f 6465 6669      element_defi
-000024c0: 6e69 7469 6f6e 5f63 6f64 653a 2054 6865  nition_code: The
-000024d0: 2065 6c65 6d65 6e74 2064 6566 696e 6974   element definit
-000024e0: 696f 6e20 636f 6465 2e0a 0a20 2020 2020  ion code...     
-000024f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00002500: 2020 2020 2020 2020 5468 6520 656c 656d          The elem
-00002510: 656e 7420 7661 6c75 6520 6173 2061 2064  ent value as a d
-00002520: 6174 652e 0a20 2020 2020 2020 2029 0272  ate..        ).r
-00002530: 1400 0000 723c 0000 0072 3d00 0000 723e  ....r<...r=...r>
-00002540: 0000 0072 3e00 0000 723f 0000 0072 1400  ...r>...r?...r..
-00002550: 0000 5301 0000 7302 0000 0000 0c7a 2750  ..S...s......z'P
-00002560: 726f 6365 7373 5574 696c 732e 6669 6e64  rocessUtils.find
-00002570: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f61  _element_value_a
-00002580: 735f 6461 7465 6302 0000 0000 0000 0000  s_datec.........
-00002590: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-000025a0: 0e00 0000 7400 7401 7c00 7c01 8302 8301  ....t.t.|.|.....
-000025b0: 5300 2901 7ae3 0a20 2020 2020 2020 2047  S.).z..        G
-000025c0: 6574 2061 6c6c 2065 6c65 6d65 6e74 7320  et all elements 
-000025d0: 6173 2064 6174 6520 6c69 7374 2e0a 0a20  as date list... 
-000025e0: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-000025f0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00002600: 6f63 6573 733a 2054 6865 2070 726f 6365  ocess: The proce
-00002610: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
-00002620: 656c 656d 656e 745f 6465 6669 6e69 7469  element_definiti
-00002630: 6f6e 5f63 6f64 653a 2054 6865 2065 6c65  on_code: The ele
-00002640: 6d65 6e74 2064 6566 696e 6974 696f 6e20  ment definition 
-00002650: 636f 6465 2e0a 0a20 2020 2020 2020 2052  code...        R
-00002660: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00002670: 2020 2020 5468 6520 656c 656d 656e 7420      The element 
-00002680: 7661 6c75 6520 6173 2061 2064 6174 652e  value as a date.
-00002690: 0a20 2020 2020 2020 2029 0272 1800 0000  .        ).r....
-000026a0: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
-000026b0: 3e00 0000 723f 0000 0072 1800 0000 6101  >...r?...r....a.
-000026c0: 0000 7302 0000 0000 0c7a 2b50 726f 6365  ..s......z+Proce
-000026d0: 7373 5574 696c 732e 6765 745f 656c 656d  ssUtils.get_elem
-000026e0: 656e 745f 7661 6c75 655f 6173 5f64 6174  ent_value_as_dat
-000026f0: 655f 6c69 7374 2903 7239 0000 00da 0d70  e_list).r9.....p
-00002700: 726f 7065 7274 795f 7061 7468 723b 0000  roperty_pathr;..
-00002710: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00002720: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00002730: 0074 017c 0083 017c 0183 0253 0029 0161  .t.|...|...S.).a
-00002740: 7901 0000 0a20 2020 2020 2020 2047 6574  y....        Get
-00002750: 2061 206a 736f 6e20 7072 6f70 6572 7479   a json property
-00002760: 2061 7320 2273 7472 2220 666f 6c6c 6f77   as "str" follow
-00002770: 696e 6720 7468 6520 2270 726f 7065 7274  ing the "propert
-00002780: 7950 6174 6822 2070 6173 7365 642e 0a0a  yPath" passed...
-00002790: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-000027a0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-000027b0: 726f 6365 7373 3a20 5468 6520 7072 6f63  rocess: The proc
-000027c0: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
-000027d0: 2070 726f 7065 7274 795f 7061 7468 3a20   property_path: 
-000027e0: 5072 6f70 6572 7479 2070 6174 6820 746f  Property path to
-000027f0: 2066 696e 642e 2069 653a 2022 7573 6572   find. ie: "user
-00002800: 2e6e 616d 6522 206f 7220 2275 7365 7273  .name" or "users
-00002810: 2e30 2e6e 616d 6522 0a0a 2020 2020 2020  .0.name"..      
-00002820: 2020 5265 7475 726e 3a0a 2020 2020 2020    Return:.      
-00002830: 2020 2020 2020 7468 6520 7072 6f70 6572        the proper
-00002840: 7479 2076 616c 7565 2069 6620 6578 6973  ty value if exis
-00002850: 7473 2e0a 0a20 2020 2020 2020 2052 6169  ts...        Rai
-00002860: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-00002870: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
-00002880: 7072 6f70 6572 7479 2076 616c 7565 2064  property value d
-00002890: 6f65 736e 2774 2065 7869 7374 206f 7220  oesn't exist or 
-000028a0: 6861 7320 696e 636f 7272 6563 7420 666f  has incorrect fo
-000028b0: 726d 6174 0a20 2020 2020 2020 2029 0272  rmat.        ).r
-000028c0: 3600 0000 da1b 4375 7272 656e 744a 736f  6.....CurrentJso
-000028d0: 6e46 6f72 6d44 6174 6141 6363 6573 736f  nFormDataAccesso
-000028e0: 72a9 0272 3900 0000 7246 0000 0072 3e00  r..r9...rF...r>.
-000028f0: 0000 723e 0000 0072 3f00 0000 da1a 6765  ..r>...r?.....ge
-00002900: 745f 656e 7469 7479 5f70 726f 7065 7274  t_entity_propert
-00002910: 795f 6173 5f73 7472 6f01 0000 7302 0000  y_as_stro...s...
-00002920: 0000 0f7a 2750 726f 6365 7373 5574 696c  ...z'ProcessUtil
-00002930: 732e 6765 745f 656e 7469 7479 5f70 726f  s.get_entity_pro
-00002940: 7065 7274 795f 6173 5f73 7472 6302 0000  perty_as_strc...
-00002950: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002960: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
-00002970: 8301 7c01 8302 5300 2901 6170 0100 000a  ..|...S.).ap....
-00002980: 2020 2020 2020 2020 5472 7920 746f 2066          Try to f
-00002990: 696e 6420 6120 6a73 6f6e 2070 726f 7065  ind a json prope
-000029a0: 7274 7920 6173 2022 7374 7222 2066 6f6c  rty as "str" fol
-000029b0: 6c6f 7769 6e67 2074 6865 2022 7072 6f70  lowing the "prop
-000029c0: 6572 7479 5061 7468 2220 7061 7373 6564  ertyPath" passed
-000029d0: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
-000029e0: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
-000029f0: 2020 7072 6f63 6573 733a 2054 6865 2070    process: The p
-00002a00: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
-00002a10: 2020 2020 7072 6f70 6572 7479 5f70 6174      property_pat
-00002a20: 683a 2050 726f 7065 7274 7920 7061 7468  h: Property path
-00002a30: 2074 6f20 6669 6e64 2e20 6965 3a20 2275   to find. ie: "u
-00002a40: 7365 722e 6e61 6d65 2220 6f72 2022 7573  ser.name" or "us
-00002a50: 6572 732e 302e 6e61 6d65 220a 0a20 2020  ers.0.name"..   
-00002a60: 2020 2020 2052 6574 7572 6e3a 0a20 2020       Return:.   
-00002a70: 2020 2020 2020 2020 2054 6865 2070 726f           The pro
-00002a80: 7065 7274 7920 7661 6c75 6520 6966 2065  perty value if e
-00002a90: 7869 7374 732e 0a0a 2020 2020 2020 2020  xists...        
-00002aa0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00002ab0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00002ac0: 4966 2070 726f 7065 7274 7920 7661 6c75  If property valu
-00002ad0: 6520 6861 7320 696e 636f 7272 6563 7420  e has incorrect 
-00002ae0: 666f 726d 6174 0a20 2020 2020 2020 2029  format.        )
-00002af0: 0272 2d00 0000 7247 0000 0072 4800 0000  .r-...rG...rH...
-00002b00: 723e 0000 0072 3e00 0000 723f 0000 00da  r>...r>...r?....
-00002b10: 1b66 696e 645f 656e 7469 7479 5f70 726f  .find_entity_pro
-00002b20: 7065 7274 795f 6173 5f73 7472 8001 0000  perty_as_str....
-00002b30: 7302 0000 0000 0f7a 2850 726f 6365 7373  s......z(Process
-00002b40: 5574 696c 732e 6669 6e64 5f65 6e74 6974  Utils.find_entit
-00002b50: 795f 7072 6f70 6572 7479 5f61 735f 7374  y_property_as_st
-00002b60: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
-00002b70: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00002b80: 0074 017c 0083 017c 0183 0253 0029 0161  .t.|...|...S.).a
-00002b90: 7901 0000 0a20 2020 2020 2020 2047 6574  y....        Get
-00002ba0: 2061 206a 736f 6e20 7072 6f70 6572 7479   a json property
-00002bb0: 2061 7320 2269 6e74 2220 666f 6c6c 6f77   as "int" follow
-00002bc0: 696e 6720 7468 6520 2270 726f 7065 7274  ing the "propert
-00002bd0: 7950 6174 6822 2070 6173 7365 642e 0a0a  yPath" passed...
-00002be0: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-00002bf0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-00002c00: 726f 6365 7373 3a20 5468 6520 7072 6f63  rocess: The proc
-00002c10: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
-00002c20: 2070 726f 7065 7274 795f 7061 7468 3a20   property_path: 
-00002c30: 5072 6f70 6572 7479 2070 6174 6820 746f  Property path to
-00002c40: 2066 696e 642e 2069 653a 2022 7573 6572   find. ie: "user
-00002c50: 2e6e 616d 6522 206f 7220 2275 7365 7273  .name" or "users
-00002c60: 2e30 2e6e 616d 6522 0a0a 2020 2020 2020  .0.name"..      
-00002c70: 2020 5265 7475 726e 3a0a 2020 2020 2020    Return:.      
-00002c80: 2020 2020 2020 7468 6520 7072 6f70 6572        the proper
-00002c90: 7479 2076 616c 7565 2069 6620 6578 6973  ty value if exis
-00002ca0: 7473 2e0a 0a20 2020 2020 2020 2052 6169  ts...        Rai
-00002cb0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-00002cc0: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
-00002cd0: 7072 6f70 6572 7479 2076 616c 7565 2064  property value d
-00002ce0: 6f65 736e 2774 2065 7869 7374 206f 7220  oesn't exist or 
-00002cf0: 6861 7320 696e 636f 7272 6563 7420 666f  has incorrect fo
-00002d00: 726d 6174 0a20 2020 2020 2020 2029 0272  rmat.        ).r
-00002d10: 3200 0000 7247 0000 0072 4800 0000 723e  2...rG...rH...r>
-00002d20: 0000 0072 3e00 0000 723f 0000 00da 1a67  ...r>...r?.....g
-00002d30: 6574 5f65 6e74 6974 795f 7072 6f70 6572  et_entity_proper
-00002d40: 7479 5f61 735f 696e 7491 0100 0073 0200  ty_as_int....s..
-00002d50: 0000 000f 7a27 5072 6f63 6573 7355 7469  ....z'ProcessUti
-00002d60: 6c73 2e67 6574 5f65 6e74 6974 795f 7072  ls.get_entity_pr
-00002d70: 6f70 6572 7479 5f61 735f 696e 7463 0200  operty_as_intc..
-00002d80: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00002d90: 0000 4300 0000 730e 0000 0074 0074 017c  ..C...s....t.t.|
-00002da0: 0083 017c 0183 0253 0029 0161 7001 0000  ...|...S.).ap...
-00002db0: 0a20 2020 2020 2020 2054 7279 2074 6f20  .        Try to 
-00002dc0: 6669 6e64 2061 206a 736f 6e20 7072 6f70  find a json prop
-00002dd0: 6572 7479 2061 7320 2269 6e74 2220 666f  erty as "int" fo
-00002de0: 6c6c 6f77 696e 6720 7468 6520 2270 726f  llowing the "pro
-00002df0: 7065 7274 7950 6174 6822 2070 6173 7365  pertyPath" passe
-00002e00: 642e 0a0a 2020 2020 2020 2020 4172 6775  d...        Argu
-00002e10: 6d65 6e74 733a 0a20 2020 2020 2020 2020  ments:.         
-00002e20: 2020 2070 726f 6365 7373 3a20 5468 6520     process: The 
-00002e30: 7072 6f63 6573 732e 0a20 2020 2020 2020  process..       
-00002e40: 2020 2020 2070 726f 7065 7274 795f 7061       property_pa
-00002e50: 7468 3a20 5072 6f70 6572 7479 2070 6174  th: Property pat
-00002e60: 6820 746f 2066 696e 642e 2069 653a 2022  h to find. ie: "
-00002e70: 7573 6572 2e6e 616d 6522 206f 7220 2275  user.name" or "u
-00002e80: 7365 7273 2e30 2e6e 616d 6522 0a0a 2020  sers.0.name"..  
-00002e90: 2020 2020 2020 5265 7475 726e 3a0a 2020        Return:.  
-00002ea0: 2020 2020 2020 2020 2020 5468 6520 7072            The pr
-00002eb0: 6f70 6572 7479 2076 616c 7565 2069 6620  operty value if 
-00002ec0: 6578 6973 7473 2e0a 0a20 2020 2020 2020  exists...       
-00002ed0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00002ee0: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
-00002ef0: 2049 6620 7072 6f70 6572 7479 2076 616c   If property val
-00002f00: 7565 2068 6173 2069 6e63 6f72 7265 6374  ue has incorrect
-00002f10: 2066 6f72 6d61 740a 2020 2020 2020 2020   format.        
-00002f20: 2902 7229 0000 0072 4700 0000 7248 0000  ).r)...rG...rH..
-00002f30: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
-00002f40: da1b 6669 6e64 5f65 6e74 6974 795f 7072  ..find_entity_pr
-00002f50: 6f70 6572 7479 5f61 735f 696e 74a2 0100  operty_as_int...
-00002f60: 0073 0200 0000 000f 7a28 5072 6f63 6573  .s......z(Proces
-00002f70: 7355 7469 6c73 2e66 696e 645f 656e 7469  sUtils.find_enti
-00002f80: 7479 5f70 726f 7065 7274 795f 6173 5f69  ty_property_as_i
-00002f90: 6e74 6302 0000 0000 0000 0000 0000 0002  ntc.............
-00002fa0: 0000 0003 0000 0043 0000 0073 0e00 0000  .......C...s....
-00002fb0: 7400 7401 7c00 8301 7c01 8302 5300 2901  t.t.|...|...S.).
-00002fc0: 617b 0100 000a 2020 2020 2020 2020 4765  a{....        Ge
-00002fd0: 7420 6120 6a73 6f6e 2070 726f 7065 7274  t a json propert
-00002fe0: 7920 6173 2022 666c 6f61 7422 2066 6f6c  y as "float" fol
-00002ff0: 6c6f 7769 6e67 2074 6865 2022 7072 6f70  lowing the "prop
-00003000: 6572 7479 5061 7468 2220 7061 7373 6564  ertyPath" passed
-00003010: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
-00003020: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
-00003030: 2020 7072 6f63 6573 733a 2054 6865 2070    process: The p
-00003040: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
-00003050: 2020 2020 7072 6f70 6572 7479 5f70 6174      property_pat
-00003060: 683a 2050 726f 7065 7274 7920 7061 7468  h: Property path
-00003070: 2074 6f20 6669 6e64 2e20 6965 3a20 2275   to find. ie: "u
-00003080: 7365 722e 6e61 6d65 2220 6f72 2022 7573  ser.name" or "us
-00003090: 6572 732e 302e 6e61 6d65 220a 0a20 2020  ers.0.name"..   
-000030a0: 2020 2020 2052 6574 7572 6e3a 0a20 2020       Return:.   
-000030b0: 2020 2020 2020 2020 2074 6865 2070 726f           the pro
-000030c0: 7065 7274 7920 7661 6c75 6520 6966 2065  perty value if e
-000030d0: 7869 7374 732e 0a0a 2020 2020 2020 2020  xists...        
-000030e0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-000030f0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00003100: 4966 2070 726f 7065 7274 7920 7661 6c75  If property valu
-00003110: 6520 646f 6573 6e27 7420 6578 6973 7420  e doesn't exist 
-00003120: 6f72 2068 6173 2069 6e63 6f72 7265 6374  or has incorrect
-00003130: 2066 6f72 6d61 740a 2020 2020 2020 2020   format.        
-00003140: 2902 7231 0000 0072 4700 0000 7248 0000  ).r1...rG...rH..
-00003150: 0072 3e00 0000 723e 0000 0072 3f00 0000  .r>...r>...r?...
-00003160: da1c 6765 745f 656e 7469 7479 5f70 726f  ..get_entity_pro
-00003170: 7065 7274 795f 6173 5f66 6c6f 6174 b301  perty_as_float..
-00003180: 0000 7302 0000 0000 0f7a 2950 726f 6365  ..s......z)Proce
-00003190: 7373 5574 696c 732e 6765 745f 656e 7469  ssUtils.get_enti
-000031a0: 7479 5f70 726f 7065 7274 795f 6173 5f66  ty_property_as_f
-000031b0: 6c6f 6174 6302 0000 0000 0000 0000 0000  loatc...........
-000031c0: 0002 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
-000031d0: 0000 7400 7401 7c00 8301 7c01 8302 5300  ..t.t.|...|...S.
-000031e0: 2901 6172 0100 000a 2020 2020 2020 2020  ).ar....        
-000031f0: 5472 7920 746f 2066 696e 6420 6120 6a73  Try to find a js
-00003200: 6f6e 2070 726f 7065 7274 7920 6173 2022  on property as "
-00003210: 666c 6f61 7422 2066 6f6c 6c6f 7769 6e67  float" following
-00003220: 2074 6865 2022 7072 6f70 6572 7479 5061   the "propertyPa
-00003230: 7468 2220 7061 7373 6564 2e0a 0a20 2020  th" passed...   
-00003240: 2020 2020 2041 7267 756d 656e 7473 3a0a       Arguments:.
-00003250: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00003260: 6573 733a 2054 6865 2070 726f 6365 7373  ess: The process
-00003270: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00003280: 6f70 6572 7479 5f70 6174 683a 2050 726f  operty_path: Pro
-00003290: 7065 7274 7920 7061 7468 2074 6f20 6669  perty path to fi
-000032a0: 6e64 2e20 6965 3a20 2275 7365 722e 6e61  nd. ie: "user.na
-000032b0: 6d65 2220 6f72 2022 7573 6572 732e 302e  me" or "users.0.
-000032c0: 6e61 6d65 220a 0a20 2020 2020 2020 2052  name"..        R
-000032d0: 6574 7572 6e3a 0a20 2020 2020 2020 2020  eturn:.         
-000032e0: 2020 2054 6865 2070 726f 7065 7274 7920     The property 
-000032f0: 7661 6c75 6520 6966 2065 7869 7374 732e  value if exists.
-00003300: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00003310: 3a0a 2020 2020 2020 2020 2020 2020 5661  :.            Va
-00003320: 6c75 6545 7272 6f72 3a20 4966 2070 726f  lueError: If pro
-00003330: 7065 7274 7920 7661 6c75 6520 6861 7320  perty value has 
-00003340: 696e 636f 7272 6563 7420 666f 726d 6174  incorrect format
-00003350: 0a20 2020 2020 2020 2029 0272 2800 0000  .        ).r(...
-00003360: 7247 0000 0072 4800 0000 723e 0000 0072  rG...rH...r>...r
-00003370: 3e00 0000 723f 0000 00da 1d66 696e 645f  >...r?.....find_
-00003380: 656e 7469 7479 5f70 726f 7065 7274 795f  entity_property_
-00003390: 6173 5f66 6c6f 6174 c401 0000 7302 0000  as_float....s...
-000033a0: 0000 0f7a 2a50 726f 6365 7373 5574 696c  ...z*ProcessUtil
-000033b0: 732e 6669 6e64 5f65 6e74 6974 795f 7072  s.find_entity_pr
-000033c0: 6f70 6572 7479 5f61 735f 666c 6f61 7463  operty_as_floatc
-000033d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000033e0: 0300 0000 4300 0000 730e 0000 0074 0074  ....C...s....t.t
-000033f0: 017c 0083 017c 0183 0253 0029 0161 7a01  .|...|...S.).az.
-00003400: 0000 0a20 2020 2020 2020 2047 6574 2061  ...        Get a
-00003410: 206a 736f 6e20 7072 6f70 6572 7479 2061   json property a
-00003420: 7320 2264 6174 6522 2066 6f6c 6c6f 7769  s "date" followi
-00003430: 6e67 2074 6865 2022 7072 6f70 6572 7479  ng the "property
-00003440: 5061 7468 2220 7061 7373 6564 2e0a 0a20  Path" passed... 
-00003450: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-00003460: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00003470: 6f63 6573 733a 2054 6865 2070 726f 6365  ocess: The proce
-00003480: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
-00003490: 7072 6f70 6572 7479 5f70 6174 683a 2050  property_path: P
-000034a0: 726f 7065 7274 7920 7061 7468 2074 6f20  roperty path to 
-000034b0: 6669 6e64 2e20 6965 3a20 2275 7365 722e  find. ie: "user.
-000034c0: 6e61 6d65 2220 6f72 2022 7573 6572 732e  name" or "users.
-000034d0: 302e 6e61 6d65 220a 0a20 2020 2020 2020  0.name"..       
-000034e0: 2052 6574 7572 6e3a 0a20 2020 2020 2020   Return:.       
-000034f0: 2020 2020 2074 6865 2070 726f 7065 7274       the propert
-00003500: 7920 7661 6c75 6520 6966 2065 7869 7374  y value if exist
-00003510: 732e 0a0a 2020 2020 2020 2020 5261 6973  s...        Rais
-00003520: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00003530: 5661 6c75 6545 7272 6f72 3a20 4966 2070  ValueError: If p
-00003540: 726f 7065 7274 7920 7661 6c75 6520 646f  roperty value do
-00003550: 6573 6e27 7420 6578 6973 7420 6f72 2068  esn't exist or h
-00003560: 6173 2069 6e63 6f72 7265 6374 2066 6f72  as incorrect for
-00003570: 6d61 740a 2020 2020 2020 2020 2902 722e  mat.        ).r.
-00003580: 0000 0072 4700 0000 7248 0000 0072 3e00  ...rG...rH...r>.
-00003590: 0000 723e 0000 0072 3f00 0000 da1b 6765  ..r>...r?.....ge
-000035a0: 745f 656e 7469 7479 5f70 726f 7065 7274  t_entity_propert
-000035b0: 795f 6173 5f64 6174 65d5 0100 0073 0200  y_as_date....s..
-000035c0: 0000 000f 7a28 5072 6f63 6573 7355 7469  ....z(ProcessUti
-000035d0: 6c73 2e67 6574 5f65 6e74 6974 795f 7072  ls.get_entity_pr
-000035e0: 6f70 6572 7479 5f61 735f 6461 7465 6302  operty_as_datec.
-000035f0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00003600: 0000 0043 0000 0073 0e00 0000 7400 7401  ...C...s....t.t.
-00003610: 7c00 8301 7c01 8302 5300 2901 6171 0100  |...|...S.).aq..
-00003620: 000a 2020 2020 2020 2020 5472 7920 746f  ..        Try to
-00003630: 2066 696e 6420 6120 6a73 6f6e 2070 726f   find a json pro
-00003640: 7065 7274 7920 6173 2022 6461 7465 2220  perty as "date" 
-00003650: 666f 6c6c 6f77 696e 6720 7468 6520 2270  following the "p
-00003660: 726f 7065 7274 7950 6174 6822 2070 6173  ropertyPath" pas
-00003670: 7365 642e 0a0a 2020 2020 2020 2020 4172  sed...        Ar
-00003680: 6775 6d65 6e74 733a 0a20 2020 2020 2020  guments:.       
-00003690: 2020 2020 2070 726f 6365 7373 3a20 5468       process: Th
-000036a0: 6520 7072 6f63 6573 732e 0a20 2020 2020  e process..     
-000036b0: 2020 2020 2020 2070 726f 7065 7274 795f         property_
-000036c0: 7061 7468 3a20 5072 6f70 6572 7479 2070  path: Property p
-000036d0: 6174 6820 746f 2066 696e 642e 2069 653a  ath to find. ie:
-000036e0: 2022 7573 6572 2e6e 616d 6522 206f 7220   "user.name" or 
-000036f0: 2275 7365 7273 2e30 2e6e 616d 6522 0a0a  "users.0.name"..
-00003700: 2020 2020 2020 2020 5265 7475 726e 3a0a          Return:.
-00003710: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00003720: 7072 6f70 6572 7479 2076 616c 7565 2069  property value i
-00003730: 6620 6578 6973 7473 2e0a 0a20 2020 2020  f exists...     
-00003740: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-00003750: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
-00003760: 723a 2049 6620 7072 6f70 6572 7479 2076  r: If property v
-00003770: 616c 7565 2068 6173 2069 6e63 6f72 7265  alue has incorre
-00003780: 6374 2066 6f72 6d61 740a 2020 2020 2020  ct format.      
-00003790: 2020 2902 7225 0000 0072 4700 0000 7248    ).r%...rG...rH
-000037a0: 0000 0072 3e00 0000 723e 0000 0072 3f00  ...r>...r>...r?.
-000037b0: 0000 da1c 6669 6e64 5f65 6e74 6974 795f  ....find_entity_
-000037c0: 7072 6f70 6572 7479 5f61 735f 6461 7465  property_as_date
-000037d0: e601 0000 7302 0000 0000 0f7a 2950 726f  ....s......z)Pro
-000037e0: 6365 7373 5574 696c 732e 6669 6e64 5f65  cessUtils.find_e
-000037f0: 6e74 6974 795f 7072 6f70 6572 7479 5f61  ntity_property_a
-00003800: 735f 6461 7465 6302 0000 0000 0000 0000  s_datec.........
-00003810: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00003820: 0e00 0000 7400 7401 7c00 8301 7c01 8302  ....t.t.|...|...
-00003830: 5300 2901 617e 0100 000a 2020 2020 2020  S.).a~....      
-00003840: 2020 4765 7420 6120 6a73 6f6e 2070 726f    Get a json pro
-00003850: 7065 7274 7920 6173 2022 6461 7465 7469  perty as "dateti
-00003860: 6d65 2220 666f 6c6c 6f77 696e 6720 7468  me" following th
-00003870: 6520 2270 726f 7065 7274 7950 6174 6822  e "propertyPath"
-00003880: 2070 6173 7365 642e 0a0a 2020 2020 2020   passed...      
-00003890: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
-000038a0: 2020 2020 2020 2020 2070 726f 6365 7373           process
-000038b0: 3a20 5468 6520 7072 6f63 6573 732e 0a20  : The process.. 
-000038c0: 2020 2020 2020 2020 2020 2070 726f 7065             prope
-000038d0: 7274 795f 7061 7468 3a20 5072 6f70 6572  rty_path: Proper
-000038e0: 7479 2070 6174 6820 746f 2066 696e 642e  ty path to find.
-000038f0: 2069 653a 2022 7573 6572 2e6e 616d 6522   ie: "user.name"
-00003900: 206f 7220 2275 7365 7273 2e30 2e6e 616d   or "users.0.nam
-00003910: 6522 0a0a 2020 2020 2020 2020 5265 7475  e"..        Retu
-00003920: 726e 3a0a 2020 2020 2020 2020 2020 2020  rn:.            
-00003930: 7468 6520 7072 6f70 6572 7479 2076 616c  the property val
-00003940: 7565 2069 6620 6578 6973 7473 2e0a 0a20  ue if exists... 
-00003950: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00003960: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00003970: 4572 726f 723a 2049 6620 7072 6f70 6572  Error: If proper
-00003980: 7479 2076 616c 7565 2064 6f65 736e 2774  ty value doesn't
-00003990: 2065 7869 7374 206f 7220 6861 7320 696e   exist or has in
-000039a0: 636f 7272 6563 7420 666f 726d 6174 0a20  correct format. 
-000039b0: 2020 2020 2020 2029 0272 2f00 0000 7247         ).r/...rG
-000039c0: 0000 0072 4800 0000 723e 0000 0072 3e00  ...rH...r>...r>.
-000039d0: 0000 723f 0000 00da 1f67 6574 5f65 6e74  ..r?.....get_ent
-000039e0: 6974 795f 7072 6f70 6572 7479 5f61 735f  ity_property_as_
-000039f0: 6461 7465 7469 6d65 f701 0000 7302 0000  datetime....s...
-00003a00: 0000 0f7a 2c50 726f 6365 7373 5574 696c  ...z,ProcessUtil
-00003a10: 732e 6765 745f 656e 7469 7479 5f70 726f  s.get_entity_pro
-00003a20: 7065 7274 795f 6173 5f64 6174 6574 696d  perty_as_datetim
-00003a30: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00003a40: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00003a50: 0074 017c 0083 017c 0183 0253 0029 0161  .t.|...|...S.).a
-00003a60: 7501 0000 0a20 2020 2020 2020 2054 7279  u....        Try
-00003a70: 2074 6f20 6669 6e64 2061 206a 736f 6e20   to find a json 
-00003a80: 7072 6f70 6572 7479 2061 7320 2264 6174  property as "dat
-00003a90: 6574 696d 6522 2066 6f6c 6c6f 7769 6e67  etime" following
-00003aa0: 2074 6865 2022 7072 6f70 6572 7479 5061   the "propertyPa
-00003ab0: 7468 2220 7061 7373 6564 2e0a 0a20 2020  th" passed...   
-00003ac0: 2020 2020 2041 7267 756d 656e 7473 3a0a       Arguments:.
-00003ad0: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-00003ae0: 6573 733a 2054 6865 2070 726f 6365 7373  ess: The process
-00003af0: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00003b00: 6f70 6572 7479 5f70 6174 683a 2050 726f  operty_path: Pro
-00003b10: 7065 7274 7920 7061 7468 2074 6f20 6669  perty path to fi
-00003b20: 6e64 2e20 6965 3a20 2275 7365 722e 6e61  nd. ie: "user.na
-00003b30: 6d65 2220 6f72 2022 7573 6572 732e 302e  me" or "users.0.
-00003b40: 6e61 6d65 220a 0a20 2020 2020 2020 2052  name"..        R
-00003b50: 6574 7572 6e3a 0a20 2020 2020 2020 2020  eturn:.         
-00003b60: 2020 2054 6865 2070 726f 7065 7274 7920     The property 
-00003b70: 7661 6c75 6520 6966 2065 7869 7374 732e  value if exists.
-00003b80: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00003b90: 3a0a 2020 2020 2020 2020 2020 2020 5661  :.            Va
-00003ba0: 6c75 6545 7272 6f72 3a20 4966 2070 726f  lueError: If pro
-00003bb0: 7065 7274 7920 7661 6c75 6520 6861 7320  perty value has 
-00003bc0: 696e 636f 7272 6563 7420 666f 726d 6174  incorrect format
-00003bd0: 0a20 2020 2020 2020 2029 0272 2600 0000  .        ).r&...
-00003be0: 7247 0000 0072 4800 0000 723e 0000 0072  rG...rH...r>...r
-00003bf0: 3e00 0000 723f 0000 00da 2066 696e 645f  >...r?.... find_
-00003c00: 656e 7469 7479 5f70 726f 7065 7274 795f  entity_property_
-00003c10: 6173 5f64 6174 6574 696d 6508 0200 0073  as_datetime....s
-00003c20: 0200 0000 000f 7a2d 5072 6f63 6573 7355  ......z-ProcessU
-00003c30: 7469 6c73 2e66 696e 645f 656e 7469 7479  tils.find_entity
-00003c40: 5f70 726f 7065 7274 795f 6173 5f64 6174  _property_as_dat
-00003c50: 6574 696d 6563 0200 0000 0000 0000 0000  etimec..........
-00003c60: 0000 0200 0000 0300 0000 4300 0000 730e  ..........C...s.
-00003c70: 0000 0074 0074 017c 0083 017c 0183 0253  ...t.t.|...|...S
-00003c80: 0029 0161 8301 0000 0a20 2020 2020 2020  .).a.....       
-00003c90: 2047 6574 2061 206a 736f 6e20 7072 6f70   Get a json prop
-00003ca0: 6572 7479 2061 7320 224a 736f 6e46 6f72  erty as "JsonFor
-00003cb0: 6d73 4669 6c65 2220 666f 6c6c 6f77 696e  msFile" followin
-00003cc0: 6720 7468 6520 2270 726f 7065 7274 7950  g the "propertyP
-00003cd0: 6174 6822 2070 6173 7365 642e 0a0a 2020  ath" passed...  
-00003ce0: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
-00003cf0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00003d00: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
-00003d10: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
-00003d20: 726f 7065 7274 795f 7061 7468 3a20 5072  roperty_path: Pr
-00003d30: 6f70 6572 7479 2070 6174 6820 746f 2066  operty path to f
-00003d40: 696e 642e 2069 653a 2022 7573 6572 2e6e  ind. ie: "user.n
-00003d50: 616d 6522 206f 7220 2275 7365 7273 2e30  ame" or "users.0
-00003d60: 2e6e 616d 6522 0a0a 2020 2020 2020 2020  .name"..        
-00003d70: 5265 7475 726e 3a0a 2020 2020 2020 2020  Return:.        
-00003d80: 2020 2020 7468 6520 7072 6f70 6572 7479      the property
-00003d90: 2076 616c 7565 2069 6620 6578 6973 7473   value if exists
-00003da0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00003db0: 733a 0a20 2020 2020 2020 2020 2020 2056  s:.            V
-00003dc0: 616c 7565 4572 726f 723a 2049 6620 7072  alueError: If pr
-00003dd0: 6f70 6572 7479 2076 616c 7565 2064 6f65  operty value doe
-00003de0: 736e 2774 2065 7869 7374 206f 7220 6861  sn't exist or ha
-00003df0: 7320 696e 636f 7272 6563 7420 666f 726d  s incorrect form
-00003e00: 6174 0a20 2020 2020 2020 2029 0272 3300  at.        ).r3.
-00003e10: 0000 7247 0000 0072 4800 0000 723e 0000  ..rG...rH...r>..
-00003e20: 0072 3e00 0000 723f 0000 00da 1b67 6574  .r>...r?.....get
-00003e30: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
-00003e40: 5f61 735f 6669 6c65 1902 0000 7302 0000  _as_file....s...
-00003e50: 0000 0f7a 2850 726f 6365 7373 5574 696c  ...z(ProcessUtil
-00003e60: 732e 6765 745f 656e 7469 7479 5f70 726f  s.get_entity_pro
-00003e70: 7065 7274 795f 6173 5f66 696c 6563 0200  perty_as_filec..
-00003e80: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00003e90: 0000 4300 0000 730e 0000 0074 0074 017c  ..C...s....t.t.|
-00003ea0: 0083 017c 0183 0253 0029 0161 7a01 0000  ...|...S.).az...
-00003eb0: 0a20 2020 2020 2020 2054 7279 2074 6f20  .        Try to 
-00003ec0: 6669 6e64 2061 206a 736f 6e20 7072 6f70  find a json prop
-00003ed0: 6572 7479 2061 7320 224a 736f 6e46 6f72  erty as "JsonFor
-00003ee0: 6d73 4669 6c65 2220 666f 6c6c 6f77 696e  msFile" followin
-00003ef0: 6720 7468 6520 2270 726f 7065 7274 7950  g the "propertyP
-00003f00: 6174 6822 2070 6173 7365 642e 0a0a 2020  ath" passed...  
-00003f10: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
-00003f20: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00003f30: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
-00003f40: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
-00003f50: 726f 7065 7274 795f 7061 7468 3a20 5072  roperty_path: Pr
-00003f60: 6f70 6572 7479 2070 6174 6820 746f 2066  operty path to f
-00003f70: 696e 642e 2069 653a 2022 7573 6572 2e6e  ind. ie: "user.n
-00003f80: 616d 6522 206f 7220 2275 7365 7273 2e30  ame" or "users.0
-00003f90: 2e6e 616d 6522 0a0a 2020 2020 2020 2020  .name"..        
-00003fa0: 5265 7475 726e 3a0a 2020 2020 2020 2020  Return:.        
-00003fb0: 2020 2020 5468 6520 7072 6f70 6572 7479      The property
-00003fc0: 2076 616c 7565 2069 6620 6578 6973 7473   value if exists
-00003fd0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00003fe0: 733a 0a20 2020 2020 2020 2020 2020 2056  s:.            V
-00003ff0: 616c 7565 4572 726f 723a 2049 6620 7072  alueError: If pr
-00004000: 6f70 6572 7479 2076 616c 7565 2068 6173  operty value has
-00004010: 2069 6e63 6f72 7265 6374 2066 6f72 6d61   incorrect forma
-00004020: 740a 2020 2020 2020 2020 2902 722a 0000  t.        ).r*..
-00004030: 0072 4700 0000 7248 0000 0072 3e00 0000  .rG...rH...r>...
-00004040: 723e 0000 0072 3f00 0000 da1c 6669 6e64  r>...r?.....find
-00004050: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
-00004060: 5f61 735f 6669 6c65 2a02 0000 7302 0000  _as_file*...s...
-00004070: 0000 0f7a 2950 726f 6365 7373 5574 696c  ...z)ProcessUtil
-00004080: 732e 6669 6e64 5f65 6e74 6974 795f 7072  s.find_entity_pr
-00004090: 6f70 6572 7479 5f61 735f 6669 6c65 6302  operty_as_filec.
-000040a0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000040b0: 0000 0043 0000 0073 0e00 0000 7400 7401  ...C...s....t.t.
-000040c0: 7c00 8301 7c01 8302 5300 2901 6188 0100  |...|...S.).a...
-000040d0: 000a 2020 2020 2020 2020 4765 7420 6120  ..        Get a 
-000040e0: 6a73 6f6e 2070 726f 7065 7274 7920 6173  json property as
-000040f0: 2022 4a73 6f6e 466f 726d 7350 7269 6e63   "JsonFormsPrinc
-00004100: 6970 616c 2220 666f 6c6c 6f77 696e 6720  ipal" following 
-00004110: 7468 6520 2270 726f 7065 7274 7950 6174  the "propertyPat
-00004120: 6822 2070 6173 7365 642e 0a0a 2020 2020  h" passed...    
-00004130: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
-00004140: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-00004150: 7373 3a20 5468 6520 7072 6f63 6573 732e  ss: The process.
-00004160: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00004170: 7065 7274 795f 7061 7468 3a20 5072 6f70  perty_path: Prop
-00004180: 6572 7479 2070 6174 6820 746f 2066 696e  erty path to fin
-00004190: 642e 2069 653a 2022 7573 6572 2e6e 616d  d. ie: "user.nam
-000041a0: 6522 206f 7220 2275 7365 7273 2e30 2e6e  e" or "users.0.n
-000041b0: 616d 6522 0a0a 2020 2020 2020 2020 5265  ame"..        Re
-000041c0: 7475 726e 3a0a 2020 2020 2020 2020 2020  turn:.          
-000041d0: 2020 7468 6520 7072 6f70 6572 7479 2076    the property v
-000041e0: 616c 7565 2069 6620 6578 6973 7473 2e0a  alue if exists..
-000041f0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-00004200: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00004210: 7565 4572 726f 723a 2049 6620 7072 6f70  ueError: If prop
-00004220: 6572 7479 2076 616c 7565 2064 6f65 736e  erty value doesn
-00004230: 2774 2065 7869 7374 206f 7220 6861 7320  't exist or has 
-00004240: 696e 636f 7272 6563 7420 666f 726d 6174  incorrect format
-00004250: 0a20 2020 2020 2020 2029 0272 3400 0000  .        ).r4...
-00004260: 7247 0000 0072 4800 0000 723e 0000 0072  rG...rH...r>...r
-00004270: 3e00 0000 723f 0000 00da 2067 6574 5f65  >...r?.... get_e
-00004280: 6e74 6974 795f 7072 6f70 6572 7479 5f61  ntity_property_a
-00004290: 735f 7072 696e 6369 7061 6c3b 0200 0073  s_principal;...s
-000042a0: 0200 0000 000f 7a2d 5072 6f63 6573 7355  ......z-ProcessU
-000042b0: 7469 6c73 2e67 6574 5f65 6e74 6974 795f  tils.get_entity_
-000042c0: 7072 6f70 6572 7479 5f61 735f 7072 696e  property_as_prin
-000042d0: 6369 7061 6c63 0200 0000 0000 0000 0000  cipalc..........
-000042e0: 0000 0200 0000 0300 0000 4300 0000 730e  ..........C...s.
-000042f0: 0000 0074 0074 017c 0083 017c 0183 0253  ...t.t.|...|...S
-00004300: 0029 0161 7f01 0000 0a20 2020 2020 2020  .).a.....       
-00004310: 2054 7279 2074 6f20 6669 6e64 2061 206a   Try to find a j
-00004320: 736f 6e20 7072 6f70 6572 7479 2061 7320  son property as 
-00004330: 224a 736f 6e46 6f72 6d73 5072 696e 6369  "JsonFormsPrinci
-00004340: 7061 6c22 2066 6f6c 6c6f 7769 6e67 2074  pal" following t
-00004350: 6865 2022 7072 6f70 6572 7479 5061 7468  he "propertyPath
-00004360: 2220 7061 7373 6564 2e0a 0a20 2020 2020  " passed...     
-00004370: 2020 2041 7267 756d 656e 7473 3a0a 2020     Arguments:.  
-00004380: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
-00004390: 733a 2054 6865 2070 726f 6365 7373 2e0a  s: The process..
-000043a0: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
-000043b0: 6572 7479 5f70 6174 683a 2050 726f 7065  erty_path: Prope
-000043c0: 7274 7920 7061 7468 2074 6f20 6669 6e64  rty path to find
-000043d0: 2e20 6965 3a20 2275 7365 722e 6e61 6d65  . ie: "user.name
-000043e0: 2220 6f72 2022 7573 6572 732e 302e 6e61  " or "users.0.na
-000043f0: 6d65 220a 0a20 2020 2020 2020 2052 6574  me"..        Ret
-00004400: 7572 6e3a 0a20 2020 2020 2020 2020 2020  urn:.           
-00004410: 2054 6865 2070 726f 7065 7274 7920 7661   The property va
-00004420: 6c75 6520 6966 2065 7869 7374 732e 0a0a  lue if exists...
-00004430: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-00004440: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-00004450: 6545 7272 6f72 3a20 4966 2070 726f 7065  eError: If prope
-00004460: 7274 7920 7661 6c75 6520 6861 7320 696e  rty value has in
-00004470: 636f 7272 6563 7420 666f 726d 6174 0a20  correct format. 
-00004480: 2020 2020 2020 2029 0272 2b00 0000 7247         ).r+...rG
-00004490: 0000 0072 4800 0000 723e 0000 0072 3e00  ...rH...r>...r>.
-000044a0: 0000 723f 0000 00da 2166 696e 645f 656e  ..r?....!find_en
-000044b0: 7469 7479 5f70 726f 7065 7274 795f 6173  tity_property_as
-000044c0: 5f70 7269 6e63 6970 616c 4c02 0000 7302  _principalL...s.
-000044d0: 0000 0000 0f7a 2e50 726f 6365 7373 5574  .....z.ProcessUt
-000044e0: 696c 732e 6669 6e64 5f65 6e74 6974 795f  ils.find_entity_
-000044f0: 7072 6f70 6572 7479 5f61 735f 7072 696e  property_as_prin
-00004500: 6369 7061 6c63 0200 0000 0000 0000 0000  cipalc..........
-00004510: 0000 0200 0000 0300 0000 4300 0000 730e  ..........C...s.
-00004520: 0000 0074 0074 017c 0083 017c 0183 0253  ...t.t.|...|...S
-00004530: 0029 0161 7a01 0000 0a20 2020 2020 2020  .).az....       
-00004540: 2047 6574 2061 206a 736f 6e20 7072 6f70   Get a json prop
-00004550: 6572 7479 2061 7320 226c 6973 7422 2066  erty as "list" f
-00004560: 6f6c 6c6f 7769 6e67 2074 6865 2022 7072  ollowing the "pr
-00004570: 6f70 6572 7479 5061 7468 2220 7061 7373  opertyPath" pass
-00004580: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
-00004590: 756d 656e 7473 3a0a 2020 2020 2020 2020  uments:.        
-000045a0: 2020 2020 7072 6f63 6573 733a 2054 6865      process: The
-000045b0: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
-000045c0: 2020 2020 2020 7072 6f70 6572 7479 5f70        property_p
-000045d0: 6174 683a 2050 726f 7065 7274 7920 7061  ath: Property pa
-000045e0: 7468 2074 6f20 6669 6e64 2e20 6965 3a20  th to find. ie: 
-000045f0: 2275 7365 722e 6e61 6d65 2220 6f72 2022  "user.name" or "
-00004600: 7573 6572 732e 302e 6e61 6d65 220a 0a20  users.0.name".. 
-00004610: 2020 2020 2020 2052 6574 7572 6e3a 0a20         Return:. 
-00004620: 2020 2020 2020 2020 2020 2074 6865 2070             the p
-00004630: 726f 7065 7274 7920 7661 6c75 6520 6966  roperty value if
-00004640: 2065 7869 7374 732e 0a0a 2020 2020 2020   exists...      
-00004650: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-00004660: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-00004670: 3a20 4966 2070 726f 7065 7274 7920 7661  : If property va
-00004680: 6c75 6520 646f 6573 6e27 7420 6578 6973  lue doesn't exis
-00004690: 7420 6f72 2068 6173 2069 6e63 6f72 7265  t or has incorre
-000046a0: 6374 2066 6f72 6d61 740a 2020 2020 2020  ct format.      
-000046b0: 2020 2902 7235 0000 0072 4700 0000 7248    ).r5...rG...rH
-000046c0: 0000 0072 3e00 0000 723e 0000 0072 3f00  ...r>...r>...r?.
-000046d0: 0000 da1b 6765 745f 656e 7469 7479 5f70  ....get_entity_p
-000046e0: 726f 7065 7274 795f 6173 5f6c 6973 745d  roperty_as_list]
-000046f0: 0200 0073 0200 0000 000f 7a28 5072 6f63  ...s......z(Proc
-00004700: 6573 7355 7469 6c73 2e67 6574 5f65 6e74  essUtils.get_ent
-00004710: 6974 795f 7072 6f70 6572 7479 5f61 735f  ity_property_as_
-00004720: 6c69 7374 6302 0000 0000 0000 0000 0000  listc...........
-00004730: 0002 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
-00004740: 0000 7400 7401 7c00 8301 7c01 8302 5300  ..t.t.|...|...S.
-00004750: 2901 6171 0100 000a 2020 2020 2020 2020  ).aq....        
-00004760: 5472 7920 746f 2066 696e 6420 6120 6a73  Try to find a js
-00004770: 6f6e 2070 726f 7065 7274 7920 6173 2022  on property as "
-00004780: 6c69 7374 2220 666f 6c6c 6f77 696e 6720  list" following 
-00004790: 7468 6520 2270 726f 7065 7274 7950 6174  the "propertyPat
-000047a0: 6822 2070 6173 7365 642e 0a0a 2020 2020  h" passed...    
-000047b0: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
-000047c0: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-000047d0: 7373 3a20 5468 6520 7072 6f63 6573 732e  ss: The process.
-000047e0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-000047f0: 7065 7274 795f 7061 7468 3a20 5072 6f70  perty_path: Prop
-00004800: 6572 7479 2070 6174 6820 746f 2066 696e  erty path to fin
-00004810: 642e 2069 653a 2022 7573 6572 2e6e 616d  d. ie: "user.nam
-00004820: 6522 206f 7220 2275 7365 7273 2e30 2e6e  e" or "users.0.n
-00004830: 616d 6522 0a0a 2020 2020 2020 2020 5265  ame"..        Re
-00004840: 7475 726e 3a0a 2020 2020 2020 2020 2020  turn:.          
-00004850: 2020 5468 6520 7072 6f70 6572 7479 2076    The property v
-00004860: 616c 7565 2069 6620 6578 6973 7473 2e0a  alue if exists..
-00004870: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-00004880: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00004890: 7565 4572 726f 723a 2049 6620 7072 6f70  ueError: If prop
-000048a0: 6572 7479 2076 616c 7565 2068 6173 2069  erty value has i
-000048b0: 6e63 6f72 7265 6374 2066 6f72 6d61 740a  ncorrect format.
-000048c0: 2020 2020 2020 2020 2902 722c 0000 0072          ).r,...r
-000048d0: 4700 0000 7248 0000 0072 3e00 0000 723e  G...rH...r>...r>
-000048e0: 0000 0072 3f00 0000 da1c 6669 6e64 5f65  ...r?.....find_e
-000048f0: 6e74 6974 795f 7072 6f70 6572 7479 5f61  ntity_property_a
-00004900: 735f 6c69 7374 6e02 0000 7302 0000 0000  s_listn...s.....
-00004910: 0f7a 2950 726f 6365 7373 5574 696c 732e  .z)ProcessUtils.
-00004920: 6669 6e64 5f65 6e74 6974 795f 7072 6f70  find_entity_prop
-00004930: 6572 7479 5f61 735f 6c69 7374 6302 0000  erty_as_listc...
-00004940: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00004950: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
-00004960: 8301 7c01 8302 5300 2901 617a 0100 000a  ..|...S.).az....
-00004970: 2020 2020 2020 2020 4765 7420 6120 6a73          Get a js
-00004980: 6f6e 2070 726f 7065 7274 7920 6173 2022  on property as "
-00004990: 6469 6374 2220 666f 6c6c 6f77 696e 6720  dict" following 
-000049a0: 7468 6520 2270 726f 7065 7274 7950 6174  the "propertyPat
-000049b0: 6822 2070 6173 7365 642e 0a0a 2020 2020  h" passed...    
-000049c0: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
-000049d0: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-000049e0: 7373 3a20 5468 6520 7072 6f63 6573 732e  ss: The process.
-000049f0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00004a00: 7065 7274 795f 7061 7468 3a20 5072 6f70  perty_path: Prop
-00004a10: 6572 7479 2070 6174 6820 746f 2066 696e  erty path to fin
-00004a20: 642e 2069 653a 2022 7573 6572 2e6e 616d  d. ie: "user.nam
-00004a30: 6522 206f 7220 2275 7365 7273 2e30 2e6e  e" or "users.0.n
-00004a40: 616d 6522 0a0a 2020 2020 2020 2020 5265  ame"..        Re
-00004a50: 7475 726e 3a0a 2020 2020 2020 2020 2020  turn:.          
-00004a60: 2020 7468 6520 7072 6f70 6572 7479 2076    the property v
-00004a70: 616c 7565 2069 6620 6578 6973 7473 2e0a  alue if exists..
-00004a80: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-00004a90: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00004aa0: 7565 4572 726f 723a 2049 6620 7072 6f70  ueError: If prop
-00004ab0: 6572 7479 2076 616c 7565 2064 6f65 736e  erty value doesn
-00004ac0: 2774 2065 7869 7374 206f 7220 6861 7320  't exist or has 
-00004ad0: 696e 636f 7272 6563 7420 666f 726d 6174  incorrect format
-00004ae0: 0a20 2020 2020 2020 2029 0272 3000 0000  .        ).r0...
-00004af0: 7247 0000 0072 4800 0000 723e 0000 0072  rG...rH...r>...r
-00004b00: 3e00 0000 723f 0000 00da 1b67 6574 5f65  >...r?.....get_e
-00004b10: 6e74 6974 795f 7072 6f70 6572 7479 5f61  ntity_property_a
-00004b20: 735f 6469 6374 7f02 0000 7302 0000 0000  s_dict....s.....
-00004b30: 0f7a 2850 726f 6365 7373 5574 696c 732e  .z(ProcessUtils.
-00004b40: 6765 745f 656e 7469 7479 5f70 726f 7065  get_entity_prope
-00004b50: 7274 795f 6173 5f64 6963 7463 0200 0000  rty_as_dictc....
-00004b60: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00004b70: 4300 0000 730e 0000 0074 0074 017c 0083  C...s....t.t.|..
-00004b80: 017c 0183 0253 0029 0161 7101 0000 0a20  .|...S.).aq.... 
-00004b90: 2020 2020 2020 2054 7279 2074 6f20 6669         Try to fi
-00004ba0: 6e64 2061 206a 736f 6e20 7072 6f70 6572  nd a json proper
-00004bb0: 7479 2061 7320 2264 6963 7422 2066 6f6c  ty as "dict" fol
-00004bc0: 6c6f 7769 6e67 2074 6865 2022 7072 6f70  lowing the "prop
-00004bd0: 6572 7479 5061 7468 2220 7061 7373 6564  ertyPath" passed
-00004be0: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
-00004bf0: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
-00004c00: 2020 7072 6f63 6573 733a 2054 6865 2070    process: The p
-00004c10: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
-00004c20: 2020 2020 7072 6f70 6572 7479 5f70 6174      property_pat
-00004c30: 683a 2050 726f 7065 7274 7920 7061 7468  h: Property path
-00004c40: 2074 6f20 6669 6e64 2e20 6965 3a20 2275   to find. ie: "u
-00004c50: 7365 722e 6e61 6d65 2220 6f72 2022 7573  ser.name" or "us
-00004c60: 6572 732e 302e 6e61 6d65 220a 0a20 2020  ers.0.name"..   
-00004c70: 2020 2020 2052 6574 7572 6e3a 0a20 2020       Return:.   
-00004c80: 2020 2020 2020 2020 2054 6865 2070 726f           The pro
-00004c90: 7065 7274 7920 7661 6c75 6520 6966 2065  perty value if e
-00004ca0: 7869 7374 732e 0a0a 2020 2020 2020 2020  xists...        
-00004cb0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00004cc0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00004cd0: 4966 2070 726f 7065 7274 7920 7661 6c75  If property valu
-00004ce0: 6520 6861 7320 696e 636f 7272 6563 7420  e has incorrect 
-00004cf0: 666f 726d 6174 0a20 2020 2020 2020 2029  format.        )
-00004d00: 0272 2700 0000 7247 0000 0072 4800 0000  .r'...rG...rH...
-00004d10: 723e 0000 0072 3e00 0000 723f 0000 00da  r>...r>...r?....
-00004d20: 1c66 696e 645f 656e 7469 7479 5f70 726f  .find_entity_pro
-00004d30: 7065 7274 795f 6173 5f64 6963 7490 0200  perty_as_dict...
-00004d40: 0073 0200 0000 000f 7a29 5072 6f63 6573  .s......z)Proces
-00004d50: 7355 7469 6c73 2e66 696e 645f 656e 7469  sUtils.find_enti
-00004d60: 7479 5f70 726f 7065 7274 795f 6173 5f64  ty_property_as_d
-00004d70: 6963 7429 0472 3900 0000 7246 0000 00da  ict).r9...rF....
-00004d80: 0576 616c 7565 723b 0000 0063 0300 0000  .valuer;...c....
-00004d90: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00004da0: 4300 0000 7314 0000 0074 0074 017c 0083  C...s....t.t.|..
-00004db0: 017c 017c 0283 0301 0064 0153 0029 0261  .|.|.....d.S.).a
-00004dc0: 6201 0000 0a20 2020 2020 2020 2055 7064  b....        Upd
-00004dd0: 6174 6520 6120 6a73 6f6e 2066 6f72 6d73  ate a json forms
-00004de0: 2064 6174 6120 7072 6f70 6572 7479 2069   data property i
-00004df0: 6e20 7468 6520 7461 736b 2070 6173 7365  n the task passe
-00004e00: 6420 666f 6c6c 6f77 696e 6720 7468 6520  d following the 
-00004e10: 2270 726f 7065 7274 795f 7061 7468 222e  "property_path".
-00004e20: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
-00004e30: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
-00004e40: 2070 726f 6365 7373 3a20 5468 6520 7072   process: The pr
-00004e50: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
-00004e60: 2020 2070 726f 7065 7274 795f 7061 7468     property_path
-00004e70: 3a20 5072 6f70 6572 7479 2070 6174 6820  : Property path 
-00004e80: 746f 2066 696e 642e 2069 653a 2022 7573  to find. ie: "us
-00004e90: 6572 2e6e 616d 6522 206f 7220 2275 7365  er.name" or "use
-00004ea0: 7273 2e30 2e6e 616d 6522 0a20 2020 2020  rs.0.name".     
-00004eb0: 2020 2020 2020 2076 616c 7565 3a20 5661         value: Va
-00004ec0: 6c75 6520 746f 2075 7064 6174 650a 0a20  lue to update.. 
-00004ed0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00004ee0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00004ef0: 4572 726f 723a 2049 6620 7072 6f70 6572  Error: If proper
-00004f00: 7479 2076 616c 7565 2068 6173 2069 6e63  ty value has inc
-00004f10: 6f72 7265 6374 2066 6f72 6d61 740a 2020  orrect format.  
-00004f20: 2020 2020 2020 4e29 0272 3700 0000 7247        N).r7...rG
-00004f30: 0000 0029 0372 3900 0000 7246 0000 0072  ...).r9...rF...r
-00004f40: 5b00 0000 723e 0000 0072 3e00 0000 723f  [...r>...r>...r?
-00004f50: 0000 00da 1675 7064 6174 655f 656e 7469  .....update_enti
-00004f60: 7479 5f70 726f 7065 7274 79a1 0200 0073  ty_property....s
-00004f70: 0200 0000 000d 7a23 5072 6f63 6573 7355  ......z#ProcessU
-00004f80: 7469 6c73 2e75 7064 6174 655f 656e 7469  tils.update_enti
-00004f90: 7479 5f70 726f 7065 7274 7929 014e 2901  ty_property).N).
-00004fa0: 4e29 014e 2901 4e29 37da 085f 5f6e 616d  N).N).N)7..__nam
-00004fb0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00004fc0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c73  .__qualname__..s
-00004fd0: 7461 7469 636d 6574 686f 6472 0d00 0000  taticmethodr....
-00004fe0: da03 7374 72da 0462 6f6f 6c72 1d00 0000  ..str..boolr....
-00004ff0: da03 696e 7472 1e00 0000 7207 0000 0072  ..intr....r....r
-00005000: 2100 0000 7222 0000 0072 0f00 0000 721f  !...r"...r....r.
-00005010: 0000 0072 0600 0000 7220 0000 0072 1200  ...r....r ...r..
-00005020: 0000 7213 0000 0072 1b00 0000 7216 0000  ..r....r....r...
-00005030: 0072 1c00 0000 da05 666c 6f61 7472 1900  .r......floatr..
-00005040: 0000 7215 0000 0072 1a00 0000 7202 0000  ..r....r....r...
-00005050: 0072 1700 0000 7214 0000 0072 1800 0000  .r....r....r....
-00005060: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
-00005070: 4c00 0000 724d 0000 0072 4e00 0000 724f  L...rM...rN...rO
-00005080: 0000 0072 5000 0000 7203 0000 0072 5100  ...rP...r....rQ.
-00005090: 0000 7252 0000 0072 0a00 0000 7253 0000  ..rR...r....rS..
-000050a0: 0072 5400 0000 720b 0000 0072 5500 0000  .rT...r....rU...
-000050b0: 7256 0000 00da 046c 6973 7472 5700 0000  rV.....listrW...
-000050c0: 7258 0000 00da 0464 6963 7472 5900 0000  rX.....dictrY...
-000050d0: 725a 0000 0072 2400 0000 725c 0000 0072  rZ...r$...r\...r
-000050e0: 3e00 0000 723e 0000 0072 3e00 0000 723f  >...r>...r>...r?
-000050f0: 0000 0072 3800 0000 4d00 0000 73d2 0000  ...r8...M...s...
-00005100: 0008 0102 0114 0d02 0202 0102 0102 0102  ................
-00005110: fc0e 1202 011a 1002 0202 0102 0106 0102  ................
-00005120: 0102 fb0e 1602 0400 fd02 0102 0102 0106  ................
-00005130: 0102 fc0e 1402 0400 fd02 0102 0102 010a  ................
-00005140: 0102 fc0e 1702 0400 fd02 0102 0102 0106  ................
-00005150: 0102 fc0e 1402 0400 fd02 0102 0102 010a  ................
-00005160: 0102 fc0e 1702 0114 0d02 0118 0d02 0118  ................
-00005170: 0d02 0114 0d02 0114 0d02 0118 0d02 0114  ................
-00005180: 0d02 0118 0d02 0118 0d02 0114 1002 0118  ................
-00005190: 1002 0114 1002 0118 1002 0114 1002 0118  ................
-000051a0: 1002 0114 1002 0118 1002 0114 1002 0118  ................
-000051b0: 1002 0114 1002 0118 1002 0114 1002 0118  ................
-000051c0: 1002 0114 1002 0118 1002 0114 1002 0118  ................
-000051d0: 1002 0172 3800 0000 6300 0000 0000 0000  ...r8...c.......
-000051e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000051f0: 0073 4000 0000 6500 5a01 6400 5a02 6503  .s@...e.Z.d.Z.e.
-00005200: 6504 6401 9c02 6402 6403 8404 5a05 6506  e.d...d.d...Z.e.
-00005210: 6507 1900 6404 9c01 6405 6406 8404 5a08  e...d...d.d...Z.
-00005220: 6506 6509 1900 6407 9c01 6408 6409 8404  e.e...d...d.d...
-00005230: 5a0a 640a 5300 290b 723c 0000 0072 3d00  Z.d.S.).r<...r=.
-00005240: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00005250: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
-00005260: 7c01 7c00 5f00 7c02 7c00 5f01 6400 5300  |.|._.|.|._.d.S.
-00005270: a901 4e72 3d00 0000 2903 da04 7365 6c66  ..Nr=...)...self
-00005280: 7239 0000 0072 3a00 0000 723e 0000 0072  r9...r:...r>...r
-00005290: 3e00 0000 723f 0000 00da 085f 5f69 6e69  >...r?.....__ini
-000052a0: 745f 5fb2 0200 0073 0400 0000 0001 0601  t__....s........
-000052b0: 7a24 4375 7272 656e 7445 6c65 6d65 6e74  z$CurrentElement
-000052c0: 5661 6c75 6541 6363 6573 736f 722e 5f5f  ValueAccessor.__
-000052d0: 696e 6974 5f5f 2901 7244 0000 0063 0200  init__).rD...c..
-000052e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000052f0: 0000 4300 0000 7346 0000 007c 006a 006a  ..C...sF...|.j.j
-00005300: 0164 006b 0872 1469 007c 006a 005f 0174  .d.k.r.i.|.j._.t
-00005310: 027c 0183 0164 016b 0272 347c 006a 006a  .|...d.k.r4|.j.j
-00005320: 01a0 037c 006a 0464 00a1 0201 006e 0e7c  ...|.j.d.....n.|
-00005330: 017c 006a 006a 017c 006a 043c 0064 0053  .|.j.j.|.j.<.d.S
-00005340: 00a9 024e 7201 0000 0029 0572 3900 0000  ...Nr....).r9...
-00005350: 7244 0000 00da 036c 656e da03 706f 7072  rD.....len..popr
-00005360: 3a00 0000 2902 7268 0000 0072 4400 0000  :...).rh...rD...
-00005370: 723e 0000 0072 3e00 0000 723f 0000 00da  r>...r>...r?....
-00005380: 1273 6574 5f65 6c65 6d65 6e74 5f76 616c  .set_element_val
-00005390: 7565 73b6 0200 0073 0a00 0000 0001 0c01  ues....s........
-000053a0: 0802 0c01 1402 7a2e 4375 7272 656e 7445  ......z.CurrentE
-000053b0: 6c65 6d65 6e74 5661 6c75 6541 6363 6573  lementValueAcces
-000053c0: 736f 722e 7365 745f 656c 656d 656e 745f  sor.set_element_
-000053d0: 7661 6c75 6573 a901 723b 0000 0063 0100  values..r;...c..
-000053e0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000053f0: 0000 4300 0000 733c 0000 007c 006a 006a  ..C...s<...|.j.j
-00005400: 0164 006b 0872 1067 0053 007c 006a 006a  .d.k.r.g.S.|.j.j
-00005410: 01a0 027c 006a 03a1 017d 017c 0164 006b  ...|.j...}.|.d.k
-00005420: 0873 3474 047c 0183 0164 016b 0272 3867  .s4t.|...d.k.r8g
-00005430: 0053 007c 0153 0072 6a00 0000 2905 7239  .S.|.S.rj...).r9
-00005440: 0000 0072 4400 0000 da03 6765 7472 3a00  ...rD.....getr:.
-00005450: 0000 726b 0000 0029 0272 6800 0000 da16  ..rk...).rh.....
-00005460: 656c 656d 656e 745f 7661 6c75 6573 5f62  element_values_b
-00005470: 795f 636f 6465 723e 0000 0072 3e00 0000  y_coder>...r>...
-00005480: 723f 0000 00da 1267 6574 5f65 6c65 6d65  r?.....get_eleme
-00005490: 6e74 5f76 616c 7565 73bf 0200 0073 0c00  nt_values....s..
-000054a0: 0000 0001 0c01 0402 1001 1401 0402 7a2e  ..............z.
-000054b0: 4375 7272 656e 7445 6c65 6d65 6e74 5661  CurrentElementVa
-000054c0: 6c75 6541 6363 6573 736f 722e 6765 745f  lueAccessor.get_
-000054d0: 656c 656d 656e 745f 7661 6c75 6573 4e29  element_valuesN)
-000054e0: 0b72 5d00 0000 725e 0000 0072 5f00 0000  .r]...r^...r_...
-000054f0: 720d 0000 0072 6100 0000 7269 0000 0072  r....ra...ri...r
-00005500: 0600 0000 7210 0000 0072 6d00 0000 7209  ....r....rm...r.
-00005510: 0000 0072 7100 0000 723e 0000 0072 3e00  ...rq...r>...r>.
-00005520: 0000 723e 0000 0072 3f00 0000 723c 0000  ..r>...r?...r<..
-00005530: 00b1 0200 0073 0600 0000 0801 1004 1209  .....s..........
-00005540: 723c 0000 0063 0000 0000 0000 0000 0000  r<...c..........
-00005550: 0000 0000 0000 0400 0000 4000 0000 734e  ..........@...sN
-00005560: 0000 0065 005a 0164 005a 0265 0364 019c  ...e.Z.d.Z.e.d..
-00005570: 0164 0264 0384 045a 0465 0565 0665 0765  .d.d...Z.e.e.e.e
-00005580: 0866 0219 0019 0064 049c 0164 0564 0684  .f.....d...d.d..
-00005590: 045a 0965 0565 0665 0765 0866 0219 0019  .Z.e.e.e.e.f....
-000055a0: 0064 079c 0164 0864 0984 045a 0a64 0a53  .d...d.d...Z.d.S
-000055b0: 0029 0b72 4700 0000 a901 7239 0000 0063  .).rG.....r9...c
-000055c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000055d0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-000055e0: 005f 0064 0053 0072 6700 0000 7272 0000  ._.d.S.rg...rr..
-000055f0: 0029 0272 6800 0000 7239 0000 0072 3e00  .).rh...r9...r>.
-00005600: 0000 723e 0000 0072 3f00 0000 7269 0000  ..r>...r?...ri..
-00005610: 00cb 0200 0073 0200 0000 0001 7a24 4375  .....s......z$Cu
-00005620: 7272 656e 744a 736f 6e46 6f72 6d44 6174  rrentJsonFormDat
-00005630: 6141 6363 6573 736f 722e 5f5f 696e 6974  aAccessor.__init
-00005640: 5f5f 726e 0000 0063 0100 0000 0000 0000  __rn...c........
-00005650: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00005660: 731a 0000 007c 006a 006a 0164 006b 0872  s....|.j.j.d.k.r
-00005670: 1064 0053 007c 006a 006a 016a 0253 0072  .d.S.|.j.j.j.S.r
-00005680: 6700 0000 2903 7239 0000 00da 0665 6e74  g...).r9.....ent
-00005690: 6974 79da 0464 6174 6129 0172 6800 0000  ity..data).rh...
-000056a0: 723e 0000 0072 3e00 0000 723f 0000 00da  r>...r>...r?....
-000056b0: 0867 6574 5f64 6174 61ce 0200 0073 0600  .get_data....s..
-000056c0: 0000 0001 0c01 0402 7a24 4375 7272 656e  ........z$Curren
-000056d0: 744a 736f 6e46 6f72 6d44 6174 6141 6363  tJsonFormDataAcc
-000056e0: 6573 736f 722e 6765 745f 6461 7461 2901  essor.get_data).
-000056f0: 7274 0000 0063 0200 0000 0000 0000 0000  rt...c..........
-00005700: 0000 0200 0000 0200 0000 4300 0000 7324  ..........C...s$
-00005710: 0000 007c 006a 006a 0164 006b 0872 1674  ...|.j.j.d.k.r.t
-00005720: 0283 007c 006a 005f 017c 017c 006a 006a  ...|.j._.|.|.j.j
-00005730: 015f 0364 0053 0072 6700 0000 2904 7239  ._.d.S.rg...).r9
-00005740: 0000 0072 7300 0000 720c 0000 0072 7400  ...rs...r....rt.
-00005750: 0000 2902 7268 0000 0072 7400 0000 723e  ..).rh...rt...r>
-00005760: 0000 0072 3e00 0000 723f 0000 00da 0873  ...r>...r?.....s
-00005770: 6574 5f64 6174 61d4 0200 0073 0600 0000  et_data....s....
-00005780: 0001 0c01 0a02 7a24 4375 7272 656e 744a  ......z$CurrentJ
-00005790: 736f 6e46 6f72 6d44 6174 6141 6363 6573  sonFormDataAcces
-000057a0: 736f 722e 7365 745f 6461 7461 4e29 0b72  sor.set_dataN).r
-000057b0: 5d00 0000 725e 0000 0072 5f00 0000 720d  ]...r^...r_...r.
-000057c0: 0000 0072 6900 0000 7207 0000 0072 0500  ...ri...r....r..
-000057d0: 0000 7261 0000 0072 0400 0000 7275 0000  ..ra...r....ru..
-000057e0: 0072 7600 0000 723e 0000 0072 3e00 0000  .rv...r>...r>...
-000057f0: 723e 0000 0072 3f00 0000 7247 0000 00ca  r>...r?...rG....
-00005800: 0200 0073 0600 0000 0801 0e03 1a06 7247  ...s..........rG
-00005810: 0000 004e 293c 7203 0000 0072 0200 0000  ...N)<r....r....
-00005820: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
-00005830: 0000 7206 0000 0072 0700 0000 5a11 5f67  ..r....r....Z._g
-00005840: 656e 6572 6174 6564 2e6d 6f64 656c 7372  enerated.modelsr
-00005850: 0900 0000 da06 6d6f 6465 6c73 720a 0000  ......modelsr...
-00005860: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00005870: 7244 0000 0072 0f00 0000 7210 0000 0072  rD...r....r....r
-00005880: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00005890: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-000058a0: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000058b0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-000058c0: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-000058d0: 2100 0000 7222 0000 005a 0a6a 736f 6e5f  !...r"...Z.json_
-000058e0: 666f 726d 7372 2300 0000 7224 0000 0072  formsr#...r$...r
-000058f0: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
-00005900: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00005910: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00005920: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
-00005930: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
-00005940: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
-00005950: 0000 0072 3c00 0000 7247 0000 0072 3e00  ...r<...rG...r>.
-00005960: 0000 723e 0000 0072 3e00 0000 723f 0000  ..r>...r>...r?..
-00005970: 00da 083c 6d6f 6475 6c65 3e19 0000 0073  ...<module>....s
-00005980: 1800 0000 1001 1802 0c01 1801 5816 5c19  ............X.\.
-00005990: 0e7f 007f 007f 007f 0068 1019            .........h..
+00000120: 6d36 5a36 0100 4700 6409 640a 8400 640a  m6Z6..G.d.d...d.
+00000130: 8302 5a37 4700 640b 640c 8400 640c 6511  ..Z7G.d.d...d.e.
+00000140: 8303 5a38 4700 640d 640e 8400 640e 6524  ..Z8G.d.d...d.e$
+00000150: 8303 5a39 640f 5300 2910 e900 0000 0029  ..Z9d.S.)......)
+00000160: 02da 0464 6174 65da 0864 6174 6574 696d  ...date..datetim
+00000170: 6529 04da 0341 6e79 da04 4469 6374 da04  e)...Any..Dict..
+00000180: 4c69 7374 da08 4f70 7469 6f6e 616c e902  List..Optional..
+00000190: 0000 0029 01da 1350 726f 6365 7373 456c  ...)...ProcessEl
+000001a0: 656d 656e 7456 616c 7565 2904 da0d 4a73  ementValue)...Js
+000001b0: 6f6e 466f 726d 7346 696c 65da 124a 736f  onFormsFile..Jso
+000001c0: 6e46 6f72 6d73 5072 696e 6369 7061 6cda  nFormsPrincipal.
+000001d0: 0e4a 736f 6e46 6f72 6d73 5661 6c75 65da  .JsonFormsValue.
+000001e0: 0750 726f 6365 7373 e901 0000 0029 14da  .Process.....)..
+000001f0: 1645 6c65 6d65 6e74 5661 6c75 6553 696d  .ElementValueSim
+00000200: 706c 6554 7970 65da 1145 6c65 6d65 6e74  pleType..Element
+00000210: 5661 6c75 6555 6e69 6f6e da1b 5072 6f63  ValueUnion..Proc
+00000220: 6573 7345 6c65 6d65 6e74 5661 6c75 6541  essElementValueA
+00000230: 6363 6573 736f 72da 1161 6464 5f65 6c65  ccessor..add_ele
+00000240: 6d65 6e74 5f76 616c 7565 da16 6164 645f  ment_value..add_
+00000250: 656c 656d 656e 745f 7661 6c75 655f 6c69  element_value_li
+00000260: 7374 da1a 6669 6e64 5f65 6c65 6d65 6e74  st..find_element
+00000270: 5f76 616c 7565 5f61 735f 6461 7465 da1b  _value_as_date..
+00000280: 6669 6e64 5f65 6c65 6d65 6e74 5f76 616c  find_element_val
+00000290: 7565 5f61 735f 666c 6f61 74da 1966 696e  ue_as_float..fin
+000002a0: 645f 656c 656d 656e 745f 7661 6c75 655f  d_element_value_
+000002b0: 6173 5f73 7472 da19 6765 745f 656c 656d  as_str..get_elem
+000002c0: 656e 745f 7661 6c75 655f 6173 5f64 6174  ent_value_as_dat
+000002d0: 65da 1e67 6574 5f65 6c65 6d65 6e74 5f76  e..get_element_v
+000002e0: 616c 7565 5f61 735f 6461 7465 5f6c 6973  alue_as_date_lis
+000002f0: 74da 1a67 6574 5f65 6c65 6d65 6e74 5f76  t..get_element_v
+00000300: 616c 7565 5f61 735f 666c 6f61 74da 1f67  alue_as_float..g
+00000310: 6574 5f65 6c65 6d65 6e74 5f76 616c 7565  et_element_value
+00000320: 5f61 735f 666c 6f61 745f 6c69 7374 da18  _as_float_list..
+00000330: 6765 745f 656c 656d 656e 745f 7661 6c75  get_element_valu
+00000340: 655f 6173 5f73 7472 da1d 6765 745f 656c  e_as_str..get_el
+00000350: 656d 656e 745f 7661 6c75 655f 6173 5f73  ement_value_as_s
+00000360: 7472 5f6c 6973 74da 1767 6574 5f65 6c65  tr_list..get_ele
+00000370: 6d65 6e74 5f76 616c 7565 5f76 616c 6964  ment_value_valid
+00000380: da1a 6765 745f 656c 656d 656e 745f 7661  ..get_element_va
+00000390: 6c75 655f 7661 6c69 645f 6174 da11 7365  lue_valid_at..se
+000003a0: 745f 656c 656d 656e 745f 7661 6c75 65da  t_element_value.
+000003b0: 1673 6574 5f65 6c65 6d65 6e74 5f76 616c  .set_element_val
+000003c0: 7565 5f6c 6973 74da 1773 6574 5f65 6c65  ue_list..set_ele
+000003d0: 6d65 6e74 5f76 616c 7565 5f76 616c 6964  ment_value_valid
+000003e0: da1a 7365 745f 656c 656d 656e 745f 7661  ..set_element_va
+000003f0: 6c75 655f 7661 6c69 645f 6174 2913 da14  lue_valid_at)...
+00000400: 4a73 6f6e 466f 726d 4461 7461 4163 6365  JsonFormDataAcce
+00000410: 7373 6f72 da20 6669 6e64 5f6a 736f 6e5f  ssor. find_json_
+00000420: 666f 726d 735f 7072 6f70 6572 7479 5f61  forms_property_a
+00000430: 735f 6461 7465 da24 6669 6e64 5f6a 736f  s_date.$find_jso
+00000440: 6e5f 666f 726d 735f 7072 6f70 6572 7479  n_forms_property
+00000450: 5f61 735f 6461 7465 7469 6d65 da20 6669  _as_datetime. fi
+00000460: 6e64 5f6a 736f 6e5f 666f 726d 735f 7072  nd_json_forms_pr
+00000470: 6f70 6572 7479 5f61 735f 6469 6374 da21  operty_as_dict.!
+00000480: 6669 6e64 5f6a 736f 6e5f 666f 726d 735f  find_json_forms_
+00000490: 7072 6f70 6572 7479 5f61 735f 666c 6f61  property_as_floa
+000004a0: 74da 1f66 696e 645f 6a73 6f6e 5f66 6f72  t..find_json_for
+000004b0: 6d73 5f70 726f 7065 7274 795f 6173 5f69  ms_property_as_i
+000004c0: 6e74 da2b 6669 6e64 5f6a 736f 6e5f 666f  nt.+find_json_fo
+000004d0: 726d 735f 7072 6f70 6572 7479 5f61 735f  rms_property_as_
+000004e0: 6a73 6f6e 5f66 6f72 6d73 5f66 696c 65da  json_forms_file.
+000004f0: 3066 696e 645f 6a73 6f6e 5f66 6f72 6d73  0find_json_forms
+00000500: 5f70 726f 7065 7274 795f 6173 5f6a 736f  _property_as_jso
+00000510: 6e5f 666f 726d 735f 7072 696e 6369 7061  n_forms_principa
+00000520: 6cda 2066 696e 645f 6a73 6f6e 5f66 6f72  l. find_json_for
+00000530: 6d73 5f70 726f 7065 7274 795f 6173 5f6c  ms_property_as_l
+00000540: 6973 74da 1f66 696e 645f 6a73 6f6e 5f66  ist..find_json_f
+00000550: 6f72 6d73 5f70 726f 7065 7274 795f 6173  orms_property_as
+00000560: 5f73 7472 da1f 6765 745f 6a73 6f6e 5f66  _str..get_json_f
+00000570: 6f72 6d73 5f70 726f 7065 7274 795f 6173  orms_property_as
+00000580: 5f64 6174 65da 2367 6574 5f6a 736f 6e5f  _date.#get_json_
+00000590: 666f 726d 735f 7072 6f70 6572 7479 5f61  forms_property_a
+000005a0: 735f 6461 7465 7469 6d65 da1f 6765 745f  s_datetime..get_
+000005b0: 6a73 6f6e 5f66 6f72 6d73 5f70 726f 7065  json_forms_prope
+000005c0: 7274 795f 6173 5f64 6963 74da 2067 6574  rty_as_dict. get
+000005d0: 5f6a 736f 6e5f 666f 726d 735f 7072 6f70  _json_forms_prop
+000005e0: 6572 7479 5f61 735f 666c 6f61 74da 1e67  erty_as_float..g
+000005f0: 6574 5f6a 736f 6e5f 666f 726d 735f 7072  et_json_forms_pr
+00000600: 6f70 6572 7479 5f61 735f 696e 74da 2a67  operty_as_int.*g
+00000610: 6574 5f6a 736f 6e5f 666f 726d 735f 7072  et_json_forms_pr
+00000620: 6f70 6572 7479 5f61 735f 6a73 6f6e 5f66  operty_as_json_f
+00000630: 6f72 6d73 5f66 696c 65da 2f67 6574 5f6a  orms_file./get_j
+00000640: 736f 6e5f 666f 726d 735f 7072 6f70 6572  son_forms_proper
+00000650: 7479 5f61 735f 6a73 6f6e 5f66 6f72 6d73  ty_as_json_forms
+00000660: 5f70 7269 6e63 6970 616c da1f 6765 745f  _principal..get_
+00000670: 6a73 6f6e 5f66 6f72 6d73 5f70 726f 7065  json_forms_prope
+00000680: 7274 795f 6173 5f6c 6973 74da 1e67 6574  rty_as_list..get
+00000690: 5f6a 736f 6e5f 666f 726d 735f 7072 6f70  _json_forms_prop
+000006a0: 6572 7479 5f61 735f 7374 7263 0000 0000  erty_as_strc....
+000006b0: 0000 0000 0000 0000 0000 0000 0700 0000  ................
+000006c0: 4000 0000 737e 0300 0065 005a 0164 005a  @...s~...e.Z.d.Z
+000006d0: 0265 0365 0465 0565 0664 019c 0364 0264  .e.e.e.e.d...d.d
+000006e0: 0384 0483 015a 0765 0365 0465 0565 0865  .....Z.e.e.e.e.e
+000006f0: 0664 049c 0464 0564 0684 0483 015a 0965  .d...d.d.....Z.e
+00000700: 0365 0465 0565 0a65 0619 0065 0464 079c  .e.e.e.e...e.d..
+00000710: 0464 0864 0984 0483 015a 0b65 0365 0465  .d.d.....Z.e.e.e
+00000720: 0565 0a65 0619 0065 0865 0464 0a9c 0564  .e.e...e.e.d...d
+00000730: 0b64 0c84 0483 015a 0c65 0364 4f65 0465  .d.....Z.e.dOe.e
+00000740: 0565 0a65 0d19 0065 0464 0e9c 0464 0f64  .e.e...e.d...d.d
+00000750: 1084 0583 015a 0e65 0364 5065 0465 0565  .....Z.e.dPe.e.e
+00000760: 0a65 0f65 0d19 0019 0065 0464 119c 0464  .e.e.....e.d...d
+00000770: 1264 1384 0583 015a 1065 0364 5165 0465  .d.....Z.e.dQe.e
+00000780: 0565 0a65 0d19 0065 0464 0e9c 0464 1464  .e.e...e.d...d.d
+00000790: 1584 0583 015a 1165 0364 5265 0465 0565  .....Z.e.dRe.e.e
+000007a0: 0a65 0f65 0d19 0019 0065 0464 119c 0464  .e.e.....e.d...d
+000007b0: 1664 1784 0583 015a 1265 0365 0465 0565  .d.....Z.e.e.e.e
+000007c0: 0564 019c 0364 1864 1984 0483 015a 1365  .d...d.d.....Z.e
+000007d0: 0365 0465 0565 0a65 0519 0064 019c 0364  .e.e.e.e...d...d
+000007e0: 1a64 1b84 0483 015a 1465 0365 0465 0565  .d.....Z.e.e.e.e
+000007f0: 0f65 0519 0064 019c 0364 1c64 1d84 0483  .e...d...d.d....
+00000800: 015a 1565 0365 0465 0565 1664 019c 0364  .Z.e.e.e.e.d...d
+00000810: 1e64 1f84 0483 015a 1765 0365 0465 0565  .d.....Z.e.e.e.e
+00000820: 1664 019c 0364 2064 2184 0483 015a 1865  .d...d d!....Z.e
+00000830: 0365 0465 0565 0f65 1619 0064 019c 0364  .e.e.e.e...d...d
+00000840: 2264 2384 0483 015a 1965 0365 0465 0565  "d#....Z.e.e.e.e
+00000850: 1a64 019c 0364 2464 2584 0483 015a 1b65  .d...d$d%....Z.e
+00000860: 0365 0465 0565 0a65 1a19 0064 019c 0364  .e.e.e.e...d...d
+00000870: 2664 2784 0483 015a 1c65 0365 0465 0565  &d'....Z.e.e.e.e
+00000880: 0f65 1a19 0064 019c 0364 2864 2984 0483  .e...d...d(d)...
+00000890: 015a 1d65 0365 0465 0565 0564 2a9c 0364  .Z.e.e.e.e.d*..d
+000008a0: 2b64 2c84 0483 015a 1e65 0365 0465 0565  +d,....Z.e.e.e.e
+000008b0: 0a65 0519 0064 2a9c 0364 2d64 2e84 0483  .e...d*..d-d....
+000008c0: 015a 1f65 0365 0465 0565 0864 2a9c 0364  .Z.e.e.e.e.d*..d
+000008d0: 2f64 3084 0483 015a 2065 0365 0465 0565  /d0....Z e.e.e.e
+000008e0: 0a65 0819 0064 2a9c 0364 3164 3284 0483  .e...d*..d1d2...
+000008f0: 015a 2165 0365 0465 0565 1664 2a9c 0364  .Z!e.e.e.e.d*..d
+00000900: 3364 3484 0483 015a 2265 0365 0465 0565  3d4....Z"e.e.e.e
+00000910: 0a65 1619 0064 2a9c 0364 3564 3684 0483  .e...d*..d5d6...
+00000920: 015a 2365 0365 0465 0565 1a64 2a9c 0364  .Z#e.e.e.e.d*..d
+00000930: 3764 3884 0483 015a 2465 0365 0465 0565  7d8....Z$e.e.e.e
+00000940: 0a65 1a19 0064 2a9c 0364 3964 3a84 0483  .e...d*..d9d:...
+00000950: 015a 2565 0365 0465 0565 2664 2a9c 0364  .Z%e.e.e.e&d*..d
+00000960: 3b64 3c84 0483 015a 2765 0365 0465 0565  ;d<....Z'e.e.e.e
+00000970: 0a65 2619 0064 2a9c 0364 3d64 3e84 0483  .e&..d*..d=d>...
+00000980: 015a 2865 0365 0465 0565 2964 2a9c 0364  .Z(e.e.e.e)d*..d
+00000990: 3f64 4084 0483 015a 2a65 0365 0465 0565  ?d@....Z*e.e.e.e
+000009a0: 0a65 2919 0064 2a9c 0364 4164 4284 0483  .e)..d*..dAdB...
+000009b0: 015a 2b65 0365 0465 0565 2c64 2a9c 0364  .Z+e.e.e.e,d*..d
+000009c0: 4364 4484 0483 015a 2d65 0365 0465 0565  CdD....Z-e.e.e.e
+000009d0: 0a65 2c19 0064 2a9c 0364 4564 4684 0483  .e,..d*..dEdF...
+000009e0: 015a 2e65 0365 0465 0565 2f64 2a9c 0364  .Z.e.e.e.e/d*..d
+000009f0: 4764 4884 0483 015a 3065 0365 0465 0565  GdH....Z0e.e.e.e
+00000a00: 0a65 2f19 0064 2a9c 0364 4964 4a84 0483  .e/..d*..dIdJ...
+00000a10: 015a 3165 0365 0465 0565 3264 2a9c 0364  .Z1e.e.e.e2d*..d
+00000a20: 4b64 4c84 0483 015a 3365 0365 0465 0565  KdL....Z3e.e.e.e
+00000a30: 0a65 3219 0064 2a9c 0364 4d64 4e84 0483  .e2..d*..dMdN...
+00000a40: 015a 3464 0d53 0029 53da 0c50 726f 6365  .Z4d.S.)S..Proce
+00000a50: 7373 5574 696c 7329 03da 0770 726f 6365  ssUtils)...proce
+00000a60: 7373 da17 656c 656d 656e 745f 6465 6669  ss..element_defi
+00000a70: 6e69 7469 6f6e 5f63 6f64 65da 0672 6574  nition_code..ret
+00000a80: 7572 6e63 0200 0000 0000 0000 0000 0000  urnc............
+00000a90: 0200 0000 0400 0000 4300 0000 730e 0000  ........C...s...
+00000aa0: 0074 0074 017c 007c 0183 0283 0153 0029  .t.t.|.|.....S.)
+00000ab0: 0161 0b01 0000 0a20 2020 2020 2020 2043  .a.....        C
+00000ac0: 6865 636b 2069 6620 616c 6c20 7265 6c61  heck if all rela
+00000ad0: 7465 6420 7661 6c69 6420 7661 6c75 6573  ted valid values
+00000ae0: 2061 7265 2054 5255 452e 0a0a 2020 2020   are TRUE...    
+00000af0: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
+00000b00: 2020 2020 2020 2020 2020 2070 726f 6365             proce
+00000b10: 7373 3a20 5468 6520 7072 6f63 6573 732e  ss: The process.
+00000b20: 0a20 2020 2020 2020 2020 2020 2065 6c65  .            ele
+00000b30: 6d65 6e74 5f64 6566 696e 6974 696f 6e5f  ment_definition_
+00000b40: 636f 6465 3a20 456c 656d 656e 7420 4465  code: Element De
+00000b50: 6669 6e69 7469 6f6e 2043 6f64 652e 0a0a  finition Code...
+00000b60: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00000b70: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
+00000b80: 6520 6966 2061 6c6c 2072 656c 6174 6564  e if all related
+00000b90: 2076 616c 6964 2076 616c 7565 7320 6172   valid values ar
+00000ba0: 6520 5452 5545 2c20 6f74 6865 7277 6973  e TRUE, otherwis
+00000bb0: 6520 4661 6c73 652e 0a20 2020 2020 2020  e False..       
+00000bc0: 2029 0272 1d00 0000 da1b 4375 7272 656e   ).r......Curren
+00000bd0: 7445 6c65 6d65 6e74 5661 6c75 6541 6363  tElementValueAcc
+00000be0: 6573 736f 72a9 0272 3700 0000 7238 0000  essor..r7...r8..
+00000bf0: 00a9 0072 3c00 0000 fa47 2f77 6f72 6b2f  ...r<....G/work/
+00000c00: 6b75 666c 6f77 2d73 646b 2d70 7974 686f  kuflow-sdk-pytho
+00000c10: 6e2f 6b75 666c 6f77 2d72 6573 742f 6b75  n/kuflow-rest/ku
+00000c20: 666c 6f77 5f72 6573 742f 7574 696c 732f  flow_rest/utils/
+00000c30: 5f70 726f 6365 7373 5f75 7469 6c73 2e70  _process_utils.p
+00000c40: 7972 1d00 0000 4c00 0000 7302 0000 0000  yr....L...s.....
+00000c50: 0c7a 2450 726f 6365 7373 5574 696c 732e  .z$ProcessUtils.
+00000c60: 6765 745f 656c 656d 656e 745f 7661 6c75  get_element_valu
+00000c70: 655f 7661 6c69 6429 0472 3700 0000 7238  e_valid).r7...r8
+00000c80: 0000 00da 0569 6e64 6578 7239 0000 0063  .....indexr9...c
+00000c90: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000ca0: 0400 0000 4300 0000 7310 0000 0074 0074  ....C...s....t.t
+00000cb0: 017c 007c 0183 027c 0283 0253 0029 0161  .|.|...|...S.).a
+00000cc0: 4a01 0000 0a20 2020 2020 2020 2043 6865  J....        Che
+00000cd0: 636b 2069 6620 7468 6520 7265 7175 6573  ck if the reques
+00000ce0: 7465 6420 7661 6c69 6420 7661 6c75 6520  ted valid value 
+00000cf0: 6174 2074 6865 2067 6976 656e 2069 6e64  at the given ind
+00000d00: 6578 2069 7320 5452 5545 2e0a 0a20 2020  ex is TRUE...   
+00000d10: 2020 2020 2041 7267 756d 656e 7473 3a0a       Arguments:.
+00000d20: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+00000d30: 6573 733a 2054 6865 2070 726f 6365 7373  ess: The process
+00000d40: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00000d50: 656d 656e 745f 6465 6669 6e69 7469 6f6e  ement_definition
+00000d60: 5f63 6f64 653a 2054 6865 2065 6c65 6d65  _code: The eleme
+00000d70: 6e74 2064 6566 696e 6974 696f 6e20 636f  nt definition co
+00000d80: 6465 2e0a 2020 2020 2020 2020 2020 2020  de..            
+00000d90: 696e 6465 783a 2054 6865 2065 6c65 6d65  index: The eleme
+00000da0: 6e74 2076 616c 7565 2069 6e64 6578 2e0a  nt value index..
+00000db0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00000dc0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00000dd0: 6520 7265 7175 6573 7465 6420 7661 6c69  e requested vali
+00000de0: 6420 7661 6c75 6520 6966 2069 7420 6578  d value if it ex
+00000df0: 6973 7473 2c20 6f74 6865 7277 6973 6520  ists, otherwise 
+00000e00: 4e6f 6e65 2e0a 2020 2020 2020 2020 2902  None..        ).
+00000e10: 721e 0000 0072 3a00 0000 2903 7237 0000  r....r:...).r7..
+00000e20: 0072 3800 0000 723e 0000 0072 3c00 0000  .r8...r>...r<...
+00000e30: 723c 0000 0072 3d00 0000 721e 0000 005a  r<...r=...r....Z
+00000e40: 0000 0073 0200 0000 0011 7a27 5072 6f63  ...s......z'Proc
+00000e50: 6573 7355 7469 6c73 2e67 6574 5f65 6c65  essUtils.get_ele
+00000e60: 6d65 6e74 5f76 616c 7565 5f76 616c 6964  ment_value_valid
+00000e70: 5f61 7429 0472 3700 0000 7238 0000 00da  _at).r7...r8....
+00000e80: 0576 616c 6964 7239 0000 0063 0300 0000  .validr9...c....
+00000e90: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000ea0: 4300 0000 7314 0000 0074 0074 017c 007c  C...s....t.t.|.|
+00000eb0: 0183 027c 0283 0201 007c 0053 0029 0161  ...|.....|.S.).a
+00000ec0: 0b01 0000 0a20 2020 2020 2020 2053 6574  .....        Set
+00000ed0: 2074 6865 2076 616c 6964 2076 616c 7565   the valid value
+00000ee0: 2066 6f72 2061 6c6c 2065 6c65 6d65 6e74   for all element
+00000ef0: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00000f00: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+00000f10: 2020 2020 2020 2020 2070 726f 6365 7373           process
+00000f20: 3a20 5468 6520 7072 6f63 6573 732e 0a20  : The process.. 
+00000f30: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
+00000f40: 6e74 5f64 6566 696e 6974 696f 6e5f 636f  nt_definition_co
+00000f50: 6465 3a20 5468 6520 656c 656d 656e 7420  de: The element 
+00000f60: 6465 6669 6e69 7469 6f6e 2063 6f64 652e  definition code.
+00000f70: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00000f80: 6964 3a20 5468 6520 7661 6c69 6420 7661  id: The valid va
+00000f90: 6c75 652e 0a0a 2020 2020 2020 2020 5265  lue...        Re
+00000fa0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00000fb0: 2020 2054 6865 2070 6173 7365 6420 7072     The passed pr
+00000fc0: 6f63 6573 732e 0a20 2020 2020 2020 2029  ocess..        )
+00000fd0: 0272 2100 0000 723a 0000 0029 0372 3700  .r!...r:...).r7.
+00000fe0: 0000 7238 0000 0072 3f00 0000 723c 0000  ..r8...r?...r<..
+00000ff0: 0072 3c00 0000 723d 0000 0072 2100 0000  .r<...r=...r!...
+00001000: 6d00 0000 7304 0000 0000 0d10 027a 2450  m...s........z$P
+00001010: 726f 6365 7373 5574 696c 732e 7365 745f  rocessUtils.set_
+00001020: 656c 656d 656e 745f 7661 6c75 655f 7661  element_value_va
+00001030: 6c69 6429 0572 3700 0000 7238 0000 0072  lid).r7...r8...r
+00001040: 3f00 0000 723e 0000 0072 3900 0000 6304  ?...r>...r9...c.
+00001050: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00001060: 0000 0043 0000 0073 1600 0000 7400 7401  ...C...s....t.t.
+00001070: 7c00 7c01 8302 7c02 7c03 8303 0100 7c00  |.|...|.|.....|.
+00001080: 5300 2901 613f 0100 000a 2020 2020 2020  S.).a?....      
+00001090: 2020 5365 7420 7468 6520 7661 6c69 6420    Set the valid 
+000010a0: 7661 6c75 6520 666f 7220 7468 6520 7365  value for the se
+000010b0: 6c65 6374 6564 2065 6c65 6d65 6e74 2076  lected element v
+000010c0: 616c 7565 2e0a 0a20 2020 2020 2020 2041  alue...        A
+000010d0: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
+000010e0: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
+000010f0: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
+00001100: 2020 2020 2020 2020 656c 656d 656e 745f          element_
+00001110: 6465 6669 6e69 7469 6f6e 5f63 6f64 653a  definition_code:
+00001120: 2054 6865 2065 6c65 6d65 6e74 2064 6566   The element def
+00001130: 696e 6974 696f 6e20 636f 6465 2e0a 2020  inition code..  
+00001140: 2020 2020 2020 2020 2020 7661 6c69 643a            valid:
+00001150: 2054 6865 2076 616c 6964 2076 616c 7565   The valid value
+00001160: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00001170: 6465 783a 2054 6865 2065 6c65 6d65 6e74  dex: The element
+00001180: 2076 616c 7565 2069 6e64 6578 2e0a 0a20   value index... 
+00001190: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+000011a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000011b0: 7061 7373 6564 2070 726f 6365 7373 2e0a  passed process..
+000011c0: 2020 2020 2020 2020 2902 7222 0000 0072          ).r"...r
+000011d0: 3a00 0000 2904 7237 0000 0072 3800 0000  :...).r7...r8...
+000011e0: 723f 0000 0072 3e00 0000 723c 0000 0072  r?...r>...r<...r
+000011f0: 3c00 0000 723d 0000 0072 2200 0000 7e00  <...r=...r"...~.
+00001200: 0000 7304 0000 0000 1312 027a 2750 726f  ..s........z'Pro
+00001210: 6365 7373 5574 696c 732e 7365 745f 656c  cessUtils.set_el
+00001220: 656d 656e 745f 7661 6c75 655f 7661 6c69  ement_value_vali
+00001230: 645f 6174 4e29 0472 3700 0000 7238 0000  d_atN).r7...r8..
+00001240: 00da 0d65 6c65 6d65 6e74 5f76 616c 7565  ...element_value
+00001250: 7239 0000 0063 0300 0000 0000 0000 0000  r9...c..........
+00001260: 0000 0300 0000 0400 0000 4300 0000 7314  ..........C...s.
+00001270: 0000 0074 0074 017c 007c 0183 027c 0283  ...t.t.|.|...|..
+00001280: 0201 007c 0053 0029 0161 3501 0000 0a20  ...|.S.).a5.... 
+00001290: 2020 2020 2020 2053 6574 2061 6e20 656c         Set an el
+000012a0: 656d 656e 7420 7661 6c75 652e 0a0a 2020  ement value...  
+000012b0: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
+000012c0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000012d0: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
+000012e0: 732e 0a20 2020 2020 2020 2020 2020 2065  s..            e
+000012f0: 6c65 6d65 6e74 5f64 6566 696e 6974 696f  lement_definitio
+00001300: 6e5f 636f 6465 3a20 5468 6520 656c 656d  n_code: The elem
+00001310: 656e 7420 6465 6669 6e69 7469 6f6e 2063  ent definition c
+00001320: 6f64 652e 0a20 2020 2020 2020 2020 2020  ode..           
+00001330: 2065 6c65 6d65 6e74 5f76 616c 7565 3a20   element_value: 
+00001340: 5468 6520 656c 656d 656e 7420 7661 6c75  The element valu
+00001350: 652e 2049 6620 7468 6520 7661 6c75 6520  e. If the value 
+00001360: 6973 204e 6f6e 652c 2061 6c6c 2063 7572  is None, all cur
+00001370: 7265 6e74 2076 616c 7565 7320 6172 6520  rent values are 
+00001380: 7265 6d6f 7665 642e 0a0a 2020 2020 2020  removed...      
+00001390: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000013a0: 2020 2020 2020 2054 6865 2070 6173 7365         The passe
+000013b0: 6420 7072 6f63 6573 732e 0a20 2020 2020  d process..     
+000013c0: 2020 2029 0272 1f00 0000 723a 0000 00a9     ).r....r:....
+000013d0: 0372 3700 0000 7238 0000 0072 4000 0000  .r7...r8...r@...
+000013e0: 723c 0000 0072 3c00 0000 723d 0000 0072  r<...r<...r=...r
+000013f0: 1f00 0000 9500 0000 7304 0000 0000 1110  ........s.......
+00001400: 027a 1e50 726f 6365 7373 5574 696c 732e  .z.ProcessUtils.
+00001410: 7365 745f 656c 656d 656e 745f 7661 6c75  set_element_valu
+00001420: 6529 0472 3700 0000 7238 0000 00da 0e65  e).r7...r8.....e
+00001430: 6c65 6d65 6e74 5f76 616c 7565 7372 3900  lement_valuesr9.
+00001440: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00001450: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
+00001460: 7400 7401 7c00 7c01 8302 7c02 8302 0100  t.t.|.|...|.....
+00001470: 7c00 5300 2901 613f 0100 000a 2020 2020  |.S.).a?....    
+00001480: 2020 2020 5365 7420 616e 2065 6c65 6d65      Set an eleme
+00001490: 6e74 2076 616c 7565 2e0a 0a20 2020 2020  nt value...     
+000014a0: 2020 2041 7267 756d 656e 7473 3a0a 2020     Arguments:.  
+000014b0: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+000014c0: 733a 2054 6865 2070 726f 6365 7373 2e0a  s: The process..
+000014d0: 2020 2020 2020 2020 2020 2020 656c 656d              elem
+000014e0: 656e 745f 6465 6669 6e69 7469 6f6e 5f63  ent_definition_c
+000014f0: 6f64 653a 2054 6865 2065 6c65 6d65 6e74  ode: The element
+00001500: 2064 6566 696e 6974 696f 6e20 636f 6465   definition code
+00001510: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00001520: 656d 656e 745f 7661 6c75 6573 3a20 5468  ement_values: Th
+00001530: 6520 656c 656d 656e 7420 7661 6c75 652e  e element value.
+00001540: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+00001550: 204e 6f6e 6520 6f72 2065 6d70 7479 2c20   None or empty, 
+00001560: 616c 6c20 6375 7272 656e 7420 7661 6c75  all current valu
+00001570: 6573 2061 7265 2072 656d 6f76 6564 2e0a  es are removed..
+00001580: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001590: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+000015a0: 6520 7061 7373 6564 2070 726f 6365 7373  e passed process
+000015b0: 2e0a 2020 2020 2020 2020 2902 7220 0000  ..        ).r ..
+000015c0: 0072 3a00 0000 a903 7237 0000 0072 3800  .r:.....r7...r8.
+000015d0: 0000 7242 0000 0072 3c00 0000 723c 0000  ..rB...r<...r<..
+000015e0: 0072 3d00 0000 7220 0000 00aa 0000 0073  .r=...r .......s
+000015f0: 0a00 0000 0011 0201 0801 02fe 0405 7a23  ..............z#
+00001600: 5072 6f63 6573 7355 7469 6c73 2e73 6574  ProcessUtils.set
+00001610: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f6c  _element_value_l
+00001620: 6973 7463 0300 0000 0000 0000 0000 0000  istc............
+00001630: 0300 0000 0400 0000 4300 0000 7314 0000  ........C...s...
+00001640: 0074 0074 017c 007c 0183 027c 0283 0201  .t.t.|.|...|....
+00001650: 007c 0053 0029 0161 3501 0000 0a20 2020  .|.S.).a5....   
+00001660: 2020 2020 2041 6464 2061 6e20 656c 656d       Add an elem
+00001670: 656e 7420 7661 6c75 652e 0a0a 2020 2020  ent value...    
+00001680: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
+00001690: 2020 2020 2020 2020 2020 2070 726f 6365             proce
+000016a0: 7373 3a20 5468 6520 7072 6f63 6573 732e  ss: The process.
+000016b0: 0a20 2020 2020 2020 2020 2020 2065 6c65  .            ele
+000016c0: 6d65 6e74 5f64 6566 696e 6974 696f 6e5f  ment_definition_
+000016d0: 636f 6465 3a20 5468 6520 656c 656d 656e  code: The elemen
+000016e0: 7420 6465 6669 6e69 7469 6f6e 2063 6f64  t definition cod
+000016f0: 652e 0a20 2020 2020 2020 2020 2020 2065  e..            e
+00001700: 6c65 6d65 6e74 5f76 616c 7565 3a20 5468  lement_value: Th
+00001710: 6520 656c 656d 656e 7420 7661 6c75 652e  e element value.
+00001720: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+00001730: 204e 6f6e 652c 2061 6c6c 2063 7572 7265   None, all curre
+00001740: 6e74 2076 616c 7565 7320 6172 6520 7265  nt values are re
+00001750: 6d6f 7665 642e 0a0a 2020 2020 2020 2020  moved...        
+00001760: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00001770: 2020 2020 2054 6865 2070 6173 7365 6420       The passed 
+00001780: 7072 6f63 6573 732e 0a20 2020 2020 2020  process..       
+00001790: 2029 0272 1200 0000 723a 0000 0072 4100   ).r....r:...rA.
+000017a0: 0000 723c 0000 0072 3c00 0000 723d 0000  ..r<...r<...r=..
+000017b0: 0072 1200 0000 c200 0000 7304 0000 0000  .r........s.....
+000017c0: 1110 027a 1e50 726f 6365 7373 5574 696c  ...z.ProcessUtil
+000017d0: 732e 6164 645f 656c 656d 656e 745f 7661  s.add_element_va
+000017e0: 6c75 6563 0300 0000 0000 0000 0000 0000  luec............
+000017f0: 0300 0000 0400 0000 4300 0000 7314 0000  ........C...s...
+00001800: 0074 0074 017c 007c 0183 027c 0283 0201  .t.t.|.|...|....
+00001810: 007c 0053 0029 0161 4c01 0000 0a20 2020  .|.S.).aL....   
+00001820: 2020 2020 2041 6464 2065 6c65 6d65 6e74       Add element
+00001830: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00001840: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+00001850: 2020 2020 2020 2020 2070 726f 6365 7373           process
+00001860: 3a20 5468 6520 7072 6f63 6573 732e 0a20  : The process.. 
+00001870: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
+00001880: 6e74 5f64 6566 696e 6974 696f 6e5f 636f  nt_definition_co
+00001890: 6465 3a20 5468 6520 656c 656d 656e 7420  de: The element 
+000018a0: 6465 6669 6e69 7469 6f6e 2063 6f64 652e  definition code.
+000018b0: 0a20 2020 2020 2020 2020 2020 2065 6c65  .            ele
+000018c0: 6d65 6e74 5f76 616c 7565 733a 2054 6865  ment_values: The
+000018d0: 2065 6c65 6d65 6e74 2076 616c 7565 732e   element values.
+000018e0: 2049 6620 7468 6520 7661 6c75 6573 2069   If the values i
+000018f0: 7320 4e6f 6e65 206f 7220 656d 7074 792c  s None or empty,
+00001900: 2061 6c6c 2063 7572 7265 6e74 2076 616c   all current val
+00001910: 7565 7320 6172 6520 7265 6d6f 7665 642e  ues are removed.
+00001920: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001930: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+00001940: 6865 2070 6173 7365 6420 6d6f 6465 6c20  he passed model 
+00001950: 7265 6c61 7465 6420 6f62 6a65 6374 2e0a  related object..
+00001960: 2020 2020 2020 2020 2902 7213 0000 0072          ).r....r
+00001970: 3a00 0000 7243 0000 0072 3c00 0000 723c  :...rC...r<...r<
+00001980: 0000 0072 3d00 0000 7213 0000 00d7 0000  ...r=...r.......
+00001990: 0073 0a00 0000 0011 0201 0801 02fe 0405  .s..............
+000019a0: 7a23 5072 6f63 6573 7355 7469 6c73 2e61  z#ProcessUtils.a
+000019b0: 6464 5f65 6c65 6d65 6e74 5f76 616c 7565  dd_element_value
+000019c0: 5f6c 6973 7463 0200 0000 0000 0000 0000  _listc..........
+000019d0: 0000 0200 0000 0400 0000 4300 0000 730e  ..........C...s.
+000019e0: 0000 0074 0074 017c 007c 0183 0283 0153  ...t.t.|.|.....S
+000019f0: 0029 017a dc0a 2020 2020 2020 2020 4765  .).z..        Ge
+00001a00: 7420 616e 2065 6c65 6d65 6e74 2061 7320  t an element as 
+00001a10: 6120 7374 722e 0a0a 2020 2020 2020 2020  a str...        
+00001a20: 4172 6775 6d65 6e74 733a 0a20 2020 2020  Arguments:.     
+00001a30: 2020 2020 2020 2070 726f 6365 7373 3a20         process: 
+00001a40: 5468 6520 7072 6f63 6573 732e 0a20 2020  The process..   
+00001a50: 2020 2020 2020 2020 2065 6c65 6d65 6e74           element
+00001a60: 5f64 6566 696e 6974 696f 6e5f 636f 6465  _definition_code
+00001a70: 3a20 5468 6520 656c 656d 656e 7420 6465  : The element de
+00001a80: 6669 6e69 7469 6f6e 2063 6f64 652e 0a0a  finition code...
+00001a90: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00001aa0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00001ab0: 2065 6c65 6d65 6e74 2076 616c 7565 2061   element value a
+00001ac0: 7320 6120 7374 722e 0a20 2020 2020 2020  s a str..       
+00001ad0: 2029 0272 1b00 0000 723a 0000 0072 3b00   ).r....r:...r;.
+00001ae0: 0000 723c 0000 0072 3c00 0000 723d 0000  ..r<...r<...r=..
+00001af0: 0072 1b00 0000 ef00 0000 7302 0000 0000  .r........s.....
+00001b00: 0c7a 2550 726f 6365 7373 5574 696c 732e  .z%ProcessUtils.
+00001b10: 6765 745f 656c 656d 656e 745f 7661 6c75  get_element_valu
+00001b20: 655f 6173 5f73 7472 6302 0000 0000 0000  e_as_strc.......
+00001b30: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00001b40: 0073 0e00 0000 7400 7401 7c00 7c01 8302  .s....t.t.|.|...
+00001b50: 8301 5300 2901 7ae3 0a20 2020 2020 2020  ..S.).z..       
+00001b60: 2054 7279 2074 6f20 6765 7420 616e 2065   Try to get an e
+00001b70: 6c65 6d65 6e74 2061 7320 6120 7374 722e  lement as a str.
+00001b80: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+00001b90: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00001ba0: 2070 726f 6365 7373 3a20 5468 6520 7072   process: The pr
+00001bb0: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
+00001bc0: 2020 2065 6c65 6d65 6e74 5f64 6566 696e     element_defin
+00001bd0: 6974 696f 6e5f 636f 6465 3a20 5468 6520  ition_code: The 
+00001be0: 656c 656d 656e 7420 6465 6669 6e69 7469  element definiti
+00001bf0: 6f6e 2063 6f64 652e 0a0a 2020 2020 2020  on code...      
+00001c00: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001c10: 2020 2020 2020 2054 6865 2065 6c65 6d65         The eleme
+00001c20: 6e74 2076 616c 7565 2061 7320 6120 7374  nt value as a st
+00001c30: 722e 0a20 2020 2020 2020 2029 0272 1600  r..        ).r..
+00001c40: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
+00001c50: 0072 3c00 0000 723d 0000 0072 1600 0000  .r<...r=...r....
+00001c60: fd00 0000 7302 0000 0000 0c7a 2650 726f  ....s......z&Pro
+00001c70: 6365 7373 5574 696c 732e 6669 6e64 5f65  cessUtils.find_e
+00001c80: 6c65 6d65 6e74 5f76 616c 7565 5f61 735f  lement_value_as_
+00001c90: 7374 7263 0200 0000 0000 0000 0000 0000  strc............
+00001ca0: 0200 0000 0400 0000 4300 0000 730e 0000  ........C...s...
+00001cb0: 0074 0074 017c 007c 0183 0283 0153 0029  .t.t.|.|.....S.)
+00001cc0: 017a ee0a 2020 2020 2020 2020 5472 7920  .z..        Try 
+00001cd0: 746f 2067 6574 2061 6e20 656c 656d 656e  to get an elemen
+00001ce0: 7420 6173 2061 2073 7472 206c 6973 742e  t as a str list.
+00001cf0: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+00001d00: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00001d10: 2070 726f 6365 7373 3a20 5468 6520 7072   process: The pr
+00001d20: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
+00001d30: 2020 2065 6c65 6d65 6e74 5f64 6566 696e     element_defin
+00001d40: 6974 696f 6e5f 636f 6465 3a20 5468 6520  ition_code: The 
+00001d50: 656c 656d 656e 7420 6465 6669 6e69 7469  element definiti
+00001d60: 6f6e 2063 6f64 652e 0a0a 2020 2020 2020  on code...      
+00001d70: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001d80: 2020 2020 2020 2054 6865 2065 6c65 6d65         The eleme
+00001d90: 6e74 2076 616c 7565 7320 6173 2061 2073  nt values as a s
+00001da0: 7472 206c 6973 742e 0a20 2020 2020 2020  tr list..       
+00001db0: 2029 0272 1c00 0000 723a 0000 0072 3b00   ).r....r:...r;.
+00001dc0: 0000 723c 0000 0072 3c00 0000 723d 0000  ..r<...r<...r=..
+00001dd0: 0072 1c00 0000 0b01 0000 7302 0000 0000  .r........s.....
+00001de0: 0c7a 2a50 726f 6365 7373 5574 696c 732e  .z*ProcessUtils.
+00001df0: 6765 745f 656c 656d 656e 745f 7661 6c75  get_element_valu
+00001e00: 655f 6173 5f73 7472 5f6c 6973 7463 0200  e_as_str_listc..
+00001e10: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001e20: 0000 4300 0000 730e 0000 0074 0074 017c  ..C...s....t.t.|
+00001e30: 007c 0183 0283 0153 0029 017a e00a 2020  .|.....S.).z..  
+00001e40: 2020 2020 2020 4765 7420 616e 2065 6c65        Get an ele
+00001e50: 6d65 6e74 2061 7320 6120 666c 6f61 742e  ment as a float.
+00001e60: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+00001e70: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00001e80: 2070 726f 6365 7373 3a20 5468 6520 7072   process: The pr
+00001e90: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
+00001ea0: 2020 2065 6c65 6d65 6e74 5f64 6566 696e     element_defin
+00001eb0: 6974 696f 6e5f 636f 6465 3a20 5468 6520  ition_code: The 
+00001ec0: 656c 656d 656e 7420 6465 6669 6e69 7469  element definiti
+00001ed0: 6f6e 2063 6f64 652e 0a0a 2020 2020 2020  on code...      
+00001ee0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001ef0: 2020 2020 2020 2054 6865 2065 6c65 6d65         The eleme
+00001f00: 6e74 2076 616c 7565 2061 7320 6120 666c  nt value as a fl
+00001f10: 6f61 742e 0a20 2020 2020 2020 2029 0272  oat..        ).r
+00001f20: 1900 0000 723a 0000 0072 3b00 0000 723c  ....r:...r;...r<
+00001f30: 0000 0072 3c00 0000 723d 0000 0072 1900  ...r<...r=...r..
+00001f40: 0000 1901 0000 7302 0000 0000 0c7a 2750  ......s......z'P
+00001f50: 726f 6365 7373 5574 696c 732e 6765 745f  rocessUtils.get_
+00001f60: 656c 656d 656e 745f 7661 6c75 655f 6173  element_value_as
+00001f70: 5f66 6c6f 6174 6302 0000 0000 0000 0000  _floatc.........
+00001f80: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00001f90: 0e00 0000 7400 7401 7c00 7c01 8302 8301  ....t.t.|.|.....
+00001fa0: 5300 2901 7ae7 0a20 2020 2020 2020 2054  S.).z..        T
+00001fb0: 7279 2074 6f20 6765 7420 616e 2065 6c65  ry to get an ele
+00001fc0: 6d65 6e74 2061 7320 6120 666c 6f61 742e  ment as a float.
+00001fd0: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+00001fe0: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00001ff0: 2070 726f 6365 7373 3a20 5468 6520 7072   process: The pr
+00002000: 6f63 6573 732e 0a20 2020 2020 2020 2020  ocess..         
+00002010: 2020 2065 6c65 6d65 6e74 5f64 6566 696e     element_defin
+00002020: 6974 696f 6e5f 636f 6465 3a20 5468 6520  ition_code: The 
+00002030: 656c 656d 656e 7420 6465 6669 6e69 7469  element definiti
+00002040: 6f6e 2063 6f64 652e 0a0a 2020 2020 2020  on code...      
+00002050: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00002060: 2020 2020 2020 2054 6865 2065 6c65 6d65         The eleme
+00002070: 6e74 2076 616c 7565 2061 7320 6120 666c  nt value as a fl
+00002080: 6f61 742e 0a20 2020 2020 2020 2029 0272  oat..        ).r
+00002090: 1500 0000 723a 0000 0072 3b00 0000 723c  ....r:...r;...r<
+000020a0: 0000 0072 3c00 0000 723d 0000 0072 1500  ...r<...r=...r..
+000020b0: 0000 2701 0000 7302 0000 0000 0c7a 2850  ..'...s......z(P
+000020c0: 726f 6365 7373 5574 696c 732e 6669 6e64  rocessUtils.find
+000020d0: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f61  _element_value_a
+000020e0: 735f 666c 6f61 7463 0200 0000 0000 0000  s_floatc........
+000020f0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00002100: 730e 0000 0074 0074 017c 007c 0183 0283  s....t.t.|.|....
+00002110: 0153 0029 017a e70a 2020 2020 2020 2020  .S.).z..        
+00002120: 4765 7420 616c 6c20 656c 656d 656e 7473  Get all elements
+00002130: 2061 7320 6120 666c 6f61 7420 6c69 7374   as a float list
+00002140: 2e0a 0a20 2020 2020 2020 2041 7267 756d  ...        Argum
+00002150: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
+00002160: 2020 7072 6f63 6573 733a 2054 6865 2070    process: The p
+00002170: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
+00002180: 2020 2020 656c 656d 656e 745f 6465 6669      element_defi
+00002190: 6e69 7469 6f6e 5f63 6f64 653a 2054 6865  nition_code: The
+000021a0: 2065 6c65 6d65 6e74 2064 6566 696e 6974   element definit
+000021b0: 696f 6e20 636f 6465 2e0a 0a20 2020 2020  ion code...     
+000021c0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000021d0: 2020 2020 2020 2020 5468 6520 656c 656d          The elem
+000021e0: 656e 7420 7661 6c75 6520 6173 2061 2066  ent value as a f
+000021f0: 6c6f 6174 2e0a 2020 2020 2020 2020 2902  loat..        ).
+00002200: 721a 0000 0072 3a00 0000 723b 0000 0072  r....r:...r;...r
+00002210: 3c00 0000 723c 0000 0072 3d00 0000 721a  <...r<...r=...r.
+00002220: 0000 0035 0100 0073 0200 0000 000c 7a2c  ...5...s......z,
+00002230: 5072 6f63 6573 7355 7469 6c73 2e67 6574  ProcessUtils.get
+00002240: 5f65 6c65 6d65 6e74 5f76 616c 7565 5f61  _element_value_a
+00002250: 735f 666c 6f61 745f 6c69 7374 6302 0000  s_float_listc...
+00002260: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00002270: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
+00002280: 7c01 8302 8301 5300 2901 7ade 0a20 2020  |.....S.).z..   
+00002290: 2020 2020 2047 6574 2061 6e20 656c 656d       Get an elem
+000022a0: 656e 7420 6173 2061 2064 6174 652e 0a0a  ent as a date...
+000022b0: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
+000022c0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+000022d0: 726f 6365 7373 3a20 5468 6520 7072 6f63  rocess: The proc
+000022e0: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
+000022f0: 2065 6c65 6d65 6e74 5f64 6566 696e 6974   element_definit
+00002300: 696f 6e5f 636f 6465 3a20 5468 6520 656c  ion_code: The el
+00002310: 656d 656e 7420 6465 6669 6e69 7469 6f6e  ement definition
+00002320: 2063 6f64 652e 0a0a 2020 2020 2020 2020   code...        
+00002330: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00002340: 2020 2020 2054 6865 2065 6c65 6d65 6e74       The element
+00002350: 2076 616c 7565 2061 7320 6120 6461 7465   value as a date
+00002360: 2e0a 2020 2020 2020 2020 2902 7217 0000  ..        ).r...
+00002370: 0072 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
+00002380: 723c 0000 0072 3d00 0000 7217 0000 0043  r<...r=...r....C
+00002390: 0100 0073 0200 0000 000c 7a26 5072 6f63  ...s......z&Proc
+000023a0: 6573 7355 7469 6c73 2e67 6574 5f65 6c65  essUtils.get_ele
+000023b0: 6d65 6e74 5f76 616c 7565 5f61 735f 6461  ment_value_as_da
+000023c0: 7465 6302 0000 0000 0000 0000 0000 0002  tec.............
+000023d0: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
+000023e0: 7400 7401 7c00 7c01 8302 8301 5300 2901  t.t.|.|.....S.).
+000023f0: 7ae6 0a20 2020 2020 2020 2054 7279 2074  z..        Try t
+00002400: 6f20 6765 7420 2061 6e20 656c 656d 656e  o get  an elemen
+00002410: 7420 6173 2061 2064 6174 652e 0a0a 2020  t as a date...  
+00002420: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
+00002430: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00002440: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
+00002450: 732e 0a20 2020 2020 2020 2020 2020 2065  s..            e
+00002460: 6c65 6d65 6e74 5f64 6566 696e 6974 696f  lement_definitio
+00002470: 6e5f 636f 6465 3a20 5468 6520 656c 656d  n_code: The elem
+00002480: 656e 7420 6465 6669 6e69 7469 6f6e 2063  ent definition c
+00002490: 6f64 652e 0a0a 2020 2020 2020 2020 5265  ode...        Re
+000024a0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000024b0: 2020 2054 6865 2065 6c65 6d65 6e74 2076     The element v
+000024c0: 616c 7565 2061 7320 6120 6461 7465 2e0a  alue as a date..
+000024d0: 2020 2020 2020 2020 2902 7214 0000 0072          ).r....r
+000024e0: 3a00 0000 723b 0000 0072 3c00 0000 723c  :...r;...r<...r<
+000024f0: 0000 0072 3d00 0000 7214 0000 0051 0100  ...r=...r....Q..
+00002500: 0073 0200 0000 000c 7a27 5072 6f63 6573  .s......z'Proces
+00002510: 7355 7469 6c73 2e66 696e 645f 656c 656d  sUtils.find_elem
+00002520: 656e 745f 7661 6c75 655f 6173 5f64 6174  ent_value_as_dat
+00002530: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00002540: 0000 0400 0000 4300 0000 730e 0000 0074  ......C...s....t
+00002550: 0074 017c 007c 0183 0283 0153 0029 017a  .t.|.|.....S.).z
+00002560: e30a 2020 2020 2020 2020 4765 7420 616c  ..        Get al
+00002570: 6c20 656c 656d 656e 7473 2061 7320 6461  l elements as da
+00002580: 7465 206c 6973 742e 0a0a 2020 2020 2020  te list...      
+00002590: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+000025a0: 2020 2020 2020 2020 2070 726f 6365 7373           process
+000025b0: 3a20 5468 6520 7072 6f63 6573 732e 0a20  : The process.. 
+000025c0: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
+000025d0: 6e74 5f64 6566 696e 6974 696f 6e5f 636f  nt_definition_co
+000025e0: 6465 3a20 5468 6520 656c 656d 656e 7420  de: The element 
+000025f0: 6465 6669 6e69 7469 6f6e 2063 6f64 652e  definition code.
+00002600: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00002610: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+00002620: 6865 2065 6c65 6d65 6e74 2076 616c 7565  he element value
+00002630: 2061 7320 6120 6461 7465 2e0a 2020 2020   as a date..    
+00002640: 2020 2020 2902 7218 0000 0072 3a00 0000      ).r....r:...
+00002650: 723b 0000 0072 3c00 0000 723c 0000 0072  r;...r<...r<...r
+00002660: 3d00 0000 7218 0000 005f 0100 0073 0200  =...r...._...s..
+00002670: 0000 000c 7a2b 5072 6f63 6573 7355 7469  ....z+ProcessUti
+00002680: 6c73 2e67 6574 5f65 6c65 6d65 6e74 5f76  ls.get_element_v
+00002690: 616c 7565 5f61 735f 6461 7465 5f6c 6973  alue_as_date_lis
+000026a0: 7429 0372 3700 0000 da0d 7072 6f70 6572  t).r7.....proper
+000026b0: 7479 5f70 6174 6872 3900 0000 6302 0000  ty_pathr9...c...
+000026c0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+000026d0: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
+000026e0: 8301 7c01 8302 5300 2901 6179 0100 000a  ..|...S.).ay....
+000026f0: 2020 2020 2020 2020 4765 7420 6120 6a73          Get a js
+00002700: 6f6e 2070 726f 7065 7274 7920 6173 2022  on property as "
+00002710: 7374 7222 2066 6f6c 6c6f 7769 6e67 2074  str" following t
+00002720: 6865 2022 7072 6f70 6572 7479 5061 7468  he "propertyPath
+00002730: 2220 7061 7373 6564 2e0a 0a20 2020 2020  " passed...     
+00002740: 2020 2041 7267 756d 656e 7473 3a0a 2020     Arguments:.  
+00002750: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+00002760: 733a 2054 6865 2070 726f 6365 7373 2e0a  s: The process..
+00002770: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+00002780: 6572 7479 5f70 6174 683a 2050 726f 7065  erty_path: Prope
+00002790: 7274 7920 7061 7468 2074 6f20 6669 6e64  rty path to find
+000027a0: 2e20 6965 3a20 2275 7365 722e 6e61 6d65  . ie: "user.name
+000027b0: 2220 6f72 2022 7573 6572 732e 302e 6e61  " or "users.0.na
+000027c0: 6d65 220a 0a20 2020 2020 2020 2052 6574  me"..        Ret
+000027d0: 7572 6e3a 0a20 2020 2020 2020 2020 2020  urn:.           
+000027e0: 2074 6865 2070 726f 7065 7274 7920 7661   the property va
+000027f0: 6c75 6520 6966 2065 7869 7374 732e 0a0a  lue if exists...
+00002800: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00002810: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+00002820: 6545 7272 6f72 3a20 4966 2070 726f 7065  eError: If prope
+00002830: 7274 7920 7661 6c75 6520 646f 6573 6e27  rty value doesn'
+00002840: 7420 6578 6973 7420 6f72 2068 6173 2069  t exist or has i
+00002850: 6e63 6f72 7265 6374 2066 6f72 6d61 740a  ncorrect format.
+00002860: 2020 2020 2020 2020 2902 7235 0000 00da          ).r5....
+00002870: 1b43 7572 7265 6e74 4a73 6f6e 466f 726d  .CurrentJsonForm
+00002880: 4461 7461 4163 6365 7373 6f72 a902 7237  DataAccessor..r7
+00002890: 0000 0072 4400 0000 723c 0000 0072 3c00  ...rD...r<...r<.
+000028a0: 0000 723d 0000 00da 1a67 6574 5f65 6e74  ..r=.....get_ent
+000028b0: 6974 795f 7072 6f70 6572 7479 5f61 735f  ity_property_as_
+000028c0: 7374 726d 0100 0073 0200 0000 000f 7a27  strm...s......z'
+000028d0: 5072 6f63 6573 7355 7469 6c73 2e67 6574  ProcessUtils.get
+000028e0: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
+000028f0: 5f61 735f 7374 7263 0200 0000 0000 0000  _as_strc........
+00002900: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00002910: 730e 0000 0074 0074 017c 0083 017c 0183  s....t.t.|...|..
+00002920: 0253 0029 0161 7001 0000 0a20 2020 2020  .S.).ap....     
+00002930: 2020 2054 7279 2074 6f20 6669 6e64 2061     Try to find a
+00002940: 206a 736f 6e20 7072 6f70 6572 7479 2061   json property a
+00002950: 7320 2273 7472 2220 666f 6c6c 6f77 696e  s "str" followin
+00002960: 6720 7468 6520 2270 726f 7065 7274 7950  g the "propertyP
+00002970: 6174 6822 2070 6173 7365 642e 0a0a 2020  ath" passed...  
+00002980: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
+00002990: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000029a0: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
+000029b0: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
+000029c0: 726f 7065 7274 795f 7061 7468 3a20 5072  roperty_path: Pr
+000029d0: 6f70 6572 7479 2070 6174 6820 746f 2066  operty path to f
+000029e0: 696e 642e 2069 653a 2022 7573 6572 2e6e  ind. ie: "user.n
+000029f0: 616d 6522 206f 7220 2275 7365 7273 2e30  ame" or "users.0
+00002a00: 2e6e 616d 6522 0a0a 2020 2020 2020 2020  .name"..        
+00002a10: 5265 7475 726e 3a0a 2020 2020 2020 2020  Return:.        
+00002a20: 2020 2020 5468 6520 7072 6f70 6572 7479      The property
+00002a30: 2076 616c 7565 2069 6620 6578 6973 7473   value if exists
+00002a40: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00002a50: 733a 0a20 2020 2020 2020 2020 2020 2056  s:.            V
+00002a60: 616c 7565 4572 726f 723a 2049 6620 7072  alueError: If pr
+00002a70: 6f70 6572 7479 2076 616c 7565 2068 6173  operty value has
+00002a80: 2069 6e63 6f72 7265 6374 2066 6f72 6d61   incorrect forma
+00002a90: 740a 2020 2020 2020 2020 2902 722c 0000  t.        ).r,..
+00002aa0: 0072 4500 0000 7246 0000 0072 3c00 0000  .rE...rF...r<...
+00002ab0: 723c 0000 0072 3d00 0000 da1b 6669 6e64  r<...r=.....find
+00002ac0: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
+00002ad0: 5f61 735f 7374 727e 0100 0073 0200 0000  _as_str~...s....
+00002ae0: 000f 7a28 5072 6f63 6573 7355 7469 6c73  ..z(ProcessUtils
+00002af0: 2e66 696e 645f 656e 7469 7479 5f70 726f  .find_entity_pro
+00002b00: 7065 7274 795f 6173 5f73 7472 6302 0000  perty_as_strc...
+00002b10: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002b20: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
+00002b30: 8301 7c01 8302 5300 2901 6179 0100 000a  ..|...S.).ay....
+00002b40: 2020 2020 2020 2020 4765 7420 6120 6a73          Get a js
+00002b50: 6f6e 2070 726f 7065 7274 7920 6173 2022  on property as "
+00002b60: 696e 7422 2066 6f6c 6c6f 7769 6e67 2074  int" following t
+00002b70: 6865 2022 7072 6f70 6572 7479 5061 7468  he "propertyPath
+00002b80: 2220 7061 7373 6564 2e0a 0a20 2020 2020  " passed...     
+00002b90: 2020 2041 7267 756d 656e 7473 3a0a 2020     Arguments:.  
+00002ba0: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+00002bb0: 733a 2054 6865 2070 726f 6365 7373 2e0a  s: The process..
+00002bc0: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+00002bd0: 6572 7479 5f70 6174 683a 2050 726f 7065  erty_path: Prope
+00002be0: 7274 7920 7061 7468 2074 6f20 6669 6e64  rty path to find
+00002bf0: 2e20 6965 3a20 2275 7365 722e 6e61 6d65  . ie: "user.name
+00002c00: 2220 6f72 2022 7573 6572 732e 302e 6e61  " or "users.0.na
+00002c10: 6d65 220a 0a20 2020 2020 2020 2052 6574  me"..        Ret
+00002c20: 7572 6e3a 0a20 2020 2020 2020 2020 2020  urn:.           
+00002c30: 2074 6865 2070 726f 7065 7274 7920 7661   the property va
+00002c40: 6c75 6520 6966 2065 7869 7374 732e 0a0a  lue if exists...
+00002c50: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00002c60: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+00002c70: 6545 7272 6f72 3a20 4966 2070 726f 7065  eError: If prope
+00002c80: 7274 7920 7661 6c75 6520 646f 6573 6e27  rty value doesn'
+00002c90: 7420 6578 6973 7420 6f72 2068 6173 2069  t exist or has i
+00002ca0: 6e63 6f72 7265 6374 2066 6f72 6d61 740a  ncorrect format.
+00002cb0: 2020 2020 2020 2020 2902 7231 0000 0072          ).r1...r
+00002cc0: 4500 0000 7246 0000 0072 3c00 0000 723c  E...rF...r<...r<
+00002cd0: 0000 0072 3d00 0000 da1a 6765 745f 656e  ...r=.....get_en
+00002ce0: 7469 7479 5f70 726f 7065 7274 795f 6173  tity_property_as
+00002cf0: 5f69 6e74 8f01 0000 7302 0000 0000 0f7a  _int....s......z
+00002d00: 2750 726f 6365 7373 5574 696c 732e 6765  'ProcessUtils.ge
+00002d10: 745f 656e 7469 7479 5f70 726f 7065 7274  t_entity_propert
+00002d20: 795f 6173 5f69 6e74 6302 0000 0000 0000  y_as_intc.......
+00002d30: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00002d40: 0073 0e00 0000 7400 7401 7c00 8301 7c01  .s....t.t.|...|.
+00002d50: 8302 5300 2901 6170 0100 000a 2020 2020  ..S.).ap....    
+00002d60: 2020 2020 5472 7920 746f 2066 696e 6420      Try to find 
+00002d70: 6120 6a73 6f6e 2070 726f 7065 7274 7920  a json property 
+00002d80: 6173 2022 696e 7422 2066 6f6c 6c6f 7769  as "int" followi
+00002d90: 6e67 2074 6865 2022 7072 6f70 6572 7479  ng the "property
+00002da0: 5061 7468 2220 7061 7373 6564 2e0a 0a20  Path" passed... 
+00002db0: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
+00002dc0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00002dd0: 6f63 6573 733a 2054 6865 2070 726f 6365  ocess: The proce
+00002de0: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
+00002df0: 7072 6f70 6572 7479 5f70 6174 683a 2050  property_path: P
+00002e00: 726f 7065 7274 7920 7061 7468 2074 6f20  roperty path to 
+00002e10: 6669 6e64 2e20 6965 3a20 2275 7365 722e  find. ie: "user.
+00002e20: 6e61 6d65 2220 6f72 2022 7573 6572 732e  name" or "users.
+00002e30: 302e 6e61 6d65 220a 0a20 2020 2020 2020  0.name"..       
+00002e40: 2052 6574 7572 6e3a 0a20 2020 2020 2020   Return:.       
+00002e50: 2020 2020 2054 6865 2070 726f 7065 7274       The propert
+00002e60: 7920 7661 6c75 6520 6966 2065 7869 7374  y value if exist
+00002e70: 732e 0a0a 2020 2020 2020 2020 5261 6973  s...        Rais
+00002e80: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00002e90: 5661 6c75 6545 7272 6f72 3a20 4966 2070  ValueError: If p
+00002ea0: 726f 7065 7274 7920 7661 6c75 6520 6861  roperty value ha
+00002eb0: 7320 696e 636f 7272 6563 7420 666f 726d  s incorrect form
+00002ec0: 6174 0a20 2020 2020 2020 2029 0272 2800  at.        ).r(.
+00002ed0: 0000 7245 0000 0072 4600 0000 723c 0000  ..rE...rF...r<..
+00002ee0: 0072 3c00 0000 723d 0000 00da 1b66 696e  .r<...r=.....fin
+00002ef0: 645f 656e 7469 7479 5f70 726f 7065 7274  d_entity_propert
+00002f00: 795f 6173 5f69 6e74 a001 0000 7302 0000  y_as_int....s...
+00002f10: 0000 0f7a 2850 726f 6365 7373 5574 696c  ...z(ProcessUtil
+00002f20: 732e 6669 6e64 5f65 6e74 6974 795f 7072  s.find_entity_pr
+00002f30: 6f70 6572 7479 5f61 735f 696e 7463 0200  operty_as_intc..
+00002f40: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002f50: 0000 4300 0000 730e 0000 0074 0074 017c  ..C...s....t.t.|
+00002f60: 0083 017c 0183 0253 0029 0161 7b01 0000  ...|...S.).a{...
+00002f70: 0a20 2020 2020 2020 2047 6574 2061 206a  .        Get a j
+00002f80: 736f 6e20 7072 6f70 6572 7479 2061 7320  son property as 
+00002f90: 2266 6c6f 6174 2220 666f 6c6c 6f77 696e  "float" followin
+00002fa0: 6720 7468 6520 2270 726f 7065 7274 7950  g the "propertyP
+00002fb0: 6174 6822 2070 6173 7365 642e 0a0a 2020  ath" passed...  
+00002fc0: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
+00002fd0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00002fe0: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
+00002ff0: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
+00003000: 726f 7065 7274 795f 7061 7468 3a20 5072  roperty_path: Pr
+00003010: 6f70 6572 7479 2070 6174 6820 746f 2066  operty path to f
+00003020: 696e 642e 2069 653a 2022 7573 6572 2e6e  ind. ie: "user.n
+00003030: 616d 6522 206f 7220 2275 7365 7273 2e30  ame" or "users.0
+00003040: 2e6e 616d 6522 0a0a 2020 2020 2020 2020  .name"..        
+00003050: 5265 7475 726e 3a0a 2020 2020 2020 2020  Return:.        
+00003060: 2020 2020 7468 6520 7072 6f70 6572 7479      the property
+00003070: 2076 616c 7565 2069 6620 6578 6973 7473   value if exists
+00003080: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00003090: 733a 0a20 2020 2020 2020 2020 2020 2056  s:.            V
+000030a0: 616c 7565 4572 726f 723a 2049 6620 7072  alueError: If pr
+000030b0: 6f70 6572 7479 2076 616c 7565 2064 6f65  operty value doe
+000030c0: 736e 2774 2065 7869 7374 206f 7220 6861  sn't exist or ha
+000030d0: 7320 696e 636f 7272 6563 7420 666f 726d  s incorrect form
+000030e0: 6174 0a20 2020 2020 2020 2029 0272 3000  at.        ).r0.
+000030f0: 0000 7245 0000 0072 4600 0000 723c 0000  ..rE...rF...r<..
+00003100: 0072 3c00 0000 723d 0000 00da 1c67 6574  .r<...r=.....get
+00003110: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
+00003120: 5f61 735f 666c 6f61 74b1 0100 0073 0200  _as_float....s..
+00003130: 0000 000f 7a29 5072 6f63 6573 7355 7469  ....z)ProcessUti
+00003140: 6c73 2e67 6574 5f65 6e74 6974 795f 7072  ls.get_entity_pr
+00003150: 6f70 6572 7479 5f61 735f 666c 6f61 7463  operty_as_floatc
+00003160: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00003170: 0300 0000 4300 0000 730e 0000 0074 0074  ....C...s....t.t
+00003180: 017c 0083 017c 0183 0253 0029 0161 7201  .|...|...S.).ar.
+00003190: 0000 0a20 2020 2020 2020 2054 7279 2074  ...        Try t
+000031a0: 6f20 6669 6e64 2061 206a 736f 6e20 7072  o find a json pr
+000031b0: 6f70 6572 7479 2061 7320 2266 6c6f 6174  operty as "float
+000031c0: 2220 666f 6c6c 6f77 696e 6720 7468 6520  " following the 
+000031d0: 2270 726f 7065 7274 7950 6174 6822 2070  "propertyPath" p
+000031e0: 6173 7365 642e 0a0a 2020 2020 2020 2020  assed...        
+000031f0: 4172 6775 6d65 6e74 733a 0a20 2020 2020  Arguments:.     
+00003200: 2020 2020 2020 2070 726f 6365 7373 3a20         process: 
+00003210: 5468 6520 7072 6f63 6573 732e 0a20 2020  The process..   
+00003220: 2020 2020 2020 2020 2070 726f 7065 7274           propert
+00003230: 795f 7061 7468 3a20 5072 6f70 6572 7479  y_path: Property
+00003240: 2070 6174 6820 746f 2066 696e 642e 2069   path to find. i
+00003250: 653a 2022 7573 6572 2e6e 616d 6522 206f  e: "user.name" o
+00003260: 7220 2275 7365 7273 2e30 2e6e 616d 6522  r "users.0.name"
+00003270: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00003280: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00003290: 6520 7072 6f70 6572 7479 2076 616c 7565  e property value
+000032a0: 2069 6620 6578 6973 7473 2e0a 0a20 2020   if exists...   
+000032b0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+000032c0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+000032d0: 726f 723a 2049 6620 7072 6f70 6572 7479  ror: If property
+000032e0: 2076 616c 7565 2068 6173 2069 6e63 6f72   value has incor
+000032f0: 7265 6374 2066 6f72 6d61 740a 2020 2020  rect format.    
+00003300: 2020 2020 2902 7227 0000 0072 4500 0000      ).r'...rE...
+00003310: 7246 0000 0072 3c00 0000 723c 0000 0072  rF...r<...r<...r
+00003320: 3d00 0000 da1d 6669 6e64 5f65 6e74 6974  =.....find_entit
+00003330: 795f 7072 6f70 6572 7479 5f61 735f 666c  y_property_as_fl
+00003340: 6f61 74c2 0100 0073 0200 0000 000f 7a2a  oat....s......z*
+00003350: 5072 6f63 6573 7355 7469 6c73 2e66 696e  ProcessUtils.fin
+00003360: 645f 656e 7469 7479 5f70 726f 7065 7274  d_entity_propert
+00003370: 795f 6173 5f66 6c6f 6174 6302 0000 0000  y_as_floatc.....
+00003380: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00003390: 0000 0073 0e00 0000 7400 7401 7c00 8301  ...s....t.t.|...
+000033a0: 7c01 8302 5300 2901 617a 0100 000a 2020  |...S.).az....  
+000033b0: 2020 2020 2020 4765 7420 6120 6a73 6f6e        Get a json
+000033c0: 2070 726f 7065 7274 7920 6173 2022 6461   property as "da
+000033d0: 7465 2220 666f 6c6c 6f77 696e 6720 7468  te" following th
+000033e0: 6520 2270 726f 7065 7274 7950 6174 6822  e "propertyPath"
+000033f0: 2070 6173 7365 642e 0a0a 2020 2020 2020   passed...      
+00003400: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+00003410: 2020 2020 2020 2020 2070 726f 6365 7373           process
+00003420: 3a20 5468 6520 7072 6f63 6573 732e 0a20  : The process.. 
+00003430: 2020 2020 2020 2020 2020 2070 726f 7065             prope
+00003440: 7274 795f 7061 7468 3a20 5072 6f70 6572  rty_path: Proper
+00003450: 7479 2070 6174 6820 746f 2066 696e 642e  ty path to find.
+00003460: 2069 653a 2022 7573 6572 2e6e 616d 6522   ie: "user.name"
+00003470: 206f 7220 2275 7365 7273 2e30 2e6e 616d   or "users.0.nam
+00003480: 6522 0a0a 2020 2020 2020 2020 5265 7475  e"..        Retu
+00003490: 726e 3a0a 2020 2020 2020 2020 2020 2020  rn:.            
+000034a0: 7468 6520 7072 6f70 6572 7479 2076 616c  the property val
+000034b0: 7565 2069 6620 6578 6973 7473 2e0a 0a20  ue if exists... 
+000034c0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
+000034d0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
+000034e0: 4572 726f 723a 2049 6620 7072 6f70 6572  Error: If proper
+000034f0: 7479 2076 616c 7565 2064 6f65 736e 2774  ty value doesn't
+00003500: 2065 7869 7374 206f 7220 6861 7320 696e   exist or has in
+00003510: 636f 7272 6563 7420 666f 726d 6174 0a20  correct format. 
+00003520: 2020 2020 2020 2029 0272 2d00 0000 7245         ).r-...rE
+00003530: 0000 0072 4600 0000 723c 0000 0072 3c00  ...rF...r<...r<.
+00003540: 0000 723d 0000 00da 1b67 6574 5f65 6e74  ..r=.....get_ent
+00003550: 6974 795f 7072 6f70 6572 7479 5f61 735f  ity_property_as_
+00003560: 6461 7465 d301 0000 7302 0000 0000 0f7a  date....s......z
+00003570: 2850 726f 6365 7373 5574 696c 732e 6765  (ProcessUtils.ge
+00003580: 745f 656e 7469 7479 5f70 726f 7065 7274  t_entity_propert
+00003590: 795f 6173 5f64 6174 6563 0200 0000 0000  y_as_datec......
+000035a0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000035b0: 0000 730e 0000 0074 0074 017c 0083 017c  ..s....t.t.|...|
+000035c0: 0183 0253 0029 0161 7101 0000 0a20 2020  ...S.).aq....   
+000035d0: 2020 2020 2054 7279 2074 6f20 6669 6e64       Try to find
+000035e0: 2061 206a 736f 6e20 7072 6f70 6572 7479   a json property
+000035f0: 2061 7320 2264 6174 6522 2066 6f6c 6c6f   as "date" follo
+00003600: 7769 6e67 2074 6865 2022 7072 6f70 6572  wing the "proper
+00003610: 7479 5061 7468 2220 7061 7373 6564 2e0a  tyPath" passed..
+00003620: 0a20 2020 2020 2020 2041 7267 756d 656e  .        Argumen
+00003630: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00003640: 7072 6f63 6573 733a 2054 6865 2070 726f  process: The pro
+00003650: 6365 7373 2e0a 2020 2020 2020 2020 2020  cess..          
+00003660: 2020 7072 6f70 6572 7479 5f70 6174 683a    property_path:
+00003670: 2050 726f 7065 7274 7920 7061 7468 2074   Property path t
+00003680: 6f20 6669 6e64 2e20 6965 3a20 2275 7365  o find. ie: "use
+00003690: 722e 6e61 6d65 2220 6f72 2022 7573 6572  r.name" or "user
+000036a0: 732e 302e 6e61 6d65 220a 0a20 2020 2020  s.0.name"..     
+000036b0: 2020 2052 6574 7572 6e3a 0a20 2020 2020     Return:.     
+000036c0: 2020 2020 2020 2054 6865 2070 726f 7065         The prope
+000036d0: 7274 7920 7661 6c75 6520 6966 2065 7869  rty value if exi
+000036e0: 7374 732e 0a0a 2020 2020 2020 2020 5261  sts...        Ra
+000036f0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+00003700: 2020 5661 6c75 6545 7272 6f72 3a20 4966    ValueError: If
+00003710: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
+00003720: 6861 7320 696e 636f 7272 6563 7420 666f  has incorrect fo
+00003730: 726d 6174 0a20 2020 2020 2020 2029 0272  rmat.        ).r
+00003740: 2400 0000 7245 0000 0072 4600 0000 723c  $...rE...rF...r<
+00003750: 0000 0072 3c00 0000 723d 0000 00da 1c66  ...r<...r=.....f
+00003760: 696e 645f 656e 7469 7479 5f70 726f 7065  ind_entity_prope
+00003770: 7274 795f 6173 5f64 6174 65e4 0100 0073  rty_as_date....s
+00003780: 0200 0000 000f 7a29 5072 6f63 6573 7355  ......z)ProcessU
+00003790: 7469 6c73 2e66 696e 645f 656e 7469 7479  tils.find_entity
+000037a0: 5f70 726f 7065 7274 795f 6173 5f64 6174  _property_as_dat
+000037b0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+000037c0: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
+000037d0: 0074 017c 0083 017c 0183 0253 0029 0161  .t.|...|...S.).a
+000037e0: 7e01 0000 0a20 2020 2020 2020 2047 6574  ~....        Get
+000037f0: 2061 206a 736f 6e20 7072 6f70 6572 7479   a json property
+00003800: 2061 7320 2264 6174 6574 696d 6522 2066   as "datetime" f
+00003810: 6f6c 6c6f 7769 6e67 2074 6865 2022 7072  ollowing the "pr
+00003820: 6f70 6572 7479 5061 7468 2220 7061 7373  opertyPath" pass
+00003830: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
+00003840: 756d 656e 7473 3a0a 2020 2020 2020 2020  uments:.        
+00003850: 2020 2020 7072 6f63 6573 733a 2054 6865      process: The
+00003860: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
+00003870: 2020 2020 2020 7072 6f70 6572 7479 5f70        property_p
+00003880: 6174 683a 2050 726f 7065 7274 7920 7061  ath: Property pa
+00003890: 7468 2074 6f20 6669 6e64 2e20 6965 3a20  th to find. ie: 
+000038a0: 2275 7365 722e 6e61 6d65 2220 6f72 2022  "user.name" or "
+000038b0: 7573 6572 732e 302e 6e61 6d65 220a 0a20  users.0.name".. 
+000038c0: 2020 2020 2020 2052 6574 7572 6e3a 0a20         Return:. 
+000038d0: 2020 2020 2020 2020 2020 2074 6865 2070             the p
+000038e0: 726f 7065 7274 7920 7661 6c75 6520 6966  roperty value if
+000038f0: 2065 7869 7374 732e 0a0a 2020 2020 2020   exists...      
+00003900: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00003910: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+00003920: 3a20 4966 2070 726f 7065 7274 7920 7661  : If property va
+00003930: 6c75 6520 646f 6573 6e27 7420 6578 6973  lue doesn't exis
+00003940: 7420 6f72 2068 6173 2069 6e63 6f72 7265  t or has incorre
+00003950: 6374 2066 6f72 6d61 740a 2020 2020 2020  ct format.      
+00003960: 2020 2902 722e 0000 0072 4500 0000 7246    ).r....rE...rF
+00003970: 0000 0072 3c00 0000 723c 0000 0072 3d00  ...r<...r<...r=.
+00003980: 0000 da1f 6765 745f 656e 7469 7479 5f70  ....get_entity_p
+00003990: 726f 7065 7274 795f 6173 5f64 6174 6574  roperty_as_datet
+000039a0: 696d 65f5 0100 0073 0200 0000 000f 7a2c  ime....s......z,
+000039b0: 5072 6f63 6573 7355 7469 6c73 2e67 6574  ProcessUtils.get
+000039c0: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
+000039d0: 5f61 735f 6461 7465 7469 6d65 6302 0000  _as_datetimec...
+000039e0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+000039f0: 0043 0000 0073 0e00 0000 7400 7401 7c00  .C...s....t.t.|.
+00003a00: 8301 7c01 8302 5300 2901 6175 0100 000a  ..|...S.).au....
+00003a10: 2020 2020 2020 2020 5472 7920 746f 2066          Try to f
+00003a20: 696e 6420 6120 6a73 6f6e 2070 726f 7065  ind a json prope
+00003a30: 7274 7920 6173 2022 6461 7465 7469 6d65  rty as "datetime
+00003a40: 2220 666f 6c6c 6f77 696e 6720 7468 6520  " following the 
+00003a50: 2270 726f 7065 7274 7950 6174 6822 2070  "propertyPath" p
+00003a60: 6173 7365 642e 0a0a 2020 2020 2020 2020  assed...        
+00003a70: 4172 6775 6d65 6e74 733a 0a20 2020 2020  Arguments:.     
+00003a80: 2020 2020 2020 2070 726f 6365 7373 3a20         process: 
+00003a90: 5468 6520 7072 6f63 6573 732e 0a20 2020  The process..   
+00003aa0: 2020 2020 2020 2020 2070 726f 7065 7274           propert
+00003ab0: 795f 7061 7468 3a20 5072 6f70 6572 7479  y_path: Property
+00003ac0: 2070 6174 6820 746f 2066 696e 642e 2069   path to find. i
+00003ad0: 653a 2022 7573 6572 2e6e 616d 6522 206f  e: "user.name" o
+00003ae0: 7220 2275 7365 7273 2e30 2e6e 616d 6522  r "users.0.name"
+00003af0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00003b00: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00003b10: 6520 7072 6f70 6572 7479 2076 616c 7565  e property value
+00003b20: 2069 6620 6578 6973 7473 2e0a 0a20 2020   if exists...   
+00003b30: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+00003b40: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+00003b50: 726f 723a 2049 6620 7072 6f70 6572 7479  ror: If property
+00003b60: 2076 616c 7565 2068 6173 2069 6e63 6f72   value has incor
+00003b70: 7265 6374 2066 6f72 6d61 740a 2020 2020  rect format.    
+00003b80: 2020 2020 2902 7225 0000 0072 4500 0000      ).r%...rE...
+00003b90: 7246 0000 0072 3c00 0000 723c 0000 0072  rF...r<...r<...r
+00003ba0: 3d00 0000 da20 6669 6e64 5f65 6e74 6974  =.... find_entit
+00003bb0: 795f 7072 6f70 6572 7479 5f61 735f 6461  y_property_as_da
+00003bc0: 7465 7469 6d65 0602 0000 7302 0000 0000  tetime....s.....
+00003bd0: 0f7a 2d50 726f 6365 7373 5574 696c 732e  .z-ProcessUtils.
+00003be0: 6669 6e64 5f65 6e74 6974 795f 7072 6f70  find_entity_prop
+00003bf0: 6572 7479 5f61 735f 6461 7465 7469 6d65  erty_as_datetime
+00003c00: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00003c10: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
+00003c20: 7401 7c00 8301 7c01 8302 5300 2901 6183  t.|...|...S.).a.
+00003c30: 0100 000a 2020 2020 2020 2020 4765 7420  ....        Get 
+00003c40: 6120 6a73 6f6e 2070 726f 7065 7274 7920  a json property 
+00003c50: 6173 2022 4a73 6f6e 466f 726d 7346 696c  as "JsonFormsFil
+00003c60: 6522 2066 6f6c 6c6f 7769 6e67 2074 6865  e" following the
+00003c70: 2022 7072 6f70 6572 7479 5061 7468 2220   "propertyPath" 
+00003c80: 7061 7373 6564 2e0a 0a20 2020 2020 2020  passed...       
+00003c90: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
+00003ca0: 2020 2020 2020 2020 7072 6f63 6573 733a          process:
+00003cb0: 2054 6865 2070 726f 6365 7373 2e0a 2020   The process..  
+00003cc0: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
+00003cd0: 7479 5f70 6174 683a 2050 726f 7065 7274  ty_path: Propert
+00003ce0: 7920 7061 7468 2074 6f20 6669 6e64 2e20  y path to find. 
+00003cf0: 6965 3a20 2275 7365 722e 6e61 6d65 2220  ie: "user.name" 
+00003d00: 6f72 2022 7573 6572 732e 302e 6e61 6d65  or "users.0.name
+00003d10: 220a 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
+00003d20: 6e3a 0a20 2020 2020 2020 2020 2020 2074  n:.            t
+00003d30: 6865 2070 726f 7065 7274 7920 7661 6c75  he property valu
+00003d40: 6520 6966 2065 7869 7374 732e 0a0a 2020  e if exists...  
+00003d50: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+00003d60: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
+00003d70: 7272 6f72 3a20 4966 2070 726f 7065 7274  rror: If propert
+00003d80: 7920 7661 6c75 6520 646f 6573 6e27 7420  y value doesn't 
+00003d90: 6578 6973 7420 6f72 2068 6173 2069 6e63  exist or has inc
+00003da0: 6f72 7265 6374 2066 6f72 6d61 740a 2020  orrect format.  
+00003db0: 2020 2020 2020 2902 7232 0000 0072 4500        ).r2...rE.
+00003dc0: 0000 7246 0000 0072 3c00 0000 723c 0000  ..rF...r<...r<..
+00003dd0: 0072 3d00 0000 da1b 6765 745f 656e 7469  .r=.....get_enti
+00003de0: 7479 5f70 726f 7065 7274 795f 6173 5f66  ty_property_as_f
+00003df0: 696c 6517 0200 0073 0200 0000 000f 7a28  ile....s......z(
+00003e00: 5072 6f63 6573 7355 7469 6c73 2e67 6574  ProcessUtils.get
+00003e10: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
+00003e20: 5f61 735f 6669 6c65 6302 0000 0000 0000  _as_filec.......
+00003e30: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00003e40: 0073 0e00 0000 7400 7401 7c00 8301 7c01  .s....t.t.|...|.
+00003e50: 8302 5300 2901 617a 0100 000a 2020 2020  ..S.).az....    
+00003e60: 2020 2020 5472 7920 746f 2066 696e 6420      Try to find 
+00003e70: 6120 6a73 6f6e 2070 726f 7065 7274 7920  a json property 
+00003e80: 6173 2022 4a73 6f6e 466f 726d 7346 696c  as "JsonFormsFil
+00003e90: 6522 2066 6f6c 6c6f 7769 6e67 2074 6865  e" following the
+00003ea0: 2022 7072 6f70 6572 7479 5061 7468 2220   "propertyPath" 
+00003eb0: 7061 7373 6564 2e0a 0a20 2020 2020 2020  passed...       
+00003ec0: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
+00003ed0: 2020 2020 2020 2020 7072 6f63 6573 733a          process:
+00003ee0: 2054 6865 2070 726f 6365 7373 2e0a 2020   The process..  
+00003ef0: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
+00003f00: 7479 5f70 6174 683a 2050 726f 7065 7274  ty_path: Propert
+00003f10: 7920 7061 7468 2074 6f20 6669 6e64 2e20  y path to find. 
+00003f20: 6965 3a20 2275 7365 722e 6e61 6d65 2220  ie: "user.name" 
+00003f30: 6f72 2022 7573 6572 732e 302e 6e61 6d65  or "users.0.name
+00003f40: 220a 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
+00003f50: 6e3a 0a20 2020 2020 2020 2020 2020 2054  n:.            T
+00003f60: 6865 2070 726f 7065 7274 7920 7661 6c75  he property valu
+00003f70: 6520 6966 2065 7869 7374 732e 0a0a 2020  e if exists...  
+00003f80: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+00003f90: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
+00003fa0: 7272 6f72 3a20 4966 2070 726f 7065 7274  rror: If propert
+00003fb0: 7920 7661 6c75 6520 6861 7320 696e 636f  y value has inco
+00003fc0: 7272 6563 7420 666f 726d 6174 0a20 2020  rrect format.   
+00003fd0: 2020 2020 2029 0272 2900 0000 7245 0000       ).r)...rE..
+00003fe0: 0072 4600 0000 723c 0000 0072 3c00 0000  .rF...r<...r<...
+00003ff0: 723d 0000 00da 1c66 696e 645f 656e 7469  r=.....find_enti
+00004000: 7479 5f70 726f 7065 7274 795f 6173 5f66  ty_property_as_f
+00004010: 696c 6528 0200 0073 0200 0000 000f 7a29  ile(...s......z)
+00004020: 5072 6f63 6573 7355 7469 6c73 2e66 696e  ProcessUtils.fin
+00004030: 645f 656e 7469 7479 5f70 726f 7065 7274  d_entity_propert
+00004040: 795f 6173 5f66 696c 6563 0200 0000 0000  y_as_filec......
+00004050: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00004060: 0000 730e 0000 0074 0074 017c 0083 017c  ..s....t.t.|...|
+00004070: 0183 0253 0029 0161 8801 0000 0a20 2020  ...S.).a.....   
+00004080: 2020 2020 2047 6574 2061 206a 736f 6e20       Get a json 
+00004090: 7072 6f70 6572 7479 2061 7320 224a 736f  property as "Jso
+000040a0: 6e46 6f72 6d73 5072 696e 6369 7061 6c22  nFormsPrincipal"
+000040b0: 2066 6f6c 6c6f 7769 6e67 2074 6865 2022   following the "
+000040c0: 7072 6f70 6572 7479 5061 7468 2220 7061  propertyPath" pa
+000040d0: 7373 6564 2e0a 0a20 2020 2020 2020 2041  ssed...        A
+000040e0: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
+000040f0: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
+00004100: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
+00004110: 2020 2020 2020 2020 7072 6f70 6572 7479          property
+00004120: 5f70 6174 683a 2050 726f 7065 7274 7920  _path: Property 
+00004130: 7061 7468 2074 6f20 6669 6e64 2e20 6965  path to find. ie
+00004140: 3a20 2275 7365 722e 6e61 6d65 2220 6f72  : "user.name" or
+00004150: 2022 7573 6572 732e 302e 6e61 6d65 220a   "users.0.name".
+00004160: 0a20 2020 2020 2020 2052 6574 7572 6e3a  .        Return:
+00004170: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00004180: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
+00004190: 6966 2065 7869 7374 732e 0a0a 2020 2020  if exists...    
+000041a0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+000041b0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+000041c0: 6f72 3a20 4966 2070 726f 7065 7274 7920  or: If property 
+000041d0: 7661 6c75 6520 646f 6573 6e27 7420 6578  value doesn't ex
+000041e0: 6973 7420 6f72 2068 6173 2069 6e63 6f72  ist or has incor
+000041f0: 7265 6374 2066 6f72 6d61 740a 2020 2020  rect format.    
+00004200: 2020 2020 2902 7233 0000 0072 4500 0000      ).r3...rE...
+00004210: 7246 0000 0072 3c00 0000 723c 0000 0072  rF...r<...r<...r
+00004220: 3d00 0000 da20 6765 745f 656e 7469 7479  =.... get_entity
+00004230: 5f70 726f 7065 7274 795f 6173 5f70 7269  _property_as_pri
+00004240: 6e63 6970 616c 3902 0000 7302 0000 0000  ncipal9...s.....
+00004250: 0f7a 2d50 726f 6365 7373 5574 696c 732e  .z-ProcessUtils.
+00004260: 6765 745f 656e 7469 7479 5f70 726f 7065  get_entity_prope
+00004270: 7274 795f 6173 5f70 7269 6e63 6970 616c  rty_as_principal
+00004280: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00004290: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
+000042a0: 7401 7c00 8301 7c01 8302 5300 2901 617f  t.|...|...S.).a.
+000042b0: 0100 000a 2020 2020 2020 2020 5472 7920  ....        Try 
+000042c0: 746f 2066 696e 6420 6120 6a73 6f6e 2070  to find a json p
+000042d0: 726f 7065 7274 7920 6173 2022 4a73 6f6e  roperty as "Json
+000042e0: 466f 726d 7350 7269 6e63 6970 616c 2220  FormsPrincipal" 
+000042f0: 666f 6c6c 6f77 696e 6720 7468 6520 2270  following the "p
+00004300: 726f 7065 7274 7950 6174 6822 2070 6173  ropertyPath" pas
+00004310: 7365 642e 0a0a 2020 2020 2020 2020 4172  sed...        Ar
+00004320: 6775 6d65 6e74 733a 0a20 2020 2020 2020  guments:.       
+00004330: 2020 2020 2070 726f 6365 7373 3a20 5468       process: Th
+00004340: 6520 7072 6f63 6573 732e 0a20 2020 2020  e process..     
+00004350: 2020 2020 2020 2070 726f 7065 7274 795f         property_
+00004360: 7061 7468 3a20 5072 6f70 6572 7479 2070  path: Property p
+00004370: 6174 6820 746f 2066 696e 642e 2069 653a  ath to find. ie:
+00004380: 2022 7573 6572 2e6e 616d 6522 206f 7220   "user.name" or 
+00004390: 2275 7365 7273 2e30 2e6e 616d 6522 0a0a  "users.0.name"..
+000043a0: 2020 2020 2020 2020 5265 7475 726e 3a0a          Return:.
+000043b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000043c0: 7072 6f70 6572 7479 2076 616c 7565 2069  property value i
+000043d0: 6620 6578 6973 7473 2e0a 0a20 2020 2020  f exists...     
+000043e0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+000043f0: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
+00004400: 723a 2049 6620 7072 6f70 6572 7479 2076  r: If property v
+00004410: 616c 7565 2068 6173 2069 6e63 6f72 7265  alue has incorre
+00004420: 6374 2066 6f72 6d61 740a 2020 2020 2020  ct format.      
+00004430: 2020 2902 722a 0000 0072 4500 0000 7246    ).r*...rE...rF
+00004440: 0000 0072 3c00 0000 723c 0000 0072 3d00  ...r<...r<...r=.
+00004450: 0000 da21 6669 6e64 5f65 6e74 6974 795f  ...!find_entity_
+00004460: 7072 6f70 6572 7479 5f61 735f 7072 696e  property_as_prin
+00004470: 6369 7061 6c4a 0200 0073 0200 0000 000f  cipalJ...s......
+00004480: 7a2e 5072 6f63 6573 7355 7469 6c73 2e66  z.ProcessUtils.f
+00004490: 696e 645f 656e 7469 7479 5f70 726f 7065  ind_entity_prope
+000044a0: 7274 795f 6173 5f70 7269 6e63 6970 616c  rty_as_principal
+000044b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000044c0: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
+000044d0: 7401 7c00 8301 7c01 8302 5300 2901 617a  t.|...|...S.).az
+000044e0: 0100 000a 2020 2020 2020 2020 4765 7420  ....        Get 
+000044f0: 6120 6a73 6f6e 2070 726f 7065 7274 7920  a json property 
+00004500: 6173 2022 6c69 7374 2220 666f 6c6c 6f77  as "list" follow
+00004510: 696e 6720 7468 6520 2270 726f 7065 7274  ing the "propert
+00004520: 7950 6174 6822 2070 6173 7365 642e 0a0a  yPath" passed...
+00004530: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
+00004540: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00004550: 726f 6365 7373 3a20 5468 6520 7072 6f63  rocess: The proc
+00004560: 6573 732e 0a20 2020 2020 2020 2020 2020  ess..           
+00004570: 2070 726f 7065 7274 795f 7061 7468 3a20   property_path: 
+00004580: 5072 6f70 6572 7479 2070 6174 6820 746f  Property path to
+00004590: 2066 696e 642e 2069 653a 2022 7573 6572   find. ie: "user
+000045a0: 2e6e 616d 6522 206f 7220 2275 7365 7273  .name" or "users
+000045b0: 2e30 2e6e 616d 6522 0a0a 2020 2020 2020  .0.name"..      
+000045c0: 2020 5265 7475 726e 3a0a 2020 2020 2020    Return:.      
+000045d0: 2020 2020 2020 7468 6520 7072 6f70 6572        the proper
+000045e0: 7479 2076 616c 7565 2069 6620 6578 6973  ty value if exis
+000045f0: 7473 2e0a 0a20 2020 2020 2020 2052 6169  ts...        Rai
+00004600: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00004610: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
+00004620: 7072 6f70 6572 7479 2076 616c 7565 2064  property value d
+00004630: 6f65 736e 2774 2065 7869 7374 206f 7220  oesn't exist or 
+00004640: 6861 7320 696e 636f 7272 6563 7420 666f  has incorrect fo
+00004650: 726d 6174 0a20 2020 2020 2020 2029 0272  rmat.        ).r
+00004660: 3400 0000 7245 0000 0072 4600 0000 723c  4...rE...rF...r<
+00004670: 0000 0072 3c00 0000 723d 0000 00da 1b67  ...r<...r=.....g
+00004680: 6574 5f65 6e74 6974 795f 7072 6f70 6572  et_entity_proper
+00004690: 7479 5f61 735f 6c69 7374 5b02 0000 7302  ty_as_list[...s.
+000046a0: 0000 0000 0f7a 2850 726f 6365 7373 5574  .....z(ProcessUt
+000046b0: 696c 732e 6765 745f 656e 7469 7479 5f70  ils.get_entity_p
+000046c0: 726f 7065 7274 795f 6173 5f6c 6973 7463  roperty_as_listc
+000046d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000046e0: 0300 0000 4300 0000 730e 0000 0074 0074  ....C...s....t.t
+000046f0: 017c 0083 017c 0183 0253 0029 0161 7101  .|...|...S.).aq.
+00004700: 0000 0a20 2020 2020 2020 2054 7279 2074  ...        Try t
+00004710: 6f20 6669 6e64 2061 206a 736f 6e20 7072  o find a json pr
+00004720: 6f70 6572 7479 2061 7320 226c 6973 7422  operty as "list"
+00004730: 2066 6f6c 6c6f 7769 6e67 2074 6865 2022   following the "
+00004740: 7072 6f70 6572 7479 5061 7468 2220 7061  propertyPath" pa
+00004750: 7373 6564 2e0a 0a20 2020 2020 2020 2041  ssed...        A
+00004760: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
+00004770: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
+00004780: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
+00004790: 2020 2020 2020 2020 7072 6f70 6572 7479          property
+000047a0: 5f70 6174 683a 2050 726f 7065 7274 7920  _path: Property 
+000047b0: 7061 7468 2074 6f20 6669 6e64 2e20 6965  path to find. ie
+000047c0: 3a20 2275 7365 722e 6e61 6d65 2220 6f72  : "user.name" or
+000047d0: 2022 7573 6572 732e 302e 6e61 6d65 220a   "users.0.name".
+000047e0: 0a20 2020 2020 2020 2052 6574 7572 6e3a  .        Return:
+000047f0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00004800: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
+00004810: 6966 2065 7869 7374 732e 0a0a 2020 2020  if exists...    
+00004820: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00004830: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+00004840: 6f72 3a20 4966 2070 726f 7065 7274 7920  or: If property 
+00004850: 7661 6c75 6520 6861 7320 696e 636f 7272  value has incorr
+00004860: 6563 7420 666f 726d 6174 0a20 2020 2020  ect format.     
+00004870: 2020 2029 0272 2b00 0000 7245 0000 0072     ).r+...rE...r
+00004880: 4600 0000 723c 0000 0072 3c00 0000 723d  F...r<...r<...r=
+00004890: 0000 00da 1c66 696e 645f 656e 7469 7479  .....find_entity
+000048a0: 5f70 726f 7065 7274 795f 6173 5f6c 6973  _property_as_lis
+000048b0: 746c 0200 0073 0200 0000 000f 7a29 5072  tl...s......z)Pr
+000048c0: 6f63 6573 7355 7469 6c73 2e66 696e 645f  ocessUtils.find_
+000048d0: 656e 7469 7479 5f70 726f 7065 7274 795f  entity_property_
+000048e0: 6173 5f6c 6973 7463 0200 0000 0000 0000  as_listc........
+000048f0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00004900: 730e 0000 0074 0074 017c 0083 017c 0183  s....t.t.|...|..
+00004910: 0253 0029 0161 7a01 0000 0a20 2020 2020  .S.).az....     
+00004920: 2020 2047 6574 2061 206a 736f 6e20 7072     Get a json pr
+00004930: 6f70 6572 7479 2061 7320 2264 6963 7422  operty as "dict"
+00004940: 2066 6f6c 6c6f 7769 6e67 2074 6865 2022   following the "
+00004950: 7072 6f70 6572 7479 5061 7468 2220 7061  propertyPath" pa
+00004960: 7373 6564 2e0a 0a20 2020 2020 2020 2041  ssed...        A
+00004970: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
+00004980: 2020 2020 2020 7072 6f63 6573 733a 2054        process: T
+00004990: 6865 2070 726f 6365 7373 2e0a 2020 2020  he process..    
+000049a0: 2020 2020 2020 2020 7072 6f70 6572 7479          property
+000049b0: 5f70 6174 683a 2050 726f 7065 7274 7920  _path: Property 
+000049c0: 7061 7468 2074 6f20 6669 6e64 2e20 6965  path to find. ie
+000049d0: 3a20 2275 7365 722e 6e61 6d65 2220 6f72  : "user.name" or
+000049e0: 2022 7573 6572 732e 302e 6e61 6d65 220a   "users.0.name".
+000049f0: 0a20 2020 2020 2020 2052 6574 7572 6e3a  .        Return:
+00004a00: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00004a10: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
+00004a20: 6966 2065 7869 7374 732e 0a0a 2020 2020  if exists...    
+00004a30: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00004a40: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+00004a50: 6f72 3a20 4966 2070 726f 7065 7274 7920  or: If property 
+00004a60: 7661 6c75 6520 646f 6573 6e27 7420 6578  value doesn't ex
+00004a70: 6973 7420 6f72 2068 6173 2069 6e63 6f72  ist or has incor
+00004a80: 7265 6374 2066 6f72 6d61 740a 2020 2020  rect format.    
+00004a90: 2020 2020 2902 722f 0000 0072 4500 0000      ).r/...rE...
+00004aa0: 7246 0000 0072 3c00 0000 723c 0000 0072  rF...r<...r<...r
+00004ab0: 3d00 0000 da1b 6765 745f 656e 7469 7479  =.....get_entity
+00004ac0: 5f70 726f 7065 7274 795f 6173 5f64 6963  _property_as_dic
+00004ad0: 747d 0200 0073 0200 0000 000f 7a28 5072  t}...s......z(Pr
+00004ae0: 6f63 6573 7355 7469 6c73 2e67 6574 5f65  ocessUtils.get_e
+00004af0: 6e74 6974 795f 7072 6f70 6572 7479 5f61  ntity_property_a
+00004b00: 735f 6469 6374 6302 0000 0000 0000 0000  s_dictc.........
+00004b10: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00004b20: 0e00 0000 7400 7401 7c00 8301 7c01 8302  ....t.t.|...|...
+00004b30: 5300 2901 6171 0100 000a 2020 2020 2020  S.).aq....      
+00004b40: 2020 5472 7920 746f 2066 696e 6420 6120    Try to find a 
+00004b50: 6a73 6f6e 2070 726f 7065 7274 7920 6173  json property as
+00004b60: 2022 6469 6374 2220 666f 6c6c 6f77 696e   "dict" followin
+00004b70: 6720 7468 6520 2270 726f 7065 7274 7950  g the "propertyP
+00004b80: 6174 6822 2070 6173 7365 642e 0a0a 2020  ath" passed...  
+00004b90: 2020 2020 2020 4172 6775 6d65 6e74 733a        Arguments:
+00004ba0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00004bb0: 6365 7373 3a20 5468 6520 7072 6f63 6573  cess: The proces
+00004bc0: 732e 0a20 2020 2020 2020 2020 2020 2070  s..            p
+00004bd0: 726f 7065 7274 795f 7061 7468 3a20 5072  roperty_path: Pr
+00004be0: 6f70 6572 7479 2070 6174 6820 746f 2066  operty path to f
+00004bf0: 696e 642e 2069 653a 2022 7573 6572 2e6e  ind. ie: "user.n
+00004c00: 616d 6522 206f 7220 2275 7365 7273 2e30  ame" or "users.0
+00004c10: 2e6e 616d 6522 0a0a 2020 2020 2020 2020  .name"..        
+00004c20: 5265 7475 726e 3a0a 2020 2020 2020 2020  Return:.        
+00004c30: 2020 2020 5468 6520 7072 6f70 6572 7479      The property
+00004c40: 2076 616c 7565 2069 6620 6578 6973 7473   value if exists
+00004c50: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00004c60: 733a 0a20 2020 2020 2020 2020 2020 2056  s:.            V
+00004c70: 616c 7565 4572 726f 723a 2049 6620 7072  alueError: If pr
+00004c80: 6f70 6572 7479 2076 616c 7565 2068 6173  operty value has
+00004c90: 2069 6e63 6f72 7265 6374 2066 6f72 6d61   incorrect forma
+00004ca0: 740a 2020 2020 2020 2020 2902 7226 0000  t.        ).r&..
+00004cb0: 0072 4500 0000 7246 0000 0072 3c00 0000  .rE...rF...r<...
+00004cc0: 723c 0000 0072 3d00 0000 da1c 6669 6e64  r<...r=.....find
+00004cd0: 5f65 6e74 6974 795f 7072 6f70 6572 7479  _entity_property
+00004ce0: 5f61 735f 6469 6374 8e02 0000 7302 0000  _as_dict....s...
+00004cf0: 0000 0f7a 2950 726f 6365 7373 5574 696c  ...z)ProcessUtil
+00004d00: 732e 6669 6e64 5f65 6e74 6974 795f 7072  s.find_entity_pr
+00004d10: 6f70 6572 7479 5f61 735f 6469 6374 2901  operty_as_dict).
+00004d20: 4e29 014e 2901 4e29 014e 2935 da08 5f5f  N).N).N).N)5..__
+00004d30: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00004d40: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00004d50: da0c 7374 6174 6963 6d65 7468 6f64 720d  ..staticmethodr.
+00004d60: 0000 00da 0373 7472 da04 626f 6f6c 721d  .....str..boolr.
+00004d70: 0000 00da 0369 6e74 721e 0000 0072 0700  .....intr....r..
+00004d80: 0000 7221 0000 0072 2200 0000 720f 0000  ..r!...r"...r...
+00004d90: 0072 1f00 0000 7206 0000 0072 2000 0000  .r....r....r ...
+00004da0: 7212 0000 0072 1300 0000 721b 0000 0072  r....r....r....r
+00004db0: 1600 0000 721c 0000 00da 0566 6c6f 6174  ....r......float
+00004dc0: 7219 0000 0072 1500 0000 721a 0000 0072  r....r....r....r
+00004dd0: 0200 0000 7217 0000 0072 1400 0000 7218  ....r....r....r.
+00004de0: 0000 0072 4700 0000 7248 0000 0072 4900  ...rG...rH...rI.
+00004df0: 0000 724a 0000 0072 4b00 0000 724c 0000  ..rJ...rK...rL..
+00004e00: 0072 4d00 0000 724e 0000 0072 0300 0000  .rM...rN...r....
+00004e10: 724f 0000 0072 5000 0000 720a 0000 0072  rO...rP...r....r
+00004e20: 5100 0000 7252 0000 0072 0b00 0000 7253  Q...rR...r....rS
+00004e30: 0000 0072 5400 0000 da04 6c69 7374 7255  ...rT.....listrU
+00004e40: 0000 0072 5600 0000 da04 6469 6374 7257  ...rV.....dictrW
+00004e50: 0000 0072 5800 0000 723c 0000 0072 3c00  ...rX...r<...r<.
+00004e60: 0000 723c 0000 0072 3d00 0000 7236 0000  ..r<...r=...r6..
+00004e70: 004b 0000 0073 ce00 0000 0801 0201 140d  .K...s..........
+00004e80: 0202 0201 0201 0201 02fc 0e12 0201 1a10  ................
+00004e90: 0202 0201 0201 0601 0201 02fb 0e16 0204  ................
+00004ea0: 00fd 0201 0201 0201 0601 02fc 0e14 0204  ................
+00004eb0: 00fd 0201 0201 0201 0a01 02fc 0e17 0204  ................
+00004ec0: 00fd 0201 0201 0201 0601 02fc 0e14 0204  ................
+00004ed0: 00fd 0201 0201 0201 0a01 02fc 0e17 0201  ................
+00004ee0: 140d 0201 180d 0201 180d 0201 140d 0201  ................
+00004ef0: 140d 0201 180d 0201 140d 0201 180d 0201  ................
+00004f00: 180d 0201 1410 0201 1810 0201 1410 0201  ................
+00004f10: 1810 0201 1410 0201 1810 0201 1410 0201  ................
+00004f20: 1810 0201 1410 0201 1810 0201 1410 0201  ................
+00004f30: 1810 0201 1410 0201 1810 0201 1410 0201  ................
+00004f40: 1810 0201 1410 0201 7236 0000 0063 0000  ........r6...c..
+00004f50: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00004f60: 0000 4000 0000 7340 0000 0065 005a 0164  ..@...s@...e.Z.d
+00004f70: 005a 0265 0365 0464 019c 0264 0264 0384  .Z.e.e.d...d.d..
+00004f80: 045a 0565 0665 0719 0064 049c 0164 0564  .Z.e.e...d...d.d
+00004f90: 0684 045a 0865 0665 0919 0064 079c 0164  ...Z.e.e...d...d
+00004fa0: 0864 0984 045a 0a64 0a53 0029 0b72 3a00  .d...Z.d.S.).r:.
+00004fb0: 0000 723b 0000 0063 0300 0000 0000 0000  ..r;...c........
+00004fc0: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+00004fd0: 7310 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
+00004fe0: 0164 0053 00a9 014e 723b 0000 0029 03da  .d.S...Nr;...)..
+00004ff0: 0473 656c 6672 3700 0000 7238 0000 0072  .selfr7...r8...r
+00005000: 3c00 0000 723c 0000 0072 3d00 0000 da08  <...r<...r=.....
+00005010: 5f5f 696e 6974 5f5f a102 0000 7304 0000  __init__....s...
+00005020: 0000 0106 017a 2443 7572 7265 6e74 456c  .....z$CurrentEl
+00005030: 656d 656e 7456 616c 7565 4163 6365 7373  ementValueAccess
+00005040: 6f72 2e5f 5f69 6e69 745f 5f29 0172 4200  or.__init__).rB.
+00005050: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00005060: 0000 0004 0000 0043 0000 0073 4600 0000  .......C...sF...
+00005070: 7c00 6a00 6a01 6400 6b08 7214 6900 7c00  |.j.j.d.k.r.i.|.
+00005080: 6a00 5f01 7402 7c01 8301 6401 6b02 7234  j._.t.|...d.k.r4
+00005090: 7c00 6a00 6a01 a003 7c00 6a04 6400 a102  |.j.j...|.j.d...
+000050a0: 0100 6e0e 7c01 7c00 6a00 6a01 7c00 6a04  ..n.|.|.j.j.|.j.
+000050b0: 3c00 6400 5300 a902 4e72 0100 0000 2905  <.d.S...Nr....).
+000050c0: 7237 0000 0072 4200 0000 da03 6c65 6eda  r7...rB.....len.
+000050d0: 0370 6f70 7238 0000 0029 0272 6400 0000  .popr8...).rd...
+000050e0: 7242 0000 0072 3c00 0000 723c 0000 0072  rB...r<...r<...r
+000050f0: 3d00 0000 da12 7365 745f 656c 656d 656e  =.....set_elemen
+00005100: 745f 7661 6c75 6573 a502 0000 730a 0000  t_values....s...
+00005110: 0000 010c 0108 020c 0114 027a 2e43 7572  ...........z.Cur
+00005120: 7265 6e74 456c 656d 656e 7456 616c 7565  rentElementValue
+00005130: 4163 6365 7373 6f72 2e73 6574 5f65 6c65  Accessor.set_ele
+00005140: 6d65 6e74 5f76 616c 7565 73a9 0172 3900  ment_values..r9.
+00005150: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00005160: 0000 0003 0000 0043 0000 0073 3c00 0000  .......C...s<...
+00005170: 7c00 6a00 6a01 6400 6b08 7210 6700 5300  |.j.j.d.k.r.g.S.
+00005180: 7c00 6a00 6a01 a002 7c00 6a03 a101 7d01  |.j.j...|.j...}.
+00005190: 7c01 6400 6b08 7334 7404 7c01 8301 6401  |.d.k.s4t.|...d.
+000051a0: 6b02 7238 6700 5300 7c01 5300 7266 0000  k.r8g.S.|.S.rf..
+000051b0: 0029 0572 3700 0000 7242 0000 00da 0367  .).r7...rB.....g
+000051c0: 6574 7238 0000 0072 6700 0000 2902 7264  etr8...rg...).rd
+000051d0: 0000 00da 1665 6c65 6d65 6e74 5f76 616c  .....element_val
+000051e0: 7565 735f 6279 5f63 6f64 6572 3c00 0000  ues_by_coder<...
+000051f0: 723c 0000 0072 3d00 0000 da12 6765 745f  r<...r=.....get_
+00005200: 656c 656d 656e 745f 7661 6c75 6573 ae02  element_values..
+00005210: 0000 730c 0000 0000 010c 0104 0210 0114  ..s.............
+00005220: 0104 027a 2e43 7572 7265 6e74 456c 656d  ...z.CurrentElem
+00005230: 656e 7456 616c 7565 4163 6365 7373 6f72  entValueAccessor
+00005240: 2e67 6574 5f65 6c65 6d65 6e74 5f76 616c  .get_element_val
+00005250: 7565 734e 290b 7259 0000 0072 5a00 0000  uesN).rY...rZ...
+00005260: 725b 0000 0072 0d00 0000 725d 0000 0072  r[...r....r]...r
+00005270: 6500 0000 7206 0000 0072 1000 0000 7269  e...r....r....ri
+00005280: 0000 0072 0900 0000 726d 0000 0072 3c00  ...r....rm...r<.
+00005290: 0000 723c 0000 0072 3c00 0000 723d 0000  ..r<...r<...r=..
+000052a0: 0072 3a00 0000 a002 0000 7306 0000 0008  .r:.......s.....
+000052b0: 0110 0412 0972 3a00 0000 6300 0000 0000  .....r:...c.....
+000052c0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+000052d0: 0000 0073 4e00 0000 6500 5a01 6400 5a02  ...sN...e.Z.d.Z.
+000052e0: 6503 6401 9c01 6402 6403 8404 5a04 6505  e.d...d.d...Z.e.
+000052f0: 6506 6507 6508 6602 1900 1900 6404 9c01  e.e.e.f.....d...
+00005300: 6405 6406 8404 5a09 6505 6506 6507 6508  d.d...Z.e.e.e.e.
+00005310: 6602 1900 1900 6407 9c01 6408 6409 8404  f.....d...d.d...
+00005320: 5a0a 640a 5300 290b 7245 0000 00a9 0172  Z.d.S.).rE.....r
+00005330: 3700 0000 6302 0000 0000 0000 0000 0000  7...c...........
+00005340: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00005350: 0000 7c01 7c00 5f00 6400 5300 7263 0000  ..|.|._.d.S.rc..
+00005360: 0072 6e00 0000 2902 7264 0000 0072 3700  .rn...).rd...r7.
+00005370: 0000 723c 0000 0072 3c00 0000 723d 0000  ..r<...r<...r=..
+00005380: 0072 6500 0000 ba02 0000 7302 0000 0000  .re.......s.....
+00005390: 017a 2443 7572 7265 6e74 4a73 6f6e 466f  .z$CurrentJsonFo
+000053a0: 726d 4461 7461 4163 6365 7373 6f72 2e5f  rmDataAccessor._
+000053b0: 5f69 6e69 745f 5f72 6a00 0000 6301 0000  _init__rj...c...
+000053c0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+000053d0: 0043 0000 0073 1a00 0000 7c00 6a00 6a01  .C...s....|.j.j.
+000053e0: 6400 6b08 7210 6400 5300 7c00 6a00 6a01  d.k.r.d.S.|.j.j.
+000053f0: 6a02 5300 7263 0000 0029 0372 3700 0000  j.S.rc...).r7...
+00005400: da06 656e 7469 7479 da04 6461 7461 2901  ..entity..data).
+00005410: 7264 0000 0072 3c00 0000 723c 0000 0072  rd...r<...r<...r
+00005420: 3d00 0000 da08 6765 745f 6461 7461 bd02  =.....get_data..
+00005430: 0000 7306 0000 0000 010c 0104 027a 2443  ..s..........z$C
+00005440: 7572 7265 6e74 4a73 6f6e 466f 726d 4461  urrentJsonFormDa
+00005450: 7461 4163 6365 7373 6f72 2e67 6574 5f64  taAccessor.get_d
+00005460: 6174 6129 0172 7000 0000 6302 0000 0000  ata).rp...c.....
+00005470: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00005480: 0000 0073 2400 0000 7c00 6a00 6a01 6400  ...s$...|.j.j.d.
+00005490: 6b08 7216 7402 8300 7c00 6a00 5f01 7c01  k.r.t...|.j._.|.
+000054a0: 7c00 6a00 6a01 5f03 6400 5300 7263 0000  |.j.j._.d.S.rc..
+000054b0: 0029 0472 3700 0000 726f 0000 0072 0c00  .).r7...ro...r..
+000054c0: 0000 7270 0000 0029 0272 6400 0000 7270  ..rp...).rd...rp
+000054d0: 0000 0072 3c00 0000 723c 0000 0072 3d00  ...r<...r<...r=.
+000054e0: 0000 da08 7365 745f 6461 7461 c302 0000  ....set_data....
+000054f0: 7306 0000 0000 010c 010a 027a 2443 7572  s..........z$Cur
+00005500: 7265 6e74 4a73 6f6e 466f 726d 4461 7461  rentJsonFormData
+00005510: 4163 6365 7373 6f72 2e73 6574 5f64 6174  Accessor.set_dat
+00005520: 614e 290b 7259 0000 0072 5a00 0000 725b  aN).rY...rZ...r[
+00005530: 0000 0072 0d00 0000 7265 0000 0072 0700  ...r....re...r..
+00005540: 0000 7205 0000 0072 5d00 0000 7204 0000  ..r....r]...r...
+00005550: 0072 7100 0000 7272 0000 0072 3c00 0000  .rq...rr...r<...
+00005560: 723c 0000 0072 3c00 0000 723d 0000 0072  r<...r<...r=...r
+00005570: 4500 0000 b902 0000 7306 0000 0008 010e  E.......s.......
+00005580: 031a 0672 4500 0000 4e29 3a72 0300 0000  ...rE...N):r....
+00005590: 7202 0000 00da 0674 7970 696e 6772 0400  r......typingr..
+000055a0: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+000055b0: 005a 115f 6765 6e65 7261 7465 642e 6d6f  .Z._generated.mo
+000055c0: 6465 6c73 7209 0000 00da 066d 6f64 656c  delsr......model
+000055d0: 7372 0a00 0000 720b 0000 0072 0c00 0000  sr....r....r....
+000055e0: 720d 0000 0072 4200 0000 720f 0000 0072  r....rB...r....r
+000055f0: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00005600: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
+00005610: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00005620: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00005630: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00005640: 2000 0000 7221 0000 0072 2200 0000 5a0a   ...r!...r"...Z.
+00005650: 6a73 6f6e 5f66 6f72 6d73 7223 0000 0072  json_formsr#...r
+00005660: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+00005670: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00005680: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00005690: 0072 2e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+000056a0: 7231 0000 0072 3200 0000 7233 0000 0072  r1...r2...r3...r
+000056b0: 3400 0000 7235 0000 0072 3600 0000 723a  4...r5...r6...r:
+000056c0: 0000 0072 4500 0000 723c 0000 0072 3c00  ...rE...r<...r<.
+000056d0: 0000 723c 0000 0072 3d00 0000 da08 3c6d  ..r<...r=.....<m
+000056e0: 6f64 756c 653e 1900 0000 7318 0000 0010  odule>....s.....
+000056f0: 0118 020c 0118 0158 1654 170e 7f00 7f00  .......X.T......
+00005700: 7f00 7f00 5910 19                        ....Y..
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_page_item_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_page_item_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 18454 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 1648 0000  U........*.f.H..
+00000000: 550d 0d0a 0000 0000 5143 2a66 1648 0000  U.......QC*f.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6406 6407 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_save_element_command_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_save_element_command_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 16414 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 1e40 0000  U........*.f.@..
+00000000: 550d 0d0a 0000 0000 5143 2a66 1e40 0000  U.......QC*f.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6406 6407 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_save_json_forms_value_data_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_save_json_forms_value_data_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 15395 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 233c 0000  U........*.f#<..
+00000000: 550d 0d0a 0000 0000 5143 2a66 233c 0000  U.......QC*f#<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d00 5a00 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6403 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6405 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_task_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_task_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 29410 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 e272 0000  U........*.f.r..
+00000000: 550d 0d0a 0000 0000 5143 2a66 e272 0000  U.......QC*f.r..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e01 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 6d01 5a01 6d00 5a00 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6403 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/_tenant_user_utils.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/_tenant_user_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 14671 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 4f39 0000  U........*.fO9..
+00000000: 550d 0d0a 0000 0000 5143 2a66 4f39 0000  U.......QC*fO9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d00 5a00 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6403 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6405 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/element_values.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/element_values.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 18912 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 e049 0000  U........*.f.I..
+00000000: 550d 0d0a 0000 0000 5143 2a66 e049 0000  U.......QC*f.I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 5c03 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/__pycache__/json_forms.cpython-38.pyc` & `kuflow_rest-1.5.1/kuflow_rest/utils/__pycache__/json_forms.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  9 11:44:28 2024 UTC, .py size: 23944 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1c2a 1566 885d 0000  U........*.f.]..
+00000000: 550d 0d0a 0000 0000 5143 2a66 885d 0000  U.......QC*f.]..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 4403 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6405 6406 6c0d  m.Z.m.Z...d.d.l.
@@ -1078,15 +1078,15 @@
 00004350: 0000 0072 7900 0000 da03 6162 6372 0200  ...ry.....abcr..
 00004360: 0000 7203 0000 0072 0500 0000 7204 0000  ..r....r....r...
 00004370: 00da 0674 7970 696e 6772 0600 0000 7207  ...typingr....r.
 00004380: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
 00004390: 0000 da06 6d6f 6465 6c73 720c 0000 0072  ....modelsr....r
 000043a0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
 000043b0: 0000 0072 1100 0000 7221 0000 0072 3500  ...r....r!...r5.
-000043c0: 0000 723a 0000 0072 6600 0000 da13 4a73  ..r:...rf.....Js
+000043c0: 0000 723a 0000 0072 6600 0000 5a13 4a73  ..r:...rf...Z.Js
 000043d0: 6f6e 466f 726d 7353 696d 706c 6554 7970  onFormsSimpleTyp
 000043e0: 655a 1243 6f6e 7461 696e 6572 4172 7261  eZ.ContainerArra
 000043f0: 7954 7970 655a 1343 6f6e 7461 696e 6572  yTypeZ.Container
 00004400: 5265 636f 7264 5479 7065 7228 0000 0072  RecordTyper(...r
 00004410: 1200 0000 5a0f 4a73 6f6e 466f 726d 734d  ....Z.JsonFormsM
 00004420: 6f64 656c 7372 1300 0000 7222 0000 0072  odelsr....r"...r
 00004430: 2f00 0000 722c 0000 0072 3200 0000 7231  /...r,...r2...r1
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_process_page_item_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_process_page_item_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_process_save_element_command_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_process_save_element_command_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_process_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_process_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     set_element_value,
     set_element_value_list,
     set_element_value_valid,
     set_element_value_valid_at,
 )
 from .json_forms import (
     JsonFormDataAccessor,
-    JsonFormsSimpleType,
     find_json_forms_property_as_date,
     find_json_forms_property_as_datetime,
     find_json_forms_property_as_dict,
     find_json_forms_property_as_float,
     find_json_forms_property_as_int,
     find_json_forms_property_as_json_forms_file,
     find_json_forms_property_as_json_forms_principal,
@@ -66,15 +65,14 @@
     get_json_forms_property_as_dict,
     get_json_forms_property_as_float,
     get_json_forms_property_as_int,
     get_json_forms_property_as_json_forms_file,
     get_json_forms_property_as_json_forms_principal,
     get_json_forms_property_as_list,
     get_json_forms_property_as_str,
-    update_json_forms_property,
 )
 
 
 class ProcessUtils:
     @staticmethod
     def get_element_value_valid(process: Process, element_definition_code: str) -> bool:
         """
@@ -666,29 +664,14 @@
             The property value if exists.
 
         Raises:
             ValueError: If property value has incorrect format
         """
         return find_json_forms_property_as_dict(CurrentJsonFormDataAccessor(process), property_path)
 
-    @staticmethod
-    def update_entity_property(process: Process, property_path: str, value: Optional[JsonFormsSimpleType]) -> None:
-        """
-        Update a json forms data property in the task passed following the "property_path".
-
-        Arguments:
-            process: The process.
-            property_path: Property path to find. ie: "user.name" or "users.0.name"
-            value: Value to update
-
-        Raises:
-            ValueError: If property value has incorrect format
-        """
-        update_json_forms_property(CurrentJsonFormDataAccessor(process), property_path, value)
-
 
 class CurrentElementValueAccessor(ProcessElementValueAccessor):
     def __init__(self, process: Process, element_definition_code: str):
         self.process = process
         self.element_definition_code = element_definition_code
 
     def set_element_values(self, element_values: List[ElementValueUnion]):
```

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_task_page_item_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_task_page_item_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_task_save_element_command_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_task_save_element_command_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_task_save_json_forms_value_data_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_task_save_json_forms_value_data_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_task_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_task_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/_tenant_user_utils.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/_tenant_user_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/element_values.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/element_values.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/kuflow_rest/utils/json_forms.py` & `kuflow_rest-1.5.1/kuflow_rest/utils/json_forms.py`

 * *Files identical despite different names*

### Comparing `kuflow_rest-1.5.0/pyproject.toml` & `kuflow_rest-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-rest"
-version = "1.5.0"
+version = "1.5.1"
 description = "Client for KuFlow Rest Api"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
```

### Comparing `kuflow_rest-1.5.0/setup.py` & `kuflow_rest-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['azure-core>=1.29.3,<2.0.0', 'isodate>=0.6.1,<0.7.0']
 
 setup_kwargs = {
     'name': 'kuflow-rest',
-    'version': '1.5.0',
+    'version': '1.5.1',
     'description': 'Client for KuFlow Rest Api',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-rest.svg)](https://pypi.org/project/kuflow-rest)\n\n# KuFlow Rest\n\nThis is a client for the KuFlow API Rest that allows you to interact with our API in a comfortable way in the creation of your workers and tools.\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_rest-1.5.0/PKG-INFO` & `kuflow_rest-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuflow-rest
-Version: 1.5.0
+Version: 1.5.1
 Summary: Client for KuFlow Rest Api
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


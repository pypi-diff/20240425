# Comparing `tmp/auto-test-common-2.0.1.tar.gz` & `tmp/auto-test-common-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-2.0.1.tar", last modified: Wed Apr 24 06:12:41 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.2.tar", last modified: Thu Apr 25 00:39:22 2024, max compression
```

## Comparing `auto-test-common-2.0.1.tar` & `auto-test-common-2.0.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.441798 auto-test-common-2.0.1/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-24 06:12:41.441934 auto-test-common-2.0.1/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.409088 auto-test-common-2.0.1/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1821 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      749 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.409397 auto-test-common-2.0.1/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.1/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.411258 auto-test-common-2.0.1/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.1/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5471 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/autotest/assert_function.py
--rw-r--r--   0 edz        (502) staff       (20)    12844 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     8211 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.417272 auto-test-common-2.0.1/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.1/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7645 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.1/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.418249 auto-test-common-2.0.1/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.1/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.1/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.426408 auto-test-common-2.0.1/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.1/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/data/eval_data_handle.py
--rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/data/faker_handle.py
--rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.1/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.429420 auto-test-common-2.0.1/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.1/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.1/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.1/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.430460 auto-test-common-2.0.1/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.1/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.1/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.1/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.433243 auto-test-common-2.0.1/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.1/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.1/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.1/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.433876 auto-test-common-2.0.1/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.1/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.436114 auto-test-common-2.0.1/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.1/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.1/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.1/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.1/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.1/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.441485 auto-test-common-2.0.1/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.1/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.1/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.1/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.1/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.1/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.1/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2024-04-24 06:12:41.442641 auto-test-common-2.0.1/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     2099 2024-04-24 05:10:23.000000 auto-test-common-2.0.1/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.029030 auto-test-common-2.0.2/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-25 00:39:22.029167 auto-test-common-2.0.2/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:21.981618 auto-test-common-2.0.2/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-25 00:39:21.000000 auto-test-common-2.0.2/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1821 2024-04-25 00:39:21.000000 auto-test-common-2.0.2/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-25 00:39:21.000000 auto-test-common-2.0.2/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-25 00:39:21.000000 auto-test-common-2.0.2/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      750 2024-04-25 00:39:21.000000 auto-test-common-2.0.2/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-25 00:39:21.000000 auto-test-common-2.0.2/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:21.981973 auto-test-common-2.0.2/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.2/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:21.986652 auto-test-common-2.0.2/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.2/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.2/common/autotest/assert_function.py
+-rw-r--r--   0 edz        (502) staff       (20)    12844 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     8211 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:21.989414 auto-test-common-2.0.2/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.2/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7645 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.2/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.2/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:21.990354 auto-test-common-2.0.2/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.2/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.2/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:21.999365 auto-test-common-2.0.2/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.2/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/data/eval_data_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/data/faker_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.2/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.004396 auto-test-common-2.0.2/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.2/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.2/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.2/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.2/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.2/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.2/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.006215 auto-test-common-2.0.2/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.2/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.2/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.2/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.013099 auto-test-common-2.0.2/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.2/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.2/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.2/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.2/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.2/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.014833 auto-test-common-2.0.2/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.2/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.2/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.018778 auto-test-common-2.0.2/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.2/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.2/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.2/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.2/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.2/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-25 00:39:22.028319 auto-test-common-2.0.2/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.2/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.2/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.2/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.2/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.2/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.2/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.2/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-04-25 00:39:22.029921 auto-test-common-2.0.2/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     2100 2024-04-24 06:49:26.000000 auto-test-common-2.0.2/setup.py
```

### Comparing `auto-test-common-2.0.1/PKG-INFO` & `auto-test-common-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.1
+Version: 2.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.1/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.2/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.1
+Version: 2.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.1/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.2/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.2/auto_test_common.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 PyMySQL==0.10.1
 ruamel.yaml==0.18.5
 pytest-rerunfailures==9.1.1
 allure-pytest==2.9.45
 pytest-asyncio==0.23.6
 pytest-mimesis==1.1.0
 pytest-bdd==7.1.2
-faker==21.0.0pytest-xdist==2.5.0
+faker==21.0.0
+pytest-xdist==2.5.0
 allure-python-commons==2.9.45
 xlrd==2.0.1
 xlutils==2.0.0
 xlwt==1.3.0
 zipp==3.7.0
 xmltodict==0.13.0
 python-dateutil==2.8.2
```

### Comparing `auto-test-common-2.0.1/common/autotest/assert_function.py` & `auto-test-common-2.0.2/common/autotest/assert_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Any, Union, Text
-# 第三方库导入
 import allure
 
 @allure.step("预期结果：{expect_value}  == 实际结果：{actual_value}")
 def equals(expect_value: Any, actual_value: Any, message: Text = ""):
     """
     判断是否相等
     """
```

### Comparing `auto-test-common-2.0.1/common/autotest/base_requests.py` & `auto-test-common-2.0.2/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/autotest/handle_allure.py` & `auto-test-common-2.0.2/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/autotest/handle_assert.py` & `auto-test-common-2.0.2/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/common/api_driver.py` & `auto-test-common-2.0.2/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/common/constant.py` & `auto-test-common-2.0.2/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/common/test.py` & `auto-test-common-2.0.2/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/config/config.py` & `auto-test-common-2.0.2/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/data/data_process.py` & `auto-test-common-2.0.2/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/data/faker_handle.py` & `auto-test-common-2.0.2/common/data/faker_handle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/data/handle_common.py` & `auto-test-common-2.0.2/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/data/template_data.py` & `auto-test-common-2.0.2/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/db/handle_db.py` & `auto-test-common-2.0.2/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/db/handle_db_batch.py` & `auto-test-common-2.0.2/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/db/handle_mongo.py` & `auto-test-common-2.0.2/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/db/handle_mysqldb.py` & `auto-test-common-2.0.2/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/db/handle_oracle.py` & `auto-test-common-2.0.2/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/db/handle_sqlserver.py` & `auto-test-common-2.0.2/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/driver/ui_page.py` & `auto-test-common-2.0.2/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/file/ReadFile.py` & `auto-test-common-2.0.2/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/file/handle_excel.py` & `auto-test-common-2.0.2/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/file/handle_file.py` & `auto-test-common-2.0.2/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/file/handle_reques.py` & `auto-test-common-2.0.2/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/file/handle_system.py` & `auto-test-common-2.0.2/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/file/handle_yaml.py` & `auto-test-common-2.0.2/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/mq/handle_rabbit.py` & `auto-test-common-2.0.2/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plat/ATF_platform.py` & `auto-test-common-2.0.2/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plat/jenkin_platform.py` & `auto-test-common-2.0.2/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plat/jira_platform.py` & `auto-test-common-2.0.2/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plat/mysql_platform.py` & `auto-test-common-2.0.2/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plat/service_platform.py` & `auto-test-common-2.0.2/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/allure_plugin.py` & `auto-test-common-2.0.2/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/assert_plugin.py` & `auto-test-common-2.0.2/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/atf_plugin.py` & `auto-test-common-2.0.2/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/data_bus.py` & `auto-test-common-2.0.2/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/data_plugin.py` & `auto-test-common-2.0.2/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/file_plugin.py` & `auto-test-common-2.0.2/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.2/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.2/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.2/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/template_plugin.py` & `auto-test-common-2.0.2/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.2/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.1/setup.py` & `auto-test-common-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "PyMySQL==0.10.1",
         "ruamel.yaml==0.18.5",
         "pytest-rerunfailures==9.1.1",
         "allure-pytest==2.9.45",
         "pytest-asyncio==0.23.6",
         "pytest-mimesis==1.1.0",
         "pytest-bdd==7.1.2",
-        "faker==21.0.0"
+        "faker==21.0.0",
         "pytest-xdist==2.5.0",
         "allure-python-commons==2.9.45",
         "xlrd==2.0.1",
         "xlutils==2.0.0",
         "xlwt==1.3.0",
         "zipp==3.7.0",
         "xmltodict==0.13.0",
```


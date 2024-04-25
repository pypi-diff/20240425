# Comparing `tmp/linktest-2.6.1.tar.gz` & `tmp/linktest-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.6.1.tar", last modified: Thu Apr 25 07:29:13 2024, max compression
+gzip compressed data, was "linktest-2.6.2.tar", last modified: Thu Apr 25 07:39:19 2024, max compression
```

## Comparing `linktest-2.6.1.tar` & `linktest-2.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:29:13.937445 linktest-2.6.1/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 07:29:13.937128 linktest-2.6.1/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:29:13.934951 linktest-2.6.1/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-25 07:27:10.000000 linktest-2.6.1/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106616 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 07:27:17.000000 linktest-2.6.1/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14264 2024-04-25 07:25:23.000000 linktest-2.6.1/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-25 06:38:35.000000 linktest-2.6.1/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:29:13.936747 linktest-2.6.1/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 07:29:13.000000 linktest-2.6.1/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-25 07:29:13.000000 linktest-2.6.1/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-25 07:29:13.000000 linktest-2.6.1/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-25 07:29:13.000000 linktest-2.6.1/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-25 07:29:13.000000 linktest-2.6.1/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-25 07:29:13.937607 linktest-2.6.1/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 07:29:07.000000 linktest-2.6.1/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:39:19.328985 linktest-2.6.2/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 07:39:19.328741 linktest-2.6.2/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:39:19.324402 linktest-2.6.2/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-25 07:38:02.000000 linktest-2.6.2/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106616 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 07:38:08.000000 linktest-2.6.2/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13784 2024-04-25 07:37:42.000000 linktest-2.6.2/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:39:19.328395 linktest-2.6.2/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-25 07:39:19.329032 linktest-2.6.2/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 07:39:13.000000 linktest-2.6.2/setup.py
```

### Comparing `linktest-2.6.1/linktest/appium_utils.py` & `linktest-2.6.2/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/auto_generate_testcase_list.py` & `linktest-2.6.2/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.6.2/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/base_testcase.py` & `linktest-2.6.2/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/clean_data.py` & `linktest-2.6.2/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/conver_xml_into_db.py` & `linktest-2.6.2/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/database_helper.py` & `linktest-2.6.2/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/date_utilities.py` & `linktest-2.6.2/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/doctor.py` & `linktest-2.6.2/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/framework_log.py` & `linktest-2.6.2/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/generate_html_log.py` & `linktest-2.6.2/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/get_adb_devices.py` & `linktest-2.6.2/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/get_ios_devices_list.py` & `linktest-2.6.2/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/get_platform_info.py` & `linktest-2.6.2/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/get_project_info.py` & `linktest-2.6.2/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/html_report.py` & `linktest-2.6.2/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/logged_requests.py` & `linktest-2.6.2/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/main.py` & `linktest-2.6.2/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/memory_usage.py` & `linktest-2.6.2/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/re_func.py` & `linktest-2.6.2/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/run.py` & `linktest-2.6.2/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/run_testcase_thread.py` & `linktest-2.6.2/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/scp_report_to_specified_path.py` & `linktest-2.6.2/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/selenium_helper.py` & `linktest-2.6.2/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/timeout_thread.py` & `linktest-2.6.2/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/ui_testcase.py` & `linktest-2.6.2/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/update_config.py` & `linktest-2.6.2/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest/webdriver_wrapper.py` & `linktest-2.6.2/linktest/webdriver_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,23 +48,16 @@
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 # from selenium.webdriver import Keys
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
-from selenium.webdriver.common.options import BaseOptions
-from selenium.webdriver.common.print_page_options import PrintOptions
-from selenium.webdriver.common.timeouts import Timeouts
-
 from selenium.webdriver import Chrome
-from selenium.webdriver.common.by import By
-
 from selenium.webdriver.remote.webelement import WebElement
-from typing import Union, Any
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
 except BaseException:
     raise ("No settings module found ....")
@@ -357,20 +350,14 @@
 
     def back(self) -> None:
         super().back()
         self._log_action("back")
         if AUTO_SCREENSHOT_ON_ACTION:
             self.save_screenshot()
 
-
-    def print_page(self, print_options: Optional[PrintOptions] = None) -> str:
-        return_value = super().print_page(print_options)
-        self._log_action("print_page", print_options)
-        return return_value
-
     def get_cookies(self) -> List[dict]:
         return_value = super().get_cookies()
         self._log_action("get_cookies")
         return return_value
 
     def add_cookie(self, cookie_dict) -> None:
         super().add_cookie(cookie_dict)
```

### Comparing `linktest-2.6.1/linktest/xml_report.py` & `linktest-2.6.2/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.1/linktest.egg-info/SOURCES.txt` & `linktest-2.6.2/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*


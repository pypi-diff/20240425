# Comparing `tmp/linktest-2.6.2.tar.gz` & `tmp/linktest-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.6.2.tar", last modified: Thu Apr 25 07:39:19 2024, max compression
+gzip compressed data, was "linktest-2.6.3.tar", last modified: Thu Apr 25 08:06:05 2024, max compression
```

## Comparing `linktest-2.6.2.tar` & `linktest-2.6.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:39:19.328985 linktest-2.6.2/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 07:39:19.328741 linktest-2.6.2/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:39:19.324402 linktest-2.6.2/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-25 07:38:02.000000 linktest-2.6.2/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106616 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 07:38:08.000000 linktest-2.6.2/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13784 2024-04-25 07:37:42.000000 linktest-2.6.2/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-25 07:29:38.000000 linktest-2.6.2/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 07:39:19.328395 linktest-2.6.2/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-25 07:39:19.000000 linktest-2.6.2/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-25 07:39:19.329032 linktest-2.6.2/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 07:39:13.000000 linktest-2.6.2/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 08:06:05.221820 linktest-2.6.3/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 08:06:05.221541 linktest-2.6.3/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 08:06:05.214582 linktest-2.6.3/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-25 08:04:32.000000 linktest-2.6.3/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106616 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 08:04:36.000000 linktest-2.6.3/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14347 2024-04-25 08:03:17.000000 linktest-2.6.3/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-25 07:39:46.000000 linktest-2.6.3/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 08:06:05.221189 linktest-2.6.3/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 08:06:04.000000 linktest-2.6.3/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-25 08:06:04.000000 linktest-2.6.3/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-25 08:06:04.000000 linktest-2.6.3/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-25 08:06:04.000000 linktest-2.6.3/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-25 08:06:04.000000 linktest-2.6.3/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-25 08:06:05.221887 linktest-2.6.3/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 08:05:59.000000 linktest-2.6.3/setup.py
```

### Comparing `linktest-2.6.2/linktest/appium_utils.py` & `linktest-2.6.3/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/auto_generate_testcase_list.py` & `linktest-2.6.3/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.6.3/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/base_testcase.py` & `linktest-2.6.3/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/clean_data.py` & `linktest-2.6.3/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/conver_xml_into_db.py` & `linktest-2.6.3/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/database_helper.py` & `linktest-2.6.3/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/date_utilities.py` & `linktest-2.6.3/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/doctor.py` & `linktest-2.6.3/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/framework_log.py` & `linktest-2.6.3/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/generate_html_log.py` & `linktest-2.6.3/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/get_adb_devices.py` & `linktest-2.6.3/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/get_ios_devices_list.py` & `linktest-2.6.3/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/get_platform_info.py` & `linktest-2.6.3/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/get_project_info.py` & `linktest-2.6.3/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/html_report.py` & `linktest-2.6.3/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/logged_requests.py` & `linktest-2.6.3/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/main.py` & `linktest-2.6.3/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/memory_usage.py` & `linktest-2.6.3/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/re_func.py` & `linktest-2.6.3/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/run.py` & `linktest-2.6.3/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/run_testcase_thread.py` & `linktest-2.6.3/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/scp_report_to_specified_path.py` & `linktest-2.6.3/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/selenium_helper.py` & `linktest-2.6.3/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/timeout_thread.py` & `linktest-2.6.3/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/ui_testcase.py` & `linktest-2.6.3/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/update_config.py` & `linktest-2.6.3/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest/webdriver_wrapper.py` & `linktest-2.6.3/linktest/webdriver_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,18 +45,22 @@
 import os
 import typing
 from typing import List
 from typing import Dict
 from typing import Optional
 from typing import Union
 
-# from selenium.webdriver import Keys
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
-from selenium.webdriver import Chrome
+
+# from selenium.webdriver import Chrome
+from selenium.webdriver.chrome.webdriver import WebDriver as Chrome
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.chrome.service import Service
+
 from selenium.webdriver.remote.webelement import WebElement
 
 AUTO_SCREENSHOT_ON_ACTION = False
 
 try:
     import settings
 except BaseException:
@@ -226,15 +230,25 @@
     # todo:可以继续封装 WebElement 的其他方法
 
 
 class WebDriverWrapper(Chrome):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
-        super().__init__(*args, **kwargs)
+
+        # Default options and service for Chrome, if not provided in kwargs
+        options = kwargs.pop('options', Options())
+        service = kwargs.pop('service', Service())
+        keep_alive = kwargs.pop('keep_alive', True)
+
+        # Initialization of the Chrome WebDriver with the correct parameters
+        super().__init__(options=options, service=service, keep_alive=keep_alive, *args, **kwargs)
+
+        #
+        # super().__init__(*args, **kwargs)
 
     def _log_action(self, action, *args):
         if args:
             msg = f"- WebDriver Action: '{action}' with args: {', '.join(map(str, args))}"
         else:
             msg = f"- WebDriver Action: '{action}'"
         self.logger.info(msg)
```

### Comparing `linktest-2.6.2/linktest/xml_report.py` & `linktest-2.6.3/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.2/linktest.egg-info/SOURCES.txt` & `linktest-2.6.3/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*


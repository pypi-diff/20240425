# Comparing `tmp/linktest-2.5.8.tar.gz` & `tmp/linktest-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.5.8.tar", last modified: Mon Apr 22 06:52:25 2024, max compression
+gzip compressed data, was "linktest-2.6.0.tar", last modified: Thu Apr 25 02:38:01 2024, max compression
```

## Comparing `linktest-2.5.8.tar` & `linktest-2.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-22 06:52:25.281407 linktest-2.5.8/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-22 06:52:25.281186 linktest-2.5.8/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-22 06:52:25.279598 linktest-2.5.8/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-22 06:48:17.000000 linktest-2.5.8/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34732 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105788 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-22 06:48:22.000000 linktest-2.5.8/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14214 2024-04-22 06:46:24.000000 linktest-2.5.8/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-22 06:52:25.280954 linktest-2.5.8/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-22 06:52:25.281444 linktest-2.5.8/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-22 06:52:10.000000 linktest-2.5.8/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 02:38:01.481885 linktest-2.6.0/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 02:38:01.481611 linktest-2.6.0/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 02:38:01.478243 linktest-2.6.0/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-24 09:19:46.000000 linktest-2.6.0/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-23 03:26:41.000000 linktest-2.6.0/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34827 2024-04-23 14:58:22.000000 linktest-2.6.0/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106616 2024-04-24 07:43:57.000000 linktest-2.6.0/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-22 14:08:31.000000 linktest-2.6.0/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-24 09:19:56.000000 linktest-2.6.0/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14214 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-22 06:53:02.000000 linktest-2.6.0/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-25 02:38:01.481078 linktest-2.6.0/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-25 02:38:01.000000 linktest-2.6.0/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-25 02:38:01.000000 linktest-2.6.0/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-25 02:38:01.000000 linktest-2.6.0/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-25 02:38:01.000000 linktest-2.6.0/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-25 02:38:01.000000 linktest-2.6.0/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-25 02:38:01.481930 linktest-2.6.0/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-25 02:37:55.000000 linktest-2.6.0/setup.py
```

### Comparing `linktest-2.5.8/linktest/appium_utils.py` & `linktest-2.6.0/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/auto_generate_testcase_list.py` & `linktest-2.6.0/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.6.0/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/base_testcase.py` & `linktest-2.6.0/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/clean_data.py` & `linktest-2.6.0/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/conver_xml_into_db.py` & `linktest-2.6.0/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/database_helper.py` & `linktest-2.6.0/linktest/database_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                            testcase.rerun_tag,
                            conn.escape_string(error_message) if error_message else "",
                            screenshot_list_for_db,
                            testcase.testcase_start_time)
 
             # print("-------- executed done insert_tc_sql: %s" % insert_tc_sql)
             cursor.execute(insert_tc_sql)
-        print("-------- saved execution details into database ========")
+        print("-------- saved execution details into database --------")
     except BaseException:
         traceback.print_exc()
         print(traceback.format_exc())
     finally:
         conn.commit()
         cursor.close()
         conn.close()
```

### Comparing `linktest-2.5.8/linktest/date_utilities.py` & `linktest-2.6.0/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/doctor.py` & `linktest-2.6.0/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/framework_log.py` & `linktest-2.6.0/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/generate_html_log.py` & `linktest-2.6.0/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/get_adb_devices.py` & `linktest-2.6.0/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/get_ios_devices_list.py` & `linktest-2.6.0/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/get_platform_info.py` & `linktest-2.6.0/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/get_project_info.py` & `linktest-2.6.0/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/html_report.py` & `linktest-2.6.0/linktest/html_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,17 +410,17 @@
                     od = collections.OrderedDict(sorted(failed_cases_dict.items()))
                     for k in od.keys():
                         sorted_failed_cases.append(od[k])
                 else:
                     sorted_failed_cases = failed_cases
 
                 for index, failed_testcase in enumerate(sorted_failed_cases):
-                    screenshot_exists = isinstance(failed_testcase, UITestCase) and getattr(failed_testcase,
-                                                                                            'screenshot', None)
-                    screenshot_id = f"screenshot_{index}"
+                    # screenshot_exists = isinstance(failed_testcase, UITestCase) and getattr(failed_testcase,
+                    #                                                                         'screenshot', None)
+                    # screenshot_id = f"screenshot_{index}"
 
                     module_name = failed_testcase.__module__.replace(".", "_") + os.sep + failed_testcase.__class__.__name__
                     module_name_display = failed_testcase.__module__.replace("tests.", "&#x0009;")
                     module_name_display += os.sep + failed_testcase.__class__.__name__
                     report_file_handler.write(
                         "<tr class='all_failed_case' name=%s>" % failed_testcase.testcase_filter_tag)
 
@@ -460,41 +460,41 @@
                                 failed_testcase.log_file_path)
                             report_file_handler.write(
                                 " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML]</font></a>" %
                                 failed_testcase.log_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
-                        try:
-                            if isinstance(failed_testcase, UITestCase):
-                                report_file_handler.write(
-                                    "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='click to see the Screenshot' href='%s'> <font color='#DC3912'> - Screenshot</font> </a>" %
-                                    failed_testcase.screenshot)
-
-                        except BaseException:
-                            print(traceback.format_exc())
+                        # try:
+                        #     if isinstance(failed_testcase, UITestCase):
+                        #         report_file_handler.write(
+                        #             "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='click to see the Screenshot' href='%s'> <font color='#DC3912'> - Screenshot</font> </a>" %
+                        #             failed_testcase.screenshot)
+                        #
+                        # except BaseException:
+                        #     print(traceback.format_exc())
 
                     elif failed_testcase.rerun_tag == 1:
                         try:
                             report_file_handler.write(
                                 "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
                                 failed_testcase.log_file_path)
                             report_file_handler.write(
                                 " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
                                 failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
-                        try:
-                            if isinstance(failed_testcase, UITestCase):
-                                report_file_handler.write(
-                                    "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='Click to see the rerun_Screenshot' href='%s'> <font color='#DC3912'> - rerun_Screenshot</font> </a>" %
-                                    failed_testcase.rerun_screenshot)
-                        except BaseException:
-                            print(traceback.format_exc())
+                        # try:
+                        #     if isinstance(failed_testcase, UITestCase):
+                        #         report_file_handler.write(
+                        #             "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='Click to see the rerun_Screenshot' href='%s'> <font color='#DC3912'> - rerun_Screenshot</font> </a>" %
+                        #             failed_testcase.rerun_screenshot)
+                        # except BaseException:
+                        #     print(traceback.format_exc())
 
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center' >")
                     report_file_handler.write("<font>")
                     if not hasattr(failed_testcase, "execution_time"):
                         failed_testcase.execution_time = ""
@@ -570,44 +570,44 @@
                             passed_testcase.log_file_path)
                         report_file_handler.write(
                             " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
                             passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
-                    try:
-                        if isinstance(passed_testcase, UITestCase):
-                            if getattr(passed_testcase, "screenshot"):
-                                report_file_handler.write(
-                                    "<a title='Screenshot' href='%s'> <font color='green'> - Screenshot</font> </a>" %
-                                    passed_testcase.screenshot)
-                    except BaseException:
-                        traceback.print_exc()
-                        print(traceback.format_exc())
+                    # try:
+                    #     if isinstance(passed_testcase, UITestCase):
+                    #         if getattr(passed_testcase, "screenshot"):
+                    #             report_file_handler.write(
+                    #                 "<a title='Screenshot' href='%s'> <font color='green'> - Screenshot</font> </a>" %
+                    #                 passed_testcase.screenshot)
+                    # except BaseException:
+                    #     traceback.print_exc()
+                    #     print(traceback.format_exc())
 
                     try:
                         if passed_testcase.rerun_tag == 1:
                             report_file_handler.write(
                                 "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a title='rerun_Log' href='%s'> &nbsp;[TXT </a>" %
                                 passed_testcase.log_file_path)
                             report_file_handler.write(
                                 " | <a title='rerun_Log' href='%s'> HTML] </a>" %
                                 passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
-                    try:
-                        if getattr(settings, "SAVE_SCREENSHOT_FOR_PASSED_TESTS", False):
-                            if isinstance(passed_testcase, UITestCase):
-                                if passed_testcase.rerun_tag == 1:
-                                    report_file_handler.write(
-                                        "<a title='rerun_Screenshot' href='%s'> - rerun_Screenshot </a>" %
-                                        passed_testcase.rerun_screenshot)
-                    except BaseException:
-                        print(traceback.format_exc())
+                    # try:
+                    #     if getattr(settings, "SAVE_SCREENSHOT_FOR_PASSED_TESTS", False):
+                    #         if isinstance(passed_testcase, UITestCase):
+                    #             if passed_testcase.rerun_tag == 1:
+                    #                 report_file_handler.write(
+                    #                     "<a title='rerun_Screenshot' href='%s'> - rerun_Screenshot </a>" %
+                    #                     passed_testcase.rerun_screenshot)
+                    # except BaseException:
+                    #     print(traceback.format_exc())
 
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center'>")
                     report_file_handler.write("<font color='#333'>")
 
                     if not hasattr(passed_testcase, "execution_time"):
```

### Comparing `linktest-2.5.8/linktest/logged_requests.py` & `linktest-2.6.0/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/main.py` & `linktest-2.6.0/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,14 +400,28 @@
     settings.LOG_FORMAT = '%(asctime)s %(levelname)s %(filename)s %(lineno)d: %(message)s'
 
 try:
     from settings import AUTO_DOWNLOAD_CHROMEDRIVER
 except ImportError:
     settings.AUTO_DOWNLOAD_CHROMEDRIVER = False
 
+try:
+    from settings import AUTO_SCREENSHOT_ON_ACTION
+except ImportError:
+    settings.AUTO_SCREENSHOT_ON_ACTION = False
+
+try:
+    from settings import SAVE_SCREENSHOT_FOR_PASSED_TESTS
+except ImportError:
+    settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS = False
+
+if settings.AUTO_SCREENSHOT_ON_ACTION:
+    settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS = False
+
+
 
 # set Default time_zone = 'Asia/Shanghai'
 if hasattr(settings, "TIME_ZONE"):
     if settings.TIME_ZONE:
         os.environ['TZ'] = '%s' % settings.TIME_ZONE
 else:
     os.environ['TZ'] = 'Asia/Shanghai'
@@ -1137,46 +1151,48 @@
                             close_browser_after_done_flag = settings.CLOSE_BROWSER
 
                         for browser in webdriver_list:
                             webdriver = getattr(executing_testcase, browser)
 
                             try:
                                 if executing_testcase.ExecutionStatusSetByFramework == "failed":
-                                    webdriver.save_screenshot(
-                                        testcase_full_folder + os.sep + browser + "_" +
-                                        executing_testcase.screenshot_name)
-                                    executing_testcase.screenshot_path_list_for_db.append(
-                                        testcase_full_folder + os.sep + browser + "_" +
-                                        executing_testcase.screenshot_name)
+                                    if executing_testcase.rerun_tag == 0:
+                                        webdriver.save_screenshot(
+                                            testcase_full_folder + os.sep + browser + "_" +
+                                            executing_testcase.screenshot_name)
+                                        executing_testcase.screenshot_path_list_for_db.append(
+                                            testcase_full_folder + os.sep + browser + "_" +
+                                            executing_testcase.screenshot_name)
+                                    elif executing_testcase.rerun_tag == 1:
+                                        webdriver.save_screenshot(
+                                            executing_testcase.full_tc_folder + os.sep + browser + "_" +
+                                            executing_testcase.rerun_screenshot_name)
                                 elif hasattr(settings, "SAVE_SCREENSHOT_FOR_PASSED_TESTS"):
-                                    if settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS is True:
+                                    if settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS:
                                         if executing_testcase.rerun_tag == 0:
                                             webdriver.save_screenshot(
                                                 testcase_full_folder + os.sep + browser + "_" +
                                                 executing_testcase.screenshot_name)
                                             executing_testcase.screenshot_path_list_for_db.append(
                                                 testcase_full_folder + os.sep + browser + "_" +
                                                 executing_testcase.screenshot_name)
 
-                                if executing_testcase.rerun_tag == 0:
-                                    executing_testcase.screenshot = testcase_full_folder.replace(
-                                        project_info.output_folder, ".") \
-                                                                    + os.sep + browser + "_" + \
-                                                                    executing_testcase.screenshot_name
-                                elif executing_testcase.rerun_tag == 1:
-                                    executing_testcase.screenshot = testcase_full_folder.replace(
-                                        project_info.output_folder, ".") \
-                                                                    + os.sep + browser + "_" + \
-                                                                    executing_testcase.screenshot_name
-
-                                    executing_testcase.rerun_screenshot = testcase_full_folder.replace(
-                                        project_info.output_folder,
-                                        ".") + os.sep + browser + "_" + executing_testcase.rerun_screenshot_name
+                                            executing_testcase.screenshot = testcase_full_folder.replace(
+                                                project_info.output_folder, ".") \
+                                                                            + os.sep + browser + "_" + \
+                                                                            executing_testcase.screenshot_name
+                                        elif executing_testcase.rerun_tag == 1:
+                                            webdriver.save_screenshot(
+                                                executing_testcase.full_tc_folder + os.sep + browser + "_"
+                                                + executing_testcase.rerun_screenshot_name)
+
+                                            executing_testcase.rerun_screenshot = testcase_full_folder.replace(
+                                                project_info.output_folder,
+                                                ".") + os.sep + browser + "_" + executing_testcase.rerun_screenshot_name
 
-                                    webdriver.save_screenshot(executing_testcase.full_tc_folder + os.sep + browser + "_" + executing_testcase.rerun_screenshot_name)
                             except BaseException:
                                 traceback.print_exc()
                             finally:
                                 try:
                                     is_appium_installed = True
                                     try:
                                         import appium
@@ -1960,15 +1976,18 @@
 
         if total_testcases_count < thread_pool_size:
             thread_pool_size = total_testcases_count
 
         if include_android_testcase_flag is True:
             thread_pool_size = len(get_adb_devices())
 
-        print("***" * 20 + " will start %s threads" % thread_pool_size)
+        if thread_pool_size == 1:
+            print("***" * 20 + " will start %s thread" % thread_pool_size)
+        else:
+            print("***" * 20 + " will start %s threads" % thread_pool_size)
         for i in range(thread_pool_size):
             testcase_executor_list.append(TestCaseExecutor(queue, total_testcases_count, output_folder, begin_time))
 
         BaseTestCase.GlobalTotalCaseCount = total_testcases_count
 
         for testcase_executor in testcase_executor_list:
             time.sleep(0.5)
@@ -2035,14 +2054,17 @@
                                          begin_time,
                                          PLATFORM_INFO,
                                          len(BaseTestCase.GlobalDataList) > 0,
                                          True)
                 except BaseException:
                     traceback.print_exc()
 
+            print(
+                "=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
+
             # save the execution summary into DB (environment, total_execution_time,
             try:
                 import linktest
                 from . import database_helper
                 if hasattr(settings, "SAVE_LOG_TO_DB"):
                     if settings.SAVE_LOG_TO_DB is True:
                         end_time = datetime.datetime.now()
@@ -2062,15 +2084,15 @@
                             rerun_flag=1 if settings.RERUN_FLAG else 0
                         )
             except BaseException:
                 traceback.print_exc()
             finally:
                 pass
 
-        print("=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
+        # print("=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
 
         if hasattr(settings, "COPY_REPORT_TO_SPECIFIED_PATH"):
             if settings.COPY_REPORT_TO_SPECIFIED_PATH is True:
                 if not hasattr(settings, "SPECIFIED_REPORT_PATH") or not hasattr(settings, "SPECIFIED_REPORT_HOST_IP") \
                         or not hasattr(settings, "SPECIFIED_REPORT_HOST_PORT") or not hasattr(settings,
                                                                                               "SPECIFIED_REPORT_HOST_USERNAME") \
                         or not hasattr(settings, "SPECIFIED_REPORT_HOST_PASSWORD"):
```

### Comparing `linktest-2.5.8/linktest/memory_usage.py` & `linktest-2.6.0/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/re_func.py` & `linktest-2.6.0/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/run.py` & `linktest-2.6.0/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/run_testcase_thread.py` & `linktest-2.6.0/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/scp_report_to_specified_path.py` & `linktest-2.6.0/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/selenium_helper.py` & `linktest-2.6.0/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/timeout_thread.py` & `linktest-2.6.0/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/ui_testcase.py` & `linktest-2.6.0/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/update_config.py` & `linktest-2.6.0/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/webdriver_wrapper.py` & `linktest-2.6.0/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest/xml_report.py` & `linktest-2.6.0/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.8/linktest.egg-info/SOURCES.txt` & `linktest-2.6.0/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*


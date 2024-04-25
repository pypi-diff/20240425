# Comparing `tmp/qlv-client-0.1.1.tar.gz` & `tmp/qlv-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.1.1.tar", last modified: Wed Apr 17 08:30:42 2024, max compression
+gzip compressed data, was "qlv-client-0.1.2.tar", last modified: Thu Apr 25 02:20:32 2024, max compression
```

## Comparing `qlv-client-0.1.1.tar` & `qlv-client-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:30:42.495136 qlv-client-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      456 2024-04-17 08:30:42.494639 qlv-client-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 08:30:42.491163 qlv-client-0.1.1/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.1/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.1/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.1/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.1/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.1/qlv_client/http_client.py
--rw-rw-rw-   0        0        0     4409 2024-04-17 08:27:22.000000 qlv-client-0.1.1/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.1/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.1/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.1/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:30:42.494143 qlv-client-0.1.1/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-04-17 08:30:42.000000 qlv-client-0.1.1/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-04-17 08:30:42.000000 qlv-client-0.1.1/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:30:42.000000 qlv-client-0.1.1/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 08:30:42.000000 qlv-client-0.1.1/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 08:30:42.000000 qlv-client-0.1.1/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 08:30:42.495136 qlv-client-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-04-17 08:29:27.000000 qlv-client-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:20:32.585598 qlv-client-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-04-25 02:20:32.585101 qlv-client-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 02:20:32.581127 qlv-client-0.1.2/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.2/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.2/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.2/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.2/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.2/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0     5771 2024-04-25 02:20:01.000000 qlv-client-0.1.2/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.2/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.2/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.2/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:20:32.584604 qlv-client-0.1.2/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-04-25 02:20:32.000000 qlv-client-0.1.2/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:20:32.000000 qlv-client-0.1.2/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:20:32.000000 qlv-client-0.1.2/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 02:20:32.000000 qlv-client-0.1.2/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 02:20:32.000000 qlv-client-0.1.2/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:20:32.585598 qlv-client-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-04-25 02:20:20.000000 qlv-client-0.1.2/setup.py
```

### Comparing `qlv-client-0.1.1/LICENSE` & `qlv-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/api.py` & `qlv-client-0.1.2/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/config.py` & `qlv-client-0.1.2/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/converter.py` & `qlv-client-0.1.2/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/http_client.py` & `qlv-client-0.1.2/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/proxy.py` & `qlv-client-0.1.2/qlv_client/proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,7 +86,35 @@
         result = order_ser.fill_order_itinerary_info(**args)
         if result.get("code") == 0:
             logger.error("向劲旅系统回填乘客票单信息失败...")
             return False
         else:
             logger.error("向劲旅系统回填乘客票单信息成功.")
             return True
+
+    @classmethod
+    def save_itinerary_info_by_batch_itinerary(cls, pre_order_id: int, oper: str, itinerary_info: list) -> bool:
+        logger.info("开始向劲旅系统回填乘客票单信息...")
+        args = QlvConfigRepository.get_request_base_params(inter_name="fill_order_itinerary_info")
+        ticket_infos = list()
+        for info in itinerary_info:
+            passenger = info.get("passenger")
+            card_id = info.get("card_id")
+            itinerary_id = info.get("itinerary_id")
+            departure_city = info.get("departure_city")
+            arrive_city = info.get("arrive_city")
+            val: str = "#".join([passenger, card_id, itinerary_id, departure_city, arrive_city])
+            ticket_infos.append(val)
+        order_itinerary_info = {
+            "order_id": pre_order_id,
+            "oper": oper,
+            "ticket_infos": ";".join(ticket_infos)
+        }
+        args.update(order_itinerary_info)
+        order_ser = OrderService(**QlvConfigRepository.get_host_params())
+        result = order_ser.fill_order_itinerary_info(**args)
+        if result.get("code") == 0:
+            logger.error("向劲旅系统回填乘客票单信息失败...")
+            return False
+        else:
+            logger.error("向劲旅系统回填乘客票单信息成功.")
+            return True
```

### Comparing `qlv-client-0.1.1/qlv_client/repository.py` & `qlv-client-0.1.2/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/test.py` & `qlv-client-0.1.2/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/qlv_client/utils.py` & `qlv-client-0.1.2/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.1/setup.py` & `qlv-client-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.1.1',
+    version='0.1.2',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```


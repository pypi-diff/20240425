# Comparing `tmp/okx-sdk-1.3.1.tar.gz` & `tmp/okx-sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okx-sdk-1.3.1.tar", last modified: Sun Apr 14 07:05:07 2024, max compression
+gzip compressed data, was "okx-sdk-1.3.2.tar", last modified: Thu Apr 25 18:46:17 2024, max compression
```

## Comparing `okx-sdk-1.3.1.tar` & `okx-sdk-1.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.753131 okx-sdk-1.3.1/
--rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.1/LICENSE
--rw-rw-rw-   0        0        0    33887 2024-04-14 07:05:07.752132 okx-sdk-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    32434 2024-04-14 07:04:21.000000 okx-sdk-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.529128 okx-sdk-1.3.1/okx/
--rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.1/okx/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.1/okx/clients.py
--rw-rw-rw-   0        0        0    21787 2024-04-14 07:02:59.000000 okx-sdk-1.3.1/okx/constants.py
--rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.1/okx/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.680131 okx-sdk-1.3.1/okx/restapi/
--rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.1/okx/restapi/Account.py
--rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.1/okx/restapi/AlgoTrading.py
--rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.1/okx/restapi/BaseClient.py
--rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.1/okx/restapi/BlockTrading.py
--rw-rw-rw-   0        0        0     8252 2024-04-14 07:02:40.000000 okx-sdk-1.3.1/okx/restapi/Broker.py
--rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.1/okx/restapi/CopyTrading.py
--rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.1/okx/restapi/Finance.py
--rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.1/okx/restapi/Funding.py
--rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.1/okx/restapi/GridTrading.py
--rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.1/okx/restapi/PublicData.py
--rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.1/okx/restapi/RecurringBuy.py
--rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.1/okx/restapi/Rubik.py
--rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.1/okx/restapi/SignalTrading.py
--rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.1/okx/restapi/SpreadTrading.py
--rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.1/okx/restapi/SubAccount.py
--rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.1/okx/restapi/Trading.py
--rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.1/okx/restapi/__init__.py
--rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.1/okx/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.722132 okx-sdk-1.3.1/okx/wsapi/
--rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.1/okx/wsapi/Factory.py
--rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.1/okx/wsapi/PrivateAsync.py
--rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.1/okx/wsapi/PublicAsync.py
--rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.1/okx/wsapi/__init__.py
--rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.1/okx/wsapi/wsutils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.751131 okx-sdk-1.3.1/okx_sdk.egg-info/
--rw-rw-rw-   0        0        0    33887 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 07:05:07.754131 okx-sdk-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1198 2024-04-14 07:04:36.000000 okx-sdk-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.750137 okx-sdk-1.3.1/tests/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:46:17.603673 okx-sdk-1.3.2/
+-rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0    33887 2024-04-25 18:46:17.603673 okx-sdk-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    32434 2024-04-14 07:04:21.000000 okx-sdk-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:46:17.330779 okx-sdk-1.3.2/okx/
+-rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.2/okx/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.2/okx/clients.py
+-rw-rw-rw-   0        0        0    21787 2024-04-14 07:02:59.000000 okx-sdk-1.3.2/okx/constants.py
+-rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.2/okx/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:46:17.503623 okx-sdk-1.3.2/okx/restapi/
+-rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.2/okx/restapi/Account.py
+-rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.2/okx/restapi/AlgoTrading.py
+-rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.2/okx/restapi/BaseClient.py
+-rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.2/okx/restapi/BlockTrading.py
+-rw-rw-rw-   0        0        0     8252 2024-04-14 07:02:40.000000 okx-sdk-1.3.2/okx/restapi/Broker.py
+-rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.2/okx/restapi/CopyTrading.py
+-rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.2/okx/restapi/Finance.py
+-rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.2/okx/restapi/Funding.py
+-rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.2/okx/restapi/GridTrading.py
+-rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.2/okx/restapi/PublicData.py
+-rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.2/okx/restapi/RecurringBuy.py
+-rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.2/okx/restapi/Rubik.py
+-rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.2/okx/restapi/SignalTrading.py
+-rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.2/okx/restapi/SpreadTrading.py
+-rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.2/okx/restapi/SubAccount.py
+-rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.2/okx/restapi/Trading.py
+-rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.2/okx/restapi/__init__.py
+-rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.2/okx/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:46:17.570222 okx-sdk-1.3.2/okx/wsapi/
+-rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.2/okx/wsapi/Factory.py
+-rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.2/okx/wsapi/PrivateAsync.py
+-rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.2/okx/wsapi/PublicAsync.py
+-rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.2/okx/wsapi/__init__.py
+-rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.2/okx/wsapi/wsutils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:46:17.603673 okx-sdk-1.3.2/okx_sdk.egg-info/
+-rw-rw-rw-   0        0        0    33887 2024-04-25 18:46:17.000000 okx-sdk-1.3.2/okx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-04-25 18:46:17.000000 okx-sdk-1.3.2/okx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:46:17.000000 okx-sdk-1.3.2/okx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-25 18:46:17.000000 okx-sdk-1.3.2/okx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 18:46:17.000000 okx-sdk-1.3.2/okx_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:46:17.603673 okx-sdk-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2024-04-25 18:45:56.000000 okx-sdk-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:46:17.603673 okx-sdk-1.3.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.2/tests/__init__.py
```

### Comparing `okx-sdk-1.3.1/LICENSE` & `okx-sdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/PKG-INFO` & `okx-sdk-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `okx-sdk-1.3.1/README.md` & `okx-sdk-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/__init__.py` & `okx-sdk-1.3.2/okx/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/clients.py` & `okx-sdk-1.3.2/okx/clients.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/constants.py` & `okx-sdk-1.3.2/okx/constants.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/exceptions.py` & `okx-sdk-1.3.2/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/Account.py` & `okx-sdk-1.3.2/okx/restapi/Account.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/AlgoTrading.py` & `okx-sdk-1.3.2/okx/restapi/AlgoTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/BaseClient.py` & `okx-sdk-1.3.2/okx/restapi/BaseClient.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/BlockTrading.py` & `okx-sdk-1.3.2/okx/restapi/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/Broker.py` & `okx-sdk-1.3.2/okx/restapi/Broker.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/CopyTrading.py` & `okx-sdk-1.3.2/okx/restapi/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/Finance.py` & `okx-sdk-1.3.2/okx/restapi/Finance.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/Funding.py` & `okx-sdk-1.3.2/okx/restapi/Funding.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/GridTrading.py` & `okx-sdk-1.3.2/okx/restapi/GridTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/PublicData.py` & `okx-sdk-1.3.2/okx/restapi/PublicData.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/RecurringBuy.py` & `okx-sdk-1.3.2/okx/restapi/RecurringBuy.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/Rubik.py` & `okx-sdk-1.3.2/okx/restapi/Rubik.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/SignalTrading.py` & `okx-sdk-1.3.2/okx/restapi/SignalTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/SpreadTrading.py` & `okx-sdk-1.3.2/okx/restapi/SpreadTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/SubAccount.py` & `okx-sdk-1.3.2/okx/restapi/SubAccount.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/Trading.py` & `okx-sdk-1.3.2/okx/restapi/Trading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/restapi/__init__.py` & `okx-sdk-1.3.2/okx/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/utils.py` & `okx-sdk-1.3.2/okx/utils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/wsapi/Factory.py` & `okx-sdk-1.3.2/okx/wsapi/Factory.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/wsapi/PrivateAsync.py` & `okx-sdk-1.3.2/okx/wsapi/PrivateAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/wsapi/PublicAsync.py` & `okx-sdk-1.3.2/okx/wsapi/PublicAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx/wsapi/wsutils.py` & `okx-sdk-1.3.2/okx/wsapi/wsutils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/okx_sdk.egg-info/PKG-INFO` & `okx-sdk-1.3.2/okx_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `okx-sdk-1.3.1/okx_sdk.egg-info/SOURCES.txt` & `okx-sdk-1.3.2/okx_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.1/setup.py` & `okx-sdk-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
     
-VERSION = '1.3.1'
+VERSION = '1.3.2'
 DESCRIPTION = 'Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python'
 
 setuptools.setup(
     name="okx-sdk",
     version=VERSION,
     author="Burak Öner",
     author_email="info@burakoner.com",
```


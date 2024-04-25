# Comparing `tmp/clife_svc2-2.0.0.tar.gz` & `tmp/clife_svc2-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clife_svc2-2.0.0.tar", last modified: Fri Apr 19 08:13:35 2024, max compression
+gzip compressed data, was "clife_svc2-2.0.0rc1.tar", last modified: Thu Apr 25 02:50:26 2024, max compression
```

## Comparing `clife_svc2-2.0.0.tar` & `clife_svc2-2.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:13:35.427606 clife_svc2-2.0.0/
--rw-rw-rw-   0        0        0      635 2024-04-19 08:13:35.426610 clife_svc2-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc2-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:13:35.296574 clife_svc2-2.0.0/clife_svc/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc2-2.0.0/clife_svc/__init__.py
--rw-rw-rw-   0        0        0     9562 2024-04-19 07:59:36.000000 clife_svc2-2.0.0/clife_svc/application.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:13:35.356007 clife_svc2-2.0.0/clife_svc/config/
--rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc2-2.0.0/clife_svc/config/__init__.py
--rw-rw-rw-   0        0        0     1949 2024-03-14 06:53:15.000000 clife_svc2-2.0.0/clife_svc/config/configmap.py
--rw-rw-rw-   0        0        0     5514 2024-04-11 05:42:09.000000 clife_svc2-2.0.0/clife_svc/config/disconf.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:13:35.380761 clife_svc2-2.0.0/clife_svc/errors/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc2-2.0.0/clife_svc/errors/__init__.py
--rw-rw-rw-   0        0        0     3055 2024-03-14 09:02:59.000000 clife_svc2-2.0.0/clife_svc/errors/error_code.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:13:35.423616 clife_svc2-2.0.0/clife_svc/libs/
--rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc2-2.0.0/clife_svc/libs/__init__.py
--rw-rw-rw-   0        0        0      188 2024-04-11 02:54:23.000000 clife_svc2-2.0.0/clife_svc/libs/context.py
--rw-rw-rw-   0        0        0    11100 2024-04-19 08:06:50.000000 clife_svc2-2.0.0/clife_svc/libs/http_request.py
--rw-rw-rw-   0        0        0     2804 2024-04-19 07:58:06.000000 clife_svc2-2.0.0/clife_svc/libs/log.py
--rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc2-2.0.0/clife_svc/libs/mq_handler.py
--rw-rw-rw-   0        0        0     1181 2024-03-15 01:44:31.000000 clife_svc2-2.0.0/clife_svc/libs/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:13:35.307546 clife_svc2-2.0.0/clife_svc2.egg-info/
--rw-rw-rw-   0        0        0      635 2024-04-19 08:13:35.000000 clife_svc2-2.0.0/clife_svc2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2024-04-19 08:13:35.000000 clife_svc2-2.0.0/clife_svc2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:13:35.000000 clife_svc2-2.0.0/clife_svc2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-04-19 08:13:35.000000 clife_svc2-2.0.0/clife_svc2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 08:13:35.000000 clife_svc2-2.0.0/clife_svc2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 08:13:35.428632 clife_svc2-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1221 2024-03-15 02:37:48.000000 clife_svc2-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:50:26.071365 clife_svc2-2.0.0rc1/
+-rw-rw-rw-   0        0        0      638 2024-04-25 02:50:26.055739 clife_svc2-2.0.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2021-12-20 11:08:06.000000 clife_svc2-2.0.0rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 02:50:25.910287 clife_svc2-2.0.0rc1/clife_svc/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc2-2.0.0rc1/clife_svc/__init__.py
+-rw-rw-rw-   0        0        0     9199 2024-04-25 02:02:22.000000 clife_svc2-2.0.0rc1/clife_svc/application.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:50:25.957151 clife_svc2-2.0.0rc1/clife_svc/config/
+-rw-rw-rw-   0        0        0        0 2023-01-13 06:18:27.000000 clife_svc2-2.0.0rc1/clife_svc/config/__init__.py
+-rw-rw-rw-   0        0        0     1949 2024-03-14 06:53:15.000000 clife_svc2-2.0.0rc1/clife_svc/config/configmap.py
+-rw-rw-rw-   0        0        0     5514 2024-04-11 05:42:09.000000 clife_svc2-2.0.0rc1/clife_svc/config/disconf.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:50:25.972772 clife_svc2-2.0.0rc1/clife_svc/errors/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc2-2.0.0rc1/clife_svc/errors/__init__.py
+-rw-rw-rw-   0        0        0     3055 2024-03-14 09:02:59.000000 clife_svc2-2.0.0rc1/clife_svc/errors/error_code.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:50:26.055739 clife_svc2-2.0.0rc1/clife_svc/libs/
+-rw-rw-rw-   0        0        0        2 2021-12-20 11:08:06.000000 clife_svc2-2.0.0rc1/clife_svc/libs/__init__.py
+-rw-rw-rw-   0        0        0      188 2024-04-11 02:54:23.000000 clife_svc2-2.0.0rc1/clife_svc/libs/context.py
+-rw-rw-rw-   0        0        0    11100 2024-04-19 08:06:50.000000 clife_svc2-2.0.0rc1/clife_svc/libs/http_request.py
+-rw-rw-rw-   0        0        0     2783 2024-04-22 01:56:25.000000 clife_svc2-2.0.0rc1/clife_svc/libs/log.py
+-rw-rw-rw-   0        0        0     3510 2023-06-13 07:17:16.000000 clife_svc2-2.0.0rc1/clife_svc/libs/mq_handler.py
+-rw-rw-rw-   0        0        0     1181 2024-03-15 01:44:31.000000 clife_svc2-2.0.0rc1/clife_svc/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 02:50:25.925914 clife_svc2-2.0.0rc1/clife_svc2.egg-info/
+-rw-rw-rw-   0        0        0      638 2024-04-25 02:50:25.000000 clife_svc2-2.0.0rc1/clife_svc2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2024-04-25 02:50:25.000000 clife_svc2-2.0.0rc1/clife_svc2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 02:50:25.000000 clife_svc2-2.0.0rc1/clife_svc2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2024-04-25 02:50:25.000000 clife_svc2-2.0.0rc1/clife_svc2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-25 02:50:25.000000 clife_svc2-2.0.0rc1/clife_svc2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 02:50:26.071365 clife_svc2-2.0.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2024-04-25 02:49:11.000000 clife_svc2-2.0.0rc1/setup.py
```

### Comparing `clife_svc2-2.0.0/PKG-INFO` & `clife_svc2-2.0.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clife_svc2
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: A module for service
 Home-page: 
 Author: andy.hu
 Author-email: hlp0@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clife_svc2-2.0.0/clife_svc/application.py` & `clife_svc2-2.0.0rc1/clife_svc/application.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import os
-if os.environ.get("ENVIRONMENT"):
-    from gevent import monkey
-    monkey.patch_all()
-
 import re
 import time
-import threading
-from typing import Any, Callable, List, Optional, Set, Union
 
-from flask import Flask, request
 from flask_cors import CORS
+from flask import Flask, request
 
 from clife_svc.libs import utils
 from clife_svc.libs.context import app_id, request_id
 from clife_svc.config.disconf import Disconf
 from clife_svc.config.configmap import ConfigMap
 from clife_svc.errors.error_code import ApiException
 from clife_svc.libs.http_request import ClientRequest
@@ -80,24 +74,21 @@
 
 
 class App:
     """
     http接口服务上下文对象，单实例对象
     """
     _instance = None
-    _instance_lock = threading.Lock()
 
     def __new__(cls, *args, **kwargs):
         """
         实现单例模式
         """
         if not cls._instance:
-            with cls._instance_lock:
-                if not cls._instance:
-                    cls._instance = super().__new__(cls)
+            cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, app_name, log_root_path='/www/logs', conf='', log_level='DEBUG'):
         """
         构造函数
         :param app_name 项目名称
         :param log_root_path 项目输出的日志根路径，推荐使用/www/logs，便于线上统一采集日志
@@ -167,15 +158,15 @@
         :return:
         """
         all_config = {}
         all_config.update(self.__disConf)
         all_config.update(self.__configMap.get_all())
         return all_config
 
-    def add_api(self, path: str, view_func: Callable[..., Any], methods: Optional[Union[Set[str], List[str]]] = None):
+    def add_api(self, path: str, view_func, methods):
         """
         增加服务接口，此函数需要在init_api前调用
         :param path:接口访问路径
         :param view_func:接口实现函数
         :param methods:接口访问方式，如GET、POST等
         :return:
         """
@@ -248,8 +239,7 @@
         :param retry:失败重试次数，默认为2次，建议不大于3次
         :param timeout: 回调超时时间（秒），默认为配置文件ai-commons.properties中http.timeout，目前为15秒
         :return:回调请求响应体
         """
         if not re.match(r'[0-9a-f]{8}(-[0-9a-f]{4}){3}-[0-9a-f]{12}', body.get('uuid', '')):
             raise Exception('The request body of call back must contain the correct UUID.')
         return self.__client.call_back(url, body, retry, timeout)
-
```

### Comparing `clife_svc2-2.0.0/clife_svc/config/configmap.py` & `clife_svc2-2.0.0rc1/clife_svc/config/configmap.py`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/clife_svc/config/disconf.py` & `clife_svc2-2.0.0rc1/clife_svc/config/disconf.py`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/clife_svc/errors/error_code.py` & `clife_svc2-2.0.0rc1/clife_svc/errors/error_code.py`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/clife_svc/libs/http_request.py` & `clife_svc2-2.0.0rc1/clife_svc/libs/http_request.py`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/clife_svc/libs/log.py` & `clife_svc2-2.0.0rc1/clife_svc/libs/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import sys
 
 from loguru import logger as klogger
-from flask import g
 
 from clife_svc.libs.context import app_id, request_id
 
 
 def _console_log_filter(record) -> bool:
     record['app_id'] = app_id.get()
     record['request_id'] = request_id.get()
```

### Comparing `clife_svc2-2.0.0/clife_svc/libs/mq_handler.py` & `clife_svc2-2.0.0rc1/clife_svc/libs/mq_handler.py`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/clife_svc/libs/utils.py` & `clife_svc2-2.0.0rc1/clife_svc/libs/utils.py`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/clife_svc2.egg-info/PKG-INFO` & `clife_svc2-2.0.0rc1/clife_svc2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clife-svc2
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: A module for service
 Home-page: 
 Author: andy.hu
 Author-email: hlp0@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clife_svc2-2.0.0/clife_svc2.egg-info/SOURCES.txt` & `clife_svc2-2.0.0rc1/clife_svc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clife_svc2-2.0.0/setup.py` & `clife_svc2-2.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if line.startswith('-e git+'):
             dependency_links.append(line.replace('-e ', ''))
         else:
             requirements.append(line)
 
 setuptools.setup(
     name='clife_svc2',   # 需要打包的名字,即本模块要发布的名字
-    version='2.0.0',     # 版本
+    version='2.0.0rc1',     # 版本
     author='andy.hu',  # 作者名
     author_email='hlp0@163.com',  # 作者邮件
     description='A module for service',   # 简要描述
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',       # 项目地址,一般是代码托管的网站
     packages=setuptools.find_packages(),
```


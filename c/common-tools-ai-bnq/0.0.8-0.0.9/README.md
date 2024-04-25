# Comparing `tmp/common-tools-ai-bnq-0.0.8.tar.gz` & `tmp/common-tools-ai-bnq-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.0.8.tar", last modified: Mon Apr 22 10:06:38 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.0.9.tar", last modified: Thu Apr 25 12:07:20 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.0.8.tar` & `common-tools-ai-bnq-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 10:06:38.368506 common-tools-ai-bnq-0.0.8/
--rw-rw-rw-   0        0        0     1991 2024-04-22 10:06:38.368506 common-tools-ai-bnq-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1671 2024-04-22 10:04:23.000000 common-tools-ai-bnq-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 10:06:38.350507 common-tools-ai-bnq-0.0.8/bnq_py_core/
--rw-rw-rw-   0        0        0      305 2024-04-22 09:58:02.000000 common-tools-ai-bnq-0.0.8/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     4574 2024-04-19 09:14:08.000000 common-tools-ai-bnq-0.0.8/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3561 2024-04-22 09:45:20.000000 common-tools-ai-bnq-0.0.8/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.0.8/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.0.8/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:06:38.363507 common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     1991 2024-04-22 10:06:38.000000 common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2024-04-22 10:06:38.000000 common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 10:06:38.000000 common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-22 10:06:38.000000 common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-22 10:06:38.000000 common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 10:06:38.369506 common-tools-ai-bnq-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      790 2024-04-22 10:06:34.000000 common-tools-ai-bnq-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:06:38.367506 common-tools-ai-bnq-0.0.8/test/
--rw-rw-rw-   0        0        0      122 2024-04-10 03:16:38.000000 common-tools-ai-bnq-0.0.8/test/__init__.py
--rw-rw-rw-   0        0        0      221 2024-04-22 02:30:57.000000 common-tools-ai-bnq-0.0.8/test/gen_key.py
--rw-rw-rw-   0        0        0    27286 2024-04-10 03:37:31.000000 common-tools-ai-bnq-0.0.8/test/test_batch_triton.py
--rw-rw-rw-   0        0        0     3464 2024-04-10 07:43:55.000000 common-tools-ai-bnq-0.0.8/test/test_decorator.py
--rw-rw-rw-   0        0        0      520 2024-04-22 07:28:44.000000 common-tools-ai-bnq-0.0.8/test/test_global.py
--rw-rw-rw-   0        0        0      897 2024-04-16 08:13:06.000000 common-tools-ai-bnq-0.0.8/test/test_pymysql.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:07:20.231041 common-tools-ai-bnq-0.0.9/
+-rw-rw-rw-   0        0        0     2598 2024-04-25 12:07:20.229768 common-tools-ai-bnq-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2024-04-24 02:51:54.000000 common-tools-ai-bnq-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 12:07:20.208773 common-tools-ai-bnq-0.0.9/bnq_py_core/
+-rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.0.9/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1626 2024-04-24 07:12:55.000000 common-tools-ai-bnq-0.0.9/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     4627 2024-04-25 10:38:46.000000 common-tools-ai-bnq-0.0.9/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3617 2024-04-23 07:40:19.000000 common-tools-ai-bnq-0.0.9/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.0.9/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.0.9/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:07:20.224770 common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     2598 2024-04-25 12:07:20.000000 common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2024-04-25 12:07:20.000000 common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:07:20.000000 common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-25 12:07:20.000000 common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 12:07:20.000000 common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:07:20.231041 common-tools-ai-bnq-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-04-25 12:07:16.000000 common-tools-ai-bnq-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:07:20.228770 common-tools-ai-bnq-0.0.9/test/
+-rw-rw-rw-   0        0        0      122 2024-04-10 03:16:38.000000 common-tools-ai-bnq-0.0.9/test/__init__.py
+-rw-rw-rw-   0        0        0      221 2024-04-22 02:30:57.000000 common-tools-ai-bnq-0.0.9/test/gen_key.py
+-rw-rw-rw-   0        0        0    27286 2024-04-10 03:37:31.000000 common-tools-ai-bnq-0.0.9/test/test_batch_triton.py
+-rw-rw-rw-   0        0        0     3464 2024-04-10 07:43:55.000000 common-tools-ai-bnq-0.0.9/test/test_decorator.py
+-rw-rw-rw-   0        0        0      520 2024-04-22 07:28:44.000000 common-tools-ai-bnq-0.0.9/test/test_global.py
+-rw-rw-rw-   0        0        0      897 2024-04-16 08:13:06.000000 common-tools-ai-bnq-0.0.9/test/test_pymysql.py
```

### Comparing `common-tools-ai-bnq-0.0.8/PKG-INFO` & `common-tools-ai-bnq-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common tools of AI module for BNQ
 Author: BNQ
 Description-Content-Type: text/markdown
 Requires-Dist: structlog==23.1.0
 Requires-Dist: concurrent-log-handler==0.9.22
 Requires-Dist: nacos-sdk-python==0.1.12
 Requires-Dist: PyYAML==6.0.1
+Requires-Dist: cos-python-sdk-v5==1.9.28
 
 1.NacConnect类，用于连接nacos服务，获取配置文件信息
 
     NacConnect类中参数信息如下：
         server_addresses: 地址
         namespace: 命名空间
         username: 用户名
@@ -51,7 +52,23 @@
 
 3.SingletonMeta类，用于实现单例模式
 
     示例如下：
         class TestClass(metaclass=SingletonMeta):
             def __init__(self):
                 pass
+
+4.CosConnect类，用于连接腾讯云存储平台cos
+
+    CosConnect类中参数信息如下：
+        secret_id: 腾讯云secret_id
+        secret_key: 腾讯云secret_key
+        region: 腾讯云存储区域
+
+    示例如下：
+        test_data = {
+                        'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+                        'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+                        'region': 'ap-guangzhou'
+                    }
+        cos_test = CosConnect(**test_data)
+        print(cos_test())
```

### Comparing `common-tools-ai-bnq-0.0.8/README.md` & `common-tools-ai-bnq-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,8 +39,24 @@
             testLog.exception(i)
 
 3.SingletonMeta类，用于实现单例模式
 
     示例如下：
         class TestClass(metaclass=SingletonMeta):
             def __init__(self):
-                pass
+                pass
+
+4.CosConnect类，用于连接腾讯云存储平台cos
+
+    CosConnect类中参数信息如下：
+        secret_id: 腾讯云secret_id
+        secret_key: 腾讯云secret_key
+        region: 腾讯云存储区域
+
+    示例如下：
+        test_data = {
+                        'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+                        'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+                        'region': 'ap-guangzhou'
+                    }
+        cos_test = CosConnect(**test_data)
+        print(cos_test())
```

### Comparing `common-tools-ai-bnq-0.0.8/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.0.9/bnq_py_core/logger_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
         """初始化log模块
 
         Returns:
 
         """
         if self.log_record_path is None:
             # 获取根目录路径，并创建日志文件夹
-            self.log_record_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log")
+            # self.log_record_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log")
+            raise ValueError("log_dir is None")
+
         pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
         log_filename = os.path.join(self.log_record_path, self.__filename)
         logging.config.dictConfig({
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
                 "default": {
```

### Comparing `common-tools-ai-bnq-0.0.8/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.0.9/bnq_py_core/nacos_connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         Returns:
 
         """
         if pre_conf is None:
             pre_conf = {}
         conf_resolve = {}
         conf = self.client.get_config(data_id, group)  # 获取配置
+        self.client.add_config_watcher(data_id, group)
         if conf is None:
             return pre_conf
         if self.conf_type == "json":
             conf_resolve = json.loads(conf)  # 转换为json
         elif self.conf_type == "yaml":
             conf_resolve = yaml.load(conf, Loader=yaml.FullLoader)
         else:
```

### Comparing `common-tools-ai-bnq-0.0.8/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.0.9/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.8/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.0.9/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.8/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.0.9/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common tools of AI module for BNQ
 Author: BNQ
 Description-Content-Type: text/markdown
 Requires-Dist: structlog==23.1.0
 Requires-Dist: concurrent-log-handler==0.9.22
 Requires-Dist: nacos-sdk-python==0.1.12
 Requires-Dist: PyYAML==6.0.1
+Requires-Dist: cos-python-sdk-v5==1.9.28
 
 1.NacConnect类，用于连接nacos服务，获取配置文件信息
 
     NacConnect类中参数信息如下：
         server_addresses: 地址
         namespace: 命名空间
         username: 用户名
@@ -51,7 +52,23 @@
 
 3.SingletonMeta类，用于实现单例模式
 
     示例如下：
         class TestClass(metaclass=SingletonMeta):
             def __init__(self):
                 pass
+
+4.CosConnect类，用于连接腾讯云存储平台cos
+
+    CosConnect类中参数信息如下：
+        secret_id: 腾讯云secret_id
+        secret_key: 腾讯云secret_key
+        region: 腾讯云存储区域
+
+    示例如下：
+        test_data = {
+                        'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+                        'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+                        'region': 'ap-guangzhou'
+                    }
+        cos_test = CosConnect(**test_data)
+        print(cos_test())
```

### Comparing `common-tools-ai-bnq-0.0.8/setup.py` & `common-tools-ai-bnq-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
+        'cos-python-sdk-v5==1.9.28',
     ],
     # 其他元数据，如作者、描述等
     author='BNQ',
     description='Common tools of AI module for BNQ',
     long_description=long_description,
     long_description_content_type="text/markdown",  # 指明内容类型为markdown
 )
```

### Comparing `common-tools-ai-bnq-0.0.8/test/test_batch_triton.py` & `common-tools-ai-bnq-0.0.9/test/test_batch_triton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.8/test/test_decorator.py` & `common-tools-ai-bnq-0.0.9/test/test_decorator.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.8/test/test_global.py` & `common-tools-ai-bnq-0.0.9/test/test_global.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.8/test/test_pymysql.py` & `common-tools-ai-bnq-0.0.9/test/test_pymysql.py`

 * *Files identical despite different names*


# Comparing `tmp/yuanfen-2024.4.24.4.tar.gz` & `tmp/yuanfen-2024.4.24.5.tar.gz`

## Comparing `yuanfen-2024.4.24.4.tar` & `yuanfen-2024.4.24.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/__init__.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/config.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/email.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/env.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/group_robot.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/ip.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/logger.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/redis.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/response.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/time.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/src/yuanfen/version.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/.gitignore
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/pyproject.toml
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.4/PKG-INFO
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/__init__.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/config.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/email.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/env.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/group_robot.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/ip.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/logger.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/redis.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/response.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/time.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/src/yuanfen/version.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/.gitignore
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/pyproject.toml
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.5/PKG-INFO
```

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/__init__.py` & `yuanfen-2024.4.24.5/src/yuanfen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .env import APP_ENV
 from .group_robot import GroupRobot
 from .logger import Logger
 from .redis import Redis, RedisLock
 from .response import BaseResponse, ErrorResponse, SuccessResponse
 from .version import Version
 
-__version__ = "2024.4.24.4"
+__version__ = "2024.4.24.5"
 
 __all__ = [
     "APP_ENV",
     "BaseResponse",
     "Config",
     "Email",
     "ErrorResponse",
```

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/config.py` & `yuanfen-2024.4.24.5/src/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/email.py` & `yuanfen-2024.4.24.5/src/yuanfen/email.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/ip.py` & `yuanfen-2024.4.24.5/src/yuanfen/ip.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/logger.py` & `yuanfen-2024.4.24.5/src/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/redis.py` & `yuanfen-2024.4.24.5/src/yuanfen/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,11 +43,11 @@
     def prefixed(self, key: str):
         return f"{self.prefix}:{key}" if self.prefix else key
 
     def get(self, key: str):
         return self.redis_client.get(self.prefixed(key))
 
     def set(self, key: str, value: str, ex=None, px=None, nx=False):
-        self.redis_client.set(self.prefixed(key), value, ex=ex, px=px, nx=nx)
+        return self.redis_client.set(self.prefixed(key), value, ex=ex, px=px, nx=nx)
 
     def delete(self, key: str):
-        self.redis_client.delete(self.prefixed(key))
+        return self.redis_client.delete(self.prefixed(key))
```

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/time.py` & `yuanfen-2024.4.24.5/src/yuanfen/time.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/src/yuanfen/version.py` & `yuanfen-2024.4.24.5/src/yuanfen/version.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/.gitignore` & `yuanfen-2024.4.24.5/.gitignore`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/README.md` & `yuanfen-2024.4.24.5/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/pyproject.toml` & `yuanfen-2024.4.24.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.4/PKG-INFO` & `yuanfen-2024.4.24.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yuanfen
-Version: 2024.4.24.4
+Version: 2024.4.24.5
 Summary: Yuanfen Python Library
 Project-URL: Homepage, https://github.com/YuanfenNet/yf-lib-py
 Author-email: Bean <bean@yuanfen.net>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```


# Comparing `tmp/nb_time-1.7.tar.gz` & `tmp/nb_time-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_time-1.7.tar", last modified: Mon Apr 22 10:43:14 2024, max compression
+gzip compressed data, was "dist\nb_time-1.8.tar", last modified: Thu Apr 25 03:33:27 2024, max compression
```

## Comparing `nb_time-1.7.tar` & `nb_time-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 10:43:14.000000 nb_time-1.7/
--rw-rw-rw-   0        0        0     8849 2024-04-22 10:43:14.000000 nb_time-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     8045 2024-03-28 02:09:03.000000 nb_time-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 10:43:14.000000 nb_time-1.7/nb_time/
--rw-rw-rw-   0        0        0    14860 2024-04-22 10:42:26.000000 nb_time-1.7/nb_time/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:43:14.000000 nb_time-1.7/nb_time.egg-info/
--rw-rw-rw-   0        0        0     8849 2024-04-22 10:43:13.000000 nb_time-1.7/nb_time.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-22 10:43:13.000000 nb_time-1.7/nb_time.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 10:43:13.000000 nb_time-1.7/nb_time.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-22 10:43:13.000000 nb_time-1.7/nb_time.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 10:43:13.000000 nb_time-1.7/nb_time.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 10:43:14.000000 nb_time-1.7/setup.cfg
--rw-rw-rw-   0        0        0     2055 2024-04-22 10:42:57.000000 nb_time-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:33:27.000000 nb_time-1.8/
+-rw-rw-rw-   0        0        0     8849 2024-04-25 03:33:27.000000 nb_time-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8045 2024-03-28 02:09:03.000000 nb_time-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 03:33:27.000000 nb_time-1.8/nb_time/
+-rw-rw-rw-   0        0        0    15023 2024-04-25 03:32:48.000000 nb_time-1.8/nb_time/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:33:27.000000 nb_time-1.8/nb_time.egg-info/
+-rw-rw-rw-   0        0        0     8849 2024-04-25 03:33:25.000000 nb_time-1.8/nb_time.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-25 03:33:26.000000 nb_time-1.8/nb_time.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 03:33:25.000000 nb_time-1.8/nb_time.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-25 03:33:25.000000 nb_time-1.8/nb_time.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 03:33:25.000000 nb_time-1.8/nb_time.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 03:33:27.000000 nb_time-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2055 2024-04-25 03:33:09.000000 nb_time-1.8/setup.py
```

### Comparing `nb_time-1.7/PKG-INFO` & `nb_time-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_time
-Version: 1.7
+Version: 1.8
 Summary: Awesome time conversion handling with support for chaining operations. 
 Home-page: https://github.com/ydf0509/nb_time
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_time-1.7/README.md` & `nb_time-1.8/README.md`

 * *Files identical despite different names*

### Comparing `nb_time-1.7/nb_time/__init__.py` & `nb_time-1.8/nb_time/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import functools
+import types
 import typing
 import re
 import time
 import datetime
 import pytz
 from pydantic import BaseModel
 
@@ -67,37 +68,40 @@
         # print(f'get the system time zone is "{zone}"')
         return zone
 
     def __init__(self,
                  datetimex: typing.Union[None, int, float, datetime.datetime, str, 'NbTime', DateTimeValue] = None,
                  *,
                  datetime_formatter: str = None,
-                 time_zone: typing.Union[str, datetime.tzinfo] = None):
+                 time_zone: typing.Union[str, datetime.tzinfo,None] = None):
         """
         :param datetimex: 接受时间戳  datatime类型 和 时间字符串 和类对象本身四种类型,如果为None，则默认当前时间now。
         :param time_zone  时区例如 Asia/Shanghai， UTC  UTC+8  GMT+8  Etc/GMT-8 等,也可以是 datetime.timezone(datetime.timedelta(hours=7))东7区,
                           默认是操作系统时区
         """
         init_params = copy.copy(locals())
         init_params.pop('self')
         init_params.pop('datetimex')
         self.init_params = init_params
 
-        self.time_zone_str = time_zone or self.default_time_zone or self.get_localzone_name()
+        self.time_zone_str = self.get_time_zone_str(time_zone)
         self.datetime_formatter = datetime_formatter or self.default_formatter or self.FORMATTER_DATETIME
         '''
         将 time_zone 转成 pytz 可以识别的对应时区
         '''
         self.time_zone_obj = self.build_pytz_timezone(self.time_zone_str)
         self.datetime_obj = self.build_datetime_obj(datetimex)
         self.datetime = self.datetime_obj
 
     def _build_nb_time(self, datetimex) -> 'NbTime':
         return self.__class__(datetimex, **self.init_params)
 
+    def get_time_zone_str(self,time_zone: typing.Union[str, datetime.tzinfo,None] = None):
+        return time_zone or self.default_time_zone or self.get_localzone_name()
+
     def build_datetime_obj(self, datetimex):
         if isinstance(datetimex, DateTimeValue):
             datetime_obj = datetime.datetime(**datetimex.dict(), tzinfo=self.time_zone_obj)
         elif isinstance(datetimex, str):
             # print(self.datetime_formatter)
             if '%z' in self.datetime_formatter and ('+' not in datetimex or '-' not in datetimex):
                 datetimex = self.add_timezone_to_time_str(datetimex, self.time_zone_str)
```

### Comparing `nb_time-1.7/nb_time.egg-info/PKG-INFO` & `nb_time-1.8/nb_time.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-time
-Version: 1.7
+Version: 1.8
 Summary: Awesome time conversion handling with support for chaining operations. 
 Home-page: https://github.com/ydf0509/nb_time
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_time-1.7/setup.py` & `nb_time-1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # if os.name == 'nt':
 #     install_requires.append('pywin32')
 
 print(f'nb_time install_requires:{install_requires}')
 setup(
     name='nb_time',  #
-    version="1.7",
+    version="1.8",
     description=(
         'Awesome time conversion handling with support for chaining operations. '
     ),
     keywords=['arrow','time','datetime','time_utils'],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
```


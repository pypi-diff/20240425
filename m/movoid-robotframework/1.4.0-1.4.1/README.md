# Comparing `tmp/movoid_robotframework-1.4.0.tar.gz` & `tmp/movoid_robotframework-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.4.0.tar", last modified: Wed Apr 24 14:03:12 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.1.tar", last modified: Wed Apr 24 14:23:39 2024, max compression
```

## Comparing `movoid_robotframework-1.4.0.tar` & `movoid_robotframework-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.981059 movoid_robotframework-1.4.0/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2024-04-24 14:03:12.979885 movoid_robotframework-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.966046 movoid_robotframework-1.4.0/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.969123 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     5494 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/config.py
--rw-rw-rw-   0        0        0     4476 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.978876 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      290 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:03:12.981059 movoid_robotframework-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-24 13:51:26.000000 movoid_robotframework-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:23:39.661768 movoid_robotframework-1.4.1/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-04-24 14:23:39.659715 movoid_robotframework-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:23:39.645298 movoid_robotframework-1.4.1/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:23:39.649403 movoid_robotframework-1.4.1/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     5818 2024-04-24 14:21:04.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     4476 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.1/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:23:39.658700 movoid_robotframework-1.4.1/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-04-24 14:23:39.000000 movoid_robotframework-1.4.1/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-24 14:23:39.000000 movoid_robotframework-1.4.1/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:23:39.000000 movoid_robotframework-1.4.1/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-24 14:23:39.000000 movoid_robotframework-1.4.1/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-24 14:23:39.000000 movoid_robotframework-1.4.1/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:23:39.661768 movoid_robotframework-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-04-24 14:21:55.000000 movoid_robotframework-1.4.1/setup.py
```

### Comparing `movoid_robotframework-1.4.0/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.1/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.0/RobotFrameworkBasic/action/config.py` & `movoid_robotframework-1.4.1/RobotFrameworkBasic/action/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 class ConfigItem:
     def __init__(self, value: Any, source: str):
         self._value: Any = value
         self._root: str = source
         self._source: str = source
 
+    def __getitem__(self, item):
+        return self._value
+
     @property
     def value(self) -> Any:
         return self._value
 
     @property
     def source(self) -> str:
         return self._source
@@ -69,14 +72,15 @@
     def __config_ori_init(self, config_dict: Dict[str, Dict[str, Any]]):
         self._config_ori = {}
         for i, v in config_dict.items():
             if i.startswith('$'):
                 continue
             else:
                 self.__config_ori_update(i, v, file=False)
+        self.__config_write_file()
 
     def __config_ori_update(self, label: str, kv_dict: Dict[str, Any], override=True, file=True):
         label_now = f'${label}'
         self._config_ori[label] = {}
         self._config_ori[label_now] = {}
         for i, v in kv_dict.items():
             self._config_ori[label][i] = v
@@ -95,14 +99,18 @@
         if file:
             self.__config_write_file()
 
     def __config_write_file(self):
         temp_dict = {_k: _v for _k, _v in self._config_ori.items() if not _k.startswith('$')}
         with self._config_path.open(mode='w') as f:
             json.dump(temp_dict, f, default=lambda x: x.value)
+        temp_path = self._config_path.parent / f'${self._config_path.name}'
+        self.print(temp_path)
+        with temp_path.open(mode='w') as f:
+            json.dump(self._config_ori, f, default=lambda x: x.value)
 
     def config_use_label(self, *labels, override=True, clear=False):
         if clear:
             self._config_now.clear()
             self._config_label_list = []
         for label in labels:
             label_now = f'${label}'
```

### Comparing `movoid_robotframework-1.4.0/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.1/RobotFrameworkBasic/common.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.0/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.1/RobotFrameworkBasic/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.0/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.1/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.0/movoid_robotframework.egg-info/SOURCES.txt` & `movoid_robotframework-1.4.1/movoid_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.0/setup.py` & `movoid_robotframework-1.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.4.0',
+    version='1.4.1',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```


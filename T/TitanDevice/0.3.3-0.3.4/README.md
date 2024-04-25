# Comparing `tmp/TitanDevice-0.3.3.tar.gz` & `tmp/TitanDevice-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.3.tar", last modified: Wed Apr 24 10:15:31 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.4.tar", last modified: Thu Apr 25 02:18:47 2024, max compression
```

## Comparing `TitanDevice-0.3.3.tar` & `TitanDevice-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.3/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 10:15:29.000000 TitanDevice-0.3.3/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.3/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.3/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4536 2024-04-24 10:15:29.000000 TitanDevice-0.3.3/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.3/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:18:46.996854 TitanDevice-0.3.4/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-25 02:18:46.996854 TitanDevice-0.3.4/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.4/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:18:46.996854 TitanDevice-0.3.4/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-25 02:18:46.000000 TitanDevice-0.3.4/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-25 02:18:46.000000 TitanDevice-0.3.4/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-25 02:18:46.000000 TitanDevice-0.3.4/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-25 02:18:46.000000 TitanDevice-0.3.4/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-25 02:18:46.000000 TitanDevice-0.3.4/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-25 02:18:46.996854 TitanDevice-0.3.4/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-25 02:18:35.000000 TitanDevice-0.3.4/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:18:46.996854 TitanDevice-0.3.4/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3278 2024-04-25 02:18:35.000000 TitanDevice-0.3.4/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1242 2024-04-25 02:18:35.000000 TitanDevice-0.3.4/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5730 2024-04-25 02:18:35.000000 TitanDevice-0.3.4/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      465 2024-04-25 01:48:01.000000 TitanDevice-0.3.4/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.3/PKG-INFO` & `TitanDevice-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.3/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.3.4/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.3/setup.py` & `TitanDevice-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.3",
+    version="0.3.4",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.3/titan/__init__.py` & `TitanDevice-0.3.4/titan/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,87 @@
 from titan._device_exception import *
 from titan._device_manager import _DeviceManager
-from titan._device_models import DeviceInfo, FridaInfo
+from titan._device_models import DeviceInfo, FridaInfo, PackageInfo
 
 device_manager_list: list[_DeviceManager] = _DeviceManager.get_all_device_manager_list()
 
 
 def get_all_devices() -> list[DeviceInfo]:
     global device_manager_list
     device_manager_list = _DeviceManager.get_all_device_manager_list()
-    return [device.get_info() for device in device_manager_list]
+    return [device.get_device_info() for device in device_manager_list]
 
 
 def get_frida_info(
         device_serial: str,
         frida_server_name='frida-server',
         frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
-        if device.get_info().serial == device_serial:
+        if device.get_device_info().serial == device_serial:
             return device.get_frida_info(frida_server_path, frida_server_name)
     raise DeviceNoFoundException(device_serial)
 
 
 def install_frida(
         device_serial: str, frida_server_path: str,
         dist_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
-        if device.get_info().serial == device_serial:
+        if device.get_device_info().serial == device_serial:
             return device.install_frida(frida_server_path, dist_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def start_frida(
         device_serial: str, frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
-        if device.get_info().serial == device_serial:
+        if device.get_device_info().serial == device_serial:
             return device.start_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def stop_frida(
         device_serial: str, frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
-        if device.get_info().serial == device_serial:
+        if device.get_device_info().serial == device_serial:
             return device.stop_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def uninstall_frida(
         device_serial: str, frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
-        if device.get_info().serial == device_serial:
+        if device.get_device_info().serial == device_serial:
             return device.uninstall_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
+
+
+def get_installed_packages(device_serial: str) -> list[str]:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.get_installed_packages()
+    raise DeviceNoFoundException(device_serial)
+
+
+def get_package_info(device_serial: str, package_name: str) -> PackageInfo:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.get_package_info(package_name)
+    raise DeviceNoFoundException(device_serial)
+
+
+def install_package(device_serial: str, package_path: str) -> PackageInfo:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.install_package(package_path)
+    raise DeviceNoFoundException(device_serial)
+
+
+def uninstall_package(device_serial: str, package_name: str) -> list[str]:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.uninstall_package(package_name)
+    raise DeviceNoFoundException(device_serial)
```

### Comparing `TitanDevice-0.3.3/titan/_device_manager.py` & `TitanDevice-0.3.4/titan/_device_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os.path
 import subprocess
 import time
 from typing import Optional
 
+import apkutils2
 from adbutils import adb, adb_path
 
-from titan._device_exception import DeviceNoFoundException, DeviceMustBeRootedException, \
-    FridaServerNotInstalled, FridaServerNotRunning
-from titan._device_models import DeviceInfo, FridaInfo
+from titan._device_exception import *
+from titan._device_models import DeviceInfo, FridaInfo, PackageInfo
 
 
 class _DeviceManager(object):
     _device: adb.device
     _serial: str
     _is_root: bool = False
     _device_info: Optional[DeviceInfo] = None
@@ -62,25 +62,52 @@
         ).strip()
 
     def __is_root(self):
         return self.__file_exists("/system/xbin/su") or self.__file_exists(
             "/system/bin/su"
         )
 
-    def get_info(self) -> DeviceInfo:
+    def get_device_info(self) -> DeviceInfo:
         if self._device_info is None:
             self._device_info = DeviceInfo(
                 serial=self._device.serial,
                 product=self._device.prop.name,
                 model=self._device.prop.model,
                 device=self._device.prop.device,
                 is_root=self._is_root,
             )
         return self._device_info
 
+    def __is_package_installed(self, package_name: str) -> bool:
+        return package_name in self.get_installed_packages()
+
+    def get_installed_packages(self) -> list[str]:
+        return self._device.list_packages()
+
+    def get_package_info(self, package_name: str) -> PackageInfo:
+        if not self.__is_package_installed(package_name):
+            raise PackageNotInstalled(self._serial, package_name)
+        return PackageInfo(**self._device.package_info(package_name))
+
+    def install_package(
+            self, package_path, uninstall=False, no_launch=True
+    ) -> PackageInfo:
+        apk = apkutils2.APK(package_path.filepath())
+        package_name = apk.manifest.package_name
+        if (not uninstall) and self.__is_package_installed(package_name):
+            raise InstallPackageMustUninstallFirst(self._serial, package_name)
+        self._device.install(package_path, uninstall=uninstall, nolaunch=no_launch)
+        return self.get_package_info(package_name)
+
+    def uninstall_package(self, package_name) -> list[str]:
+        if not self.__is_package_installed(package_name):
+            raise PackageNotInstalled(self._serial, package_name)
+        self._device.uninstall(package_name)
+        return self.get_installed_packages()
+
     @check_is_root
     def install_frida(self, input_file_path, frida_server_path):
         self._device.push(input_file_path, frida_server_path)
         self._device.shell(f"su -c chmod +x {frida_server_path}")
         time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
```


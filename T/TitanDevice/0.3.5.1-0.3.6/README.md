# Comparing `tmp/TitanDevice-0.3.5.1.tar.gz` & `tmp/TitanDevice-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.5.1.tar", last modified: Thu Apr 25 02:45:05 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.6.tar", last modified: Thu Apr 25 06:43:19 2024, max compression
```

## Comparing `TitanDevice-0.3.5.1.tar` & `TitanDevice-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/
--rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.5.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      598 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-25 02:45:05.000000 TitanDevice-0.3.5.1/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      798 2024-04-25 02:45:02.000000 TitanDevice-0.3.5.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 02:45:05.453466 TitanDevice-0.3.5.1/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     3278 2024-04-25 02:18:35.000000 TitanDevice-0.3.5.1/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1242 2024-04-25 02:18:35.000000 TitanDevice-0.3.5.1/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6152 2024-04-25 02:43:20.000000 TitanDevice-0.3.5.1/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      472 2024-04-25 02:45:02.000000 TitanDevice-0.3.5.1/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 06:43:19.375174 TitanDevice-0.3.6/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-25 06:43:19.375174 TitanDevice-0.3.6/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.6/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 06:43:19.375174 TitanDevice-0.3.6/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-25 06:43:19.000000 TitanDevice-0.3.6/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-25 06:43:19.000000 TitanDevice-0.3.6/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-25 06:43:19.000000 TitanDevice-0.3.6/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-25 06:43:19.000000 TitanDevice-0.3.6/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-25 06:43:19.000000 TitanDevice-0.3.6/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-25 06:43:19.375174 TitanDevice-0.3.6/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-25 06:42:55.000000 TitanDevice-0.3.6/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-25 06:43:19.375174 TitanDevice-0.3.6/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4205 2024-04-25 06:42:55.000000 TitanDevice-0.3.6/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1242 2024-04-25 02:18:35.000000 TitanDevice-0.3.6/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7033 2024-04-25 06:42:55.000000 TitanDevice-0.3.6/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 TitanDevice-0.3.6/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.5.1/PKG-INFO` & `TitanDevice-0.3.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.5.1
+Version: 0.3.6
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.5.1/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.3.6/TitanDevice.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.3.5.1
+Version: 0.3.6
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.3.5.1/setup.py` & `TitanDevice-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.5.1",
+    version="0.3.6",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.5.1/titan/__init__.py` & `TitanDevice-0.3.6/titan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from titan._device_exception import *
 from titan._device_manager import _DeviceManager
-from titan._device_models import DeviceInfo, FridaInfo, PackageInfo
+from titan._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
 
 device_manager_list: list[_DeviceManager] = _DeviceManager.get_all_device_manager_list()
 
 
 def get_all_devices() -> list[DeviceInfo]:
     global device_manager_list
     device_manager_list = _DeviceManager.get_all_device_manager_list()
@@ -69,19 +69,44 @@
 def get_package_info(device_serial: str, package_name: str) -> PackageInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.get_package_info(package_name)
     raise DeviceNoFoundException(device_serial)
 
 
-def install_package(device_serial: str, package_path: str) -> PackageInfo:
+def install_package(
+        device_serial: str, package_path: str, uninstall=False, no_launch=True
+) -> PackageInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
-            return device.install_package(package_path)
+            return device.install_package(package_path, uninstall, no_launch)
     raise DeviceNoFoundException(device_serial)
 
 
 def uninstall_package(device_serial: str, package_name: str) -> list[str]:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.uninstall_package(package_name)
     raise DeviceNoFoundException(device_serial)
+
+
+def get_current_app(device_serial: str) -> RunningAppInfo:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.get_current_app()
+    raise DeviceNoFoundException(device_serial)
+
+
+def start_package(
+        device_serial: str, package_name: str, activity=None
+) -> RunningAppInfo:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.start_package(package_name, activity)
+    raise DeviceNoFoundException(device_serial)
+
+
+def stop_package(device_serial: str, package_name: str) -> RunningAppInfo:
+    for device in device_manager_list:
+        if device.get_device_info().serial == device_serial:
+            return device.stop_package(package_name)
+    raise DeviceNoFoundException(device_serial)
```

### Comparing `TitanDevice-0.3.5.1/titan/_device_exception.py` & `TitanDevice-0.3.6/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.5.1/titan/_device_manager.py` & `TitanDevice-0.3.6/titan/_device_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from typing import Optional
 
 import apkutils2
 from adbutils import adb, adb_path
 
 from titan._device_exception import *
-from titan._device_models import DeviceInfo, FridaInfo, PackageInfo
+from titan._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
 
 
 class _DeviceManager(object):
     _device: adb.device
     _serial: str
     _is_root: bool = False
     _device_info: Optional[DeviceInfo] = None
@@ -73,51 +73,14 @@
                 product=self._device.prop.name,
                 model=self._device.prop.model,
                 device=self._device.prop.device,
                 is_root=self._is_root,
             )
         return self._device_info
 
-    def __is_package_installed(self, package_name: str) -> bool:
-        return package_name in self.get_installed_packages()
-
-    def get_installed_packages(self) -> list[str]:
-        return self._device.list_packages()
-
-    def get_package_info(self, package_name: str) -> PackageInfo:
-        if not self.__is_package_installed(package_name):
-            raise PackageNotInstalled(self._serial, package_name)
-        app_info = self._device.app_info(package_name)
-        return PackageInfo(
-            package_name=app_info.package_name,
-            version_name=app_info.version_name,
-            version_code=app_info.version_code,
-            flags=app_info.flags,
-            first_install_time=app_info.first_install_time.timestamp(),
-            last_update_time=app_info.last_update_time.timestamp(),
-            path=app_info.path,
-            sub_apk_paths=app_info.sub_apk_paths
-        )
-
-    def install_package(
-            self, package_path, uninstall=False, no_launch=True
-    ) -> PackageInfo:
-        apk = apkutils2.APK(package_path.filepath())
-        package_name = apk.manifest.package_name
-        if (not uninstall) and self.__is_package_installed(package_name):
-            raise InstallPackageMustUninstallFirst(self._serial, package_name)
-        self._device.install(package_path, uninstall=uninstall, nolaunch=no_launch)
-        return self.get_package_info(package_name)
-
-    def uninstall_package(self, package_name) -> list[str]:
-        if not self.__is_package_installed(package_name):
-            raise PackageNotInstalled(self._serial, package_name)
-        self._device.uninstall(package_name)
-        return self.get_installed_packages()
-
     @check_is_root
     def install_frida(self, input_file_path, frida_server_path):
         self._device.push(input_file_path, frida_server_path)
         self._device.shell(f"su -c chmod +x {frida_server_path}")
         time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
 
@@ -154,7 +117,66 @@
     @check_is_root
     def uninstall_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c rm {frida_server_path}")
         time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
+
+    def __is_package_installed(self, package_name: str) -> bool:
+        return package_name in self.get_installed_packages()
+
+    def get_installed_packages(self) -> list[str]:
+        return self._device.list_packages()
+
+    def get_package_info(self, package_name: str) -> PackageInfo:
+        if not self.__is_package_installed(package_name):
+            raise PackageNotInstalled(self._serial, package_name)
+        app_info = self._device.app_info(package_name)
+        return PackageInfo(
+            package_name=app_info.package_name,
+            version_name=app_info.version_name,
+            version_code=app_info.version_code,
+            flags=app_info.flags,
+            first_install_time=app_info.first_install_time.timestamp(),
+            last_update_time=app_info.last_update_time.timestamp(),
+            path=app_info.path,
+            sub_apk_paths=app_info.sub_apk_paths
+        )
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
+    def get_current_app(self) -> RunningAppInfo:
+        app_current = self._device.app_current()
+        return RunningAppInfo(
+            package=app_current.package,
+            activity=app_current.activity,
+            pid=app_current.pid
+        )
+
+    def start_package(self, package_name, activity=None) -> RunningAppInfo:
+        if not self.__is_package_installed(package_name):
+            raise PackageNotInstalled(self._serial, package_name)
+        self._device.app_start(package_name, activity)
+        time.sleep(0.1)
+        return self.get_current_app()
+
+    def stop_package(self, package_name) -> RunningAppInfo:
+        if not self.__is_package_installed(package_name):
+            raise PackageNotInstalled(self._serial, package_name)
+        self._device.app_stop(package_name)
+        time.sleep(0.1)
+        return self.get_current_app()
```


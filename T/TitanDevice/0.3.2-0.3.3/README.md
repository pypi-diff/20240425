# Comparing `tmp/TitanDevice-0.3.2.tar.gz` & `tmp/TitanDevice-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.2.tar", last modified: Wed Apr 24 10:08:51 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.3.tar", last modified: Wed Apr 24 10:15:31 2024, max compression
```

## Comparing `TitanDevice-0.3.2.tar` & `TitanDevice-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.2/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 10:08:49.000000 TitanDevice-0.3.2/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.2/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.2/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4708 2024-04-24 10:08:49.000000 TitanDevice-0.3.2/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.2/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.3/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 10:15:31.000000 TitanDevice-0.3.3/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 10:15:29.000000 TitanDevice-0.3.3/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:15:31.198907 TitanDevice-0.3.3/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.3/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.3/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4536 2024-04-24 10:15:29.000000 TitanDevice-0.3.3/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.3/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.2/setup.py` & `TitanDevice-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.2",
+    version="0.3.3",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.2/titan/__init__.py` & `TitanDevice-0.3.3/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.2/titan/_device_exception.py` & `TitanDevice-0.3.3/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.2/titan/_device_manager.py` & `TitanDevice-0.3.3/titan/_device_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,19 +74,19 @@
                 model=self._device.prop.model,
                 device=self._device.prop.device,
                 is_root=self._is_root,
             )
         return self._device_info
 
     @check_is_root
-    def install_frida(self, file_path, dist_path):
-        self._device.push(file_path, dist_path)
-        self._device.shell(f"su -c chmod 755 {dist_path}")
-        self._device.shell(f"su -c {dist_path} &")
-        return self.get_frida_info(dist_path)
+    def install_frida(self, input_file_path, frida_server_path):
+        self._device.push(input_file_path, frida_server_path)
+        self._device.shell(f"su -c chmod +x {frida_server_path}")
+        time.sleep(0.1)
+        return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def get_frida_info(self, frida_server_path, frida_server_name=None) -> FridaInfo:
         if frida_server_name is None:
             frida_server_name = self.get_frida_server_name_from_path(frida_server_path)
         return FridaInfo(
             is_running=self.__is_frida_running(frida_server_name),
@@ -94,33 +94,30 @@
             version=self.__get_frida_version(frida_server_path)
         )
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
-        while not self.__is_frida_running(
-                self.get_frida_server_name_from_path(frida_server_path)
-        ):
-            subprocess.Popen(
-                [adb_path(), '-s', self._serial, 'shell', 'nohup',
-                 'su -c "{}" &'.format(frida_server_path)]
-            )
-            time.sleep(0.1)
+        subprocess.Popen(
+            [adb_path(), '-s', self._serial, 'shell', 'nohup',
+             'su -c "{}" &'.format(frida_server_path)]
+        )
+        time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def stop_frida(self, frida_server_path):
         frida_server_name = self.get_frida_server_name_from_path(frida_server_path)
         if not self.__is_frida_running(frida_server_name):
             raise FridaServerNotRunning(self._serial, frida_server_name)
-        while self.__is_frida_running(frida_server_name):
-            self._device.shell(f"su -c pkill {frida_server_name}")
-            time.sleep(0.1)
+        self._device.shell(f"su -c pkill {frida_server_name}")
+        time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def uninstall_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c rm {frida_server_path}")
+        time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
```


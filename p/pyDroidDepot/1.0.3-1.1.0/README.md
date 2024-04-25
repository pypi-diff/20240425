# Comparing `tmp/pyDroidDepot-1.0.3.tar.gz` & `tmp/pydroiddepot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDroidDepot-1.0.3.tar", last modified: Sat Aug 26 23:40:17 2023, max compression
+gzip compressed data, was "pydroiddepot-1.1.0.tar", last modified: Thu Apr 25 06:14:59 2024, max compression
```

## Comparing `pyDroidDepot-1.0.3.tar` & `pydroiddepot-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:40:17.340460 pyDroidDepot-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (999)     1071 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1655 2023-08-26 23:40:17.340460 pyDroidDepot-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1267 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:40:17.340460 pyDroidDepot-1.0.3/droiddepot/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8273 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/audio.py
--rw-r--r--   0 runner    (1001) docker     (999)     1005 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/beacon.py
--rw-r--r--   0 runner    (1001) docker     (999)    13477 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/connection.py
--rw-r--r--   0 runner    (1001) docker     (999)    11254 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/hardware.py
--rw-r--r--   0 runner    (1001) docker     (999)     5345 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/motor.py
--rw-r--r--   0 runner    (1001) docker     (999)     8492 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/notify.py
--rw-r--r--   0 runner    (1001) docker     (999)     2923 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/protocol.py
--rw-r--r--   0 runner    (1001) docker     (999)     7640 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/script.py
--rw-r--r--   0 runner    (1001) docker     (999)     1728 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     3392 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/droiddepot/voice.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:40:17.340460 pyDroidDepot-1.0.3/pyDroidDepot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1655 2023-08-26 23:40:17.000000 pyDroidDepot-1.0.3/pyDroidDepot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      407 2023-08-26 23:40:17.000000 pyDroidDepot-1.0.3/pyDroidDepot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-26 23:40:17.000000 pyDroidDepot-1.0.3/pyDroidDepot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-26 23:40:17.000000 pyDroidDepot-1.0.3/pyDroidDepot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-26 23:40:17.340460 pyDroidDepot-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      727 2023-08-26 23:40:06.000000 pyDroidDepot-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:14:59.452071 pydroiddepot-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-25 06:14:59.452071 pydroiddepot-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:14:59.452071 pydroiddepot-1.1.0/droiddepot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/droiddepot/voice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:14:59.452071 pydroiddepot-1.1.0/pyDroidDepot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-25 06:14:59.000000 pydroiddepot-1.1.0/pyDroidDepot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-25 06:14:59.000000 pydroiddepot-1.1.0/pyDroidDepot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:14:59.000000 pydroiddepot-1.1.0/pyDroidDepot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 06:14:59.000000 pydroiddepot-1.1.0/pyDroidDepot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:14:59.452071 pydroiddepot-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 06:14:52.000000 pydroiddepot-1.1.0/setup.py
```

### Comparing `pyDroidDepot-1.0.3/LICENSE` & `pydroiddepot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/PKG-INFO` & `pydroiddepot-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDroidDepot
-Version: 1.0.3
+Version: 1.1.0
 Summary: Module for controlling droids built and purchased at the Droid Depot in Disney's Galaxys Edge
 Home-page: https://github.com/thetestgame/pyDroidDepot
 Author: Jordan Maxwell
 Maintainer: Jordan Maxwell
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,14 +12,22 @@
 
 <img src="https://static.wikia.nocookie.net/frstarwars/images/e/e4/Logo_Droid_Depot_SWGE.png/revision/latest?cb=20200730141444" align="right" width="150">
 
 # PyDroidDepot
 
 PyDroidDepot is an open-source project that aims to provide Python access to the Starwars Galaxy's Edge droid depot droids. It allows users to manually control their custom built droids using custom applications.
 
+# Supported Droid Types
+
+* R Units 
+* B Unit (WIP)
+* BD Unit (WIP)
+
+Droids types that are marked as work in progress will function though they may have unexpected behaviour or may be missing functionality.
+
 ## Installation
 
 PyDroidDepot can be installed using `pip`, or by downloading the source code and running the `setup.py` script.
 
 ### Installing with pip
 
 To install PyDroidDepot using `pip`, simply run:
```

### Comparing `pyDroidDepot-1.0.3/README.md` & `pydroiddepot-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 <img src="https://static.wikia.nocookie.net/frstarwars/images/e/e4/Logo_Droid_Depot_SWGE.png/revision/latest?cb=20200730141444" align="right" width="150">
 
 # PyDroidDepot
 
 PyDroidDepot is an open-source project that aims to provide Python access to the Starwars Galaxy's Edge droid depot droids. It allows users to manually control their custom built droids using custom applications.
 
+# Supported Droid Types
+
+* R Units 
+* B Unit (WIP)
+* BD Unit (WIP)
+
+Droids types that are marked as work in progress will function though they may have unexpected behaviour or may be missing functionality.
+
 ## Installation
 
 PyDroidDepot can be installed using `pip`, or by downloading the source code and running the `setup.py` script.
 
 ### Installing with pip
 
 To install PyDroidDepot using `pip`, simply run:
```

### Comparing `pyDroidDepot-1.0.3/droiddepot/audio.py` & `pydroiddepot-1.1.0/droiddepot/audio.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/beacon.py` & `pydroiddepot-1.1.0/droiddepot/beacon.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/connection.py` & `pydroiddepot-1.1.0/droiddepot/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,19 +269,17 @@
         retry (bool): whether or not to continue scanning until a device is found or the function is interrupted
 
     Returns:
         a list of DroidConnection objects representing the discovered "DROID" Bluetooth devices if any. Otherwise an empty list
     """
 
     async with BleakScanner() as scanner:      
-        await scanner.start()
-
         droid_connections = []
-
         droids = []
+        
         while True:
             possible_droids = scanner.discovered_devices_and_advertisement_data
             if len(possible_droids) == 0:
                 await asyncio.sleep(5)
                 continue
 
             for possible_droid_address in possible_droids:
```

### Comparing `pyDroidDepot-1.0.3/droiddepot/hardware.py` & `pydroiddepot-1.1.0/droiddepot/hardware.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/motor.py` & `pydroiddepot-1.1.0/droiddepot/motor.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/notify.py` & `pydroiddepot-1.1.0/droiddepot/notify.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/protocol.py` & `pydroiddepot-1.1.0/droiddepot/protocol.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/script.py` & `pydroiddepot-1.1.0/droiddepot/script.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/utils.py` & `pydroiddepot-1.1.0/droiddepot/utils.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/droiddepot/voice.py` & `pydroiddepot-1.1.0/droiddepot/voice.py`

 * *Files identical despite different names*

### Comparing `pyDroidDepot-1.0.3/pyDroidDepot.egg-info/PKG-INFO` & `pydroiddepot-1.1.0/pyDroidDepot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDroidDepot
-Version: 1.0.3
+Version: 1.1.0
 Summary: Module for controlling droids built and purchased at the Droid Depot in Disney's Galaxys Edge
 Home-page: https://github.com/thetestgame/pyDroidDepot
 Author: Jordan Maxwell
 Maintainer: Jordan Maxwell
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -12,14 +12,22 @@
 
 <img src="https://static.wikia.nocookie.net/frstarwars/images/e/e4/Logo_Droid_Depot_SWGE.png/revision/latest?cb=20200730141444" align="right" width="150">
 
 # PyDroidDepot
 
 PyDroidDepot is an open-source project that aims to provide Python access to the Starwars Galaxy's Edge droid depot droids. It allows users to manually control their custom built droids using custom applications.
 
+# Supported Droid Types
+
+* R Units 
+* B Unit (WIP)
+* BD Unit (WIP)
+
+Droids types that are marked as work in progress will function though they may have unexpected behaviour or may be missing functionality.
+
 ## Installation
 
 PyDroidDepot can be installed using `pip`, or by downloading the source code and running the `setup.py` script.
 
 ### Installing with pip
 
 To install PyDroidDepot using `pip`, simply run:
```

### Comparing `pyDroidDepot-1.0.3/setup.py` & `pydroiddepot-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 setup(
     name='pyDroidDepot',
     description="Module for controlling droids built and purchased at the Droid Depot in Disney's Galaxys Edge",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
-    version='1.0.3',
+    version='1.1.0',
     author='Jordan Maxwell',
     maintainer='Jordan Maxwell',
     url='https://github.com/thetestgame/pyDroidDepot',
     packages=['droiddepot'],
     classifiers=[
         'Programming Language :: Python :: 3',
     ])
```


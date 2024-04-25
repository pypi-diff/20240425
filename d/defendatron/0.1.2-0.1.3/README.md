# Comparing `tmp/defendatron-0.1.2.tar.gz` & `tmp/defendatron-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defendatron-0.1.2.tar", last modified: Wed Apr 24 02:47:04 2024, max compression
+gzip compressed data, was "defendatron-0.1.3.tar", last modified: Thu Apr 25 17:40:17 2024, max compression
```

## Comparing `defendatron-0.1.2.tar` & `defendatron-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:04.977945 defendatron-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:46:56.000000 defendatron-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-24 02:47:04.977945 defendatron-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 02:46:56.000000 defendatron-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:47:04.977945 defendatron-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 02:46:56.000000 defendatron-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:04.973945 defendatron-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:04.977945 defendatron-0.1.2/src/defendatron/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 02:46:56.000000 defendatron-0.1.2/src/defendatron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:47:04.977945 defendatron-0.1.2/src/defendatron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-24 02:47:04.000000 defendatron-0.1.2/src/defendatron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-24 02:47:04.000000 defendatron-0.1.2/src/defendatron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:47:04.000000 defendatron-0.1.2/src/defendatron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 02:47:04.000000 defendatron-0.1.2/src/defendatron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 02:47:04.000000 defendatron-0.1.2/src/defendatron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:40:17.450476 defendatron-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:40:13.000000 defendatron-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-25 17:40:17.450476 defendatron-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-25 17:40:13.000000 defendatron-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:40:17.450476 defendatron-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-25 17:40:13.000000 defendatron-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:40:17.446476 defendatron-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:40:17.450476 defendatron-0.1.3/src/defendatron/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-25 17:40:13.000000 defendatron-0.1.3/src/defendatron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 17:40:13.000000 defendatron-0.1.3/src/defendatron/nullscream_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:40:17.450476 defendatron-0.1.3/src/defendatron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-25 17:40:17.000000 defendatron-0.1.3/src/defendatron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-25 17:40:17.000000 defendatron-0.1.3/src/defendatron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:40:17.000000 defendatron-0.1.3/src/defendatron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 17:40:17.000000 defendatron-0.1.3/src/defendatron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 17:40:17.000000 defendatron-0.1.3/src/defendatron.egg-info/top_level.txt
```

### Comparing `defendatron-0.1.2/LICENSE` & `defendatron-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.2/PKG-INFO` & `defendatron-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nullscream==0.1.0
-Requires-Dist: darklock==0.1.0
-Requires-Dist: shadowlogger==0.1.0
+Requires-Dist: nullscream==0.1.2
+Requires-Dist: darklock==0.1.2
+Requires-Dist: shadowlogger==0.1.1
 
 # Defendatron
 
-Defendatron is a simple coordinator for `Protectbots`, Python modules that provide security features for your applications.
+Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
 
 ![img_1.png](img.png)
 
 [![Upload Python Package](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml)
 
@@ -31,38 +31,38 @@
 ```
 
 ## Usage
 
 ```python
 import defendatron
 
-# Activate defendatron (all protectbots)
+# Activate defendatron (all Protectabots)
 defendatron.activate()
 
-# Deactivate defendatron (all protectbots)
+# Deactivate defendatron (all Protectabots)
 defendatron.deactivate()
 
-# Activate specific protectbots
+# Activate specific Protectabots
 defendatron.nullscream.activate()
 defendatron.shadowlogger.activate()
 defendatron.darklock.activate()
 
-# Deactivate specific protectbots
+# Deactivate specific Protectabots
 defendatron.nullscream.deactivate()
 defendatron.shadowlogger.deactivate()
 defendatron.darklock.deactivate()
 ```
 
 See `src/defendatron/__init__.py` for more advanced usage.
 
-## When Protecbots assemble, they create DEFENDATRON
+## When Protectabots assemble, they create Defendatron
 ![img_2.png](img_1.png)
 
 ---
 
-Defendatron is built with `Protectbots`, Python modules that provide security features for your applications. 
-Each `Protectbot` is designed to defend against specific threats and vulnerabilities, 
+Defendatron is built with `Protectabots`, Python modules that provide security features for your applications. 
+Each `Protectabot` is designed to defend against specific threats and vulnerabilities, 
 helping to provide another layer of protection for your code. 
 
-- [NULLSCREAM](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
-- [DARKLOCK](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
-- [SHADOWLOGGER](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
+- [nullscream](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
+- [darklock](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
+- [shadowlogger](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
```

### Comparing `defendatron-0.1.2/README.md` & `defendatron-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Defendatron
 
-Defendatron is a simple coordinator for `Protectbots`, Python modules that provide security features for your applications.
+Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
 
 ![img_1.png](img.png)
 
 [![Upload Python Package](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml)
 
@@ -17,38 +17,38 @@
 ```
 
 ## Usage
 
 ```python
 import defendatron
 
-# Activate defendatron (all protectbots)
+# Activate defendatron (all Protectabots)
 defendatron.activate()
 
-# Deactivate defendatron (all protectbots)
+# Deactivate defendatron (all Protectabots)
 defendatron.deactivate()
 
-# Activate specific protectbots
+# Activate specific Protectabots
 defendatron.nullscream.activate()
 defendatron.shadowlogger.activate()
 defendatron.darklock.activate()
 
-# Deactivate specific protectbots
+# Deactivate specific Protectabots
 defendatron.nullscream.deactivate()
 defendatron.shadowlogger.deactivate()
 defendatron.darklock.deactivate()
 ```
 
 See `src/defendatron/__init__.py` for more advanced usage.
 
-## When Protecbots assemble, they create DEFENDATRON
+## When Protectabots assemble, they create Defendatron
 ![img_2.png](img_1.png)
 
 ---
 
-Defendatron is built with `Protectbots`, Python modules that provide security features for your applications. 
-Each `Protectbot` is designed to defend against specific threats and vulnerabilities, 
+Defendatron is built with `Protectabots`, Python modules that provide security features for your applications. 
+Each `Protectabot` is designed to defend against specific threats and vulnerabilities, 
 helping to provide another layer of protection for your code. 
 
-- [NULLSCREAM](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
-- [DARKLOCK](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
-- [SHADOWLOGGER](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
+- [nullscream](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
+- [darklock](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
+- [shadowlogger](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
```

### Comparing `defendatron-0.1.2/setup.py` & `defendatron-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="defendatron",
-    version="0.1.2",
+    version="0.1.3",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
     url="https://github.com/Capsize-Games/defendatron",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "nullscream==0.1.0",
-        "darklock==0.1.0",
-        "shadowlogger==0.1.0",
+        "nullscream==0.1.2",
+        "darklock==0.1.2",
+        "shadowlogger==0.1.1",
     ],
     dependency_links=[
     ],
 )
```

### Comparing `defendatron-0.1.2/src/defendatron/__init__.py` & `defendatron-0.1.3/src/defendatron/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import shadowlogger
 import darklock
 import nullscream
+from defendatron.nullscream_tracker import NullscreamTracker
 
+nullscream_tracker = NullscreamTracker()
 
 def activate(
     # Nullscream properties
     nullscream_blacklist: list = None,
     nullscream_whitelist: list = None,
+    nullscream_function_blacklist: list = None,
 
     # darklock properites
     darklock_os_whitelisted_operations: list = None,
     darklock_os_whitelisted_filenames: list = None,
     darklock_os_whitelisted_imports: list = None,
     darklock_os_blacklisted_filenames: list = None,
 
     activate_shadowlogger: bool = False,
     activate_darklock: bool = False,
     activate_nullscream: bool = False,
+
+    # Shadowlogger properties
+    show_stdout: bool = True
 ):
     print("Activating defendatron")
     if activate_shadowlogger:
-        print("Activating shadow logger")
-        shadowlogger.manager.activate()
+        print("Activating shadowlogger")
+        shadowlogger.manager.activate(
+            show_stdout=show_stdout,
+            trackers=[nullscream_tracker],
+        )
 
     if activate_darklock:
         print("Activating darklock")
         darklock.activate(
             whitelisted_operations=darklock_os_whitelisted_operations,
             whitelisted_filenames=darklock_os_whitelisted_filenames,
             whitelisted_imports=darklock_os_whitelisted_imports,
@@ -33,14 +42,15 @@
         )
 
     if activate_nullscream:
         print("Activating nullscream")
         nullscream.activate(
             blacklist=nullscream_blacklist,
             whitelist=nullscream_whitelist,
+            function_blacklist=nullscream_function_blacklist,
         )
 
 
 def deactivate(
     # Nullscream properties
     nullscream_blacklist: list = None,
 ):
```

### Comparing `defendatron-0.1.2/src/defendatron.egg-info/PKG-INFO` & `defendatron-0.1.3/src/defendatron.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nullscream==0.1.0
-Requires-Dist: darklock==0.1.0
-Requires-Dist: shadowlogger==0.1.0
+Requires-Dist: nullscream==0.1.2
+Requires-Dist: darklock==0.1.2
+Requires-Dist: shadowlogger==0.1.1
 
 # Defendatron
 
-Defendatron is a simple coordinator for `Protectbots`, Python modules that provide security features for your applications.
+Defendatron is a simple coordinator for `Protectabots`, Python modules that provide security features for your applications.
 
 ---
 
 ![img_1.png](img.png)
 
 [![Upload Python Package](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml)
 
@@ -31,38 +31,38 @@
 ```
 
 ## Usage
 
 ```python
 import defendatron
 
-# Activate defendatron (all protectbots)
+# Activate defendatron (all Protectabots)
 defendatron.activate()
 
-# Deactivate defendatron (all protectbots)
+# Deactivate defendatron (all Protectabots)
 defendatron.deactivate()
 
-# Activate specific protectbots
+# Activate specific Protectabots
 defendatron.nullscream.activate()
 defendatron.shadowlogger.activate()
 defendatron.darklock.activate()
 
-# Deactivate specific protectbots
+# Deactivate specific Protectabots
 defendatron.nullscream.deactivate()
 defendatron.shadowlogger.deactivate()
 defendatron.darklock.deactivate()
 ```
 
 See `src/defendatron/__init__.py` for more advanced usage.
 
-## When Protecbots assemble, they create DEFENDATRON
+## When Protectabots assemble, they create Defendatron
 ![img_2.png](img_1.png)
 
 ---
 
-Defendatron is built with `Protectbots`, Python modules that provide security features for your applications. 
-Each `Protectbot` is designed to defend against specific threats and vulnerabilities, 
+Defendatron is built with `Protectabots`, Python modules that provide security features for your applications. 
+Each `Protectabot` is designed to defend against specific threats and vulnerabilities, 
 helping to provide another layer of protection for your code. 
 
-- [NULLSCREAM](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
-- [DARKLOCK](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
-- [SHADOWLOGGER](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
+- [nullscream](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
+- [darklock](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
+- [shadowlogger](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
```


# Comparing `tmp/TineAutomationToolkit-1.0.6.tar.gz` & `tmp/TineAutomationToolkit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.0.6.tar", last modified: Fri Apr 19 09:33:36 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.0.7.tar", last modified: Thu Apr 25 03:31:54 2024, max compression
```

## Comparing `TineAutomationToolkit-1.0.6.tar` & `TineAutomationToolkit-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/
--rw-rw-rw-   0        0        0     2280 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      383 2024-04-17 15:32:05.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/
--rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/detectelement.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      724 2024-04-17 15:54:04.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0    18183 2024-04-19 08:45:03.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/keyevent.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/touch.py
--rw-rw-rw-   0        0        0     8386 2024-04-19 09:32:00.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-19 08:43:21.000000 TineAutomationToolkit-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/
+-rw-rw-rw-   0        0        0     2280 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      403 2024-04-25 03:30:22.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/detect/
+-rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/detect/detectelement.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      812 2024-04-25 03:30:23.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    18183 2024-04-19 08:45:03.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     1255 2024-04-25 03:30:34.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/convertobject.py
+-rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/keyevent.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/touch.py
+-rw-rw-rw-   0        0        0     8386 2024-04-19 09:32:00.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 03:31:54.000000 TineAutomationToolkit-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-25 03:18:32.000000 TineAutomationToolkit-1.0.7/setup.py
```

### Comparing `TineAutomationToolkit-1.0.6/PKG-INFO` & `TineAutomationToolkit-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.6/README.md` & `TineAutomationToolkit-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/detectelement.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/detect/detectelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,9 +4,10 @@
 from TineAutomationToolkit.keywords.controlelement import ControlElement
 from TineAutomationToolkit.keywords.waitingelement import WaitingElement
 from TineAutomationToolkit.keywords.scroll import Scroll
 from TineAutomationToolkit.keywords.toolkitstest import ToolkitsTest
 from TineAutomationToolkit.keywords.capturescreenshot import CaptureScreenShot
 from TineAutomationToolkit.keywords.keyevent import KeyEvent
 from TineAutomationToolkit.keywords.touch import Touch
+from TineAutomationToolkit.keywords.convertobject import ConvertObject
 
-__all__ = ['ToolkitsTest' , 'ConnectionManagement', 'WaitingElement', 'ControlElement','Scroll','CaptureScreenShot','KeyEvent','Touch']
+__all__ = ['ToolkitsTest' , 'ConnectionManagement', 'WaitingElement', 'ControlElement','Scroll','CaptureScreenShot','KeyEvent','Touch','ConvertObject']
```

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/controlelement.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/controlelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/keyevent.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/keyevent.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/touch.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/touch.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.0.7/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 TineAutomationToolkit.egg-info/top_level.txt
 TineAutomationToolkit/detect/__init__.py
 TineAutomationToolkit/detect/detectelement.py
 TineAutomationToolkit/keywords/__init__.py
 TineAutomationToolkit/keywords/capturescreenshot.py
 TineAutomationToolkit/keywords/connectionmanagement.py
 TineAutomationToolkit/keywords/controlelement.py
+TineAutomationToolkit/keywords/convertobject.py
 TineAutomationToolkit/keywords/keyevent.py
 TineAutomationToolkit/keywords/scroll.py
 TineAutomationToolkit/keywords/toolkitstest.py
 TineAutomationToolkit/keywords/touch.py
 TineAutomationToolkit/keywords/waitingelement.py
```

### Comparing `TineAutomationToolkit-1.0.6/setup.py` & `TineAutomationToolkit-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.0.6",
+    version="1.0.7",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```


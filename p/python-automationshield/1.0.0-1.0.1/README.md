# Comparing `tmp/python_automationshield-1.0.0.tar.gz` & `tmp/python_automationshield-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_automationshield-1.0.0.tar", max compression
+gzip compressed data, was "python_automationshield-1.0.1.tar", max compression
```

## Comparing `python_automationshield-1.0.0.tar` & `python_automationshield-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1079 2024-04-23 09:48:31.740728 python_automationshield-1.0.0/LICENSE
--rw-r--r--   0        0        0     4590 2024-04-23 09:48:31.740728 python_automationshield-1.0.0/README.md
--rw-r--r--   0        0        0      752 2024-04-23 09:48:31.741729 python_automationshield-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      776 2024-04-23 09:48:31.741729 python_automationshield-1.0.0/src/automationshield/__init__.py
--rw-r--r--   0        0        0     4473 2024-04-23 09:48:31.741729 python_automationshield-1.0.0/src/automationshield/arduino.py
--rw-r--r--   0        0        0      113 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
--rw-r--r--   0        0        0      115 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/floatshield/floatshield.ino
--rw-r--r--   0        0        0      418 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
--rw-r--r--   0        0        0      447 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
--rw-r--r--   0        0        0     2481 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
--rw-r--r--   0        0        0      986 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
--rw-r--r--   0        0        0      356 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
--rw-r--r--   0        0        0      367 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
--rw-r--r--   0        0        0      122 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
--rw-r--r--   0        0        0      269 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
--rw-r--r--   0        0        0      119 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
--rw-r--r--   0        0        0     7525 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/controller.py
--rw-r--r--   0        0        0       52 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/exception.py
--rw-r--r--   0        0        0       67 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/plotting/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/plotting/live_plotter.py
--rw-r--r--   0        0        0     1615 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/plotting/plotter.py
--rw-r--r--   0        0        0      186 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/shields/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/shields/aeroshield.py
--rw-r--r--   0        0        0    11855 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/baseshield.py
--rw-r--r--   0        0        0      468 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/dummyshield.py
--rw-r--r--   0        0        0     1060 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/floatshield.py
--rw-r--r--   0        0        0     6933 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/magnetoshield.py
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 python_automationshield-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-25 12:50:24.364680 python_automationshield-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4590 2024-04-25 12:50:24.364680 python_automationshield-1.0.1/README.md
+-rw-r--r--   0        0        0      752 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      782 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/__init__.py
+-rw-r--r--   0        0        0     4473 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino.py
+-rw-r--r--   0        0        0      113 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
+-rw-r--r--   0        0        0      115 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/floatshield/floatshield.ino
+-rw-r--r--   0        0        0      418 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
+-rw-r--r--   0        0        0      447 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
+-rw-r--r--   0        0        0     2481 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
+-rw-r--r--   0        0        0      986 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
+-rw-r--r--   0        0        0      356 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
+-rw-r--r--   0        0        0      367 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
+-rw-r--r--   0        0        0      122 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
+-rw-r--r--   0        0        0      269 2024-04-25 12:50:24.365680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
+-rw-r--r--   0        0        0      119 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
+-rw-r--r--   0        0        0     7525 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/controller.py
+-rw-r--r--   0        0        0       52 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/exception.py
+-rw-r--r--   0        0        0       67 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/plotting/__init__.py
+-rw-r--r--   0        0        0     2692 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/plotting/live_plotter.py
+-rw-r--r--   0        0        0     1615 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/plotting/plotter.py
+-rw-r--r--   0        0        0      186 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/shields/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/shields/aeroshield.py
+-rw-r--r--   0        0        0    11855 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/shields/baseshield.py
+-rw-r--r--   0        0        0      468 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/shields/dummyshield.py
+-rw-r--r--   0        0        0     1060 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/shields/floatshield.py
+-rw-r--r--   0        0        0     6933 2024-04-25 12:50:24.366680 python_automationshield-1.0.1/src/automationshield/shields/magnetoshield.py
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 python_automationshield-1.0.1/PKG-INFO
```

### Comparing `python_automationshield-1.0.0/LICENSE` & `python_automationshield-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/README.md` & `python_automationshield-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/pyproject.toml` & `python_automationshield-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-automationshield"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python interface to AutomationShield's Arduino shields"
 authors = ["Bert Van den Abbeele"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/mrtreasurer/python-automationshield"
 documentation = "https://python-automationshield.readthedocs.io"
 packages = [
```

### Comparing `python_automationshield-1.0.0/src/automationshield/__init__.py` & `python_automationshield-1.0.1/src/automationshield/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # read version from installed package
 from importlib.metadata import version
-__version__ = version("python_aeroshield")
+__version__ = version("python_automationshield")
 
 from .controller import ShieldController
 from .exception import AutomationShieldException
 from .shields import AeroShield, FloatShield, MagnetoShield, DummyShield
 
 
 import platform
```

### Comparing `python_automationshield-1.0.0/src/automationshield/arduino.py` & `python_automationshield-1.0.1/src/automationshield/arduino.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp` & `python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h` & `python_automationshield-1.0.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/controller.py` & `python_automationshield-1.0.1/src/automationshield/controller.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/plotting/live_plotter.py` & `python_automationshield-1.0.1/src/automationshield/plotting/live_plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/plotting/plotter.py` & `python_automationshield-1.0.1/src/automationshield/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/shields/aeroshield.py` & `python_automationshield-1.0.1/src/automationshield/shields/aeroshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/shields/baseshield.py` & `python_automationshield-1.0.1/src/automationshield/shields/baseshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/shields/floatshield.py` & `python_automationshield-1.0.1/src/automationshield/shields/floatshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/src/automationshield/shields/magnetoshield.py` & `python_automationshield-1.0.1/src/automationshield/shields/magnetoshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.0/PKG-INFO` & `python_automationshield-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automationshield
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python interface to AutomationShield's Arduino shields
 Home-page: https://gitlab.com/mrtreasurer/python-automationshield
 License: MIT
 Author: Bert Van den Abbeele
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


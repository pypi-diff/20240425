# Comparing `tmp/python_automationshield-1.0.2.tar.gz` & `tmp/python_automationshield-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_automationshield-1.0.2.tar", max compression
+gzip compressed data, was "python_automationshield-1.0.3.tar", max compression
```

## Comparing `python_automationshield-1.0.2.tar` & `python_automationshield-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1079 2024-04-25 12:55:35.355505 python_automationshield-1.0.2/LICENSE
--rw-r--r--   0        0        0     4590 2024-04-25 12:55:35.355505 python_automationshield-1.0.2/README.md
--rw-r--r--   0        0        0      752 2024-04-25 12:55:35.356505 python_automationshield-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      782 2024-04-25 12:55:35.356505 python_automationshield-1.0.2/src/automationshield/__init__.py
--rw-r--r--   0        0        0     4473 2024-04-25 12:55:35.356505 python_automationshield-1.0.2/src/automationshield/arduino.py
--rw-r--r--   0        0        0      113 2024-04-25 12:55:35.356505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
--rw-r--r--   0        0        0      115 2024-04-25 12:55:35.356505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/floatshield/floatshield.ino
--rw-r--r--   0        0        0      418 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
--rw-r--r--   0        0        0      447 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
--rw-r--r--   0        0        0     2481 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
--rw-r--r--   0        0        0      986 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
--rw-r--r--   0        0        0      356 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
--rw-r--r--   0        0        0      367 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
--rw-r--r--   0        0        0      122 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
--rw-r--r--   0        0        0      269 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
--rw-r--r--   0        0        0      119 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
--rw-r--r--   0        0        0     7525 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/controller.py
--rw-r--r--   0        0        0       52 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/exception.py
--rw-r--r--   0        0        0       67 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/plotting/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/plotting/live_plotter.py
--rw-r--r--   0        0        0     1615 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/plotting/plotter.py
--rw-r--r--   0        0        0      186 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/shields/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-25 12:55:35.357505 python_automationshield-1.0.2/src/automationshield/shields/aeroshield.py
--rw-r--r--   0        0        0    11855 2024-04-25 12:55:35.358505 python_automationshield-1.0.2/src/automationshield/shields/baseshield.py
--rw-r--r--   0        0        0      468 2024-04-25 12:55:35.358505 python_automationshield-1.0.2/src/automationshield/shields/dummyshield.py
--rw-r--r--   0        0        0     1060 2024-04-25 12:55:35.358505 python_automationshield-1.0.2/src/automationshield/shields/floatshield.py
--rw-r--r--   0        0        0     6892 2024-04-25 12:55:35.358505 python_automationshield-1.0.2/src/automationshield/shields/magnetoshield.py
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 python_automationshield-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-25 13:39:55.334700 python_automationshield-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4590 2024-04-25 13:39:55.334700 python_automationshield-1.0.3/README.md
+-rw-r--r--   0        0        0      752 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      655 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/__init__.py
+-rw-r--r--   0        0        0     4473 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino.py
+-rw-r--r--   0        0        0      113 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
+-rw-r--r--   0        0        0      115 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/floatshield/floatshield.ino
+-rw-r--r--   0        0        0      418 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
+-rw-r--r--   0        0        0      447 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
+-rw-r--r--   0        0        0     2481 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
+-rw-r--r--   0        0        0      986 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
+-rw-r--r--   0        0        0      356 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
+-rw-r--r--   0        0        0      367 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
+-rw-r--r--   0        0        0      122 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
+-rw-r--r--   0        0        0      269 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
+-rw-r--r--   0        0        0      119 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
+-rw-r--r--   0        0        0     7525 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/controller.py
+-rw-r--r--   0        0        0       52 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/exception.py
+-rw-r--r--   0        0        0       67 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/plotting/__init__.py
+-rw-r--r--   0        0        0     2692 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/plotting/live_plotter.py
+-rw-r--r--   0        0        0     1615 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/plotting/plotter.py
+-rw-r--r--   0        0        0      186 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/aeroshield.py
+-rw-r--r--   0        0        0    11947 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/baseshield.py
+-rw-r--r--   0        0        0      468 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/dummyshield.py
+-rw-r--r--   0        0        0     1060 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/floatshield.py
+-rw-r--r--   0        0        0     6892 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/magnetoshield.py
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 python_automationshield-1.0.3/PKG-INFO
```

### Comparing `python_automationshield-1.0.2/LICENSE` & `python_automationshield-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/README.md` & `python_automationshield-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/pyproject.toml` & `python_automationshield-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-automationshield"
-version = "1.0.2"
+version = "1.0.3"
 description = "A Python interface to AutomationShield's Arduino shields"
 authors = ["Bert Van den Abbeele"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/mrtreasurer/python-automationshield"
 documentation = "https://python-automationshield.readthedocs.io"
 packages = [
```

### Comparing `python_automationshield-1.0.2/src/automationshield/__init__.py` & `python_automationshield-1.0.3/src/automationshield/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# read version from installed package
-from importlib.metadata import version
-__version__ = version("python_automationshield")
-
 from .controller import ShieldController
 from .exception import AutomationShieldException
 from .shields import AeroShield, FloatShield, MagnetoShield, DummyShield
 
 
 import platform
```

### Comparing `python_automationshield-1.0.2/src/automationshield/arduino.py` & `python_automationshield-1.0.3/src/automationshield/arduino.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp` & `python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h` & `python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/controller.py` & `python_automationshield-1.0.3/src/automationshield/controller.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/plotting/live_plotter.py` & `python_automationshield-1.0.3/src/automationshield/plotting/live_plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/plotting/plotter.py` & `python_automationshield-1.0.3/src/automationshield/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/shields/aeroshield.py` & `python_automationshield-1.0.3/src/automationshield/shields/aeroshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/shields/baseshield.py` & `python_automationshield-1.0.3/src/automationshield/shields/baseshield.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,19 @@
 
     def install_firmware(self, device:str) -> None:
         """Compile firmware for the current shield and upload to the Arduino.
 
         :param device: FQBN of Arduino. FQBNs for common devices are provided in :py:mod:`automationshield.arduino`, e.g. :py:const:`automationshield.arduino.LEONARDO`: ``arduino:avr:leonardo``.
         :type device: str
         """
+        print("Compiling Code...")
         arduino.compile_script(device, self.script)
+        print("\nUploading ...")
         arduino.upload_script(device, self.script, self.port)
+        print("\nDone")
 
     def convert_potentiometer_reading(self, raw: int) -> float:
         """Convert n-bit potentiometer reading to percentage value.
 
         :param raw: n-bit potentiometer value.
         :type raw: int
         :return: Potentiometer value as percentage [0, 100].
```

### Comparing `python_automationshield-1.0.2/src/automationshield/shields/floatshield.py` & `python_automationshield-1.0.3/src/automationshield/shields/floatshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/src/automationshield/shields/magnetoshield.py` & `python_automationshield-1.0.3/src/automationshield/shields/magnetoshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.2/PKG-INFO` & `python_automationshield-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automationshield
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python interface to AutomationShield's Arduino shields
 Home-page: https://gitlab.com/mrtreasurer/python-automationshield
 License: MIT
 Author: Bert Van den Abbeele
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


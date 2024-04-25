# Comparing `tmp/pytest_embedded_arduino-1.8.4.tar.gz` & `tmp/pytest_embedded_arduino-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_arduino-1.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_arduino-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_arduino-1.8.4.tar` & `pytest_embedded_arduino-1.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/LICENSE
--rw-r--r--   0        0        0      516 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/README.md
--rw-r--r--   0        0        0     3442 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      193 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/pytest_embedded_arduino/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/pytest_embedded_arduino/app.py
--rw-r--r--   0        0        0     1530 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/pytest_embedded_arduino/serial.py
--rw-r--r--   0        0        0      747 2024-04-23 07:21:22.777428 pytest_embedded_arduino-1.8.4/tests/test_arduino.py
--rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/LICENSE
+-rw-r--r--   0        0        0      516 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/README.md
+-rw-r--r--   0        0        0     3442 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/pytest_embedded_arduino/__init__.py
+-rw-r--r--   0        0        0     2610 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/pytest_embedded_arduino/app.py
+-rw-r--r--   0        0        0     1530 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/pytest_embedded_arduino/serial.py
+-rw-r--r--   0        0        0      747 2024-04-25 11:36:08.627318 pytest_embedded_arduino-1.9.0/tests/test_arduino.py
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 pytest_embedded_arduino-1.9.0/PKG-INFO
```

### Comparing `pytest_embedded_arduino-1.8.4/LICENSE` & `pytest_embedded_arduino-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.4/README.md` & `pytest_embedded_arduino-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.4/pyproject.toml` & `pytest_embedded_arduino-1.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.4",
+    "pytest-embedded~=1.9.0",
 ]
 
 [project.optional-dependencies]
 serial = [
-    "pytest-embedded-serial-esp~=1.8.4"
+    "pytest-embedded-serial-esp~=1.9.0"
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
 changelog = "https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md"
```

### Comparing `pytest_embedded_arduino-1.8.4/pytest_embedded_arduino/app.py` & `pytest_embedded_arduino-1.9.0/pytest_embedded_arduino/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     ):
         super().__init__(**kwargs)
 
         self.sketch = os.path.basename(self.app_path)
         self.fqbn = self._get_fqbn(self.binary_path)
         self.target = self.fqbn.split(':')[2]
         self.flash_files = self._get_bin_files(self.binary_path, self.sketch, self.target)
+        self.elf_file = os.path.realpath(os.path.join(self.binary_path, self.sketch + '.ino.elf'))
 
     def _get_fqbn(self, build_path) -> str:
         options_file = os.path.realpath(os.path.join(build_path, 'build.options.json'))
         with open(options_file) as f:
             options = json.load(f)
         fqbn = options['fqbn']
         return fqbn
```

### Comparing `pytest_embedded_arduino-1.8.4/pytest_embedded_arduino/serial.py` & `pytest_embedded_arduino-1.9.0/pytest_embedded_arduino/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.4/tests/test_arduino.py` & `pytest_embedded_arduino-1.9.0/tests/test_arduino.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_arduino-1.8.4/PKG-INFO` & `pytest_embedded_arduino-1.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.8.4
+Version: 1.9.0
 Summary: Make pytest-embedded plugin work with Arduino.
 Author-email: Abdelatif Guettouche <abdelatif.guettouche@espressif.com>, Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.4
-Requires-Dist: pytest-embedded-serial-esp~=1.8.4 ; extra == "serial"
+Requires-Dist: pytest-embedded~=1.9.0
+Requires-Dist: pytest-embedded-serial-esp~=1.9.0 ; extra == "serial"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
 
 ### pytest-embedded-arduino
```


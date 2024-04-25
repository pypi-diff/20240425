# Comparing `tmp/pytest_embedded_idf-1.8.4.tar.gz` & `tmp/pytest_embedded_idf-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_idf-1.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_idf-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_idf-1.8.4.tar` & `pytest_embedded_idf-1.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1094 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/LICENSE
--rw-r--r--   0        0        0      520 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/README.md
--rw-r--r--   0        0        0     3410 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      675 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pytest_embedded_idf/__init__.py
--rw-r--r--   0        0        0     9254 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pytest_embedded_idf/app.py
--rw-r--r--   0        0        0    11146 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pytest_embedded_idf/dut.py
--rw-r--r--   0        0        0     1232 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pytest_embedded_idf/linux.py
--rw-r--r--   0        0        0    10043 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pytest_embedded_idf/serial.py
--rw-r--r--   0        0        0    33073 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/pytest_embedded_idf/unity_tester.py
--rw-r--r--   0        0        0    22581 2024-04-23 07:21:22.777428 pytest_embedded_idf-1.8.4/tests/test_idf.py
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/LICENSE
+-rw-r--r--   0        0        0      520 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/README.md
+-rw-r--r--   0        0        0     3410 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      675 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pytest_embedded_idf/__init__.py
+-rw-r--r--   0        0        0     9254 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pytest_embedded_idf/app.py
+-rw-r--r--   0        0        0    11146 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pytest_embedded_idf/dut.py
+-rw-r--r--   0        0        0     1232 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pytest_embedded_idf/linux.py
+-rw-r--r--   0        0        0    10043 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pytest_embedded_idf/serial.py
+-rw-r--r--   0        0        0    33073 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/pytest_embedded_idf/unity_tester.py
+-rw-r--r--   0        0        0    24573 2024-04-25 11:36:08.627318 pytest_embedded_idf-1.9.0/tests/test_idf.py
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.9.0/PKG-INFO
```

### Comparing `pytest_embedded_idf-1.8.4/LICENSE` & `pytest_embedded_idf-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/README.md` & `pytest_embedded_idf-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/pyproject.toml` & `pytest_embedded_idf-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.4",
+    "pytest-embedded~=1.9.0",
     "esp-idf-panic-decoder",
 ]
 
 [project.optional-dependencies]
 serial = [
-    "pytest-embedded-serial-esp~=1.8.4",
+    "pytest-embedded-serial-esp~=1.9.0",
     "esp-coredump~=1.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
```

### Comparing `pytest_embedded_idf-1.8.4/pytest_embedded_idf/__init__.py` & `pytest_embedded_idf-1.9.0/pytest_embedded_idf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     'IdfDut',
     'IdfSerial',
     'LinuxDut',
     'LinuxSerial',
     'UnittestMenuCase',
 ]
 
-__version__ = '1.8.4'
+__version__ = '1.9.0'
```

### Comparing `pytest_embedded_idf-1.8.4/pytest_embedded_idf/app.py` & `pytest_embedded_idf-1.9.0/pytest_embedded_idf/app.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/pytest_embedded_idf/dut.py` & `pytest_embedded_idf-1.9.0/pytest_embedded_idf/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/pytest_embedded_idf/linux.py` & `pytest_embedded_idf-1.9.0/pytest_embedded_idf/linux.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/pytest_embedded_idf/serial.py` & `pytest_embedded_idf-1.9.0/pytest_embedded_idf/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/pytest_embedded_idf/unity_tester.py` & `pytest_embedded_idf-1.9.0/pytest_embedded_idf/unity_tester.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.4/tests/test_idf.py` & `pytest_embedded_idf-1.9.0/tests/test_idf.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,14 +126,63 @@
         '--embedded-services', 'esp,idf',
         '--app-path', os.path.join(testdir.tmpdir, 'hello_world_esp32'),
     )
 
     result.assert_outcomes(passed=2, failed=2)
 
 
+def test_custom_idf_device_dut(testdir):
+    p = os.path.join(testdir.tmpdir, 'hello_world_esp32')
+    p_c3 = os.path.join(testdir.tmpdir, 'hello_world_esp32c3')
+    unity_test_path = os.path.join(testdir.tmpdir, 'unit_test_app_esp32')
+    unity_test_path_c3 = os.path.join(testdir.tmpdir, 'unit_test_app_esp32c3')
+    testdir.makepyfile(f"""
+        import pytest
+
+        def test_idf_custom_dev():
+            from pytest_embedded.dut_factory import DutFactory
+            dut = DutFactory.create(embedded_services='esp,idf', app_path=r'{p}')
+            dut.expect("Hello")
+
+        def test_idf_mixed(dut):
+            from pytest_embedded.dut_factory import DutFactory
+            dutc = DutFactory.create(embedded_services='esp,idf', app_path=r'{p_c3}')
+            dutc.expect("Hello")
+            dut.expect("Hello")
+            assert dutc.serial.port!=dut.serial.port
+
+        def test_idf_unity_tester():
+            from pytest_embedded.dut_factory import DutFactory
+            dut1 = DutFactory.create(embedded_services='esp,idf', app_path=r'{unity_test_path}')
+            dut2 = DutFactory.create(embedded_services='esp,idf', app_path=r'{unity_test_path_c3}')
+            tester = DutFactory.unity_tester(dut1, dut2)
+            tester.run_all_cases()
+
+        def test_idf_run_all_single_board_cases():
+            from pytest_embedded.dut_factory import DutFactory
+            dut1 = DutFactory.create(embedded_services='esp,idf', app_path=r'{unity_test_path}')
+            dut1.run_all_single_board_cases()
+    """)
+
+    result = testdir.runpytest(
+        '-s',
+        '--app-path', p,
+        '--embedded-services', 'esp,idf',
+        '--junitxml', 'report.xml',
+    )
+    result.assert_outcomes(passed=4, errors=0)
+
+    junit_report = ET.parse('report.xml').getroot()[0]
+
+    assert junit_report.attrib['errors'] == '0'
+    assert junit_report.attrib['failures'] == '2'
+    assert junit_report.attrib['skipped'] == '0'
+    assert junit_report.attrib['tests'] == '7'
+
+
 def test_idf_serial_flash_with_erase_nvs(testdir):
     testdir.makepyfile("""
         import pexpect
         import pytest
 
         def test_idf_serial_flash(dut):
             dut.expect('Hash of data verified.')  # from flash
```

### Comparing `pytest_embedded_idf-1.8.4/PKG-INFO` & `pytest_embedded_idf-1.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.8.4
+Version: 1.9.0
 Summary: Make pytest-embedded plugin work with ESP-IDF.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.4
+Requires-Dist: pytest-embedded~=1.9.0
 Requires-Dist: esp-idf-panic-decoder
-Requires-Dist: pytest-embedded-serial-esp~=1.8.4 ; extra == "serial"
+Requires-Dist: pytest-embedded-serial-esp~=1.9.0 ; extra == "serial"
 Requires-Dist: esp-coredump~=1.0 ; extra == "serial"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
```


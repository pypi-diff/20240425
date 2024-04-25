# Comparing `tmp/pytest_embedded_wokwi-1.8.4.tar.gz` & `tmp/pytest_embedded_wokwi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_wokwi-1.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_wokwi-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_wokwi-1.8.4.tar` & `pytest_embedded_wokwi-1.9.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1094 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/LICENSE
--rw-r--r--   0        0        0     1911 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/README.md
--rw-r--r--   0        0        0     3420 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/pytest_embedded_wokwi/__init__.py
--rw-r--r--   0        0        0      434 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/pytest_embedded_wokwi/dut.py
--rw-r--r--   0        0        0      293 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/pytest_embedded_wokwi/idf.py
--rw-r--r--   0        0        0     4112 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/pytest_embedded_wokwi/wokwi_cli.py
--rw-r--r--   0        0        0     1086 2024-04-23 07:21:22.781428 pytest_embedded_wokwi-1.8.4/tests/test_wokwi.py
--rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 pytest_embedded_wokwi-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.627318 pytest_embedded_wokwi-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1911 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/README.md
+-rw-r--r--   0        0        0     3420 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/__init__.py
+-rw-r--r--   0        0        0      352 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/arduino.py
+-rw-r--r--   0        0        0      434 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/dut.py
+-rw-r--r--   0        0        0      293 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/idf.py
+-rw-r--r--   0        0        0     5044 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/wokwi_cli.py
+-rw-r--r--   0        0        0     1664 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/tests/test_wokwi.py
+-rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 pytest_embedded_wokwi-1.9.0/PKG-INFO
```

### Comparing `pytest_embedded_wokwi-1.8.4/LICENSE` & `pytest_embedded_wokwi-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.8.4/README.md` & `pytest_embedded_wokwi-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.8.4/pyproject.toml` & `pytest_embedded_wokwi-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.4",
+    "pytest-embedded~=1.9.0",
     "toml~=0.10.2",
 ]
 
 [project.optional-dependencies]
 idf = [
-    "pytest-embedded-idf~=1.8.4",
+    "pytest-embedded-idf~=1.9.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
 changelog = "https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md"
```

### Comparing `pytest_embedded_wokwi-1.8.4/tests/test_wokwi.py` & `pytest_embedded_wokwi-1.9.0/tests/test_wokwi.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,7 +32,28 @@
     result = testdir.runpytest(
         '-s',
         '--embedded-services', 'idf,wokwi',
         '--app-path', os.path.join(testdir.tmpdir, 'hello_world_esp32'),
     )
 
     result.assert_outcomes(passed=1)
+
+
+@wokwi_cli_required
+@wokwi_token_required
+def test_pexpect_by_wokwi_esp32_arduino(testdir):
+    testdir.makepyfile("""
+        import pexpect
+        import pytest
+        def test_pexpect_by_wokwi(dut):
+            dut.expect('Hello Arduino!')
+            with pytest.raises(pexpect.TIMEOUT):
+                dut.expect('foo bar not found', timeout=1)
+    """)
+
+    result = testdir.runpytest(
+        '-s',
+        '--embedded-services', 'arduino,wokwi',
+        '--app-path', os.path.join(testdir.tmpdir, 'hello_world_arduino'),
+    )
+
+    result.assert_outcomes(passed=1)
```

### Comparing `pytest_embedded_wokwi-1.8.4/PKG-INFO` & `pytest_embedded_wokwi-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-wokwi
-Version: 1.8.4
+Version: 1.9.0
 Summary: Make pytest-embedded plugin work with the Wokwi CLI.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>, Uri Shaked <uri@wokwi.com>
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
 Requires-Dist: toml~=0.10.2
-Requires-Dist: pytest-embedded-idf~=1.8.4 ; extra == "idf"
+Requires-Dist: pytest-embedded-idf~=1.9.0 ; extra == "idf"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: idf
 
 ### pytest-embedded-wokwi
```


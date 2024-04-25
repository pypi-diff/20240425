# Comparing `tmp/phlop-0.0.8.tar.gz` & `tmp/phlop-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlop-0.0.8.tar", last modified: Sun Jan 21 13:24:08 2024, max compression
+gzip compressed data, was "phlop-0.0.9.tar", last modified: Thu Feb  8 16:05:43 2024, max compression
```

## Comparing `phlop-0.0.8.tar` & `phlop-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-21 13:23:57.000000 phlop-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-21 13:24:08.266070 phlop-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 13:23:57.000000 phlop-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.262071 phlop-0.0.8/phlop/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.262071 phlop-0.0.8/phlop/app/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/app/cmake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/app/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/app/perf.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/app/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/os.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/proc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/phlop/procs/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/procs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/procs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/procs/runtimer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/phlop/run/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/run/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/run/stats_man.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/run/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/string.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/phlop/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/testing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/testing/parallel_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-01-21 13:23:57.000000 phlop-0.0.8/phlop/testing/test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/phlop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-21 13:24:08.000000 phlop-0.0.8/phlop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-21 13:24:08.000000 phlop-0.0.8/phlop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 13:24:08.000000 phlop-0.0.8/phlop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-21 13:24:08.000000 phlop-0.0.8/phlop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-21 13:23:57.000000 phlop-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 13:24:08.266070 phlop-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-21 13:23:57.000000 phlop-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 13:23:57.000000 phlop-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 13:24:08.266070 phlop-0.0.8/tests/_phlop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 13:23:57.000000 phlop-0.0.8/tests/_phlop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-21 13:23:57.000000 phlop-0.0.8/tests/_phlop/os_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-21 13:23:57.000000 phlop-0.0.8/tests/all_concurrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-08 16:05:29.000000 phlop-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-08 16:05:43.407439 phlop-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:29.000000 phlop-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.403439 phlop-0.0.9/phlop/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/phlop/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/app/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/app/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/app/perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/app/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/proc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/phlop/procs/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/procs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/procs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/procs/runtimer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/phlop/run/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/run/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/run/stats_man.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/run/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/phlop/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/testing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/testing/parallel_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-02-08 16:05:29.000000 phlop-0.0.9/phlop/testing/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/phlop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-08 16:05:43.000000 phlop-0.0.9/phlop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-08 16:05:43.000000 phlop-0.0.9/phlop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 16:05:43.000000 phlop-0.0.9/phlop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-08 16:05:43.000000 phlop-0.0.9/phlop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-08 16:05:29.000000 phlop-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 16:05:43.407439 phlop-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-08 16:05:29.000000 phlop-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:29.000000 phlop-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:43.407439 phlop-0.0.9/tests/_phlop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 16:05:29.000000 phlop-0.0.9/tests/_phlop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-08 16:05:29.000000 phlop-0.0.9/tests/_phlop/os_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-08 16:05:29.000000 phlop-0.0.9/tests/all_concurrent.py
```

### Comparing `phlop-0.0.8/phlop/app/cmake.py` & `phlop-0.0.9/phlop/app/cmake.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/app/git.py` & `phlop-0.0.9/phlop/app/git.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/app/perf.py` & `phlop-0.0.9/phlop/app/perf.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/os.py` & `phlop-0.0.9/phlop/os.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/proc.py` & `phlop-0.0.9/phlop/proc.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/procs/runtimer.py` & `phlop-0.0.9/phlop/procs/runtimer.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/reflection.py` & `phlop-0.0.9/phlop/reflection.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/run/stats_man.py` & `phlop-0.0.9/phlop/run/stats_man.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/run/test_cases.py` & `phlop-0.0.9/phlop/run/test_cases.py`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/phlop/testing/parallel_processor.py` & `phlop-0.0.9/phlop/testing/parallel_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 
 def process(batches, n_cores=None, print_only=False, fail_fast=False):
     if not isinstance(batches, list):
         batches = [batches]
     if sum([len(t.tests) for t in batches]) == 0:
         return  # nothing to do
+
     if print_only:
         print_tests(batches)
         return
 
     n_cores = n_cores if n_cores else cpu_count()
 
     cc = CoreCount(n_cores)
```

### Comparing `phlop-0.0.8/phlop/testing/test_cases.py` & `phlop-0.0.9/phlop/testing/test_cases.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,21 +14,25 @@
 from phlop.os import env_sep
 from phlop.proc import run
 from phlop.reflection import classes_in_file
 from phlop.sys import extend_sys_path
 
 _LOG_DIR = Path(os.environ.get("PHLOP_LOG_DIR", os.getcwd()))
 
+CMD_PREFIX = ""
+CMD_POSTFIX = ""
+
 
 @dataclass
 class TestCase:
     cmd: str
     env: dict = field(default_factory=lambda: {})  # dict[str, str] # eventually
     working_dir: str = field(default_factory=lambda: None)
     log_file_path: str = field(default_factory=lambda: None)
+    cores: int = field(default_factory=lambda: 1)
 
     def __post_init__(self):
         self.cmd = self.cmd.strip()
 
 
 class TestBatch:
     def __init__(self, tests, cores=1):
@@ -63,28 +67,28 @@
         # print(p.stdout)
 
         return None
 
 
 class PythonUnitTestCaseExtractor:
     def __call__(self, ctest_test):
-        if "python3" in ctest_test.cmd:  # hacky
-            return load_test_cases_from_cmake(ctest_test)
+        if "python3 " in ctest_test.cmd:  # hacky
+            return load_py_test_cases_from_cmake(ctest_test)
         return None
 
 
 EXTRACTORS = [
     PythonUnitTestCaseExtractor(),
     GoogleTestCaseExtractor(),
     DefaultTestCaseExtractor(),
 ]
 
 
 def python3_default_test_cmd(clazz, test_id):
-    return f"python3 -m {clazz.__module__} {clazz.__name__}.{test_id}"
+    return f"python3 -Oum {clazz.__module__} {clazz.__name__}.{test_id}"
 
 
 def load_test_cases_in(
     classes, test_cmd_pre="", test_cmd_post="", test_cmd_fn=None, **kwargs
 ):
     test_cmd_fn = test_cmd_fn if test_cmd_fn else python3_default_test_cmd
     log_file_path = kwargs.pop("log_file_path", None)
@@ -100,43 +104,80 @@
                     else f"{log_file_path}/{suite._testMethodName}",
                     **kwargs,
                 )
             ]
     return tests
 
 
-def load_test_cases_from_cmake(ctest_test):
+def load_py_test_cases_from_cmake(ctest_test):
     ppath = ctest_test.env.get("PYTHONPATH", "")
+    bits = ctest_test.cmd.split(" ")
+    idx = [i for i, x in enumerate(bits) if "python3" in x][0]
+    prefix = " ".join(bits[:idx])
     with extend_sys_path([ctest_test.working_dir] + ppath.split(env_sep())):
-        pyfile = ctest_test.cmd.split(" ")[-1]
+        pyfile = bits[-1]
         return load_test_cases_in(
             classes_in_file(pyfile, unittest.TestCase, fail_on_import_error=True),
             env=ctest_test.env,
             working_dir=ctest_test.working_dir,
             log_file_path=_LOG_DIR
             / ".phlop"
             / f"{Path(ctest_test.working_dir).relative_to(_LOG_DIR)}",
+            test_cmd_pre=CMD_PREFIX + prefix + CMD_POSTFIX,
         )
 
 
-# probably return a list of TestBatch if we do some core count detection per test
+def determine_cores_for_test_case(test_case):
+    cores = 1
+
+    try:
+        if "mpirun -n" in test_case.cmd:
+            bits = test_case.cmd.split(" ")
+            # print(bits)
+            idx = [i for i, x in enumerate(bits) if "mpirun" in x][0]
+            test_case.cores = int(bits[idx + 2])
+    except Exception as e:
+        print("EXXXX", e)
+
+    return test_case
+
+
+def binless(test_case):
+    if test_case.cmd.startswith("/usr/bin/"):
+        test_case.cmd = test_case.cmd[9:]
+    return test_case
+
+
+MUTATORS = [determine_cores_for_test_case, binless]
+
+
 def load_cmake_tests(cmake_dir, cores=1, test_cmd_pre="", test_cmd_post=""):
     cmake_tests = get_cmake_tests(cmake_dir)
     tests = []
     for cmake_test in cmake_tests:
         tests += [
             TestCase(
                 cmd=test_cmd_pre + " ".join(cmake_test.command) + " " + test_cmd_post,
                 env=cmake_test.env,
                 working_dir=cmake_test.working_dir,
             )
         ]
 
+    test_batches = {}
+
+    def _add(test_cases):
+        for test_case in test_cases:
+            for mutator in MUTATORS:
+                test_case = mutator(test_case)
+            if test_case.cores not in test_batches:
+                test_batches[test_case.cores] = []
+            test_batches[test_case.cores].append(test_case)
+
     test_cases = []
     for test in tests:
         for extractor in EXTRACTORS:
             res = extractor(test)
             if res:
-                test_cases += res
+                _add(res)
                 break
 
-    return TestBatch(test_cases, cores)
+    return [TestBatch(v, k) for k, v in test_batches.items()]
```

### Comparing `phlop-0.0.8/phlop.egg-info/SOURCES.txt` & `phlop-0.0.9/phlop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phlop-0.0.8/tests/all_concurrent.py` & `phlop-0.0.9/tests/all_concurrent.py`

 * *Files identical despite different names*


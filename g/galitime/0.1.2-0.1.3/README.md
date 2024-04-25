# Comparing `tmp/galitime-0.1.2.tar.gz` & `tmp/galitime-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galitime-0.1.2.tar", last modified: Wed Apr 10 21:51:21 2024, max compression
+gzip compressed data, was "galitime-0.1.3.tar", last modified: Thu Apr 25 11:12:23 2024, max compression
```

## Comparing `galitime-0.1.2.tar` & `galitime-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 21:51:21.962725 galitime-0.1.2/
--rw-r--r--   0 karel      (503) staff       (20)     1070 2024-04-10 08:29:59.000000 galitime-0.1.2/LICENSE.txt
--rw-r--r--   0 karel      (503) staff       (20)     3840 2024-04-10 21:51:21.961913 galitime-0.1.2/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)     3262 2024-04-10 13:08:53.000000 galitime-0.1.2/README.rst
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 21:51:21.850400 galitime-0.1.2/galitime/
--rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 galitime-0.1.2/galitime/__init__.py
--rwxr-xr-x   0 karel      (503) staff       (20)     5687 2024-04-10 12:53:23.000000 galitime-0.1.2/galitime/galitime.py
--rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 galitime-0.1.2/galitime/increment_version.py
--rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-10 21:47:41.000000 galitime-0.1.2/galitime/version.py
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 21:51:21.961051 galitime-0.1.2/galitime.egg-info/
--rw-r--r--   0 karel      (503) staff       (20)     3840 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/SOURCES.txt
--rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/dependency_links.txt
--rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/entry_points.txt
--rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/requires.txt
--rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/top_level.txt
--rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-10 21:51:21.962809 galitime-0.1.2/setup.cfg
--rw-r--r--   0 karel      (503) staff       (20)     1351 2024-04-10 08:28:25.000000 galitime-0.1.2/setup.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-25 11:12:23.525310 galitime-0.1.3/
+-rw-r--r--   0 karel      (503) staff       (20)     1070 2024-04-10 08:29:59.000000 galitime-0.1.3/LICENSE.txt
+-rw-r--r--   0 karel      (503) staff       (20)     4141 2024-04-25 11:12:23.524659 galitime-0.1.3/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     3563 2024-04-25 11:08:44.000000 galitime-0.1.3/README.rst
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-25 11:12:23.393587 galitime-0.1.3/galitime/
+-rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 galitime-0.1.3/galitime/__init__.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     5783 2024-04-25 11:08:50.000000 galitime-0.1.3/galitime/galitime.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 galitime-0.1.3/galitime/increment_version.py
+-rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-25 11:02:30.000000 galitime-0.1.3/galitime/version.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-25 11:12:23.523815 galitime-0.1.3/galitime.egg-info/
+-rw-r--r--   0 karel      (503) staff       (20)     4141 2024-04-25 11:12:23.000000 galitime-0.1.3/galitime.egg-info/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-25 11:12:23.000000 galitime-0.1.3/galitime.egg-info/SOURCES.txt
+-rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-25 11:12:23.000000 galitime-0.1.3/galitime.egg-info/dependency_links.txt
+-rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-25 11:12:23.000000 galitime-0.1.3/galitime.egg-info/entry_points.txt
+-rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-25 11:12:23.000000 galitime-0.1.3/galitime.egg-info/requires.txt
+-rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-25 11:12:23.000000 galitime-0.1.3/galitime.egg-info/top_level.txt
+-rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-25 11:12:23.525393 galitime-0.1.3/setup.cfg
+-rw-r--r--   0 karel      (503) staff       (20)     1351 2024-04-10 08:28:25.000000 galitime-0.1.3/setup.py
```

### Comparing `galitime-0.1.2/LICENSE.txt` & `galitime-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galitime-0.1.2/PKG-INFO` & `galitime-0.1.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: galitime
-Version: 0.1.2
-Summary: description
-Home-page: https://github.com/karel-brinda/galitime
-Author: Karel Brinda
-Author-email: karel.brinda@inria.fr
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: Unix
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-License-File: LICENSE.txt
-Requires-Dist: wheel
-
 galitime
 ========
 
 .. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
     :target: https://github.com/karel-brinda/galitime
 .. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/galitime.svg
     :target: https://github.com/karel-brinda/galitime/releases/
@@ -41,17 +23,22 @@
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
-    if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
-    conda install -y -c bioconda -c conda-forge galitime
-    galitime --log time.log ls
+    $ if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
+    $ conda install -y -c bioconda -c conda-forge galitime
+
+    $ galitime --log time.log ls
+
+    $ cat time.log
+    real_s  user_s  sys_s   percent_cpu max_ram_kb  exit_code   fs_inputs   fs_outputs  real_s_alt  command
+    0.03    0.00    0.00    10% 2904    0   0   0   0.076661    ls
 
 
 
 Installation
 ------------
 
 Dependencies
@@ -107,18 +94,19 @@
 ------
 
 * ``experiment`` - Name of the experiment, if provided via ``-n``
 * ``real_s`` - Real time in seconds (wall clock time)
 * ``user_s`` - User CPU time in seconds (user mode, excluding system calls)
 * ``sys_s`` - System CPU time in seconds (kernel mode)
 * ``percent_cpu`` - CPU usage percentage
-* ``ram_kb`` - Maximum RAM usage in kilobytes
+* ``max_ram_kb`` - Maximum RAM usage in kilobytes
+* ``exit_code`` - Exit code of the command (0 if everything ok)
 * ``fs_inputs`` - File system read read operations count
 * ``fs_outputs`` - File system write operations count
-* ``python_real_s`` - Python-measured real time in seconds
+* ``real_s_alt`` - Python-measured real time in seconds (slightly higher than ``real_s``)
 * ``command`` - Command executed, with tabs replaced by spaces
 
 
 
 
 
 Issues
```

### Comparing `galitime-0.1.2/galitime/galitime.py` & `galitime-0.1.3/galitime/galitime.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 import re
 import subprocess
 import sys
 import tempfile
 
 from pathlib import Path
 
-sys.path.append(os.path.dirname(__file__))
-import version
-
 PROGRAM = 'galitime'
-VERSION = version.VERSION
 DESC = 'benchmarking of computational experiments using GNU time'
 
+try:
+    sys.path.append(os.path.dirname(__file__))
+    import version
+    VERSION = version.VERSION
+except ImportError:
+    VERSION = "(version NA)"
+
 DEFAULT_L = "stderr"
 
 
 def get_time_command():
     """
     Returns the appropriate time command based on the operating system.
 
@@ -53,17 +56,18 @@
         "real(s)", "sys(s)", "user(s)", "percent_CPU", "max_RAM(kb)", "FS_inputs", "FS_outputs",
         "elapsed_time_alt(s)"
     ]
 
     with tempfile.TemporaryDirectory() as dir_fn:
         tmp_fn = os.path.join(dir_fn, "gtime_output.txt")
         gtime_columns = (
-            "real_s", "sys_s", "user_s", "percent_cpu", "ram_kb", "fs_inputs", "fs_outputs"
+            "real_s", "user_s", "sys_s", "percent_cpu", "max_ram_kb", "exit_code", "fs_inputs",
+            "fs_outputs"
         )
-        gtime_columns_spec = "%e\t%U\t%S\t%P\t%M\t%I\t%O"
+        gtime_columns_spec = "%e\t%U\t%S\t%P\t%M\t%x\t%I\t%O"
         benchmark_wrapper = f'{get_time_command()} -o {tmp_fn} -f "{gtime_columns_spec}"'
 
         start_time = datetime.datetime.now()
         main_process = subprocess.Popen(
             f'{benchmark_wrapper} {command}', shell=True, executable='/bin/bash'
         )
         return_code = main_process.wait()
@@ -78,15 +82,15 @@
         with open(tmp_fn) as tmp_fo:
             gtime_output_values = tmp_fo.readline().strip().split("\t")
 
     for k, v in zip(gtime_columns, gtime_output_values):
         d[k] = v
 
     # 3) elapsed time
-    d["python_real_s"] = str((end_time - start_time).total_seconds())
+    d["real_s_alt"] = str((end_time - start_time).total_seconds())
 
     # 4) formatted command
     d["command"] = " ".join(command.replace("\\\n", " ").strip().split())
 
     return d
```

### Comparing `galitime-0.1.2/galitime.egg-info/PKG-INFO` & `galitime-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galitime
-Version: 0.1.2
+Version: 0.1.3
 Summary: description
 Home-page: https://github.com/karel-brinda/galitime
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,17 +41,22 @@
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
-    if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
-    conda install -y -c bioconda -c conda-forge galitime
-    galitime --log time.log ls
+    $ if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
+    $ conda install -y -c bioconda -c conda-forge galitime
+
+    $ galitime --log time.log ls
+
+    $ cat time.log
+    real_s  user_s  sys_s   percent_cpu max_ram_kb  exit_code   fs_inputs   fs_outputs  real_s_alt  command
+    0.03    0.00    0.00    10% 2904    0   0   0   0.076661    ls
 
 
 
 Installation
 ------------
 
 Dependencies
@@ -107,18 +112,19 @@
 ------
 
 * ``experiment`` - Name of the experiment, if provided via ``-n``
 * ``real_s`` - Real time in seconds (wall clock time)
 * ``user_s`` - User CPU time in seconds (user mode, excluding system calls)
 * ``sys_s`` - System CPU time in seconds (kernel mode)
 * ``percent_cpu`` - CPU usage percentage
-* ``ram_kb`` - Maximum RAM usage in kilobytes
+* ``max_ram_kb`` - Maximum RAM usage in kilobytes
+* ``exit_code`` - Exit code of the command (0 if everything ok)
 * ``fs_inputs`` - File system read read operations count
 * ``fs_outputs`` - File system write operations count
-* ``python_real_s`` - Python-measured real time in seconds
+* ``real_s_alt`` - Python-measured real time in seconds (slightly higher than ``real_s``)
 * ``command`` - Command executed, with tabs replaced by spaces
 
 
 
 
 
 Issues
```

### Comparing `galitime-0.1.2/setup.py` & `galitime-0.1.3/setup.py`

 * *Files identical despite different names*


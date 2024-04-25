# Comparing `tmp/mytot-2024.4.21.213952-py3-none-any.whl.zip` & `tmp/mytot-2024.4.25.205747-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 27543 bytes, number of entries: 9
+Zip file size: 27756 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:16 mytot/__init__.py
--rw-rw-r--  2.0 unx     3263 b- defN 24-Apr-21 13:24 mytot/main.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.21.213952.data/data/LICENSE
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/LICENSE
--rw-rw-r--  2.0 unx      777 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/WHEEL
--rw-rw-r--  2.0 unx       85 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      773 b- defN 24-Apr-21 13:39 mytot-2024.4.21.213952.dist-info/RECORD
-9 files, 75294 bytes uncompressed, 26191 bytes compressed:  65.2%
+-rw-rw-r--  2.0 unx     3951 b- defN 24-Apr-25 12:57 mytot/main.py
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.25.205747.data/data/LICENSE
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-25 12:57 mytot-2024.4.25.205747.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      777 b- defN 24-Apr-25 12:57 mytot-2024.4.25.205747.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-25 12:57 mytot-2024.4.25.205747.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       85 b- defN 24-Apr-25 12:57 mytot-2024.4.25.205747.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-25 12:57 mytot-2024.4.25.205747.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      773 b- defN 24-Apr-25 12:57 mytot-2024.4.25.205747.dist-info/RECORD
+9 files, 75982 bytes uncompressed, 26404 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: mytot/__init__.py
 Comment: 
 
 Filename: mytot/main.py
 Comment: 
 
-Filename: mytot-2024.4.21.213952.data/data/LICENSE
+Filename: mytot-2024.4.25.205747.data/data/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.21.213952.dist-info/LICENSE
+Filename: mytot-2024.4.25.205747.dist-info/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.21.213952.dist-info/METADATA
+Filename: mytot-2024.4.25.205747.dist-info/METADATA
 Comment: 
 
-Filename: mytot-2024.4.21.213952.dist-info/WHEEL
+Filename: mytot-2024.4.25.205747.dist-info/WHEEL
 Comment: 
 
-Filename: mytot-2024.4.21.213952.dist-info/entry_points.txt
+Filename: mytot-2024.4.25.205747.dist-info/entry_points.txt
 Comment: 
 
-Filename: mytot-2024.4.21.213952.dist-info/top_level.txt
+Filename: mytot-2024.4.25.205747.dist-info/top_level.txt
 Comment: 
 
-Filename: mytot-2024.4.21.213952.dist-info/RECORD
+Filename: mytot-2024.4.25.205747.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mytot/main.py

```diff
@@ -1,16 +1,39 @@
 import os
-import datetime
 import sys
+import signal
+import datetime
 import subprocess
 import psutil
 
 from loguru import logger
 
 
+def kill_process_tree(pid, sig_n=signal.SIGKILL):
+    sig = signal.SIGTERM
+    if sig_n == 9:
+        sig = signal.SIGKILL
+    pid_list = [pid]
+    while True:
+        if len(pid_list) == 0:
+            break
+        tmp_pid = pid_list.pop(0)
+        if not psutil.pid_exists(tmp_pid):
+            continue
+        parent = psutil.Process(tmp_pid)
+        if parent is not None:
+            children = parent.children(recursive=False)
+            if children is not None:
+                for child in children:
+                    pid_list.append(child.pid)
+            cmdline = " ".join(parent.cmdline())
+            print(f"kill {parent.pid} {cmdline}")
+            parent.send_signal(sig)
+
+
 def mkdir(path):
     if not os.path.exists(path):
         os.makedirs(path)
 
 
 def RUN():
     if len(sys.argv) < 2:
@@ -45,31 +68,30 @@
 
 
 def KILL():
     if len(sys.argv) < 2:
         print("usage: KILL [script_file]")
         return
     key = sys.argv[1]
-    signal = 9
+    signal_num = 9
     for arg in sys.argv[1:]:
         if arg[0] == "-":
-            signal = int(arg[1:])
+            signal_num = int(arg[1:])
             continue
         key = arg
         break
     for process in psutil.process_iter(["pid", "name", "cmdline"]):
         if process.info["cmdline"] is None:
             continue
         cmdline = " ".join(list(process.info["cmdline"]))
         if "KILL" in cmdline:
             continue
         if key in cmdline:
             pid = process.info["pid"]
-            print(f"kill -{signal} {pid}")
-            os.kill(pid, signal)
+            kill_process_tree(pid, signal_num)
 
 
 def today():
     return datetime.datetime.now().strftime("%Y%m%d")
 
 
 def TASK():
```

## Comparing `mytot-2024.4.21.213952.data/data/LICENSE` & `mytot-2024.4.25.205747.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.21.213952.dist-info/LICENSE` & `mytot-2024.4.25.205747.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.21.213952.dist-info/METADATA` & `mytot-2024.4.25.205747.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytot
-Version: 2024.4.21.213952
+Version: 2024.4.25.205747
 Summary: Tool of Tool
 Author: Xin-Xin Ma
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: psutil
```


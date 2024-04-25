# Comparing `tmp/mainshortcuts-1.6.76.tar.gz` & `tmp/mainshortcuts-1.6.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.76.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.77.tar", max compression
```

## Comparing `mainshortcuts-1.6.76.tar` & `mainshortcuts-1.6.77.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.76/README.md
--rwxr-xr-x   0        0        0      696 2024-04-25 01:33:15.000000 mainshortcuts-1.6.76/pyproject.toml
--rwxr-xr-x   0        0        0     6027 2024-03-18 12:04:56.000000 mainshortcuts-1.6.76/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0      937 2024-04-25 01:32:58.000000 mainshortcuts-1.6.76/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      456 2024-01-13 08:00:52.000000 mainshortcuts-1.6.76/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     6649 2024-03-18 10:53:54.000000 mainshortcuts-1.6.76/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0      890 2024-03-18 10:58:02.000000 mainshortcuts-1.6.76/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1467 2024-03-18 11:02:06.000000 mainshortcuts-1.6.76/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     3103 2024-04-24 14:23:52.000000 mainshortcuts-1.6.76/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     2852 2024-03-18 11:17:08.000000 mainshortcuts-1.6.76/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     5877 2024-03-18 11:35:14.000000 mainshortcuts-1.6.76/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     2549 2024-04-25 01:32:50.000000 mainshortcuts-1.6.76/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3649 2024-04-12 17:48:30.000000 mainshortcuts-1.6.76/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2120 2024-03-18 11:57:28.000000 mainshortcuts-1.6.76/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.76/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.76/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6163 2024-03-18 12:10:52.000000 mainshortcuts-1.6.76/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      783 2024-03-18 12:11:44.000000 mainshortcuts-1.6.76/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0      616 2024-03-18 12:12:40.000000 mainshortcuts-1.6.76/src/MainShortcuts/reg.py
--rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.76/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0      937 2024-03-18 12:15:06.000000 mainshortcuts-1.6.76/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    14794 2024-03-18 12:16:26.000000 mainshortcuts-1.6.76/src/MainShortcuts/values.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.76/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.77/README.md
+-rwxr-xr-x   0        0        0      696 2024-04-25 01:35:56.000000 mainshortcuts-1.6.77/pyproject.toml
+-rwxr-xr-x   0        0        0     6027 2024-03-18 12:04:56.000000 mainshortcuts-1.6.77/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0      937 2024-04-25 01:35:50.000000 mainshortcuts-1.6.77/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      456 2024-01-13 08:00:52.000000 mainshortcuts-1.6.77/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     6649 2024-03-18 10:53:54.000000 mainshortcuts-1.6.77/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0      890 2024-03-18 10:58:02.000000 mainshortcuts-1.6.77/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1467 2024-03-18 11:02:06.000000 mainshortcuts-1.6.77/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     3105 2024-04-25 01:35:32.000000 mainshortcuts-1.6.77/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     2852 2024-03-18 11:17:08.000000 mainshortcuts-1.6.77/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     5877 2024-03-18 11:35:14.000000 mainshortcuts-1.6.77/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     2549 2024-04-25 01:35:44.000000 mainshortcuts-1.6.77/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3649 2024-04-12 17:48:30.000000 mainshortcuts-1.6.77/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2120 2024-03-18 11:57:28.000000 mainshortcuts-1.6.77/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.77/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.77/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6163 2024-03-18 12:10:52.000000 mainshortcuts-1.6.77/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      783 2024-03-18 12:11:44.000000 mainshortcuts-1.6.77/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0      616 2024-03-18 12:12:40.000000 mainshortcuts-1.6.77/src/MainShortcuts/reg.py
+-rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.77/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0      937 2024-03-18 12:15:06.000000 mainshortcuts-1.6.77/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    14794 2024-03-18 12:16:26.000000 mainshortcuts-1.6.77/src/MainShortcuts/values.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.77/PKG-INFO
```

### Comparing `mainshortcuts-1.6.76/README.md` & `mainshortcuts-1.6.77/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/pyproject.toml` & `mainshortcuts-1.6.77/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "1.6.76"
+version = "1.6.77"
 name = "mainshortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
```

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.77/src/MainShortcuts/MainCore.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.77/src/MainShortcuts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
 https://t.me/MainPlay_InfoCh"""
 
-__version_tuple__=(1,6,76)
+__version_tuple__=(1,6,77)
 __depends__={
   "required":[
     "json",
     "os",
     "platform",
     "shutil",
     "subprocess",
```

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/cfg.py` & `mainshortcuts-1.6.77/src/MainShortcuts/cfg.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/dict.py` & `mainshortcuts-1.6.77/src/MainShortcuts/dict.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.77/src/MainShortcuts/dictplus.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.77/src/MainShortcuts/dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,12 +83,12 @@
       if not _os.path.islink(i):
         continue
     elif links==False:
       if _os.path.islink(i):
         continue
     else:
       raise Exception('"links" can only be True, False or None')
-    if files and os.path.isfile(i):
+    if files and _os.path.isfile(i):
       b.append(i)
-    elif dirs and os.path.isdir(i):
+    elif dirs and _os.path.isdir(i):
       b.append(i)
   return b
```

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/file.py` & `mainshortcuts-1.6.77/src/MainShortcuts/file.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.77/src/MainShortcuts/fileobj.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.77/src/MainShortcuts/imports.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/json.py` & `mainshortcuts-1.6.77/src/MainShortcuts/json.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/list.py` & `mainshortcuts-1.6.77/src/MainShortcuts/list.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/main.py` & `mainshortcuts-1.6.77/src/MainShortcuts/main.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/path.py` & `mainshortcuts-1.6.77/src/MainShortcuts/path.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/proc.py` & `mainshortcuts-1.6.77/src/MainShortcuts/proc.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/reg.py` & `mainshortcuts-1.6.77/src/MainShortcuts/reg.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/script.py` & `mainshortcuts-1.6.77/src/MainShortcuts/script.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/str.py` & `mainshortcuts-1.6.77/src/MainShortcuts/str.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/src/MainShortcuts/values.py` & `mainshortcuts-1.6.77/src/MainShortcuts/values.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.76/PKG-INFO` & `mainshortcuts-1.6.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mainshortcuts
-Version: 1.6.76
+Version: 1.6.77
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```


# Comparing `tmp/otpcr-5.tar.gz` & `tmp/otpcr-6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpcr-5.tar", last modified: Tue Apr 23 12:58:29 2024, max compression
+gzip compressed data, was "otpcr-6.tar", last modified: Wed Apr 24 05:30:20 2024, max compression
```

## Comparing `otpcr-5.tar` & `otpcr-6.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.954451 otpcr-5/
--rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-23 12:58:29.954451 otpcr-5/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1869 2024-04-23 12:52:59.000000 otpcr-5/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.946451 otpcr-5/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)     3451 2024-04-23 12:56:25.000000 otpcr-5/docs/MANUAL.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.950451 otpcr-5/files/
--rw-r--r--   0 bart      (1000) bart      (1000)   225470 2024-04-23 12:16:02.000000 otpcr-5/files/EM_Ack_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-23 12:16:02.000000 otpcr-5/files/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-23 12:16:02.000000 otpcr-5/files/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   244503 2024-04-23 12:14:34.000000 otpcr-5/files/verbatim4.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.950451 otpcr-5/otpcr/
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-23 12:01:06.000000 otpcr-5/otpcr/__init__.py
--rwxr-xr-x   0 bart      (1000) bart      (1000)     4636 2024-04-23 12:27:34.000000 otpcr-5/otpcr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-23 12:01:06.000000 otpcr-5/otpcr/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-23 12:01:06.000000 otpcr-5/otpcr/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-23 12:01:06.000000 otpcr-5/otpcr/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-23 12:01:06.000000 otpcr-5/otpcr/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-23 12:01:06.000000 otpcr-5/otpcr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-23 12:01:06.000000 otpcr-5/otpcr/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-23 12:01:06.000000 otpcr-5/otpcr/find.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-23 12:01:06.000000 otpcr-5/otpcr/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.954451 otpcr-5/otpcr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      423 2024-04-23 12:39:26.000000 otpcr-5/otpcr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      403 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      819 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17621 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      776 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17081 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      240 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2400 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1184 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1038 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5130 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5799 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-23 12:01:06.000000 otpcr-5/otpcr/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-23 12:01:06.000000 otpcr-5/otpcr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-23 12:01:06.000000 otpcr-5/otpcr/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-23 12:01:06.000000 otpcr-5/otpcr/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-23 12:01:06.000000 otpcr-5/otpcr/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-23 12:01:06.000000 otpcr-5/otpcr/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-23 12:01:06.000000 otpcr-5/otpcr/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.950451 otpcr-5/otpcr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      939 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)     1016 2024-04-23 12:50:22.000000 otpcr-5/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-23 12:58:29.954451 otpcr-5/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-23 11:57:54.000000 otpcr-5/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 05:30:20.967082 otpcr-6/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2394 2024-04-24 05:30:20.967082 otpcr-6/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1868 2024-04-24 05:29:55.000000 otpcr-6/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 05:30:20.963082 otpcr-6/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3451 2024-04-23 12:56:25.000000 otpcr-6/docs/MANUAL.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 05:30:20.963082 otpcr-6/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)   225470 2024-04-23 12:16:02.000000 otpcr-6/files/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-23 12:16:02.000000 otpcr-6/files/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-23 12:16:02.000000 otpcr-6/files/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   242205 2024-04-23 13:40:53.000000 otpcr-6/files/verbatim5.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 05:30:20.967082 otpcr-6/otpcr/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1220 2024-04-23 15:38:24.000000 otpcr-6/otpcr/__init__.py
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4313 2024-04-23 18:16:54.000000 otpcr-6/otpcr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      654 2024-04-23 13:59:26.000000 otpcr-6/otpcr/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3863 2024-04-23 14:11:26.000000 otpcr-6/otpcr/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      276 2024-04-23 14:07:23.000000 otpcr-6/otpcr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      232 2024-04-23 14:08:15.000000 otpcr-6/otpcr/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1227 2024-04-24 05:23:11.000000 otpcr-6/otpcr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      762 2024-04-23 18:13:47.000000 otpcr-6/otpcr/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1904 2024-04-23 14:00:31.000000 otpcr-6/otpcr/find.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1352 2024-04-23 14:06:41.000000 otpcr-6/otpcr/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 05:30:20.967082 otpcr-6/otpcr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      423 2024-04-23 12:39:26.000000 otpcr-6/otpcr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      213 2024-04-23 18:12:19.000000 otpcr-6/otpcr/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      376 2024-04-23 15:14:04.000000 otpcr-6/otpcr/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-23 15:14:34.000000 otpcr-6/otpcr/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      841 2024-04-23 15:14:48.000000 otpcr-6/otpcr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    18951 2024-04-24 05:12:00.000000 otpcr-6/otpcr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      805 2024-04-23 17:57:39.000000 otpcr-6/otpcr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3641 2024-04-23 18:02:43.000000 otpcr-6/otpcr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17429 2024-04-23 17:56:59.000000 otpcr-6/otpcr/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-04-23 15:25:33.000000 otpcr-6/otpcr/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2408 2024-04-23 15:26:20.000000 otpcr-6/otpcr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11003 2024-04-23 18:03:12.000000 otpcr-6/otpcr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3211 2024-04-23 18:01:55.000000 otpcr-6/otpcr/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1252 2024-04-23 15:29:42.000000 otpcr-6/otpcr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1020 2024-04-23 15:30:07.000000 otpcr-6/otpcr/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5322 2024-04-23 18:10:11.000000 otpcr-6/otpcr/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3186 2024-04-23 18:12:05.000000 otpcr-6/otpcr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5784 2024-04-23 15:32:16.000000 otpcr-6/otpcr/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6151 2024-04-23 14:04:02.000000 otpcr-6/otpcr/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      748 2024-04-23 14:11:58.000000 otpcr-6/otpcr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      226 2024-04-23 14:01:57.000000 otpcr-6/otpcr/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-23 12:01:06.000000 otpcr-6/otpcr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1871 2024-04-23 18:21:05.000000 otpcr-6/otpcr/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1036 2024-04-23 14:02:33.000000 otpcr-6/otpcr/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1093 2024-04-23 14:04:24.000000 otpcr-6/otpcr/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-24 05:30:20.967082 otpcr-6/otpcr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2394 2024-04-24 05:30:20.000000 otpcr-6/otpcr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1002 2024-04-24 05:30:20.000000 otpcr-6/otpcr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-24 05:30:20.000000 otpcr-6/otpcr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-24 05:30:20.000000 otpcr-6/otpcr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-24 05:30:20.000000 otpcr-6/otpcr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-24 05:30:20.000000 otpcr-6/otpcr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)     1016 2024-04-23 13:41:20.000000 otpcr-6/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-24 05:30:20.967082 otpcr-6/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-23 11:57:54.000000 otpcr-6/setup.py
```

### Comparing `otpcr-5/PKG-INFO` & `otpcr-6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 5
+Version: 6
 Summary: OTP-CR-117/19
 Author-email: xobjectz <objx@proton.me>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,14 @@
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 |
 
-
 Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
```

### Comparing `otpcr-5/README.rst` & `otpcr-6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 |
 
-
 Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
```

### Comparing `otpcr-5/docs/MANUAL.rst` & `otpcr-6/docs/MANUAL.rst`

 * *Files identical despite different names*

### Comparing `otpcr-5/files/EM_Ack_OTP-CR-117_19.pdf` & `otpcr-6/files/EM_Ack_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-5/files/EM_T04_OTP-CR-117_19.pdf` & `otpcr-6/files/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-5/files/EM_T07_OTP-CR-117_19_001.pdf` & `otpcr-6/files/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `otpcr-5/otpcr/__main__.py` & `otpcr-6/otpcr/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,86 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,W0611
+# pylint: disable=W0212
 # ruff: noqa: E402
 
 
-"""NAME
-
-    OTPCR - 117/19
-
-SYNOPSIS
-
-    otpcr <cmd> [key=val] [key==val]
-
-OPTIONS
-
-    -a     load all modules
-    -c     start console
-    -d     start daemon
-    -h     display help
-    -v     use verbose
-
-EXAMPLE
-
-    otpcr -cav
-
-COPYRIGHT
-
-    OTPCR is Public Domain."""
-
-
 "main"
 
 
 import getpass
 import os
 import pwd
 import readline
 import sys
 import termios
 import time
 
 
-sys.path.insert(0, os.getcwd())
-
+from .client  import Client, cmnd, parse_cmd, spl
+from .command import Command
+from .default import Default
+from .errors  import debug, enable, errors
+from .event   import Event
+from .object  import cdir
+from .runtime import broker
+from .workdir import Workdir, skel
 
-from otpcr.client  import Client, cmnd, parse_cmd, spl
-from otpcr.command import Command
-from otpcr.default import Default
-from otpcr.errors  import debug, enable, errors
-from otpcr.event   import Event
-from otpcr.object  import cdir
-from otpcr.runtime import broker
-from otpcr.workdir import Workdir, skel
 
-
-from otpcr import modules
-
-
-if os.path.exists("mods"):
-    import mods
-else:
-    mods = None
+from . import modules
 
 
 Cfg             = Default()
+Cfg.dis         = "mbx,rst,udp"
 Cfg.mod         = "cmd,mod"
 Cfg.opts        = ""
 Cfg.name        = "otpcr"
-Cfg.version     = "5"
-Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.workdir = Cfg.wd
+Cfg.version     = "6"
+Cfg.wdr          = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
+
+
+Workdir.workdir = Cfg.wdr
 
 
 dte = time.ctime(time.time()).replace("  ", " ")
 
 
 class Console(Client):
 
+    "Console"
+
     def __init__(self):
         Client.__init__(self)
         broker.add(self)
 
     def announce(self, txt):
-        pass
+        "disable announce."
 
     def callback(self, evt):
+        "wait for callback."
         Client.callback(self, evt)
         evt.wait()
 
     def poll(self):
+        "poll console and create event."
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, channel, txt):
+    def say(self, _channel, txt):
+        "print to console"
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
 def daemon(pidfile, verbose=False):
+    "switch to background."
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
         os._exit(0)
@@ -122,41 +97,45 @@
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
 def init(pkg, modstr, disable=""):
+    "init"
     mds = []
     for modname in spl(modstr):
         if skip(modname, disable):
             continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         if "init" in dir(module):
             module.init()
             mds.append(module)
     return mds
 
 
 def privileges(username):
+    "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def skip(name, skipped):
+    "check for skipping"
     for skp in spl(skipped):
         if skp in name:
             return True
     return False
 
 
 def wrap(func):
+    "restore console."
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
@@ -164,59 +143,52 @@
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
 def ver(event):
+    "show version."
     event.reply(f"{Cfg.name.upper()} {Cfg.version}")
 
 
 def main():
+    "main"
     Command.add(ver)
     enable(print)
     skel()
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
+    if Cfg.sets.dis:
+        Cfg.dis += "," + Cfg.sets.dis
     if 'a' in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
-        if mods:
-            Cfg.mod += "," + ",".join(mods.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     if "h" in Cfg.opts:
         print(__doc__)
-        return
-    if "d" in Cfg.opts:
+    elif "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
         Cfg.user = getpass.getuser()
         daemon(Cfg.pidfile, "v" in Cfg.opts)
         privileges(Cfg.user)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
-        return
-    if "c" in Cfg.opts:
-        init(modules, Cfg.mod, Cfg.sets.dis)
-        if mods:
-            Cfg.mod += "," + ",".join(mods.__dir__())
-            init(mods, Cfg.mod)
+    elif "c" in Cfg.opts:
+        init(modules, Cfg.mod, Cfg.dis)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
-        return
-    if Cfg.otxt:
-        return cmnd(Cfg.otxt, print)
-
-
-def daemoned():
-    Cfg.opts += "d"
-    main()
+    elif Cfg.otxt:
+        cmnd(Cfg.otxt, print)
 
 
 def wrapped():
+    "wrap main function."
     wrap(main)
-    errors()
 
 
 if __name__ == "__main__":
+    readline.redisplay()
     wrapped()
+    errors()
```

### Comparing `otpcr-5/otpcr/client.py` & `otpcr-6/otpcr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0718
+# pylint: disable=W0718
 
 
 "client"
 
 
 from .command import Command
 from .default import Default
```

### Comparing `otpcr-5/otpcr/errors.py` & `otpcr-6/otpcr/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+# pylint: disable=R0903
 
 
 "errors"
 
 
 import io
 import traceback
 
 
 class Errors:
 
     "Errors"
 
     errors = []
-
+    filter = []    
 
     @staticmethod
     def out(txt):
         "overload this."
 
 
 def debug(txt):
+    "print to console."
+    for skp in Errors.filter:
+        if skp in txt:
+            return
     Errors.out(txt)
 
 
 def enable(func):
+    "set output function."
     Errors.out = func
 
 
 def later(exc):
     "add an exception"
     excp = exc.with_traceback(exc.__traceback__)
     Errors.errors.append(excp)
```

### Comparing `otpcr-5/otpcr/event.py` & `otpcr-6/otpcr/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+# pylint: disable=R0902
 
 
 "event"
 
 
 import threading
```

### Comparing `otpcr-5/otpcr/find.py` & `otpcr-6/otpcr/find.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+#
 
 
 "locate"
 
 
 import os
 import time
```

### Comparing `otpcr-5/otpcr/handler.py` & `otpcr-6/otpcr/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212
+# pylint: disable=W0212
 
 
 "handler"
 
 
 import queue
 import threading
```

### Comparing `otpcr-5/otpcr/modules/fnd.py` & `otpcr-6/otpcr/modules/fnd.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..find    import find
 from ..object  import fmt
 from ..persist import long
 from ..workdir import liststore, skel
 
 
 def fnd(event):
+    "locate objects."
     skel()
     if not event.rest:
         res = sorted([x.split('.')[-1].lower() for x in liststore()])
         if res:
             event.reply(",".join(res))
         return
     otype = event.args[0]
```

### Comparing `otpcr-5/otpcr/modules/irc.py` & `otpcr-6/otpcr/modules/irc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0612,W0718,E0402,W0201,W0603
+# pylint: disable=C,R,W0105,W0718
 # ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
@@ -17,58 +17,56 @@
 import time
 import _thread
 
 
 from ..client  import Client, command
 from ..command import Command
 from ..default import Default
-from ..errors  import debug, later
 from ..event   import Event
+from ..errors  import Errors, debug, later
 from ..find    import last
-from ..object  import Object, edit, fmt, keys
+from ..object  import Object, edit, fmt, keys, values
 from ..persist import whitelist
 from ..runtime import broker
 from ..thread  import launch
 from ..workdir import sync
 
 
-NAME       = __file__.split(os.sep)[-3]
-filterlist = ["PING", "PONG", "PRIVMSG"]
-saylock    = _thread.allocate_lock()
+NAME    = __file__.split(os.sep)[-3]
+get     = broker.get
+saylock = _thread.allocate_lock()
 
 
-myirc = None
+Errors.filter = ["PING", "PONG", "PRIVMSG"]
 
 
-def dbg(txt):
-    for flt in filterlist:
-        if flt in txt:
-            return
-    debug(txt)
-
 def init():
-    global myirc
+    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
-    myirc = irc
     return irc
 
 
 def shutdown():
-    dbg(f"IRC stopping {myirc}")
-    if myirc:
-        myirc.state.pongcheck = True
-        myirc.state.keeprunning = False
-        myirc.events.connected.clear()
-        myirc.stop()
+    "shutdown irc bot."
+    for bot in values(broker.objs):
+        if "irc" not in type(bot):
+            continue
+        debug(f"IRC stopping {repr(bot)}")
+        bot.state.pongcheck = True
+        bot.state.keeprunning = False
+        bot.events.connected.clear()
+        bot.stop()
 
 
 class Config(Default):
 
+    "Config"
+
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
     realname = NAME
@@ -92,14 +90,16 @@
 
 
 whitelist(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
+    "TextWrap"
+
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -107,47 +107,54 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
+    "Output"
+
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
+        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
+        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
         chanlist = getattr(Output.cache, channel)
         chanlist.extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
+        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
+        "put text to output queue."
         if channel and channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
+        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -162,21 +169,24 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
+        "return size of channel cache."
         if chan in Output.cache:
             return len(getattr(Output.cache, chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
+    "IRC"
+
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
         self.channels = []
         self.events = Default()
@@ -202,18 +212,20 @@
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
         broker.add(self)
 
     def announce(self, txt):
+        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
+        "send command to server."
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -222,18 +234,19 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
+        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
-            dbg("using SASL")
+            debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1
             ctx.minimum_version = ssl.TLSVersion.TLSv1_2
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
@@ -248,47 +261,51 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
+        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as ex:
+               ) as _ex:
             pass
         except Exception as ex:
             later(ex)
 
     def doconnect(self, server, nck, port=6667):
+        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
                 self.state.error = str(ex)
-                dbg(str(ex))
-            dbg(f"sleeping {self.cfg.sleep} seconds")
+                debug(str(ex))
+            debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
+        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.docommand('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
@@ -307,49 +324,53 @@
         elif cmd == '433':
             self.state.error = txt
             nck = self.cfg.nick + '_'
             self.docommand('NICK', nck)
         return evt
 
     def joinall(self):
+        "join all channels."
         for channel in self.channels:
             self.docommand('JOIN', channel)
 
     def keep(self):
+        "keep alive."
         while not self.stopped.is_set():
             if self.state.stopkeep:
                 self.state.stopkeep = False
                 break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.docommand('PING', self.cfg.server)
             if self.state.pongcheck:
-                dbg("failed pongcheck, restarting")
+                debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
+        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
+        "parse text into an event."
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        dbg(txt)
+        debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
@@ -399,14 +420,15 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
+        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -416,26 +438,27 @@
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 later(ex)
                 self.stop()
-                dbg("handler stopped")
+                debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
+        "send raw text."
         txt = txt.rstrip()
-        dbg(txt)
+        debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
@@ -448,47 +471,52 @@
                 later(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        dbg(f"reconnecting to {self.cfg.server}")
+        "reconnect to server."
+        debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
+        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.docommand('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
+        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
+        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
+        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
         launch(Client.start, self)
@@ -498,101 +526,119 @@
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
+        "stop bot."
         self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
+        "wait for ready."
         self.events.ready.wait()
 
 
+"callbacks"
+
+
 def cb_auth(bot, evt):
+    "auth callback."
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
 def cb_cap(bot, evt):
+    "capabilities callback."
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
 def cb_error(bot, evt):
+    "error callback."
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
-    dbg(evt.txt)
+    debug(evt.txt)
 
 
 def cb_h903(bot, evt):
+    "auth succeded callback."
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(bot, evt):
+    "auth succeded callback."
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(bot, evt):
-    pass
+    "got killed callback."
 
 
 def cb_log(bot, evt):
-    pass
+    "log callback."
 
 
 def cb_ready(bot, evt):
-    bot.events.ready.set()
+    "bot is ready callback."
+    bot = get(evt.orig)
+    if bot:
+        bot.events.ready.set()
 
 
 def cb_001(bot, evt):
+    "first line received callback."
     bot.logon()
 
 
 def cb_notice(bot, evt):
+    "notice callback."
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
 def cb_privmsg(bot, evt):
+    "privmsg callback."
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
-        dbg(f"command from {evt.origin}: {evt.txt}")
+        debug(f"command from {evt.origin}: {evt.txt}")
         command(bot, evt)
 
 
 def cb_quit(bot, evt):
-    dbg(f"quit from {bot.cfg.server}")
+    "quit callback."
+    debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
 "commands"
 
 
 def cfg(event):
+    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
@@ -601,18 +647,16 @@
                    )
     else:
         edit(config, event.sets)
         sync(config, path)
         event.reply('ok')
 
 
-Command.add(cfg)
-
-
 def mre(event):
+    "show from output cache."
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
@@ -623,24 +667,27 @@
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
     event.reply(f'{size} more in cache')
 
 
-Command.add(mre)
-
-
 def pwd(event):
+    "create a base64 password."
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
 
 
+"register"
+
+
+Command.add(cfg)
+Command.add(mre)
 Command.add(pwd)
```

### Comparing `otpcr-5/otpcr/modules/mdl.py` & `otpcr-6/otpcr/modules/mdl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0613,E0402,W0105
+# pylint: disable=C0209,W0105
 
 
-"genocide model of the netherlands"
+"genocide model of the netherlands since 01-01-2020"
 
 
 import datetime
 import time
 
 
 from ..client   import laps
@@ -17,31 +17,31 @@
 from ..repeater import Repeater
 from ..runtime  import broker
 from ..thread   import launch
 
 
 DAY = 24*60*60
 YEAR = 365*DAY
-SOURCE = "https://github.com/bthate/genocide"
+SOURCE = "https://github.com/xobjectz/otpcr"
 STARTDATE = "2020-01-01 00:00:00"
 STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
 
 def init():
+    "start repeaters"
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
             repeater = Repeater(sec, cbstats, evt, thrname=aliases.get(key))
             repeater.start()
     launch(daily, name="daily")
-    
 
 
 oor = """"Totaal onderliggende doodsoorzaken (aantal)";
          "1 Infectieuze en parasitaire ziekten/Totaal infectieuze en parasitaire zktn (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.1 Tuberculose (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.2 Meningokokkeninfecties (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.3 Virale hepatitis (aantal)";
@@ -273,76 +273,87 @@
 
 oorzaak = Object()
 construct(oorzaak, zip(oor, aantal))
 oorzaken = Object()
 
 
 def getalias(txt):
+    "return value of alias."
+    result = None
     for key, value in aliases.items():
         if txt.lower() in key.lower():
-            return value
-
+            result = value
+            break
+    return result
 
 def getday():
+    "timestamp of current day."
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
+    "fetch mortality number."
     for k in keys(oorzaken):
         if name.lower() in k.lower():
             return int(getattr(oorzaken, k))
     return 0
 
 
 def seconds(nrs):
+    "convert nr/years to seconds."
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
 
 def iswanted(k, line):
+    "see whether filtered or not."
     for word in line:
         if word in k:
             return True
     return False
 
 
 def daily():
+    "daily job"
     while 1:
         time.sleep(24*60*60)
         evt = Event()
         cbnow(evt)
 
 
 def hourly():
+    "hourly job"
     while 1:
         time.sleep(60*60)
         evt = Event()
         cbnow(evt)
 
 
-def cbnow(evt):
+def cbnow(_evt):
+    "now callback"
     delta = time.time() - STARTTIME
     txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
-        txt += "%s: %s " % (getalias(name), nrtimes)
+        txt += f"{getalias(name)} {nrtimes} |"
     txt += " http://genocide.rtfd.io"
     for bot in values(broker.objs):
         if "announce" in dir(bot):
             bot.announce(txt)
 
 
 def cbstats(evt):
+    "stats callback."
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
         nrday = int(DAY/needed)
@@ -357,14 +368,15 @@
                                                                nryear,
                                                               )
         for bot in values(broker.objs):
             bot.announce(txt)
 
 
 def now(event):
+    "now command."
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         txt = laps(delta) + " "
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
@@ -385,22 +397,16 @@
 
 Command.add(now)
 
 
 "interface"
 
 
-def __dir__():
-    return (
-            'init',
-            'now'
-           ) 
-
-
 def boot():
+    "construct model"
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
         if _nr == 0:
             continue
         if key.startswith('"'):
             key = key[1:]
@@ -422,8 +428,15 @@
         atl = atl.replace(", bevalling en kraambed. ", "")
         atl = atl.replace("Aandoeningen v.d. ", "")
         nms = " ".join(atl.split()[1:]).capitalize()
         nms = nms.strip()
         setattr(oorzaken, nms, aantal[_nr])
 
 
+def __dir__():
+    return (
+            'init',
+            'now'
+           )
+
+
 boot()
```

### Comparing `otpcr-5/otpcr/modules/req.py` & `otpcr-6/otpcr/modules/req.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0115,C0116
-
+#
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
+|
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of
 the Rome Statute. i want to inform the prosecutor that the king of the
 netherlands and his government are commiting 3 of the 5 crimes defined
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
@@ -79,11 +79,12 @@
 """
 
 
 from ..command import Command
 
 
 def req(event):
+    "reconsider"
     event.reply(__doc__)
 
 
 Command.add(req)
```

### Comparing `otpcr-5/otpcr/modules/rss.py` & `otpcr-6/otpcr/modules/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+# pylint: disable=R0903,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
```

### Comparing `otpcr-5/otpcr/modules/tdo.py` & `otpcr-6/otpcr/modules/tdo.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 from ..find    import fntime, find
 from ..persist import whitelist
 from ..workdir import sync
 
 
 class NoDate(Exception):
 
-    pass
+    "no matching date"
 
 
 class Todo(Object):
 
+    "Todo"
+ 
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
 
 whitelist(Todo)
 
 
 def dne(event):
+    "flag todo as done."
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
     nmr = 0
     for fnm, obj in find('todo', selector):
         nmr += 1
@@ -48,14 +51,15 @@
         event.reply("nothing todo")
 
 
 Command.add(dne)
 
 
 def tdo(event):
+    "add todo."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
```

### Comparing `otpcr-5/otpcr/modules/thr.py` & `otpcr-6/otpcr/modules/thr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0116,W0105,E0402,E0401,E0611
+#
 
 
 "show running threads"
 
 
 import threading
 import time
@@ -14,14 +14,15 @@
 from ..object import Object, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
+    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
```

### Comparing `otpcr-5/otpcr/modules/tmr.py` & `otpcr-6/otpcr/modules/tmr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0612,W0105,W0702,E0402
+# pylint: disable=W0105
 
 
 "timer"
 
 
 import datetime
 import re
 import time as ttime
 
 
 from ..client  import laps
 from ..command import Command
 from ..event   import Event
 from ..find    import find
+from ..object  import update
+from ..persist import whitelist
 from ..runtime import broker
-from ..timer   import Timer
 from ..thread  import launch
-from ..persist import whitelist
-from ..object  import update
+from ..timer   import Timer
 from ..workdir import sync
 
 
-def init():
-    for fnm, obj in find("timer"):
-        if "time" not in obj:
-            continue
-        diff = float(obj.time) - ttime.time()
-        if diff > 0:
-            bot = broker.first()
-            evt = Event()
-            update(evt, obj)
-            evt.orig = object.__repr__(bot)
-            timer = Timer(diff, evt.show)
-            launch(timer.start)
-
-
 MONTHS = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
     'Apr',
     'May',
@@ -60,31 +46,31 @@
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    pass
-
-
-whitelist(Timer)
+    "NoDate"
 
 
 def extract_date(daystr):
+    "extract date from string."
+    res = None
     for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
+            break
         except ValueError:
             res = None
-        if res:
-            return res
+    return res
 
 
 def get_day(daystr):
+    "return day from string."
     day = None
     month = None
     yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
         if ymdre:
             (day, month, yea) = ymdre.groups()
@@ -96,20 +82,21 @@
                 yea = ttime.strftime("%Y", ttime.localtime())
         except Exception as ex:
             raise NoDate(daystr) from ex
     if day:
         day = int(day)
         month = int(month)
         yea = int(yea)
-        date = "%s %s %s" % (day, MONTHS[month], yea)
+        date = f"{day} {MONTHS[month]} {yea}"
         return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
     raise NoDate(daystr)
 
 
 def get_hour(daystr):
+    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -123,25 +110,27 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
+    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
 def parse_time(txt):
+    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -156,78 +145,102 @@
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
 def to_day(daystr):
+    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
+    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
+            break
         except ValueError:
             res = None
-        if res:
-            return res
         line = ""
+    return res
 
 
 def today():
+    "return date."
     return str(datetime.datetime.today()).split()[0]
 
 
 "commands"
 
 
 def tmr(event):
+    "add a timer."
+    result = ""
     if not event.rest:
         nmr = 0
-        for fnm, obj in find('timer'):
-            if "time" not in obj:
-                continue
+        for _fn, obj in find('timer'):
             lap = float(obj.time) - ttime.time()
             if lap > 0:
                 event.reply(f'{nmr} {obj.txt} {laps(lap)}')
                 nmr += 1
-        if not nmr:
-            event.reply("no timers")
-        return
+        return result
     seconds = 0
     line = ""
     for word in event.args:
         if word.startswith("+"):
             try:
                 seconds = int(word[1:])
             except (ValueError, IndexError):
-                event.reply("%s is not an integer" % seconds)
-                return
+                event.reply(f"{seconds} is not an integer")
+                return result
         else:
             line += word + " "
     if seconds:
         target = ttime.time() + seconds
     else:
         try:
             target = get_day(event.rest)
         except NoDate:
             target = to_day(today())
         hour =  get_hour(event.rest)
         if hour:
             target += hour
     if not target or ttime.time() > target:
         event.reply("already passed given time.")
-        return
+        return result
     event.time = target
     diff = target - ttime.time()
     event.reply("ok " +  laps(diff))
     event.result = []
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
+    return result
+
+
+"runtime"
+
+
+def init():
+    "start timers."
+    for _fn, obj in find("timer"):
+        if "time" not in obj:
+            continue
+        diff = float(obj.time) - ttime.time()
+        if diff > 0:
+            bot = broker.first()
+            evt = Event()
+            update(evt, obj)
+            evt.orig = object.__repr__(bot)
+            timer = Timer(diff, evt.show)
+            launch(timer.start)
+
+
+"register"
 
 
 Command.add(tmr)
+whitelist(Timer)
```

### Comparing `otpcr-5/otpcr/modules/wsd.py` & `otpcr-6/otpcr/modules/wsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,I,R,E0401,W0105
+#
 
 
 """| wijsheid, wijs !
 
 | OVERDRACHT
 | ==========
 
@@ -192,11 +192,12 @@
 from ..command import Command
 
 
 rand = SystemRandom()
 
 
 def wsd(event):
+    "show wisdom."
     event.reply(rand.choice(__doc__.split("\n")).strip()[2:])
 
 
 Command.add(wsd)
```

### Comparing `otpcr-5/otpcr/object.py` & `otpcr-6/otpcr/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+# pylint: disable=W0105
 
 
 "objects"
 
 
 import json
 import os
```

### Comparing `otpcr-5/otpcr/thread.py` & `otpcr-6/otpcr/thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0718
+# pylint: disable=W0718
 
 
 "thread"
 
 
 import queue
 import threading
@@ -28,16 +28,15 @@
         self.starttime = time.time()
         self.queue.put_nowait((func, args))
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        for k in dir(self):
-            yield k
+        yield from dir(self)
 
     def join(self, timeout=1.0):
         "join this thread."
         super().join(timeout)
         return self._result
 
     def run(self):
```

### Comparing `otpcr-5/otpcr/timer.py` & `otpcr-6/otpcr/timer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+#
 
 
 "timer"
 
 
 import threading
 import time
 
 
 from .thread import launch
 
 
 class Timer:
 
-    "run a function at a specific time."
+    "Timer"
 
     def __init__(self, sleep, func, *args, thrname=None):
         self.args  = args
         self.func  = func
         self.sleep = sleep
         self.name  = thrname or str(self.func).split()[2]
         self.state = {}
```

### Comparing `otpcr-5/otpcr/workdir.py` & `otpcr-6/otpcr/workdir.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=R0903
 
 
-"working directory"
+"workdir"
 
 
 import datetime
 import os
 
 
 from .object import Object, cdir, fqn, read, write
```

### Comparing `otpcr-5/otpcr.egg-info/PKG-INFO` & `otpcr-6/otpcr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 5
+Version: 6
 Summary: OTP-CR-117/19
 Author-email: xobjectz <objx@proton.me>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,14 @@
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 |
 
-
 Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
```

### Comparing `otpcr-5/otpcr.egg-info/SOURCES.txt` & `otpcr-6/otpcr.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 README.rst
 pyproject.toml
 setup.py
 docs/MANUAL.rst
 files/EM_Ack_OTP-CR-117_19.pdf
 files/EM_T04_OTP-CR-117_19.pdf
 files/EM_T07_OTP-CR-117_19_001.pdf
-files/verbatim4.png
+files/verbatim5.png
 otpcr/__init__.py
 otpcr/__main__.py
 otpcr/broker.py
 otpcr/client.py
 otpcr/command.py
 otpcr/default.py
 otpcr/errors.py
@@ -32,15 +32,18 @@
 otpcr/modules/__init__.py
 otpcr/modules/cmd.py
 otpcr/modules/err.py
 otpcr/modules/flt.py
 otpcr/modules/fnd.py
 otpcr/modules/irc.py
 otpcr/modules/log.py
+otpcr/modules/mbx.py
 otpcr/modules/mdl.py
 otpcr/modules/mod.py
 otpcr/modules/req.py
 otpcr/modules/rss.py
+otpcr/modules/rst.py
 otpcr/modules/tdo.py
 otpcr/modules/thr.py
 otpcr/modules/tmr.py
+otpcr/modules/udp.py
 otpcr/modules/wsd.py
```

### Comparing `otpcr-5/pyproject.toml` & `otpcr-6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otpcr"
 description = "OTP-CR-117/19"
-version = "5"
+version = "6"
 authors = [
     {name = "xobjectz", email = "objx@proton.me"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
@@ -38,12 +38,12 @@
 zip-safe=true
 
 
 [tool.setuptools.data-files]
 "share/doc/otpcr" = [
     "README.rst",
     "docs/MANUAL.rst",
-    "files/verbatim4.png",
+    "files/verbatim5.png",
     "files/EM_Ack_OTP-CR-117_19.pdf",
     "files/EM_T07_OTP-CR-117_19_001.pdf",
     "files/EM_T04_OTP-CR-117_19.pdf"
 ]
```


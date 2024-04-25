# Comparing `tmp/indipyclient-0.0.5.tar.gz` & `tmp/indipyclient-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.5.tar` & `indipyclient-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.5/LICENSE
--rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.5/README.md
--rw-r--r--   0        0        0      291 2024-04-13 20:37:30.000000 indipyclient-0.0.5/indipyclient/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.5/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.5/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.5/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.5/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   143996 2024-04-08 20:45:37.000000 indipyclient-0.0.5/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.5/indipyclient/error.py
--rw-r--r--   0        0        0    25044 2024-04-13 18:46:37.000000 indipyclient-0.0.5/indipyclient/events.py
--rw-r--r--   0        0        0    34740 2024-04-12 08:47:00.000000 indipyclient-0.0.5/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    15584 2024-04-11 11:19:29.000000 indipyclient-0.0.5/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27590 2024-04-13 18:00:12.000000 indipyclient-0.0.5/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-04-13 20:37:50.000000 indipyclient-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.6/README.md
+-rw-r--r--   0        0        0      291 2024-04-25 16:27:19.000000 indipyclient-0.0.6/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.6/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.6/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.6/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.6/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144085 2024-04-25 16:29:53.000000 indipyclient-0.0.6/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.6/indipyclient/error.py
+-rw-r--r--   0        0        0    25044 2024-04-13 18:46:37.000000 indipyclient-0.0.6/indipyclient/events.py
+-rw-r--r--   0        0        0    34740 2024-04-12 08:47:00.000000 indipyclient-0.0.6/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    15584 2024-04-11 11:19:29.000000 indipyclient-0.0.6/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27590 2024-04-13 18:00:12.000000 indipyclient-0.0.6/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-04-25 16:27:34.000000 indipyclient-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.6/PKG-INFO
```

### Comparing `indipyclient-0.0.5/LICENSE` & `indipyclient-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/README.md` & `indipyclient-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/__main__.py` & `indipyclient-0.0.6/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/console/consoleclient.py` & `indipyclient-0.0.6/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/console/widgets.py` & `indipyclient-0.0.6/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/console/windows.py` & `indipyclient-0.0.6/indipyclient/console/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,38 +489,41 @@
         if isinstance(event, events.Message):
             widgets.drawmessage(self.messwin, self.client.messages[0], maxcols=self.maxcols)
             self.messwin.noutrefresh()
             curses.doupdate()
 
 
     async def submit(self):
-        self._newpath = self.path_txt.text
+        self._newpath = self.path_txt.text.strip()
+        blobfolder = None
         if self._newpath:
             try:
                 blobfolder = pathlib.Path(self._newpath).expanduser().resolve()
             except Exception:
                 self.control.blobenabled = False
                 self.control.send_disableBLOB()
                 self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
-                await self.client.report("Warning! BLOB folder is invalid")
+                await self.client.report("Warning! Unable to parse BLOB folder")
+                self.submit_btn.focus = False
+                self.messages_btn.focus = True
+                return
+            if blobfolder.is_dir():
+                self.control.blobfolder = blobfolder
+                self._newpath = str(blobfolder)
+                self.path_txt.text = self._newpath
+                self.path_txt.draw()
+                self.control.blobenabled = True
+                self.control.send_enableBLOB()
+                self.pathwin.addstr(0, 0, "BLOBs are enabled  ", curses.A_BOLD)
+                await self.client.report("BLOB folder is set")
             else:
-                if blobfolder.is_dir():
-                    self.control.blobfolder = blobfolder
-                    self._newpath = str(blobfolder)
-                    self.path_txt.text = self._newpath
-                    self.path_txt.draw()
-                    self.control.blobenabled = True
-                    self.control.send_enableBLOB()
-                    self.pathwin.addstr(0, 0, "BLOBs are enabled  ", curses.A_BOLD)
-                    await self.client.report("BLOB folder is set")
-                else:
-                    self.control.blobenabled = False
-                    self.control.send_disableBLOB()
-                    self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
-                    await self.client.report("Warning! BLOB folder is invalid")
+                self.control.blobenabled = False
+                self.control.send_disableBLOB()
+                self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
+                await self.client.report("Warning! BLOB folder is not a directory")
         else:
             self.control.blobenabled = False
             self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
             await self.client.report("Warning! BLOB folder is invalid")
             self.control.send_disableBLOB()
         self.submit_btn.focus = False
         self.messages_btn.focus = True
```

### Comparing `indipyclient-0.0.5/indipyclient/events.py` & `indipyclient-0.0.6/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/ipyclient.py` & `indipyclient-0.0.6/indipyclient/ipyclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/propertymembers.py` & `indipyclient-0.0.6/indipyclient/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/indipyclient/propertyvectors.py` & `indipyclient-0.0.6/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.5/pyproject.toml` & `indipyclient-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.5"
+version = "0.0.6"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.5/PKG-INFO` & `indipyclient-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```


# Comparing `tmp/monisha-0.0.58.tar.gz` & `tmp/monisha-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.58.tar", last modified: Mon Apr 22 09:41:02 2024, max compression
+gzip compressed data, was "monisha-0.0.59.tar", last modified: Thu Apr 25 13:26:43 2024, max compression
```

## Comparing `monisha-0.0.58.tar` & `monisha-0.0.59.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:41:02.334771 monisha-0.0.58/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 09:40:44.000000 monisha-0.0.58/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:41:02.326771 monisha-0.0.58/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:41:02.330771 monisha-0.0.58/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/functions/function17.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:41:02.330771 monisha-0.0.58/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 09:40:44.000000 monisha-0.0.58/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-22 09:41:02.334771 monisha-0.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 09:40:44.000000 monisha-0.0.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:41:02.334771 monisha-0.0.58/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-22 09:41:02.000000 monisha-0.0.58/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 09:41:02.000000 monisha-0.0.58/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:41:02.000000 monisha-0.0.58/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 09:41:02.000000 monisha-0.0.58/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 09:41:02.000000 monisha-0.0.58/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:41:02.334771 monisha-0.0.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 09:40:44.000000 monisha-0.0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 13:26:36.000000 monisha-0.0.59/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.619930 monisha-0.0.59/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/functions/function18.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-25 13:26:36.000000 monisha-0.0.59/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 13:26:43.623930 monisha-0.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 13:26:36.000000 monisha-0.0.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:26:43.623930 monisha-0.0.59/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 13:26:43.000000 monisha-0.0.59/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:26:43.623930 monisha-0.0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-25 13:26:36.000000 monisha-0.0.59/setup.py
```

### Comparing `monisha-0.0.58/LICENSE` & `monisha-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/__init__.py` & `monisha-0.0.59/Monisha/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.58"
+version = "0.0.59"
 
 install = ["python-magic"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `monisha-0.0.58/Monisha/functions/__init__.py` & `monisha-0.0.59/Monisha/functions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from .function14 import CDirectory, UDirectory, BDirectory
 from .function01 import timend, uptime, Timemod, Timesod
 from .function06 import Okeys, Ukeys, Bkeys, Mkeys
+from .function02 import Dbytes, Hbytes, Gbytes
+from .function04 import Eimes, Mimeo, Mimes
 from .function03 import progress, Progress
-from .function04 import Rawexo, Extions
-from .function02 import Dbytes, Hbytes
 from .function06 import Skeys, Uname
 from .function07 import Cmd, Wosd
+from .function18 import Metadatas
 from .function15 import Location
+from .function17 import Filename
 from .function16 import FMagic
 from .function10 import Fonts
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
 from .function09 import Sage
 from .function13 import Guid
```

### Comparing `monisha-0.0.58/Monisha/functions/function01.py` & `monisha-0.0.59/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/functions/function03.py` & `monisha-0.0.59/Monisha/functions/function03.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ..scripts import Smbo
 #===================================================================================
 
-def progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=20):
+def progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=10):
     percenage = float(percentage)
     passngeso = min(max(percenage, 0), 100)
     cosmosses = int(passngeso // l01)
     outgoings = b01 * cosmosses
     outgoings += b02 * (l02 - cosmosses)
     return outgoings
 
 #===================================================================================
 
-async def Progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=20):
+async def Progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=10):
     percenage = float(percentage)
     passngeso = min(max(percenage, 0), 100)
     cosmosses = int(passngeso // l01)
     outgoings = b01 * cosmosses
     outgoings += b02 * (l02 - cosmosses)
     return outgoings
```

### Comparing `monisha-0.0.58/Monisha/functions/function06.py` & `monisha-0.0.59/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/functions/function07.py` & `monisha-0.0.59/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/functions/function10.py` & `monisha-0.0.59/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/functions/function14.py` & `monisha-0.0.59/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/functions/function15.py` & `monisha-0.0.59/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/Monisha/functions/function16.py` & `monisha-0.0.59/Monisha/functions/function16.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,27 +4,27 @@
         self.types = kwargs.get("types", None)
         self.error = kwargs.get("types", None)
 
 #====================================================================
 
 class FMagic:
 
-    def filestype(file):
+    def get01(file):
         try:
             from magic import Magic
             mimees = Magic(mime=True)
             mimeos = mimees.from_file(file)
             mimemo = mimeos or "text/plain"
             return SMessages(types=mimemo)
         except Exception as errors:
             return SMessages(types="application/zip", error=errors)
 
 #====================================================================
 
-    async def filextype(file):
+    async def get02(file):
         try:
             from magic import Magic
             mimees = Magic(mime=True)
             mimeos = mimees.from_file(file)
             mimemo = mimeos or "text/plain"
             return SMessages(types=mimemo)
         except Exception as errors:
```

### Comparing `monisha-0.0.58/Monisha/functions/function17.py` & `monisha-0.0.59/Monisha/functions/function17.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,43 +4,41 @@
 #=========================================================================
 
 
 class SMessages:
     def __init__(self, **kwargs):
         self.errors = kwargs.get("errors", None)
         self.result = kwargs.get("result", None)
+        self.filename = kwargs.get("filename", None)
+        self.extension = kwargs.get("extension", None)
 
 #=========================================================================
 
 class Filename:
 
     async def get01(extension=None):
         mainos = str(random.randint(10000, 100000000000000))
         moonus = mainos + extension if extension else mainos
         return moonus
 
 #=========================================================================
 
-    async def get02(filelink):
+    async def get02(filename):
+        nameas = str(filename)
+        cnames = os.path.splitext(nameas)[0]
+        exexon = os.path.splitext(nameas)[1]
+        exoexo = exexon if exexon else ".tmp"
+        moonus = finame if finame else "Unknown"
+        return SMessages(filename=moonus, extension=exoexo)
+
+#=========================================================================
+
+    async def get03(filelink):
         try:
             findoutne = urlparse(filelink)
             filenameo = os.path.basename(findoutne.path)
             filenames = unquote(filenameo)
             return SMessages(result=filenames)
         except Exception as errors:
             return SMessages(result="Unknown.tmp", errors=errors)
 
 #=========================================================================
-
-    async def get03(filelink, command):
-        from yt_dlp import YoutubeDL
-        from ..scripts.eo import Okeys
-        with YoutubeDL(command) as ydl:
-            try:
-                mainos = Okeys.DATA01
-                meawes = ydl.extract_info(filelink, download=False)
-                moonus = ydl.prepare_filename(meawes, outtmpl=mainos)
-                return SMessages(result=moonus)
-            except Exception as errors:
-                return SMessages(result="Unknown.tmp", errors=errors)
-
-#=========================================================================
```

### Comparing `monisha-0.0.58/Monisha/scripts/es.py` & `monisha-0.0.59/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.58/PKG-INFO` & `monisha-0.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.58
+Version: 0.0.59
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.58 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.59 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.58/monisha.egg-info/PKG-INFO` & `monisha-0.0.59/monisha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.58
+Version: 0.0.59
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.58 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.59 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.58/monisha.egg-info/SOURCES.txt` & `monisha-0.0.59/monisha.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 Monisha/functions/function11.py
 Monisha/functions/function12.py
 Monisha/functions/function13.py
 Monisha/functions/function14.py
 Monisha/functions/function15.py
 Monisha/functions/function16.py
 Monisha/functions/function17.py
+Monisha/functions/function18.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
```

### Comparing `monisha-0.0.58/setup.py` & `monisha-0.0.59/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/stdf_tamer-1.0.8.tar.gz` & `tmp/stdf_tamer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf_tamer-1.0.8.tar", last modified: Mon Aug 14 05:45:14 2023, max compression
+gzip compressed data, was "stdf_tamer-1.0.9.tar", last modified: Sun Aug 27 16:08:59 2023, max compression
```

## Comparing `stdf_tamer-1.0.8.tar` & `stdf_tamer-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    11558 2023-08-14 05:42:43.311645 stdf_tamer-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0      422 2023-08-14 05:42:43.315506 stdf_tamer-1.0.8/README.md
--rw-r--r--   0        0        0     1140 2023-08-14 05:45:14.701763 stdf_tamer-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      151 2023-08-14 05:42:43.360720 stdf_tamer-1.0.8/src/_ams_rw_stdf_writer_state.py
--rw-r--r--   0        0        0    24598 2023-08-14 05:42:43.363269 stdf_tamer-1.0.8/src/ams_rw_stdf.py
--rw-r--r--   0        0        0    16086 2023-08-14 05:42:43.366683 stdf_tamer-1.0.8/src/ams_rw_stdf_writer.py
--rw-r--r--   0        0        0     5709 2023-08-14 05:42:43.370061 stdf_tamer-1.0.8/src/converter.py
--rw-r--r--   0        0        0     1549 2023-08-14 05:42:43.374058 stdf_tamer-1.0.8/src/create_index_at_dropzone.py
--rw-r--r--   0        0        0      488 2023-08-14 05:42:43.376062 stdf_tamer-1.0.8/src/example.py
--rw-r--r--   0        0        0     2148 2023-08-14 05:42:43.378504 stdf_tamer-1.0.8/src/simulator.py
--rw-r--r--   0        0        0      880 2023-08-14 05:42:43.380768 stdf_tamer-1.0.8/src/stdfanalyser.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 stdf_tamer-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-14 05:42:43.311645 stdf_tamer-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      422 2023-08-14 05:42:43.315506 stdf_tamer-1.0.9/README.md
+-rw-r--r--   0        0        0     1355 2023-08-27 16:08:59.091345 stdf_tamer-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    24598 2023-08-27 16:04:59.204388 stdf_tamer-1.0.9/src/ams_rw_stdf/__init__.py
+-rw-r--r--   0        0        0      151 2023-08-27 16:04:59.204388 stdf_tamer-1.0.9/src/ams_rw_stdf/_ams_rw_stdf_writer_state.py
+-rw-r--r--   0        0        0      117 2023-08-27 16:04:59.204388 stdf_tamer-1.0.9/src/ams_rw_stdf/_opener_collection.py
+-rw-r--r--   0        0        0     2404 2023-08-27 16:04:59.204388 stdf_tamer-1.0.9/src/ams_rw_stdf/_output_workers.py
+-rw-r--r--   0        0        0     6359 2023-08-27 16:04:59.204388 stdf_tamer-1.0.9/src/ams_rw_stdf/converter.py
+-rw-r--r--   0        0        0     2411 2023-08-27 16:04:59.204388 stdf_tamer-1.0.9/src/ams_rw_stdf/pickleconvert.py
+-rw-r--r--   0        0        0     2111 2023-08-27 16:04:59.214393 stdf_tamer-1.0.9/src/ams_rw_stdf/simulator.py
+-rw-r--r--   0        0        0      900 2023-08-27 16:04:59.214393 stdf_tamer-1.0.9/src/ams_rw_stdf/stdfanalyser.py
+-rw-r--r--   0        0        0     2397 2023-08-27 16:04:59.214393 stdf_tamer-1.0.9/src/ams_rw_stdf/stdfanalyser_for_win_context.py
+-rw-r--r--   0        0        0    16086 2023-08-27 16:04:59.214393 stdf_tamer-1.0.9/src/ams_rw_stdf_writer/__init__.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 stdf_tamer-1.0.9/PKG-INFO
```

### Comparing `stdf_tamer-1.0.8/LICENSE.txt` & `stdf_tamer-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.8/pyproject.toml` & `stdf_tamer-1.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,41 +3,49 @@
 description = "a stdf reader/writer/analyser/converter and robotframework library"
 dynamic = []
 authors = [
     { name = "Labor DC jona", email = "" },
     { name = "Franz Haas", email = "franz.haas@ams-osram.com" },
 ]
 dependencies = [
-    "robotframework",
     "construct",
     "docopt",
     "rich",
-    "polars",
-    "XlsxWriter",
-    "xlsx2csv>=0.8.1",
 ]
 requires-python = ">=3.8.0"
 readme = "README.md"
 keywords = [
     "STDF",
     "ATE",
 ]
-version = "1.0.8"
+version = "1.0.9"
 
 [project.license]
 text = "apache 2.0"
 
+[project.optional-dependencies]
+file_formats = [
+    "polars",
+    "XlsxWriter",
+    "xlsx2csv>=0.8.1",
+]
+robotframework = [
+    "robotframework",
+]
+
 [project.urls]
 Homepage = "https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer"
 Repository = "https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer"
 
 [project.scripts]
-stdfconvert = "converter:main"
-stdfrerunwithnewlimits = "simulator:main"
-stdfanalyse = "stdfanalyser:main"
+stdfconvert = "ams_rw_stdf.converter:main"
+stdfrerunwithnewlimits = "ams_rw_stdf.simulator:main"
+stdfanalyse = "ams_rw_stdf.stdfanalyser:main"
+stdfanalyser_for_win_context = "ams_rw_stdf.stdfanalyser_for_win_context:main"
+pickleconvert = "ams_rw_stdf.pickleconvert:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
@@ -47,11 +55,11 @@
 ]
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pdoc>=12.3.0",
-    "ipython>=8.6.0",
-    "radon>=5.1.0",
+    "pdoc",
+    "ipython",
+    "radon",
 ]
```

### Comparing `stdf_tamer-1.0.8/src/ams_rw_stdf.py` & `stdf_tamer-1.0.9/src/ams_rw_stdf/__init__.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.8/src/ams_rw_stdf_writer.py` & `stdf_tamer-1.0.9/src/ams_rw_stdf_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.8/src/simulator.py` & `stdf_tamer-1.0.9/src/ams_rw_stdf/simulator.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,22 @@
 
 Options:
   -h --help     Show this screen.
 """
 
 
 from docopt import docopt
-import bz2
-import gzip
 import ams_rw_stdf_writer
 import ams_rw_stdf
 import construct.core
 import rich.console
+from ams_rw_stdf._opener_collection import _opener
 
 console = rich.console.Console()
 
-
-_opener = {"bz2": bz2.open, "gz": gzip.open, "stdf": open}
-
 _singleton_entries = {(0, 10): False,
                       (1, 10): False}
 
 if __name__ == '__main__':
     main()
 
 def main():
```

### Comparing `stdf_tamer-1.0.8/src/stdfanalyser.py` & `stdf_tamer-1.0.9/src/ams_rw_stdf/stdfanalyser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-"""List records in sbtdf file.
+"""Dump stdf records to console.
+
+accepts compressed stdf files (stdf.gz, stdf.bz2)
 
 Usage:
   stdfanalyse <stdf_file_name_in>
 
 Options:
   -h --help     Show this screen.
 """
 
 
 import ams_rw_stdf
-import bz2
 import construct
 import construct.lib
 from docopt import docopt
-import gzip
 from rich.console import Console
+from ams_rw_stdf._opener_collection import _opener
 
-
-_opener = {"bz2": bz2.open, "gz": gzip.open, "stdf": open}
 construct.lib.setGlobalPrintFullStrings(True)
 
 def main():
     console = Console()
     arguments = docopt(__doc__)
     si = arguments["<stdf_file_name_in>"]
     with _opener[si.split(".")[-1]](si, "rb") as f:
```

### Comparing `stdf_tamer-1.0.8/PKG-INFO` & `stdf_tamer-1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: stdf-tamer
-Version: 1.0.8
+Version: 1.0.9
 Summary: a stdf reader/writer/analyser/converter and robotframework library
 Keywords: STDF ATE
 Author: Labor DC jona
 Author-Email: Franz Haas <franz.haas@ams-osram.com>
 License: apache 2.0
 Project-URL: Homepage, https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer
 Project-URL: Repository, https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer
 Requires-Python: >=3.8.0
-Requires-Dist: robotframework
 Requires-Dist: construct
 Requires-Dist: docopt
 Requires-Dist: rich
-Requires-Dist: polars
-Requires-Dist: XlsxWriter
-Requires-Dist: xlsx2csv>=0.8.1
+Requires-Dist: polars; extra == "file-formats"
+Requires-Dist: XlsxWriter; extra == "file-formats"
+Requires-Dist: xlsx2csv>=0.8.1; extra == "file-formats"
+Requires-Dist: robotframework; extra == "robotframework"
+Provides-Extra: file_formats
+Provides-Extra: robotframework
 Description-Content-Type: text/markdown
 
 ## stdf tamer
 This package was originally developed at DC Jona / ams-OSRAM.
 
 It is a general purpose stdf file parser / generator / simulator / analyser and converter.
```


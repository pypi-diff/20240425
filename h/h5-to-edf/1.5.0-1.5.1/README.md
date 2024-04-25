# Comparing `tmp/h5_to_edf-1.5.0-py3-none-any.whl.zip` & `tmp/h5_to_edf-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 29480 bytes, number of entries: 18
--rw-r--r--  2.0 unx       47 b- defN 24-Mar-08 17:35 h5_to_edf/__init__.py
--rw-r--r--  2.0 unx    24610 b- defN 24-Mar-08 17:35 h5_to_edf/converter.py
+Zip file size: 29615 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-25 12:07 h5_to_edf/__init__.py
+-rw-r--r--  2.0 unx    24787 b- defN 24-Apr-25 12:07 h5_to_edf/converter.py
 -rw-r--r--  2.0 unx    34793 b- defN 24-Mar-08 17:35 h5_to_edf/converter_oven.py
 -rw-r--r--  2.0 unx     2467 b- defN 24-Mar-04 09:59 h5_to_edf/current_reader.py
 -rw-r--r--  2.0 unx     2032 b- defN 24-Mar-04 09:59 h5_to_edf/edf_file_series.py
--rw-r--r--  2.0 unx     1142 b- defN 24-Mar-08 17:35 h5_to_edf/exceptions.py
--rw-r--r--  2.0 unx     4164 b- defN 24-Mar-08 17:35 h5_to_edf/info_output.py
+-rw-r--r--  2.0 unx     1353 b- defN 24-Apr-25 12:07 h5_to_edf/exceptions.py
+-rw-r--r--  2.0 unx     4232 b- defN 24-Apr-25 12:07 h5_to_edf/info_output.py
 -rw-r--r--  2.0 unx     3026 b- defN 24-Mar-08 17:35 h5_to_edf/report_output.py
 -rw-r--r--  2.0 unx     5723 b- defN 24-Mar-08 17:35 h5_to_edf/xml_output.py
 -rw-r--r--  2.0 unx     8542 b- defN 23-Oct-16 12:24 h5_to_edf/yaml.py
 -rw-r--r--  2.0 unx     7404 b- defN 24-Mar-08 17:35 h5_to_edf/yaml_output.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-04 09:59 h5_to_edf/app/__init__.py
--rw-r--r--  2.0 unx     8164 b- defN 24-Mar-08 17:35 h5_to_edf/app/h5_to_edf.py
--rw-r--r--  2.0 unx     2389 b- defN 24-Mar-08 17:36 h5_to_edf-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-08 17:36 h5_to_edf-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       97 b- defN 24-Mar-08 17:36 h5_to_edf-1.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-08 17:36 h5_to_edf-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1454 b- defN 24-Mar-08 17:36 h5_to_edf-1.5.0.dist-info/RECORD
-18 files, 106156 bytes uncompressed, 27108 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx     8210 b- defN 24-Apr-25 12:07 h5_to_edf/app/h5_to_edf.py
+-rw-r--r--  2.0 unx     2389 b- defN 24-Apr-25 12:07 h5_to_edf-1.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 12:07 h5_to_edf-1.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       97 b- defN 24-Apr-25 12:07 h5_to_edf-1.5.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-25 12:07 h5_to_edf-1.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1454 b- defN 24-Apr-25 12:07 h5_to_edf-1.5.1.dist-info/RECORD
+18 files, 106658 bytes uncompressed, 27243 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: h5_to_edf/app/__init__.py
 Comment: 
 
 Filename: h5_to_edf/app/h5_to_edf.py
 Comment: 
 
-Filename: h5_to_edf-1.5.0.dist-info/METADATA
+Filename: h5_to_edf-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: h5_to_edf-1.5.0.dist-info/WHEEL
+Filename: h5_to_edf-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: h5_to_edf-1.5.0.dist-info/entry_points.txt
+Filename: h5_to_edf-1.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: h5_to_edf-1.5.0.dist-info/top_level.txt
+Filename: h5_to_edf-1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: h5_to_edf-1.5.0.dist-info/RECORD
+Filename: h5_to_edf-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h5_to_edf/__init__.py

```diff
@@ -1,3 +1,3 @@
 # -*- coding: utf-8 -*-
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

## h5_to_edf/converter.py

```diff
@@ -162,16 +162,20 @@
                 f"{self.proj_scan}/measurement/sz",
             )
         raise ValueError(f"Unknown role {role}")
 
     def _read(self, h5: h5py.File):
         # make sure everything is done
 
-        if "Bliss" not in h5.attrs.get("creator"):
-            raise exceptions.FileNotProducedByBliss
+        creator = h5.attrs.get("creator", "none")
+        publisher = h5.attrs.get("publisher", "none")
+        if creator != "Bliss" and publisher != "bliss":
+            raise exceptions.FileNotProducedByBliss(
+                creator=creator, publisher=publisher
+            )
 
         for name in h5:
             if "end_time" not in h5[name]:
                 raise exceptions.ScanNotTerminated(self.h5_name, name)
 
         for name in h5:
             if "writer" in h5[name]:
```

## h5_to_edf/exceptions.py

```diff
@@ -33,10 +33,17 @@
             f"Scan {filename} group {group_name} not successed ({status})"
         )
 
 
 class FileNotProducedByBliss(Exception):
     """Raised when a processed file was not created by BLISS"""
 
+    def __init__(self, creator, publisher):
+        self._creator = creator
+        self._publisher = publisher
+
+    def __str__(self):
+        return f"creator='{self._creator}' publisher='{self._publisher}'"
+
 
 class ScanNotComplete(Exception):
     """Raised when a the scan was halfly processed"""
```

## h5_to_edf/info_output.py

```diff
@@ -48,18 +48,22 @@
             max_expo = ""
         col_end = roi[0]
         col_beg = roi[1]
         row_end = roi[2]
         row_beg = roi[3]
         pixelsize = h5[scan.group_scan + "/technique/optic/sample_pixel_size"][()]
         date = str(h5[scan.group_scan + "/start_time"][()])
-        srcurrent = h5[scan.group_scan + "/instrument/machine/current"][()]
+        try:
+            srcurrent = h5[scan.group_scan + "/instrument/machine/current"][()]
+        except KeyError:
+            srcurrent = 0
+
         try:
             comment = str(h5[scan.group_scan + "/technique/scan/comment"][()])
-        except Exception:
+        except KeyError:
             comment = ""
 
         print("Creation of the .info file")
         infofile = os.path.join(scan.dataset_output, scan.dataset_name + "_.info")
         if os.path.isfile(infofile):
             h5 = open(infofile, "r")
             lines = [line.strip("\n") for line in h5.readlines()]
```

## h5_to_edf/app/h5_to_edf.py

```diff
@@ -155,15 +155,15 @@
 
 def search_from_raw_data(root: str):
     h5_names = []
     for i in glob("*/*.h5", root_dir=root):
         if "tomwer" in i or "nabu" in i:
             # Skip post processing
             continue
-        if '/blc' in i:
+        if "/blc" in i:
             # Skip collection root file
             continue
         h5_names.append(i)
     for i in glob("*/*/*.h5", root_dir=root):
         if "tomwer" in i or "nabu" in i:
             # Skip post processing
             continue
@@ -262,16 +262,18 @@
                 "EDF directory '%s' not writtable: Processing cancelled", edf_directory
             )
             return -1
 
     for h5_name in h5_names:
         try:
             convert_h5_file_to_edf(h5_name, config)
-        except exceptions.FileNotProducedByBliss:
-            _logger.warning(f"File {h5_name} was not produced by BLISS. Skipped")
+        except exceptions.FileNotProducedByBliss as e:
+            _logger.warning(
+                f"File {h5_name} was not produced by BLISS. Found {e}. Skipped"
+            )
         except (exceptions.ScanNotTerminated, exceptions.ScanNotSuccessed) as e:
             if config.skip_active_scans:
                 _logger.warning(e.args[0])
             else:
                 raise
 
     return 0
```

## Comparing `h5_to_edf-1.5.0.dist-info/METADATA` & `h5_to_edf-1.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5_to_edf
-Version: 1.5.0
+Version: 1.5.1
 Summary: Convert a HDF5 file to EDF files
 Author-email: Jibril MAMMERI <mammeri@esrf.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.esrf.fr/tomo/h5_to_edf
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomo/h5_to_edf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `h5_to_edf-1.5.0.dist-info/RECORD` & `h5_to_edf-1.5.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-h5_to_edf/__init__.py,sha256=yk6xJGOA8Gl7eSUk6m6iN7ZehHo2lLLGj-kJ41jgmmY,47
-h5_to_edf/converter.py,sha256=JTolHGU9pgTBITxp4Mxgx12Nq1W1vJqMLemPoWN2xIs,24610
+h5_to_edf/__init__.py,sha256=CRRMwYfcAFMesvHruZve7yvmYytGp3rOYu0XJn49wY0,47
+h5_to_edf/converter.py,sha256=QqDJAMev435MUYNh8VOyom4KS2Lu5dj-hN5wXbGK-NQ,24787
 h5_to_edf/converter_oven.py,sha256=LhT_jwc62y9COdG-PaHIdSsJTnh2yUZEK2q3wLHKCMU,34793
 h5_to_edf/current_reader.py,sha256=FluCNAlP6QM-PwU5iTWunSoNp0EDH25LfmYC3Re99S0,2467
 h5_to_edf/edf_file_series.py,sha256=v3LcRWJhqB4zbiE6snS2bm-hX0yeBq-fW9KABcBudrc,2032
-h5_to_edf/exceptions.py,sha256=DrJQL5XoJ7bz7_mHi0HEcvvIezpwtlyytPYQau4_cX0,1142
-h5_to_edf/info_output.py,sha256=xkOoDGb6e1lnRGpFRtuQddHlAmFMfL7ndhGdgsRB0mY,4164
+h5_to_edf/exceptions.py,sha256=00jrKtzjX_IdvWAEQKA1y8iWMuGIkgAMCyznHX9Yz8A,1353
+h5_to_edf/info_output.py,sha256=E78CCEB7KIo_ivTnoND1Z7b3cTh-kCZMiBfE5uKJJTM,4232
 h5_to_edf/report_output.py,sha256=rWyH3BWBJE4G-E7JcORP_cIf4Fbk54yFcTn5cnHfi-0,3026
 h5_to_edf/xml_output.py,sha256=TY8ruTdpRhmbU-e8rujvR9Mwd9QzcDaA0F_x6GDZenU,5723
 h5_to_edf/yaml.py,sha256=8DOvxGnHqr7E8Qh6MD4d_sBMU-VFLUkM4kxn4Y8LC14,8542
 h5_to_edf/yaml_output.py,sha256=aniTU7YfTWJGTM1ekYQwOFQ0GfZR2KrFcooPwkzDs4g,7404
 h5_to_edf/app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-h5_to_edf/app/h5_to_edf.py,sha256=4w1Bqs0YsaWCNK_OCtbakKRqyY1UJf42ZlQ-osgBsHk,8164
-h5_to_edf-1.5.0.dist-info/METADATA,sha256=ryeN5l6_ulAnoNbHSq2vvil37rceQEIPNhtYaRuI9GI,2389
-h5_to_edf-1.5.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-h5_to_edf-1.5.0.dist-info/entry_points.txt,sha256=IdPI6eFDQq-SYLIRyFh9hyhPFTqf2Q6fTSM9-mnd1PA,97
-h5_to_edf-1.5.0.dist-info/top_level.txt,sha256=wqXEE9P_j1tLbUXGunpfWQU6RBPkdcsSu54f9Ychk8M,10
-h5_to_edf-1.5.0.dist-info/RECORD,,
+h5_to_edf/app/h5_to_edf.py,sha256=Cb1b7uyodN6PjoSZIPRXZ9VQqTWJtR7udJMI0ccVqVg,8210
+h5_to_edf-1.5.1.dist-info/METADATA,sha256=1ZxzHNth82Obh5NCrBFfXhARjHgRzHtDz1xF78LMYWk,2389
+h5_to_edf-1.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+h5_to_edf-1.5.1.dist-info/entry_points.txt,sha256=IdPI6eFDQq-SYLIRyFh9hyhPFTqf2Q6fTSM9-mnd1PA,97
+h5_to_edf-1.5.1.dist-info/top_level.txt,sha256=wqXEE9P_j1tLbUXGunpfWQU6RBPkdcsSu54f9Ychk8M,10
+h5_to_edf-1.5.1.dist-info/RECORD,,
```


# Comparing `tmp/sqlalchemy_doris-0.2.1-py3-none-any.whl.zip` & `tmp/sqlalchemy_doris-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13515 bytes, number of entries: 10
+Zip file size: 13539 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat     1227 b- defN 23-Nov-30 05:48 sqlalchemy_doris/__init__.py
--rw-rw-rw-  2.0 fat      427 b- defN 23-Dec-17 04:38 sqlalchemy_doris/_version.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-Apr-25 06:39 sqlalchemy_doris/_version.py
 -rw-rw-rw-  2.0 fat     3778 b- defN 23-Nov-07 14:10 sqlalchemy_doris/datatype.py
--rw-rw-rw-  2.0 fat    14159 b- defN 23-Dec-17 03:55 sqlalchemy_doris/dialect.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Dec-17 04:38 sqlalchemy_doris-0.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2512 b- defN 23-Dec-17 04:38 sqlalchemy_doris-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-17 04:38 sqlalchemy_doris-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      184 b- defN 23-Dec-17 04:38 sqlalchemy_doris-0.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Dec-17 04:38 sqlalchemy_doris-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      876 b- defN 23-Dec-17 04:38 sqlalchemy_doris-0.2.1.dist-info/RECORD
-10 files, 34830 bytes uncompressed, 12005 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat    14207 b- defN 24-Apr-25 06:30 sqlalchemy_doris/dialect.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-25 06:39 sqlalchemy_doris-0.2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2512 b- defN 24-Apr-25 06:39 sqlalchemy_doris-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 06:39 sqlalchemy_doris-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      184 b- defN 24-Apr-25 06:39 sqlalchemy_doris-0.2.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-25 06:39 sqlalchemy_doris-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      876 b- defN 24-Apr-25 06:39 sqlalchemy_doris-0.2.2.dist-info/RECORD
+10 files, 34878 bytes uncompressed, 12029 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sqlalchemy_doris/datatype.py
 Comment: 
 
 Filename: sqlalchemy_doris/dialect.py
 Comment: 
 
-Filename: sqlalchemy_doris-0.2.1.dist-info/LICENSE
+Filename: sqlalchemy_doris-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: sqlalchemy_doris-0.2.1.dist-info/METADATA
+Filename: sqlalchemy_doris-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: sqlalchemy_doris-0.2.1.dist-info/WHEEL
+Filename: sqlalchemy_doris-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: sqlalchemy_doris-0.2.1.dist-info/entry_points.txt
+Filename: sqlalchemy_doris-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlalchemy_doris-0.2.1.dist-info/top_level.txt
+Filename: sqlalchemy_doris-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlalchemy_doris-0.2.1.dist-info/RECORD
+Filename: sqlalchemy_doris-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlalchemy_doris/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.2.1'
-__version_tuple__ = version_tuple = (0, 2, 1)
+__version__ = version = '0.2.2'
+__version_tuple__ = version_tuple = (0, 2, 2)
```

## sqlalchemy_doris/dialect.py

```diff
@@ -269,15 +269,16 @@
             # 1049: Unknown database '%s'  - for nonexistent schema
             #
             # also added:
             # 1051: Unknown table '%s' - not known to emit
             #
             # there's more "doesn't exist" kinds of messages but they are
             # less clear if mysql 8 would suddenly start using one of those
-            if self._extract_error_code(e.orig) in (1105, ):
+            # print('caught exception', e)
+            if self._extract_error_code(e.orig) in (1105, 1051):
                 info: str = e.orig.args[1].split('detailMessage = ')[-1]
                 if info.startswith('Unknown table'):
                     return False
             raise
 
 
     def get_schema_names(self, connection, **kw):
```

## Comparing `sqlalchemy_doris-0.2.1.dist-info/LICENSE` & `sqlalchemy_doris-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sqlalchemy_doris-0.2.1.dist-info/METADATA` & `sqlalchemy_doris-0.2.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-doris
-Version: 0.2.1
+Version: 0.2.2
 Summary: Apache Doris dialect for SQLAlchemy
 Author-email: actcwlf <actcwlf@qq.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/actcwlf/sqlalchemy-doris
 Project-URL: Issues, https://github.com/actcwlf/sqlalchemy-doris/issues
 Keywords: Apache Doris,SQLAlchemy
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `sqlalchemy_doris-0.2.1.dist-info/RECORD` & `sqlalchemy_doris-0.2.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sqlalchemy_doris/__init__.py,sha256=kOveLcu3DXBrwZqriCBAL-1mQWbJ7oPCsP6iDT8_tzo,1227
-sqlalchemy_doris/_version.py,sha256=ZX5om7Ovkz6dOhGLYm2Tr_wCABow6rirLhSHdYiHgpk,427
+sqlalchemy_doris/_version.py,sha256=v-s4jxakrueCN6kimkfkQ9BPg6G2bMmqtQPS7EYUdtc,427
 sqlalchemy_doris/datatype.py,sha256=urNnH92vulbuuQmV3tJ072BmzTB3HFTZkQJTWG1B7LM,3778
-sqlalchemy_doris/dialect.py,sha256=MhNWUP6oY38sANwnCd-LGcaXvtbK2uxTsEi0rTyrG7M,14159
-sqlalchemy_doris-0.2.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-sqlalchemy_doris-0.2.1.dist-info/METADATA,sha256=kgvcHOHreKhEcl3Bt0p6v0957rKYAnXcujG-49iIkDw,2512
-sqlalchemy_doris-0.2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-sqlalchemy_doris-0.2.1.dist-info/entry_points.txt,sha256=a-wI3Y9NUpUOrNMKwMS-WTmSJxqLScOgOoIe0A7vet0,184
-sqlalchemy_doris-0.2.1.dist-info/top_level.txt,sha256=_pUnPrVEVtY7A3j5MhbnpAx7-joFu4c_IOQQTm8qA5I,17
-sqlalchemy_doris-0.2.1.dist-info/RECORD,,
+sqlalchemy_doris/dialect.py,sha256=E0kheRqgeyLaQ0XnVxBb1xRLunNcx0jik5A56nzfnxw,14207
+sqlalchemy_doris-0.2.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+sqlalchemy_doris-0.2.2.dist-info/METADATA,sha256=-OvBob_Qv7AY5tuQJ-O4v58xRGRStDOtUEJ5Z_dLG8o,2512
+sqlalchemy_doris-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sqlalchemy_doris-0.2.2.dist-info/entry_points.txt,sha256=a-wI3Y9NUpUOrNMKwMS-WTmSJxqLScOgOoIe0A7vet0,184
+sqlalchemy_doris-0.2.2.dist-info/top_level.txt,sha256=_pUnPrVEVtY7A3j5MhbnpAx7-joFu4c_IOQQTm8qA5I,17
+sqlalchemy_doris-0.2.2.dist-info/RECORD,,
```


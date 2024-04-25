# Comparing `tmp/pycspwrapper-0.2.0-py3-none-any.whl.zip` & `tmp/pycspwrapper-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4138 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     3414 b- defN 24-Apr-04 11:07 pycspwrapper/LVStat.py
+Zip file size: 4149 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     3429 b- defN 24-Apr-25 13:08 pycspwrapper/LVStat.py
 -rw-rw-r--  2.0 unx       74 b- defN 24-Mar-21 09:50 pycspwrapper/__init__.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1814 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      569 b- defN 24-Apr-04 11:08 pycspwrapper-0.2.0.dist-info/RECORD
-7 files, 7051 bytes uncompressed, 3124 bytes compressed:  55.7%
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-25 13:13 pycspwrapper-0.2.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1814 b- defN 24-Apr-25 13:13 pycspwrapper-0.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-25 13:13 pycspwrapper-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-25 13:13 pycspwrapper-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      569 b- defN 24-Apr-25 13:13 pycspwrapper-0.2.1.dist-info/RECORD
+7 files, 7066 bytes uncompressed, 3135 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycspwrapper/LVStat.py
 Comment: 
 
 Filename: pycspwrapper/__init__.py
 Comment: 
 
-Filename: pycspwrapper-0.2.0.dist-info/LICENSE
+Filename: pycspwrapper-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: pycspwrapper-0.2.0.dist-info/METADATA
+Filename: pycspwrapper-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pycspwrapper-0.2.0.dist-info/WHEEL
+Filename: pycspwrapper-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pycspwrapper-0.2.0.dist-info/top_level.txt
+Filename: pycspwrapper-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pycspwrapper-0.2.0.dist-info/RECORD
+Filename: pycspwrapper-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycspwrapper/LVStat.py

```diff
@@ -46,16 +46,16 @@
         val_dict = {}
         try:
             variables = response['variables']
         except TypeError:
             print("Error: You are not in a leaf node.")
             return
         for item in variables:
-            val_dict[item['code']] = item['values']\
-                if values else item['valueTexts']
+            val_dict[item['code']] = item.get('values',[])\
+                if values else item.get('valueTexts', [])
         return val_dict
 
     def clear_query(self):
         """ Clears the query. Mostly an internal function to use in others. """
         self.query = {"query": [], 
                       "response": {"format": "json"}
                       }
```

## Comparing `pycspwrapper-0.2.0.dist-info/LICENSE` & `pycspwrapper-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycspwrapper-0.2.0.dist-info/METADATA` & `pycspwrapper-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycspwrapper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python wrapper for Latvian official statistics portal API: https://stat.gov.lv/en/api-and-code-list-registry.
 Home-page: https://github.com/vf42/pycspwrapper
 Author: Vadim Fedorov
 Author-email: vadim@vf42.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


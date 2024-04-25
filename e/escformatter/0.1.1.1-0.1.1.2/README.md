# Comparing `tmp/escformatter-0.1.1.1-py3-none-any.whl.zip` & `tmp/escformatter-0.1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5788 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-25 03:33 escformatter/__init__.py
--rw-rw-rw-  2.0 fat    19296 b- defN 24-Apr-25 13:20 escformatter/esc.py
--rw-rw-rw-  2.0 fat     1096 b- defN 24-Apr-25 14:24 escformatter-0.1.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1077 b- defN 24-Apr-25 14:24 escformatter-0.1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 14:24 escformatter-0.1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-25 14:24 escformatter-0.1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      577 b- defN 24-Apr-25 14:24 escformatter-0.1.1.1.dist-info/RECORD
-7 files, 22171 bytes uncompressed, 4760 bytes compressed:  78.5%
+Zip file size: 5781 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       18 b- defN 24-Apr-25 15:17 escformatter/__init__.py
+-rw-rw-rw-  2.0 fat    19330 b- defN 24-Apr-25 15:17 escformatter/esc.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 24-Apr-25 15:21 escformatter-0.1.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1039 b- defN 24-Apr-25 15:21 escformatter-0.1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 15:21 escformatter-0.1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-25 15:21 escformatter-0.1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      577 b- defN 24-Apr-25 15:21 escformatter-0.1.1.2.dist-info/RECORD
+7 files, 22165 bytes uncompressed, 4753 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: escformatter/__init__.py
 Comment: 
 
 Filename: escformatter/esc.py
 Comment: 
 
-Filename: escformatter-0.1.1.1.dist-info/LICENSE
+Filename: escformatter-0.1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: escformatter-0.1.1.1.dist-info/METADATA
+Filename: escformatter-0.1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: escformatter-0.1.1.1.dist-info/WHEEL
+Filename: escformatter-0.1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: escformatter-0.1.1.1.dist-info/top_level.txt
+Filename: escformatter-0.1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: escformatter-0.1.1.1.dist-info/RECORD
+Filename: escformatter-0.1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## escformatter/__init__.py

```diff
@@ -1 +1 @@
-from .esc import Esc
+from .esc import *
```

## escformatter/esc.py

```diff
@@ -513,14 +513,17 @@
         ### Returns:
             None
         """
         if not self._cleanup_registered:
             atexit.register(self._register_cleanup_callback)
             self._cleanup_registered = True
 
+esc = Esc()
+__all__ = ['esc']
+
 if __name__ == '__main__':
     esc = Esc()
     esc.register_cleanup()
 
     print(esc.fg_red, end='')
     print(esc.bg_blue, end='')
     print(esc.bold, end='')
```

## Comparing `escformatter-0.1.1.1.dist-info/LICENSE` & `escformatter-0.1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `escformatter-0.1.1.1.dist-info/METADATA` & `escformatter-0.1.1.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escformatter
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: A Python class for executing ANSI escape commands in the console.
 Home-page: https://github.com/devleonardoamaral/escformatter.git
 Author: Leonardo S. Amaral
 Author-email: leonardo_amaral98@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,14 @@
 ## Description
 
 This Python package provides a class named `Esc` that enables the execution of ANSI escape commands in the console. It offers functionalities for advanced text formatting, changing font colors in the console, applying text styles, and positioning the cursor.
 
 ## Usage Example
 
 ```python
-from escformatter import Esc
-
-# Create an instance of Esc
-e = Esc()
+from escformatter import esc
 
 # Register cleanup to reset console styles and colors to default
-e.register_cleanup()
+esc.register_cleanup()
 
 # Display 'Hello, World!' in red
-print(e.fg_red + 'Hello, World!')
+print(esc.fg_red + 'Hello, World!')
```

## Comparing `escformatter-0.1.1.1.dist-info/RECORD` & `escformatter-0.1.1.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-escformatter/__init__.py,sha256=Rv_Ygfk40xjxkWYa9JEh3TPa8djEwI-D4WzsgEhe420,20
-escformatter/esc.py,sha256=GHjNESF3zWEcXXyyuaLKHWHplNpvGzj8kDVAk7J8U-U,19296
-escformatter-0.1.1.1.dist-info/LICENSE,sha256=vZH2198b064FRsbKLuL4U_mz8QfugqGbJFbGRQM5PD8,1096
-escformatter-0.1.1.1.dist-info/METADATA,sha256=x3Bjzn41tSf7Fi1O_wQQ_RpMBryLodtliWXGcwgDh4k,1077
-escformatter-0.1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-escformatter-0.1.1.1.dist-info/top_level.txt,sha256=QF6QqpY78RmaTTioOWAkBbOFVB0brCKNHJur5xQYbZ0,13
-escformatter-0.1.1.1.dist-info/RECORD,,
+escformatter/__init__.py,sha256=AZ45TLALwtJgmQrVUW-n6yCCnhLvhy33ewcbKUrI1kE,18
+escformatter/esc.py,sha256=ltgWiBWygVAQ2xID_CLpbQp7-an7rUeMmjhtL7OzAUc,19330
+escformatter-0.1.1.2.dist-info/LICENSE,sha256=vZH2198b064FRsbKLuL4U_mz8QfugqGbJFbGRQM5PD8,1096
+escformatter-0.1.1.2.dist-info/METADATA,sha256=WFGSDLapJm7aIsZI23eb8efQ9N7nuqJOvFkUFYpGe3A,1039
+escformatter-0.1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+escformatter-0.1.1.2.dist-info/top_level.txt,sha256=QF6QqpY78RmaTTioOWAkBbOFVB0brCKNHJur5xQYbZ0,13
+escformatter-0.1.1.2.dist-info/RECORD,,
```


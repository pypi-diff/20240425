# Comparing `tmp/rf_userpoollibrary-0.9b8-py3-none-any.whl.zip` & `tmp/rf_userpoollibrary-0.9b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10260 bytes, number of entries: 9
--rw-rw-r--  2.0 unx    18416 b- defN 23-Sep-28 15:47 UserpoolLibrary/UserpoolLibrary.py
+Zip file size: 10255 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx    18416 b- defN 23-Sep-29 03:06 UserpoolLibrary/UserpoolLibrary.py
 -rw-rw-r--  2.0 unx     1570 b- defN 23-Sep-27 16:03 UserpoolLibrary/Utils.py
 -rw-rw-r--  2.0 unx     1166 b- defN 23-Sep-27 16:03 UserpoolLibrary/__init__.py
--rw-rw-r--  2.0 unx     1124 b- defN 23-Sep-28 16:52 UserpoolLibrary/version.py
--rw-rw-r--  2.0 unx     1072 b- defN 23-Sep-28 16:53 rf_userpoollibrary-0.9b8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2930 b- defN 23-Sep-28 16:53 rf_userpoollibrary-0.9b8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Sep-28 16:53 rf_userpoollibrary-0.9b8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Sep-28 16:53 rf_userpoollibrary-0.9b8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      781 b- defN 23-Sep-28 16:53 rf_userpoollibrary-0.9b8.dist-info/RECORD
-9 files, 27167 bytes uncompressed, 8904 bytes compressed:  67.2%
+-rw-rw-r--  2.0 unx     1124 b- defN 23-Sep-29 03:06 UserpoolLibrary/version.py
+-rw-rw-r--  2.0 unx     1072 b- defN 23-Sep-29 03:32 rf_userpoollibrary-0.9b9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2930 b- defN 23-Sep-29 03:32 rf_userpoollibrary-0.9b9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Sep-29 03:32 rf_userpoollibrary-0.9b9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Sep-29 03:32 rf_userpoollibrary-0.9b9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      781 b- defN 23-Sep-29 03:32 rf_userpoollibrary-0.9b9.dist-info/RECORD
+9 files, 27167 bytes uncompressed, 8899 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: UserpoolLibrary/__init__.py
 Comment: 
 
 Filename: UserpoolLibrary/version.py
 Comment: 
 
-Filename: rf_userpoollibrary-0.9b8.dist-info/LICENSE
+Filename: rf_userpoollibrary-0.9b9.dist-info/LICENSE
 Comment: 
 
-Filename: rf_userpoollibrary-0.9b8.dist-info/METADATA
+Filename: rf_userpoollibrary-0.9b9.dist-info/METADATA
 Comment: 
 
-Filename: rf_userpoollibrary-0.9b8.dist-info/WHEEL
+Filename: rf_userpoollibrary-0.9b9.dist-info/WHEEL
 Comment: 
 
-Filename: rf_userpoollibrary-0.9b8.dist-info/top_level.txt
+Filename: rf_userpoollibrary-0.9b9.dist-info/top_level.txt
 Comment: 
 
-Filename: rf_userpoollibrary-0.9b8.dist-info/RECORD
+Filename: rf_userpoollibrary-0.9b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## UserpoolLibrary/version.py

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-VERSION = '0.9b8'
+VERSION = '0.9b9'
```

## Comparing `rf_userpoollibrary-0.9b8.dist-info/LICENSE` & `rf_userpoollibrary-0.9b9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rf_userpoollibrary-0.9b8.dist-info/METADATA` & `rf_userpoollibrary-0.9b9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rf-userpoollibrary
-Version: 0.9b8
+Version: 0.9b9
 Summary: Test Library for userpool support.
 Home-page: https://github.com/MainSystemDev/UserpoolLibrary
 Author: Shiela Buitizon
 Author-email: shiela.buitizon@mnltechnology.com
 License: UNKNOWN
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

## Comparing `rf_userpoollibrary-0.9b8.dist-info/RECORD` & `rf_userpoollibrary-0.9b9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 UserpoolLibrary/UserpoolLibrary.py,sha256=YznYsB8BEV0FFdjJBA2GgZ_eAuwOpCSUmgzzN5r_jhE,18416
 UserpoolLibrary/Utils.py,sha256=OQia_7Jgrj8V4k9EuNq9Q9qWAiBNGaY9p9VQ4J2P1mo,1570
 UserpoolLibrary/__init__.py,sha256=IRx_z-c0GrfZk3XgQUWG2B7ZMgjW9Qvf94e_C_2UXls,1166
-UserpoolLibrary/version.py,sha256=D72r_f4Hwj4sf2aiQrwX1tRiSyMU3QhVqCI_Csjy7AI,1124
-rf_userpoollibrary-0.9b8.dist-info/LICENSE,sha256=OjWkSK0ve0yCXLlsw-7TTfFJMorgICeKeGRyICPvjdI,1072
-rf_userpoollibrary-0.9b8.dist-info/METADATA,sha256=in2DEzjYdykXUcBxYTzDCNdTkgbsEghgtyNb7lOmwWc,2930
-rf_userpoollibrary-0.9b8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-rf_userpoollibrary-0.9b8.dist-info/top_level.txt,sha256=1fE9zy8Vz-vNjh1mQYMX8EZwKWk-r3ngWzS1v7J1NoU,16
-rf_userpoollibrary-0.9b8.dist-info/RECORD,,
+UserpoolLibrary/version.py,sha256=IY9PpkKPjLRrjI7atYnkl21KANE9h5suNqchDM8QrtU,1124
+rf_userpoollibrary-0.9b9.dist-info/LICENSE,sha256=OjWkSK0ve0yCXLlsw-7TTfFJMorgICeKeGRyICPvjdI,1072
+rf_userpoollibrary-0.9b9.dist-info/METADATA,sha256=doqpEyoQ2yrQxI7NndQAs_-fLOdOw8z9IOVb7Ryf7gk,2930
+rf_userpoollibrary-0.9b9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rf_userpoollibrary-0.9b9.dist-info/top_level.txt,sha256=1fE9zy8Vz-vNjh1mQYMX8EZwKWk-r3ngWzS1v7J1NoU,16
+rf_userpoollibrary-0.9b9.dist-info/RECORD,,
```


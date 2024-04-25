# Comparing `tmp/anyon-4.2.1-cp312-none-win_amd64.whl.zip` & `tmp/anyon-4.2.2-cp312-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 470727 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-22 01:19 anyon-4.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2334 b- defN 24-Apr-22 01:19 anyon-4.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-22 01:19 anyon-4.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-22 01:19 anyon-4.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 24-Apr-22 01:19 anyon-4.2.1.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 24-Apr-22 01:18 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    96256 b- defN 24-Apr-22 01:18 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   121344 b- defN 24-Apr-22 01:18 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   233984 b- defN 24-Apr-22 01:18 anyon/server.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 24-Apr-22 01:19 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat   251904 b- defN 24-Apr-22 01:18 anyon/stage/assembler.pyd
--rw-rw-rw-  2.0 fat   100352 b- defN 24-Apr-22 01:18 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   140288 b- defN 24-Apr-22 01:19 anyon/stage/device.pyd
--rw-rw-rw-  2.0 fat    67584 b- defN 24-Apr-22 01:19 anyon/stage/processor.pyd
-14 files, 1058616 bytes uncompressed, 468967 bytes compressed:  55.7%
+Zip file size: 1062611 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-25 14:26 anyon-4.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2283 b- defN 24-Apr-25 14:26 anyon-4.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-Apr-25 14:26 anyon-4.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 14:26 anyon-4.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      376 b- defN 24-Apr-25 14:26 anyon-4.2.2.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   121664 b- defN 24-Apr-25 14:25 anyon/__init__.so
+-rwxr-xr-x  2.0 unx   322350 b- defN 24-Apr-25 14:25 anyon/loader.so
+-rwxr-xr-x  2.0 unx   393502 b- defN 24-Apr-25 14:25 anyon/remote.so
+-rwxr-xr-x  2.0 unx   703278 b- defN 24-Apr-25 14:24 anyon/server.so
+-rwxr-xr-x  2.0 unx   122000 b- defN 24-Apr-25 14:25 anyon/stage/__init__.so
+-rwxr-xr-x  2.0 unx   744945 b- defN 24-Apr-25 14:26 anyon/stage/assembler.so
+-rwxr-xr-x  2.0 unx   322802 b- defN 24-Apr-25 14:26 anyon/stage/calculator.so
+-rwxr-xr-x  2.0 unx   458174 b- defN 24-Apr-25 14:25 anyon/stage/device.so
+-rwxr-xr-x  2.0 unx   251473 b- defN 24-Apr-25 14:25 anyon/stage/processor.so
+14 files, 3444025 bytes uncompressed, 1060869 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-4.2.1.dist-info/LICENSE
+Filename: anyon-4.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-4.2.1.dist-info/METADATA
+Filename: anyon-4.2.2.dist-info/METADATA
 Comment: 
 
-Filename: anyon-4.2.1.dist-info/WHEEL
+Filename: anyon-4.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-4.2.1.dist-info/top_level.txt
+Filename: anyon-4.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-4.2.1.dist-info/RECORD
+Filename: anyon-4.2.2.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.pyd
+Filename: anyon/__init__.so
 Comment: 
 
-Filename: anyon/loader.pyd
+Filename: anyon/loader.so
 Comment: 
 
-Filename: anyon/remote.pyd
+Filename: anyon/remote.so
 Comment: 
 
-Filename: anyon/server.pyd
+Filename: anyon/server.so
 Comment: 
 
-Filename: anyon/stage/__init__.pyd
+Filename: anyon/stage/__init__.so
 Comment: 
 
-Filename: anyon/stage/assembler.pyd
+Filename: anyon/stage/assembler.so
 Comment: 
 
-Filename: anyon/stage/calculator.pyd
+Filename: anyon/stage/calculator.so
 Comment: 
 
-Filename: anyon/stage/device.pyd
+Filename: anyon/stage/device.so
 Comment: 
 
-Filename: anyon/stage/processor.pyd
+Filename: anyon/stage/processor.so
 Comment: 
 
 Zip file comment:
```

## Comparing `anyon-4.2.1.dist-info/LICENSE` & `anyon-4.2.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 YL Feng
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 YL Feng
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `anyon-4.2.1.dist-info/METADATA` & `anyon-4.2.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1
-Name: anyon
-Version: 4.2.1
-Summary: description
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL Feng
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy >=1.20.0
-Requires-Dist: axion >=3.4.5
-Requires-Dist: srpc >=4.2.8
-Requires-Dist: zee >=0.0.3
-Requires-Dist: requests >=2.28.0
-Requires-Dist: APScheduler
-
+Metadata-Version: 2.1
+Name: anyon
+Version: 4.2.2
+Summary: description
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL Feng
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy >=1.20.0
+Requires-Dist: axion >=3.4.5
+Requires-Dist: srpc >=4.2.8
+Requires-Dist: zee >=0.0.3
+Requires-Dist: requests >=2.28.0
+Requires-Dist: APScheduler
+
```


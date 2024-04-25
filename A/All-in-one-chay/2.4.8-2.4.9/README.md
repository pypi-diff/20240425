# Comparing `tmp/all_in_one_chay-2.4.8.tar.gz` & `tmp/all_in_one_chay-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all_in_one_chay-2.4.8.tar", last modified: Fri Apr 19 15:55:50 2024, max compression
+gzip compressed data, was "all_in_one_chay-2.4.9.tar", last modified: Thu Apr 25 14:59:33 2024, max compression
```

## Comparing `all_in_one_chay-2.4.8.tar` & `all_in_one_chay-2.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/
--rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-2.4.8/LICENSE
--rw-rw-rw-   0        0        0     5213 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4546 2024-04-19 15:50:47.000000 all_in_one_chay-2.4.8/README.md
--rw-rw-rw-   0        0        0      642 2024-04-19 15:53:14.000000 all_in_one_chay-2.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-19 15:55:01.000000 all_in_one_chay-2.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.704378 all_in_one_chay-2.4.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.704378 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/
--rw-rw-rw-   0        0        0     9739 2024-04-19 15:41:59.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/Allinone.py
--rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.704378 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/
--rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/book.py
--rw-rw-rw-   0        0        0    12741 2024-04-19 15:49:01.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/calculator.py
--rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
--rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/math_cal_py.py
--rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/student_py.py
--rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/tuxing_cal.py
--rw-rw-rw-   0        0        0     2804 2024-04-16 15:08:27.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/xiaogongju.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/
--rw-rw-rw-   0        0        0     5213 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.745245 all_in_one_chay-2.4.9/
+-rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-2.4.9/LICENSE
+-rw-rw-rw-   0        0        0     5329 2024-04-25 14:59:33.743243 all_in_one_chay-2.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4662 2024-04-25 14:55:07.000000 all_in_one_chay-2.4.9/README.md
+-rw-rw-rw-   0        0        0      642 2024-04-25 14:58:59.000000 all_in_one_chay-2.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:59:33.745245 all_in_one_chay-2.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-25 14:58:49.000000 all_in_one_chay-2.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.720243 all_in_one_chay-2.4.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.726243 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/
+-rw-rw-rw-   0        0        0     9838 2024-04-25 14:51:01.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/Allinone.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.735243 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/
+-rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/book.py
+-rw-rw-rw-   0        0        0    12741 2024-04-19 15:49:01.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/calculator.py
+-rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+-rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/math_cal_py.py
+-rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/student_py.py
+-rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/tuxing_cal.py
+-rw-rw-rw-   0        0        0     4090 2024-04-25 14:55:09.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/xiaogongju.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.742243 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/
+-rw-rw-rw-   0        0        0     5329 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/top_level.txt
```

### Comparing `all_in_one_chay-2.4.8/LICENSE` & `all_in_one_chay-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/PKG-INFO` & `all_in_one_chay-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.8
+Version: 2.4.9
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
+Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one-Including/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # All-in-one Including
+
 多功能一体机库版本，现已更新至2.4.8版本
 说明如下：
+
 ```python
 Help on module Allinone:
 
 NAME
     Allinone
 
 DESCRIPTION
@@ -190,24 +192,27 @@
 
 NAME
     xiaogongju
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2022/12/24 15:07
+    # @TIME:2024/4/25 22:52
     # @FILE:xiaogongju.py
     # @Software:IDLE 3.9.6
 
 FUNCTIONS
-    chouqusuiji(num1, num2, mode, weishu)
+    daorxiao(args:str,mode:int) ->str
 
-    daorxiao(args, mode)
+    twonumbers_TheBiggestCommonfactor(num1:int,num2:int) -> int
 
-    twonumbers_TheBiggestCommonfactor(num1, num2)
+    twonumbers_TheMinimumCommonmultiple(num1:int,num2:int) -> int
 
-    twonumbers_TheMinimumCommonmultiple(num1, num2)
+    chouqusuiji(num1:int,num2:int,mode:int,weishu:int) -> str
+
+    kaisamima(arg:str,mode:int,n:int) -> str
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\module\xiaogongju.py
 ```
-详见https://github.com/lichenyichay/All-in-one
+
+详见<https://github.com/lichenyichay/All-in-one>
```

### Comparing `all_in_one_chay-2.4.8/README.md` & `all_in_one_chay-2.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # All-in-one Including
+
 多功能一体机库版本，现已更新至2.4.8版本
 说明如下：
+
 ```python
 Help on module Allinone:
 
 NAME
     Allinone
 
 DESCRIPTION
@@ -174,24 +176,27 @@
 
 NAME
     xiaogongju
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2022/12/24 15:07
+    # @TIME:2024/4/25 22:52
     # @FILE:xiaogongju.py
     # @Software:IDLE 3.9.6
 
 FUNCTIONS
-    chouqusuiji(num1, num2, mode, weishu)
+    daorxiao(args:str,mode:int) ->str
 
-    daorxiao(args, mode)
+    twonumbers_TheBiggestCommonfactor(num1:int,num2:int) -> int
 
-    twonumbers_TheBiggestCommonfactor(num1, num2)
+    twonumbers_TheMinimumCommonmultiple(num1:int,num2:int) -> int
 
-    twonumbers_TheMinimumCommonmultiple(num1, num2)
+    chouqusuiji(num1:int,num2:int,mode:int,weishu:int) -> str
+
+    kaisamima(arg:str,mode:int,n:int) -> str
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\module\xiaogongju.py
 ```
-详见https://github.com/lichenyichay/All-in-one
+
+详见<https://github.com/lichenyichay/All-in-one>
```

### Comparing `all_in_one_chay-2.4.8/pyproject.toml` & `all_in_one_chay-2.4.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "All-in-one-chay"
-version = "2.4.8"
+version = "2.4.9"
 authors = [
   { name="chay", email="lichenyi_2020@qq.com" },
 ]
 description = "多功能一体机（All-in-one）"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8"
+Homepage = "https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9"
 Issues = "https://github.com/lichenyichay/All-in-one-Including/issues"
```

### Comparing `all_in_one_chay-2.4.8/setup.py` & `all_in_one_chay-2.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 setuptools.setup(
     name="All-in-one-chay",
     version="2.4.8",
     author="Chay",
     author_email="lichenyi_2020@qq.com",
-    url="https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8",
+    url="https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9",
     description="All-in-one",
     long_description="多功能一体机",
     python_requires=">=3.5",
     # packages=setuptools.find_packages("src"),
     packages_dir={"": "src"},
     packages_data={"": ["*.txt", "*.info", "*.properties"], "": ["data/*.*"]},
     exclude=["*.test", "*.test.*", "test.*", "test"],
```

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/Allinone.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/Allinone.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         return calculator.jinzhizhuanhuan(args[0],args[1],args[2])
     elif fuwu=="math库计算器":
         return math_cal.math_cal(mode,args[0],args[1])
     elif fuwu == "分解因式":
         return calculator.factorization(args[0])
     elif fuwu == "提取密码":
         return calculator.mima(args[0],args[1])
+    elif fuwu == "凯撒密码计算":
+        return xiaogongju.kaisamima(args[0],mode,args[1])
     elif fuwu == "图形计算器":
         while True:
             huida = args[0]
             try:
                 args2=[]
                 for i in range(1,len(args)):
                     args2.append(args[i])
```

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/book.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/book.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/calculator.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/calculator.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/math_cal_py.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/math_cal_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/student_py.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/student_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/tuxing_cal.py` & `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/tuxing_cal.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/PKG-INFO` & `all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.8
+Version: 2.4.9
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
+Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one-Including/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # All-in-one Including
+
 多功能一体机库版本，现已更新至2.4.8版本
 说明如下：
+
 ```python
 Help on module Allinone:
 
 NAME
     Allinone
 
 DESCRIPTION
@@ -190,24 +192,27 @@
 
 NAME
     xiaogongju
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2022/12/24 15:07
+    # @TIME:2024/4/25 22:52
     # @FILE:xiaogongju.py
     # @Software:IDLE 3.9.6
 
 FUNCTIONS
-    chouqusuiji(num1, num2, mode, weishu)
+    daorxiao(args:str,mode:int) ->str
 
-    daorxiao(args, mode)
+    twonumbers_TheBiggestCommonfactor(num1:int,num2:int) -> int
 
-    twonumbers_TheBiggestCommonfactor(num1, num2)
+    twonumbers_TheMinimumCommonmultiple(num1:int,num2:int) -> int
 
-    twonumbers_TheMinimumCommonmultiple(num1, num2)
+    chouqusuiji(num1:int,num2:int,mode:int,weishu:int) -> str
+
+    kaisamima(arg:str,mode:int,n:int) -> str
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\module\xiaogongju.py
 ```
-详见https://github.com/lichenyichay/All-in-one
+
+详见<https://github.com/lichenyichay/All-in-one>
```

### Comparing `all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/SOURCES.txt` & `all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/dovekie-0.6.0.tar.gz` & `tmp/dovekie-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dovekie-0.6.0.tar", last modified: Mon Apr 22 14:33:14 2024, max compression
+gzip compressed data, was "dovekie-0.7.0.tar", last modified: Thu Apr 25 20:14:00 2024, max compression
```

## Comparing `dovekie-0.6.0.tar` & `dovekie-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-22 14:33:14.894402 dovekie-0.6.0/
--rw-r--r--   0 cph       (1000) cph       (1000)     1071 2024-04-07 17:09:48.000000 dovekie-0.6.0/LICENSE
--rw-r--r--   0 cph       (1000) cph       (1000)     2249 2024-04-22 14:33:14.894402 dovekie-0.6.0/PKG-INFO
--rw-r--r--   0 cph       (1000) cph       (1000)     1921 2024-04-08 20:14:01.000000 dovekie-0.6.0/README.md
-drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-22 14:33:14.894402 dovekie-0.6.0/dovekie/
--rw-r--r--   0 cph       (1000) cph       (1000)        0 2024-04-22 14:29:39.000000 dovekie-0.6.0/dovekie/__init__.py
--rw-r--r--   0 cph       (1000) cph       (1000)      367 2024-04-22 14:28:14.000000 dovekie-0.6.0/dovekie/core.py
-drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-22 14:33:14.894402 dovekie-0.6.0/dovekie.egg-info/
--rw-r--r--   0 cph       (1000) cph       (1000)     2249 2024-04-22 14:33:14.000000 dovekie-0.6.0/dovekie.egg-info/PKG-INFO
--rw-r--r--   0 cph       (1000) cph       (1000)      186 2024-04-22 14:33:14.000000 dovekie-0.6.0/dovekie.egg-info/SOURCES.txt
--rw-r--r--   0 cph       (1000) cph       (1000)        1 2024-04-22 14:33:14.000000 dovekie-0.6.0/dovekie.egg-info/dependency_links.txt
--rw-r--r--   0 cph       (1000) cph       (1000)        8 2024-04-22 14:33:14.000000 dovekie-0.6.0/dovekie.egg-info/top_level.txt
--rw-r--r--   0 cph       (1000) cph       (1000)       38 2024-04-22 14:33:14.894402 dovekie-0.6.0/setup.cfg
--rw-r--r--   0 cph       (1000) cph       (1000)      457 2024-04-22 14:20:44.000000 dovekie-0.6.0/setup.py
+drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-25 20:14:00.539035 dovekie-0.7.0/
+-rw-r--r--   0 cph       (1000) cph       (1000)     1071 2024-04-07 17:09:48.000000 dovekie-0.7.0/LICENSE
+-rw-r--r--   0 cph       (1000) cph       (1000)     2252 2024-04-25 20:14:00.539035 dovekie-0.7.0/PKG-INFO
+-rw-r--r--   0 cph       (1000) cph       (1000)     1924 2024-04-22 14:36:14.000000 dovekie-0.7.0/README.md
+drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-25 20:14:00.539035 dovekie-0.7.0/dovekie/
+-rw-r--r--   0 cph       (1000) cph       (1000)       71 2024-04-25 14:42:39.000000 dovekie-0.7.0/dovekie/__init__.py
+-rw-r--r--   0 cph       (1000) cph       (1000)      367 2024-04-22 14:28:14.000000 dovekie-0.7.0/dovekie/core.py
+drwxr-xr-x   0 cph       (1000) cph       (1000)        0 2024-04-25 20:14:00.539035 dovekie-0.7.0/dovekie.egg-info/
+-rw-r--r--   0 cph       (1000) cph       (1000)     2252 2024-04-25 20:14:00.000000 dovekie-0.7.0/dovekie.egg-info/PKG-INFO
+-rw-r--r--   0 cph       (1000) cph       (1000)      186 2024-04-25 20:14:00.000000 dovekie-0.7.0/dovekie.egg-info/SOURCES.txt
+-rw-r--r--   0 cph       (1000) cph       (1000)        1 2024-04-25 20:14:00.000000 dovekie-0.7.0/dovekie.egg-info/dependency_links.txt
+-rw-r--r--   0 cph       (1000) cph       (1000)        8 2024-04-25 20:14:00.000000 dovekie-0.7.0/dovekie.egg-info/top_level.txt
+-rw-r--r--   0 cph       (1000) cph       (1000)       38 2024-04-25 20:14:00.539035 dovekie-0.7.0/setup.cfg
+-rw-r--r--   0 cph       (1000) cph       (1000)      457 2024-04-25 20:03:10.000000 dovekie-0.7.0/setup.py
```

### Comparing `dovekie-0.6.0/LICENSE` & `dovekie-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dovekie-0.6.0/PKG-INFO` & `dovekie-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dovekie
-Version: 0.6.0
+Version: 0.7.0
 Summary: A library that defines common SKI combinators from Combinatory Logic.
 Home-page: UNKNOWN
 Author: Conor Hoekstra
 Author-email: codereport@outlook.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -43,17 +43,17 @@
 ```
 
 And how to use:
 ```py
 import operator as op
 from itertools import accumulate
 
-import dovekie as d
+import dovekie as dk
 
 
 def mco(xs: list[int]) -> int:
-    return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
+    return max(accumulate(xs, dk.phi1(op.add, op.mul, dk.r)))
 
 print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dovekie Version: 0.6.0 Summary: A library that
+Metadata-Version: 2.1 Name: dovekie Version: 0.7.0 Summary: A library that
 defines common SKI combinators from Combinatory Logic. Home-page: UNKNOWN
 Author: Conor Hoekstra Author-email: codereport@outlook.com License: MIT
 Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE #
                                    `dovekie`
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
@@ -14,10 +14,10 @@
 combinators from [Combinatory Logic](https://combinatorylogic.com/) and common
 unary and binary functions that are often used with these combinators. It is
 the spiritual equivalent of the: * C++ [`blackbird` library](https://
 github.com/codereport/blackbird) * Rust [`bluebird` library](https://
 github.com/codereport/bluebird)
                            [image-removebg-preview]
 How to install: ```bash pip3 install dovekie ``` And how to use: ```py import
-operator as op from itertools import accumulate import dovekie as d def mco(xs:
-list[int]) -> int: return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
-print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
+operator as op from itertools import accumulate import dovekie as dk def mco
+(xs: list[int]) -> int: return max(accumulate(xs, dk.phi1(op.add, op.mul,
+dk.r))) print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
```

### Comparing `dovekie-0.6.0/README.md` & `dovekie-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```
 
 And how to use:
 ```py
 import operator as op
 from itertools import accumulate
 
-import dovekie as d
+import dovekie as dk
 
 
 def mco(xs: list[int]) -> int:
-    return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
+    return max(accumulate(xs, dk.phi1(op.add, op.mul, dk.r)))
 
 print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3
 ```
```

#### html2text {}

```diff
@@ -10,10 +10,10 @@
 combinators from [Combinatory Logic](https://combinatorylogic.com/) and common
 unary and binary functions that are often used with these combinators. It is
 the spiritual equivalent of the: * C++ [`blackbird` library](https://
 github.com/codereport/blackbird) * Rust [`bluebird` library](https://
 github.com/codereport/bluebird)
                            [image-removebg-preview]
 How to install: ```bash pip3 install dovekie ``` And how to use: ```py import
-operator as op from itertools import accumulate import dovekie as d def mco(xs:
-list[int]) -> int: return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
-print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
+operator as op from itertools import accumulate import dovekie as dk def mco
+(xs: list[int]) -> int: return max(accumulate(xs, dk.phi1(op.add, op.mul,
+dk.r))) print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
```

### Comparing `dovekie-0.6.0/dovekie.egg-info/PKG-INFO` & `dovekie-0.7.0/dovekie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dovekie
-Version: 0.6.0
+Version: 0.7.0
 Summary: A library that defines common SKI combinators from Combinatory Logic.
 Home-page: UNKNOWN
 Author: Conor Hoekstra
 Author-email: codereport@outlook.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -43,17 +43,17 @@
 ```
 
 And how to use:
 ```py
 import operator as op
 from itertools import accumulate
 
-import dovekie as d
+import dovekie as dk
 
 
 def mco(xs: list[int]) -> int:
-    return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
+    return max(accumulate(xs, dk.phi1(op.add, op.mul, dk.r)))
 
 print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dovekie Version: 0.6.0 Summary: A library that
+Metadata-Version: 2.1 Name: dovekie Version: 0.7.0 Summary: A library that
 defines common SKI combinators from Combinatory Logic. Home-page: UNKNOWN
 Author: Conor Hoekstra Author-email: codereport@outlook.com License: MIT
 Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE #
                                    `dovekie`
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
@@ -14,10 +14,10 @@
 combinators from [Combinatory Logic](https://combinatorylogic.com/) and common
 unary and binary functions that are often used with these combinators. It is
 the spiritual equivalent of the: * C++ [`blackbird` library](https://
 github.com/codereport/blackbird) * Rust [`bluebird` library](https://
 github.com/codereport/bluebird)
                            [image-removebg-preview]
 How to install: ```bash pip3 install dovekie ``` And how to use: ```py import
-operator as op from itertools import accumulate import dovekie as d def mco(xs:
-list[int]) -> int: return max(accumulate(xs, d.phi1(op.add, op.mul, d.r)))
-print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
+operator as op from itertools import accumulate import dovekie as dk def mco
+(xs: list[int]) -> int: return max(accumulate(xs, dk.phi1(op.add, op.mul,
+dk.r))) print(mco([1, 0, 1, 1, 1, 0, 0, 1, 1, 0])) # 3 ```
```


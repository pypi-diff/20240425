# Comparing `tmp/modlinear-1.0.0.tar.gz` & `tmp/modlinear-1.0.1.tar.gz`

## Comparing `modlinear-1.0.0.tar` & `modlinear-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 modlinear-1.0.0/tutorial.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 modlinear-1.0.0/src/modlinear/__init__.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 modlinear-1.0.0/src/modlinear/tool.py
--rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 modlinear-1.0.0/src/modlinear/utils.py
--rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 modlinear-1.0.0/tests/tutorial.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 modlinear-1.0.0/.gitignore
--rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 modlinear-1.0.0/LICENSE
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 modlinear-1.0.0/README.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 modlinear-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 modlinear-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 modlinear-1.0.1/tutorial.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 modlinear-1.0.1/src/modlinear/__init__.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 modlinear-1.0.1/src/modlinear/tool.py
+-rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 modlinear-1.0.1/src/modlinear/utils.py
+-rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 modlinear-1.0.1/tests/tutorial.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 modlinear-1.0.1/.gitignore
+-rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 modlinear-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 modlinear-1.0.1/README.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 modlinear-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    17258 2020-02-02 00:00:00.000000 modlinear-1.0.1/PKG-INFO
```

### Comparing `modlinear-1.0.0/tutorial.py` & `modlinear-1.0.1/tutorial.py`

 * *Files identical despite different names*

### Comparing `modlinear-1.0.0/src/modlinear/tool.py` & `modlinear-1.0.1/src/modlinear/tool.py`

 * *Files identical despite different names*

### Comparing `modlinear-1.0.0/src/modlinear/utils.py` & `modlinear-1.0.1/src/modlinear/utils.py`

 * *Files identical despite different names*

### Comparing `modlinear-1.0.0/tests/tutorial.py` & `modlinear-1.0.1/tests/tutorial.py`

 * *Files identical despite different names*

### Comparing `modlinear-1.0.0/LICENSE` & `modlinear-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modlinear-1.0.0/README.md` & `modlinear-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -95,8 +95,18 @@
 ## III. Tutorial 
 
 There is a [tutorial](https://github.com/QiYuan-Zhang/ModLinear/blob/main/tutorial.py) example to illustrate how to use the *modlinear* to linearize nonlinear models.
 
 
 ## License
 
-The project is released under the APACHE license. See [LICENSE](https://github.com/QiYuan-Zhang/ModLinear/blob/main/LICENSE) for details.
+The project is released under the APACHE license. See [LICENSE](https://github.com/QiYuan-Zhang/ModLinear/blob/main/LICENSE) for details.
+
+Copyright 2024 Xuewen Zhang
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
+
+```
+http://www.apache.org/licenses/LICENSE-2.0
+```
+
+Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
```

### Comparing `modlinear-1.0.0/pyproject.toml` & `modlinear-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "modlinear"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Xuewen Zhang", email="xuewen.zhang741@outlook.com"}
 ]
 maintainers = [
   { name="Xuewen Zhang", email="xuewen.zhang741@outlook.com"}
 ]
 dependencies = [
```

### Comparing `modlinear-1.0.0/PKG-INFO` & `modlinear-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: modlinear
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapped package to linearize the nonlinear continuous/discrete model. Including **numerical** and **symbolic** calculations.
 Project-URL: Homepage, https://github.com/QiYuan-Zhang/ModLinear
 Project-URL: Issues, https://github.com/QiYuan-Zhang/ModLinear/issues
 Project-URL: Introduction, https://qiyuan-zhang.github.io/my-toolbox/2024/04/25/Developed-modlinear.html
 Author-email: Xuewen Zhang <xuewen.zhang741@outlook.com>
 Maintainer-email: Xuewen Zhang <xuewen.zhang741@outlook.com>
 License:                                 Apache License
@@ -313,8 +313,18 @@
 ## III. Tutorial 
 
 There is a [tutorial](https://github.com/QiYuan-Zhang/ModLinear/blob/main/tutorial.py) example to illustrate how to use the *modlinear* to linearize nonlinear models.
 
 
 ## License
 
-The project is released under the APACHE license. See [LICENSE](https://github.com/QiYuan-Zhang/ModLinear/blob/main/LICENSE) for details.
+The project is released under the APACHE license. See [LICENSE](https://github.com/QiYuan-Zhang/ModLinear/blob/main/LICENSE) for details.
+
+Copyright 2024 Xuewen Zhang
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
+
+```
+http://www.apache.org/licenses/LICENSE-2.0
+```
+
+Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
```


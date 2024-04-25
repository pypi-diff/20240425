# Comparing `tmp/cz_kpn-3.2.5.tar.gz` & `tmp/cz_kpn-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_kpn-3.2.5.tar", max compression
+gzip compressed data, was "cz_kpn-3.2.6.tar", max compression
```

## Comparing `cz_kpn-3.2.5.tar` & `cz_kpn-3.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1417 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/CHANGELOG.md
--rw-r--r--   0        0        0     1059 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/LICENSE
--rw-r--r--   0        0        0     6272 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/README.md
--rw-r--r--   0        0        0   564052 2024-04-15 09:22:53.250926 cz_kpn-3.2.5/docs/images/bump.gif
--rw-r--r--   0        0        0  1023699 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/docs/images/commit.gif
--rw-r--r--   0        0        0      920 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/pyproject.toml
--rw-r--r--   0        0        0       52 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/__init__.py
--rw-r--r--   0        0        0      763 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/consts.py
--rw-r--r--   0        0        0     1359 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/cz_kpn_info.txt
--rw-r--r--   0        0        0     3423 2024-04-15 09:22:53.254926 cz_kpn-3.2.5/src/cz_kpn/rules.py
--rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 cz_kpn-3.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1592 2024-04-25 07:19:29.874802 cz_kpn-3.2.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1059 2024-04-25 07:19:29.874802 cz_kpn-3.2.6/LICENSE
+-rw-r--r--   0        0        0     6272 2024-04-25 07:19:29.874802 cz_kpn-3.2.6/README.md
+-rw-r--r--   0        0        0   564052 2024-04-25 07:19:29.878802 cz_kpn-3.2.6/docs/images/bump.gif
+-rw-r--r--   0        0        0  1023699 2024-04-25 07:19:29.882802 cz_kpn-3.2.6/docs/images/commit.gif
+-rw-r--r--   0        0        0      920 2024-04-25 07:19:29.882802 cz_kpn-3.2.6/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-25 07:19:29.882802 cz_kpn-3.2.6/src/cz_kpn/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-25 07:19:29.882802 cz_kpn-3.2.6/src/cz_kpn/consts.py
+-rw-r--r--   0        0        0     1359 2024-04-25 07:19:29.882802 cz_kpn-3.2.6/src/cz_kpn/cz_kpn_info.txt
+-rw-r--r--   0        0        0     3423 2024-04-25 07:19:29.882802 cz_kpn-3.2.6/src/cz_kpn/rules.py
+-rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 cz_kpn-3.2.6/PKG-INFO
```

### Comparing `cz_kpn-3.2.5/CHANGELOG.md` & `cz_kpn-3.2.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.2.6 (2024-04-25)
+
+### Improvements
+
+- Increase wait time to release to docker ([178af5e](https://github.com/kpn/cz-kpn/commit/178af5e32943be5d57e5a1f69d6fcc85de06b8a8))
+
 ## 3.2.5 (2024-04-15)
 
 ### Fixes
 
 - release pipeline ([1ab09a8](https://github.com/kpn/cz-kpn/commit/1ab09a840ba1e83ed57f524b5dba7fd385940ab0))
 
 ## 3.2.4 (2024-01-03)
```

### Comparing `cz_kpn-3.2.5/LICENSE` & `cz_kpn-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/README.md` & `cz_kpn-3.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/docs/images/bump.gif` & `cz_kpn-3.2.6/docs/images/bump.gif`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/docs/images/commit.gif` & `cz_kpn-3.2.6/docs/images/commit.gif`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/pyproject.toml` & `cz_kpn-3.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-kpn"
-version = "3.2.5"
+version = "3.2.6"
 description = "commitizen with kpn style"
 authors = ["Santiago Fraire Willemoes <santiago.fraire@kpn.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "cz_kpn", from = "src" }]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
```

### Comparing `cz_kpn-3.2.5/src/cz_kpn/consts.py` & `cz_kpn-3.2.6/src/cz_kpn/consts.py`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/src/cz_kpn/cz_kpn_info.txt` & `cz_kpn-3.2.6/src/cz_kpn/cz_kpn_info.txt`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/src/cz_kpn/rules.py` & `cz_kpn-3.2.6/src/cz_kpn/rules.py`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.5/PKG-INFO` & `cz_kpn-3.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-kpn
-Version: 3.2.5
+Version: 3.2.6
 Summary: commitizen with kpn style
 Home-page: https://github.com/kpn/cz-kpn
 License: MIT
 Keywords: commitizen,release-management,autorelease
 Author: Santiago Fraire Willemoes
 Author-email: santiago.fraire@kpn.com
 Requires-Python: >=3.9,<4.0
```


# Comparing `tmp/cz_kpn-3.2.7.tar.gz` & `tmp/cz_kpn-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_kpn-3.2.7.tar", max compression
+gzip compressed data, was "cz_kpn-3.2.8.tar", max compression
```

## Comparing `cz_kpn-3.2.7.tar` & `cz_kpn-3.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1752 2024-04-25 07:43:25.797817 cz_kpn-3.2.7/CHANGELOG.md
--rw-r--r--   0        0        0     1059 2024-04-25 07:43:25.797817 cz_kpn-3.2.7/LICENSE
--rw-r--r--   0        0        0     6272 2024-04-25 07:43:25.797817 cz_kpn-3.2.7/README.md
--rw-r--r--   0        0        0   564052 2024-04-25 07:43:25.801817 cz_kpn-3.2.7/docs/images/bump.gif
--rw-r--r--   0        0        0  1023699 2024-04-25 07:43:25.805817 cz_kpn-3.2.7/docs/images/commit.gif
--rw-r--r--   0        0        0     1074 2024-04-25 07:43:25.805817 cz_kpn-3.2.7/pyproject.toml
--rw-r--r--   0        0        0       52 2024-04-25 07:43:25.805817 cz_kpn-3.2.7/src/cz_kpn/__init__.py
--rw-r--r--   0        0        0      764 2024-04-25 07:43:25.805817 cz_kpn-3.2.7/src/cz_kpn/consts.py
--rw-r--r--   0        0        0     1359 2024-04-25 07:43:25.805817 cz_kpn-3.2.7/src/cz_kpn/cz_kpn_info.txt
--rw-r--r--   0        0        0     3423 2024-04-25 07:43:25.805817 cz_kpn-3.2.7/src/cz_kpn/rules.py
--rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 cz_kpn-3.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1901 2024-04-25 08:29:41.211217 cz_kpn-3.2.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1059 2024-04-25 08:29:41.211217 cz_kpn-3.2.8/LICENSE
+-rw-r--r--   0        0        0     6272 2024-04-25 08:29:41.211217 cz_kpn-3.2.8/README.md
+-rw-r--r--   0        0        0   564052 2024-04-25 08:29:41.215217 cz_kpn-3.2.8/docs/images/bump.gif
+-rw-r--r--   0        0        0  1023699 2024-04-25 08:29:41.215217 cz_kpn-3.2.8/docs/images/commit.gif
+-rw-r--r--   0        0        0     1074 2024-04-25 08:29:41.219218 cz_kpn-3.2.8/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-25 08:29:41.219218 cz_kpn-3.2.8/src/cz_kpn/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-25 08:29:41.219218 cz_kpn-3.2.8/src/cz_kpn/consts.py
+-rw-r--r--   0        0        0     1359 2024-04-25 08:29:41.219218 cz_kpn-3.2.8/src/cz_kpn/cz_kpn_info.txt
+-rw-r--r--   0        0        0     3423 2024-04-25 08:29:41.219218 cz_kpn-3.2.8/src/cz_kpn/rules.py
+-rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 cz_kpn-3.2.8/PKG-INFO
```

### Comparing `cz_kpn-3.2.7/CHANGELOG.md` & `cz_kpn-3.2.8/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.2.8 (2024-04-25)
+
+### Improvements
+
+- Format readme ([451178c](https://github.com/kpn/cz-kpn/commit/451178c30831769c348fe362e2d5a38e56394f9f))
+
 ## 3.2.7 (2024-04-25)
 
 ### Improvements
 
 - Use ruff latest and mypy ([d89f25e](https://github.com/kpn/cz-kpn/commit/d89f25e7613cfd7c993fd5ef68da91187c9c4321))
 
 ## 3.2.6 (2024-04-25)
```

### Comparing `cz_kpn-3.2.7/LICENSE` & `cz_kpn-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.7/README.md` & `cz_kpn-3.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,15 @@
           fetch-depth: 0
           token: ${{ secrets.PERSONAL_ACCESS_TOKEN }}
       - name: Create bump and changelog
         uses: commitizen-tools/commitizen-action@master
         with:
           github_token: ${{ secrets.PERSONAL_ACCESS_TOKEN }}
           changelog_increment_filename: body.md
-          extra_requirements: 'cz-kpn'
+          extra_requirements: "cz-kpn"
       - name: Release
         uses: softprops/action-gh-release@v1
         with:
           body_path: "body.md"
           tag_name: ${{ env.REVISION }}
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `cz_kpn-3.2.7/docs/images/bump.gif` & `cz_kpn-3.2.8/docs/images/bump.gif`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.7/docs/images/commit.gif` & `cz_kpn-3.2.8/docs/images/commit.gif`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.7/pyproject.toml` & `cz_kpn-3.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-kpn"
-version = "3.2.7"
+version = "3.2.8"
 description = "commitizen with kpn style"
 authors = ["Santiago Fraire Willemoes <santiago.fraire@kpn.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "cz_kpn", from = "src" }]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
```

### Comparing `cz_kpn-3.2.7/src/cz_kpn/consts.py` & `cz_kpn-3.2.8/src/cz_kpn/consts.py`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.7/src/cz_kpn/cz_kpn_info.txt` & `cz_kpn-3.2.8/src/cz_kpn/cz_kpn_info.txt`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.7/src/cz_kpn/rules.py` & `cz_kpn-3.2.8/src/cz_kpn/rules.py`

 * *Files identical despite different names*

### Comparing `cz_kpn-3.2.7/PKG-INFO` & `cz_kpn-3.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-kpn
-Version: 3.2.7
+Version: 3.2.8
 Summary: commitizen with kpn style
 Home-page: https://github.com/kpn/cz-kpn
 License: MIT
 Keywords: commitizen,release-management,autorelease
 Author: Santiago Fraire Willemoes
 Author-email: santiago.fraire@kpn.com
 Requires-Python: >=3.9,<4.0
@@ -254,15 +254,15 @@
           fetch-depth: 0
           token: ${{ secrets.PERSONAL_ACCESS_TOKEN }}
       - name: Create bump and changelog
         uses: commitizen-tools/commitizen-action@master
         with:
           github_token: ${{ secrets.PERSONAL_ACCESS_TOKEN }}
           changelog_increment_filename: body.md
-          extra_requirements: 'cz-kpn'
+          extra_requirements: "cz-kpn"
       - name: Release
         uses: softprops/action-gh-release@v1
         with:
           body_path: "body.md"
           tag_name: ${{ env.REVISION }}
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```


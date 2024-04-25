# Comparing `tmp/hypercoast-0.1.1.tar.gz` & `tmp/hypercoast-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.1.1.tar", last modified: Mon Apr 22 04:23:28 2024, max compression
+gzip compressed data, was "hypercoast-0.1.2.tar", last modified: Thu Apr 25 17:52:46 2024, max compression
```

## Comparing `hypercoast-0.1.1.tar` & `hypercoast-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.247961 hypercoast-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.235961 hypercoast-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.239961 hypercoast-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.239961 hypercoast-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-22 04:23:16.000000 hypercoast-0.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.243961 hypercoast-0.1.1/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-22 04:23:28.000000 hypercoast-0.1.1/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-22 04:23:28.000000 hypercoast-0.1.1/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:23:28.000000 hypercoast-0.1.1/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 04:23:28.000000 hypercoast-0.1.1/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 04:23:28.000000 hypercoast-0.1.1/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 04:23:28.000000 hypercoast-0.1.1/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 04:23:16.000000 hypercoast-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 04:23:16.000000 hypercoast-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-22 04:23:28.247961 hypercoast-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-22 04:23:16.000000 hypercoast-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.243961 hypercoast-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.243961 hypercoast-0.1.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/examples/emit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.243961 hypercoast-0.1.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/ui.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 04:23:16.000000 hypercoast-0.1.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.243961 hypercoast-0.1.1/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-22 04:23:16.000000 hypercoast-0.1.1/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-22 04:23:16.000000 hypercoast-0.1.1/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37734 2024-04-22 04:23:16.000000 hypercoast-0.1.1/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-22 04:23:16.000000 hypercoast-0.1.1/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-22 04:23:16.000000 hypercoast-0.1.1/hypercoast/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-22 04:23:16.000000 hypercoast-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 04:23:16.000000 hypercoast-0.1.1/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-22 04:23:16.000000 hypercoast-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 04:23:16.000000 hypercoast-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-22 04:23:16.000000 hypercoast-0.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:23:28.247961 hypercoast-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:23:28.243961 hypercoast-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 04:23:16.000000 hypercoast-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-22 04:23:16.000000 hypercoast-0.1.1/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.047348 hypercoast-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.051348 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.051348 hypercoast-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-25 17:52:31.000000 hypercoast-0.1.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 17:52:46.000000 hypercoast-0.1.2/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 17:52:31.000000 hypercoast-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 17:52:31.000000 hypercoast-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 17:52:46.055348 hypercoast-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 17:52:31.000000 hypercoast-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/examples/emit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 17:52:31.000000 hypercoast-0.1.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37734 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-25 17:52:31.000000 hypercoast-0.1.2/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-25 17:52:31.000000 hypercoast-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 17:52:31.000000 hypercoast-0.1.2/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 17:52:31.000000 hypercoast-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 17:52:31.000000 hypercoast-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 17:52:31.000000 hypercoast-0.1.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:52:46.055348 hypercoast-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:52:46.055348 hypercoast-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 17:52:31.000000 hypercoast-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-25 17:52:31.000000 hypercoast-0.1.2/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.1.1/.github/workflows/docs-build.yml` & `hypercoast-0.1.2/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.github/workflows/docs.yml` & `hypercoast-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.github/workflows/installation.yml` & `hypercoast-0.1.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.github/workflows/macos.yml` & `hypercoast-0.1.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.github/workflows/pypi.yml` & `hypercoast-0.1.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.github/workflows/ubuntu.yml` & `hypercoast-0.1.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.github/workflows/windows.yml` & `hypercoast-0.1.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.gitignore` & `hypercoast-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/.pre-commit-config.yaml` & `hypercoast-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.1.2/HyperCoast.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,7 +46,13 @@
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
 -   Visualize hyperspectral data
 -   Analyze hyperspectral data
+-
+## Demo
+
+-   Visualizing spectral signature interactively
+
+![](https://i.imgur.com/zeyABMq.gif)
```

### Comparing `hypercoast-0.1.1/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.1.2/HyperCoast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/LICENSE` & `hypercoast-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/PKG-INFO` & `hypercoast-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,7 +46,13 @@
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
 -   Visualize hyperspectral data
 -   Analyze hyperspectral data
+-
+## Demo
+
+-   Visualizing spectral signature interactively
+
+![](https://i.imgur.com/zeyABMq.gif)
```

### Comparing `hypercoast-0.1.1/README.md` & `hypercoast-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,7 +12,13 @@
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
 -   Visualize hyperspectral data
 -   Analyze hyperspectral data
+-
+## Demo
+
+-   Visualizing spectral signature interactively
+
+![](https://i.imgur.com/zeyABMq.gif)
```

### Comparing `hypercoast-0.1.1/docs/contributing.md` & `hypercoast-0.1.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/docs/examples/emit.ipynb` & `hypercoast-0.1.2/docs/examples/emit.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/docs/index.md` & `hypercoast-0.1.2/docs/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,7 +11,13 @@
 -   Free software: MIT License
 -   Documentation: <https://hypercoast.org>
 
 ## Features
 
 -   Visualize hyperspectral data
 -   Analyze hyperspectral data
+
+## Demo
+
+-   Visualizing spectral signature interactively
+
+![](https://i.imgur.com/zeyABMq.gif)
```

### Comparing `hypercoast-0.1.1/docs/installation.md` & `hypercoast-0.1.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/hypercoast/common.py` & `hypercoast-0.1.2/hypercoast/common.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/hypercoast/emit.py` & `hypercoast-0.1.2/hypercoast/emit.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/hypercoast/hypercoast.py` & `hypercoast-0.1.2/hypercoast/hypercoast.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,35 +36,37 @@
 
         if isinstance(obj, str):
             if obj == "spectral":
                 from .ui import SpectralWidget
 
                 SpectralWidget(self, position=position)
                 self.set_plot_options(add_marker_cluster=True)
+            else:
+                super().add(obj, **kwargs)
 
         else:
             super().add(obj, **kwargs)
 
-    def search_emit(self, default_datset="EMITL2ARFL"):
+    def search_emit(self, default_dataset="EMITL2ARFL"):
         """
         Adds a NASA Earth Data search tool to the map with a default dataset for EMIT.
 
         Args:
             default_dataset (str, optional): The default dataset to search for. Defaults to "EMITL2ARFL".
         """
-        self.add("nasa_earth_data", default_dataset=default_datset)
+        self.add("nasa_earth_data", default_dataset=default_dataset)
 
-    def search_pace(self, default_datset="PACE_OCI_L2_AOP_NRT"):
+    def search_pace(self, default_dataset="PACE_OCI_L2_AOP_NRT"):
         """
         Adds a NASA Earth Data search tool to the map with a default dataset for PACE.
 
         Args:
             default_dataset (str, optional): The default dataset to search for. Defaults to "PACE_OCI_L2_AOP_NRT".
         """
-        self.add("nasa_earth_data", default_dataset=default_datset)
+        self.add("nasa_earth_data", default_dataset=default_dataset)
 
     def add_raster(
         self,
         source,
         indexes=None,
         colormap=None,
         vmin=None,
```

### Comparing `hypercoast-0.1.1/hypercoast/ui.py` & `hypercoast-0.1.2/hypercoast/ui.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/mkdocs.yml` & `hypercoast-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.1.1/pyproject.toml` & `hypercoast-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.1.1"
+version = "0.1.2"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.1"
+current_version = "0.1.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```


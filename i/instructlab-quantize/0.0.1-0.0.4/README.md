# Comparing `tmp/instructlab_quantize-0.0.1.tar.gz` & `tmp/instructlab_quantize-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructlab_quantize-0.0.1.tar", last modified: Thu Apr 25 04:18:22 2024, max compression
+gzip compressed data, was "instructlab_quantize-0.0.4.tar", last modified: Thu Apr 25 04:55:07 2024, max compression
```

## Comparing `instructlab_quantize-0.0.1.tar` & `instructlab_quantize-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:18:22.142220 instructlab_quantize-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:18:22.138220 instructlab_quantize-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:18:22.138220 instructlab_quantize-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 04:18:22.142220 instructlab_quantize-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 04:18:22.142220 instructlab_quantize-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:18:22.138220 instructlab_quantize-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:18:22.138220 instructlab_quantize-0.0.1/src/instructlab_quantize/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/src/instructlab_quantize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)  1653384 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/src/instructlab_quantize/quantize
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:18:22.142220 instructlab_quantize-0.0.1/src/instructlab_quantize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 04:18:22.000000 instructlab_quantize-0.0.1/src/instructlab_quantize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 04:18:22.000000 instructlab_quantize-0.0.1/src/instructlab_quantize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:18:22.000000 instructlab_quantize-0.0.1/src/instructlab_quantize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 04:18:22.000000 instructlab_quantize-0.0.1/src/instructlab_quantize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-25 04:18:16.000000 instructlab_quantize-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:55:07.762806 instructlab_quantize-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:55:07.758805 instructlab_quantize-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:55:07.758805 instructlab_quantize-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 04:55:07.762806 instructlab_quantize-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 04:55:07.762806 instructlab_quantize-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:55:07.758805 instructlab_quantize-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:55:07.758805 instructlab_quantize-0.0.4/src/instructlab_quantize/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/src/instructlab_quantize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1653384 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/src/instructlab_quantize/quantize
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:55:07.762806 instructlab_quantize-0.0.4/src/instructlab_quantize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 04:55:07.000000 instructlab_quantize-0.0.4/src/instructlab_quantize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 04:55:07.000000 instructlab_quantize-0.0.4/src/instructlab_quantize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:55:07.000000 instructlab_quantize-0.0.4/src/instructlab_quantize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 04:55:07.000000 instructlab_quantize-0.0.4/src/instructlab_quantize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-25 04:55:03.000000 instructlab_quantize-0.0.4/tox.ini
```

### Comparing `instructlab_quantize-0.0.1/.github/workflows/build.yaml` & `instructlab_quantize-0.0.4/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/.github/workflows/pypi.yaml` & `instructlab_quantize-0.0.4/.github/workflows/pypi.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
             - "v*"
     pull_request:
         branches:
             - main
     release:
         types:
             - published
-    workflow_dispatch:
 
 permissions:
-    contents: read
+    # allow gh release upload
+    contents: write
     # see https://docs.pypi.org/trusted-publishers/
     id-token: write
 
 jobs:
     build-package:
         name: Build and check packages
         runs-on: ubuntu-latest
@@ -35,15 +35,14 @@
     publish-test-pypi:
         name: Publish packages to test.pypi.org
         # environment: publish-test-pypi
         # TODO: move to instructlab
         if: |
             github.repository_owner == 'tiran' && (
                 github.event.action == 'published' ||
-                github.event_name == 'workflow_dispatch' ||
                 (github.event_name == 'push' && github.ref == 'refs/heads/main')
             )
         runs-on: ubuntu-latest
         needs: build-package
 
         steps:
             - name: Fetch build artifacts
@@ -58,23 +57,37 @@
                   repository-url: https://test.pypi.org/legacy/
 
     publish-pypi:
         name: Publish release to pypi.org
         # environment: publish-pypi
         # TODO: move to instructlab
         if: |
-            github.repository_owner == 'tiran' && (
-                github.event.action == 'published' ||
-                github.event_name == 'workflow_dispatch'
-            )
+            github.repository_owner == 'tiran' && github.event.action == 'published'
         runs-on: ubuntu-latest
         needs: build-package
 
         steps:
             - name: Fetch build artifacts
               uses: actions/download-artifact@v4
               with:
                   name: Packages
                   path: dist
 
+            - uses: sigstore/gh-action-sigstore-python@v2.1.1
+              with:
+                  inputs: >-
+                      ./dist/*.tar.gz
+                      ./dist/*.whl
+
+            - name: Upload artifact signatures to GitHub Release
+              env:
+                  GITHUB_TOKEN: ${{ github.token }}
+              run: >-
+                  gh release upload '${{ github.ref_name }}' dist/* --repo '${{ github.repository }}'
+
+            # PyPI does not accept .sigstore artifacts and
+            # gh-action-pypi-publish has no option to ignore them.
+            - name: Remove sigstore signatures before uploading to PyPI
+              run: rm ./dist/*.sigstore
+
             - name: Upload to PyPI
               uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `instructlab_quantize-0.0.1/.github/workflows/tests.yml` & `instructlab_quantize-0.0.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/.gitignore` & `instructlab_quantize-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/.pylintrc` & `instructlab_quantize-0.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/LICENSE` & `instructlab_quantize-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/Makefile` & `instructlab_quantize-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/PKG-INFO` & `instructlab_quantize-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructlab-quantize
-Version: 0.0.1
+Version: 0.0.4
 Summary: Quantize binary for InstructLab
 Author-email: Christian Heimes <cheimes@redhat.com>
 License: Apache-2.0 AND MIT
 Project-URL: source, https://github.com/tiran/instructlab-quantize
 Project-URL: issues, https://github.com/tiran/instructlab-quantize/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `instructlab_quantize-0.0.1/README.md` & `instructlab_quantize-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/pyproject.toml` & `instructlab_quantize-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/src/instructlab_quantize/__init__.py` & `instructlab_quantize-0.0.4/src/instructlab_quantize/__init__.py`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/src/instructlab_quantize/quantize` & `instructlab_quantize-0.0.4/src/instructlab_quantize/quantize`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/src/instructlab_quantize.egg-info/PKG-INFO` & `instructlab_quantize-0.0.4/src/instructlab_quantize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructlab-quantize
-Version: 0.0.1
+Version: 0.0.4
 Summary: Quantize binary for InstructLab
 Author-email: Christian Heimes <cheimes@redhat.com>
 License: Apache-2.0 AND MIT
 Project-URL: source, https://github.com/tiran/instructlab-quantize
 Project-URL: issues, https://github.com/tiran/instructlab-quantize/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `instructlab_quantize-0.0.1/tests.py` & `instructlab_quantize-0.0.4/tests.py`

 * *Files identical despite different names*

### Comparing `instructlab_quantize-0.0.1/tox.ini` & `instructlab_quantize-0.0.4/tox.ini`

 * *Files identical despite different names*


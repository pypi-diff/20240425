# Comparing `tmp/muondatalib-0.3.0b0.tar.gz` & `tmp/muondatalib-0.5.0b0.tar.gz`

## Comparing `muondatalib-0.3.0b0.tar` & `muondatalib-0.5.0b0.tar`

### file list

```diff
@@ -1,41 +1,63 @@
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.readthedocs.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/MuonDataLib-dev.yml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/MuonDataLib.yml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/release.yml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/workflows/flake8.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/workflows/label_merge_conflicts.yml
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/workflows/merge.yml
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/workflows/release_next.yml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/api.rst
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/conf.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/index.rst
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/intro.rst
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/usage.rst
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/dev/index.rst
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/docs/source/dev/setup.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/__init__.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/detector1.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/hdf5.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/muon_data.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/periods.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/raw_data.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/sample.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/source.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/user.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/loader/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/src/MuonDataLib/data/loader/load_nxs2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/test/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/test/add_test.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/tools/conda_dict_to_yml.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/tools/create_conda_yml.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/tools/setup_helper.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/tools/version.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/README.md
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/pyproject.toml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 muondatalib-0.3.0b0/PKG-INFO
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.readthedocs.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/MuonDataLib-dev.yml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/MuonDataLib.yml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/release.yml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/flake8.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/label_merge_conflicts.yml
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/merge.yml
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/release_next.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/api.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/conf.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/index.rst
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/intro.rst
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/loaders.rst
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/dev/index.rst
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/dev/setup.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/__init__.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/detector1.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/hdf5.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/muon_data.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/periods.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/raw_data.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/sample.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/source.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/user.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/loader/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/loader/load_nxs2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/test_helpers/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/test_helpers/nexus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/__init__.py
+-rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/detector1_test.py
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/hdf5_test.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/muon_data_test.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/periods_test.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/raw_data_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/sample_test.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/source_test.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/user_test.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/loader/__init__.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/loader/load_nxs2_test.py
+-rw-r--r--   0        0        0  1370476 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI00180594.nxs
+-rw-r--r--   0        0        0  1977434 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI00183810.nxs
+-rw-r--r--   0        0        0   560372 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI42.nxs
+-rw-r--r--   0        0        0  1084660 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI51.nxs
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/system_tests/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/system_tests/multiperiod_test.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/system_tests/single_period_test.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/test_helpers/nexus_test.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/conda_dict_to_yml.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/create_conda_yml.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/setup_helper.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/version.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/README.md
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/pyproject.toml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/PKG-INFO
```

### Comparing `muondatalib-0.3.0b0/.pre-commit-config.yaml` & `muondatalib-0.5.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/.github/PULL_REQUEST_TEMPLATE.md` & `muondatalib-0.5.0b0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/.github/workflows/label_merge_conflicts.yml` & `muondatalib-0.5.0b0/.github/workflows/label_merge_conflicts.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/.github/workflows/merge.yml` & `muondatalib-0.5.0b0/.github/workflows/release_next.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,61 @@
-name: Build and upload to PyPI
+name: Build and upload release to PyPI
 
 on:
-  pull_request_review:
-    types: [submitted]
+  push:
+    branches:
+    - 'main'
+  pull_request:
+    branches:
+      - 'main'
+
 permissions:
   contents: write
 
 jobs:
   update_version:
     name: update version
-    if: github.event.review.state == 'approved'
     runs-on: ubuntu-latest
     steps:
       - name: checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: "0"
       - name: Update version on merge
         run:  |
-            python tools/version.py "beta"
+            python tools/version.py "minor"
       - name: Store changes
         uses: actions/upload-artifact@v3
         with:
           name: pyproject
           path: pyproject.toml
 
-  build_sdist:
-    name: Build source distribution
+  build:
+    name: Build wheels and src
     runs-on: ubuntu-latest
     needs: [update_version]
     steps:
-      - uses: actions/checkout@v4
-      - name: Build sdist
-        run: |
-          pip install numpy
-          python -m build --sdist
-      - uses: actions/upload-artifact@v3
-        with:
-          path: dist/*.tar.gz
-
-  build_wheels:
-    name: Build and test wheels on ${{ matrix.os }}
-    runs-on: ${{ matrix.os }}
-    needs: [update_version]
-    strategy:
-      matrix:
-        os: [ubuntu-latest, windows-latest, macOS-latest]
-    steps:
       - name: checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: "0"
       - uses: actions/download-artifact@v3
         with:
-          name: setup
+          name: pyproject
+      - name: install build
+        run: python -m pip install build pytest --user
       - name: build wheel
-        uses: pypa/cibuildwheel@v2.8.0
-        env:
-          # List of platforms to build on (incl. Python version)
-          CIBW_BUILD: cp3{8,9,10,11}-manylinux_x86_64 cp3{8,9,10,11}-win_amd64 cp3{8,9,10,11}-macosx_x86_64 cp3{8,9,10,11}-macosx_arm64
-
-          CIBW_BEFORE_BUILD: >
-             pip install numpy cython
-          # Install test dependencies and run tests
-          CIBW_TEST_REQUIRES: pytest
-          CIBW_TEST_COMMAND: >
-            pytest {project}/test
+        run: python -m build --sdist --wheel
       - name: upload wheel
         uses: actions/upload-artifact@v3
         with:
-          path: ./wheelhouse/*.whl
+          path: dist/
 
   upload_pypi:
-    needs: [build_wheels, build_sdist]
+    needs: [build]
     runs-on: ubuntu-latest
     permissions:
       id-token: write
     steps:
       - name: mint API token
         id: mint
         uses: tschm/token-mint-action@v1.0.2
@@ -94,28 +73,35 @@
 
   update_setup:
     needs: [upload_pypi]
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
-      - name: checkout
+      - name: checkout_release
+        if: ${{ github.event.push.head.ref }} == 'release-next'
         uses: actions/checkout@v4
         with:
           fetch-depth: "0"
-          repository: ${{github.event.pull_request.head.repo.full_name }}
-          ref: ${{ github.event.pull_request.head.ref }}
+          repository: ${{github.event.push.head.repo.full_name }}
+          ref: ${{ github.event.push.head.ref }}
 
       - uses: actions/download-artifact@v3
         with:
           name: pyproject
       - name: check
         run: |
           cat pyproject.toml
-          echo ${{github.event.pull_request.head.repo.full_name }}
+          echo ${{github.event.merge_group.head.repo.full_name }}
       - name: Commit on merge
         run: |
           git config user.name github-actions
           git config user.email github-actions@github.com
           git add pyproject.toml
           git commit -m "update version number"
           git push
+      - name: create_new_branch
+        run: |
+          git config user.name github-actions
+          git config user.email github-actions@github.com
+          git checkout --no-track -b version_bump origin/release-next
+          git push --set-upstream origin version_bump
```

### Comparing `muondatalib-0.3.0b0/.github/workflows/release_next.yml` & `muondatalib-0.5.0b0/.github/workflows/merge.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-name: Build and upload release to PyPI
+name: Build and upload to PyPI
 
 on:
-  push:
-    branches:
-    - 'main'
-  pull_request:
-    branches:
-      - 'main'
-
+  pull_request_review:
+    types: [submitted]
 permissions:
   contents: write
 
 jobs:
   update_version:
     name: update version
+    if: github.event.review.state == 'approved'
     runs-on: ubuntu-latest
     steps:
       - name: checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: "0"
       - name: Update version on merge
         run:  |
-            python tools/version.py "minor"
+            python tools/version.py "beta"
       - name: Store changes
         uses: actions/upload-artifact@v3
         with:
           name: pyproject
           path: pyproject.toml
 
   build:
@@ -41,16 +37,14 @@
       - uses: actions/download-artifact@v3
         with:
           name: pyproject
       - name: install build
         run: python -m pip install build pytest --user
       - name: build wheel
         run: python -m build --sdist --wheel
-      - name: test wheel
-        run: python -m pytest
       - name: upload wheel
         uses: actions/upload-artifact@v3
         with:
           path: dist/
 
   upload_pypi:
     needs: [build]
@@ -68,42 +62,34 @@
           path: dist
 
       - name: Publish package distribution to PYPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ steps.mint.outputs.api-token }}
 
-
   update_setup:
     needs: [upload_pypi]
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
-      - name: checkout_release
-        if: ${{ github.event.push.head.ref }} == 'release-next'
+      - name: checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: "0"
-          repository: ${{github.event.push.head.repo.full_name }}
-          ref: ${{ github.event.push.head.ref }}
+          repository: ${{github.event.pull_request.head.repo.full_name }}
+          ref: ${{ github.event.pull_request.head.ref }}
 
       - uses: actions/download-artifact@v3
         with:
           name: pyproject
       - name: check
         run: |
           cat pyproject.toml
-          echo ${{github.event.merge_group.head.repo.full_name }}
+          echo ${{github.event.pull_request.head.repo.full_name }}
       - name: Commit on merge
         run: |
           git config user.name github-actions
           git config user.email github-actions@github.com
           git add pyproject.toml
           git commit -m "update version number"
           git push
-      - name: create_new_branch
-        run: |
-          git config user.name github-actions
-          git config user.email github-actions@github.com
-          git checkout --no-track -b version_bump origin/release-next
-          git push --set-upstream origin version_bump
```

### Comparing `muondatalib-0.3.0b0/.github/workflows/run_tests.yml` & `muondatalib-0.5.0b0/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/docs/source/conf.py` & `muondatalib-0.5.0b0/docs/source/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 sys.path.insert(0, pathlib.Path(__file__).parents[2].resolve().as_posix())
 
 
 project = 'MuonDataLib'
 copyright = '2023, Anthony Lim'
 author = 'Anthony Lim'
 release = '0.0.1'
+build_triggered = True
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.autosummary']
```

### Comparing `muondatalib-0.3.0b0/docs/source/dev/setup.rst` & `muondatalib-0.5.0b0/docs/source/dev/setup.rst`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/detector1.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/detector1.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,45 +39,47 @@
 
     @property
     def resolution(self):
         """
         Get the resolution in pico seconds
         :return the resolution in pico seconds
         """
-        return self._dict['resolution']*1e6
+        return int(self._dict['resolution']*1e6)
 
     def save_nxs2(self, file):
         """
         Save the detector 1 values for a muon NXS v2 file
         :param file: the open file to write the data to
         """
         tmp = file.require_group('raw_data_1')
         tmp = tmp.require_group('instrument')
         tmp.attrs['NX_class'] = 'NXinstrument'
         tmp = tmp.require_group('detector_1')
         tmp.attrs['NX_class'] = 'NXdetector'
 
         resolution = self.save_int('resolution', self.resolution, tmp)
-        resolution.attrs.create('units', 'picoseconds', dtype='S11')
+        resolution.attrs.create('units', 'picoseconds'.encode(), dtype='S11')
 
         raw = self.save_float_array('raw_time', self._dict['raw_time'], tmp)
-        raw.attrs.create('units', 'microseconds', dtype='S12')
-        raw.attrs.create('long_name', 'time', dtype='S4')
+        raw.attrs.create('units', 'microseconds'.encode(), dtype='S12')
+        raw.attrs.create('long_name', 'time'.encode(), dtype='S4')
 
         self.save_int_array('spectrum_index',
                             self._dict['spectrum_index'],
                             tmp)
 
         counts = self.save_counts_array('counts', self.N_periods,
                                         self.N_hist, self.N_x,
                                         self._dict['counts'], tmp)
         counts.attrs.create('axes',
-                            '[period index, spectrum index, raw time bin]',
+                            ('[period index, '
+                             'spectrum index, '
+                             'raw time bin]').encode(),
                             dtype='S45')
-        counts.attrs.create('long_name', self._dict['inst'],
+        counts.attrs.create('long_name', self._dict['inst'].encode(),
                             dtype=stype(self._dict['inst']))
         counts.attrs.create('t0_bin', self._dict['time_zero'], dtype=INT32)
 
         first_bin = int(self._dict['first_good']/self._dict['resolution'])
         counts.attrs.create('first_good_bin',
                             first_bin,
                             dtype=INT32)
@@ -100,15 +102,15 @@
     # convert to micro seconds
     resolution = tmp['resolution'][0] / 1.e6
 
     raw_time = tmp['raw_time'][:]
     spec = tmp['spectrum_index'][:]
 
     tmp = tmp['counts']
-    inst = tmp.attrs['long_name']
+    inst = tmp.attrs['long_name'].decode()
     first_good = tmp.attrs['first_good_bin'] * resolution
     last_good = tmp.attrs['last_good_bin'] * resolution
     t0 = tmp.attrs['t0_bin']
     counts = tmp[:]
 
     # not used...
     # direction =  tmp['orientation'][0].decode()
```

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/muon_data.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/muon_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,7 +28,9 @@
         Method for saving the object to a muon
         nexus v2 histogram file
         :param file_name: the name of the file to save to
         """
         file = h5py.File(file_name, 'w')
         for key in self._dict.keys():
             self._dict[key].save_nxs2(file)
+        file.close()
+        return
```

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/periods.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/periods.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.save_int('number', self._dict['number'], tmp)
         self.save_int_array('sequences', self._dict['sequences'], tmp)
         self.save_str('labels', self._dict['labels'], tmp)
         self.save_int_array('type', self._dict['type'], tmp)
         self.save_int_array('frames_requested', self._dict['requested'], tmp)
         self.save_int_array('raw_frames', self._dict['raw'], tmp)
         self.save_int_array('output', self._dict['output'], tmp)
-        self.save_float_array('total_conts', self._dict['counts'], tmp)
+        self.save_float_array('total_counts', self._dict['counts'], tmp)
 
 
 def read_periods_from_histogram(file):
     """
     A method for reading the period information
     a nexus v2 histogram file
     :param file: the open file to read from
```

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/raw_data.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/raw_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,22 +52,25 @@
         self.save_int('good_frames', self._dict['good_frames'], tmp)
         self.save_int('IDF_version', self._dict['IDF'], tmp)
         self.save_str('definition', self._dict['def'], tmp)
         self.save_str('name', self._dict['inst'], tmp)
         self.save_str('title', self._dict['title'], tmp)
         self.save_str('notes', self._dict['notes'], tmp)
         self.save_int('run_number', self._dict['run_number'], tmp)
-        # duration not used for Wimda
+        self.save_float('duration', self._dict['duration'], tmp)
         self.save_int('raw_frames', self._dict['raw_frames'], tmp)
         self.save_str('start_time',
                       convert_date_for_NXS(self._dict['start']),
                       tmp)
         self.save_str('end_time', convert_date_for_NXS(self._dict['end']), tmp)
         self.save_str('experiment_identifier', self._dict['ID'], tmp)
 
+        tmp = tmp.require_group('instrument')
+        self.save_str('name', self._dict['inst'], tmp)
+
 
 def read_raw_data_from_histogram(file):
     """
     A function for reading the raw data information
     from a muon nexus v2 file
     :param file: the open file to read from
     :return: the RawData object
```

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/sample.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/sample.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/source.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/source.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,20 +23,14 @@
         Method to save the source information to a
         muon nexus v2 file
         :param file: the open file to write to
         """
         tmp = file.require_group('raw_data_1')
         tmp = tmp.require_group('instrument')
 
-        """
-        test - dont know if this is needed
-        if it is we should probably move it
-        self.save_str('name', 'HIFI', tmp)
-        """
-
         tmp = tmp.require_group('source')
         tmp.attrs['NX_class'] = 'NXsource'
         for key in self._dict.keys():
             self.save_str(key, self._dict[key], tmp)
 
 
 def read_source_from_histogram(file):
```

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/user.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/user.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/utils.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def convert_date(date):
 
     """
     Convert the muon nexus v2 file data string into a
     date object.
     Assume in the form f'{year} {month} {day}', time
-    :param date: the date in the above format
+    :param date: the date string in the above format
     :return: the date object
     """
 
     return datetime.datetime.strptime(date, '%Y-%m-%dT%H:%M:%S')
 
 
 def stype(string):
```

### Comparing `muondatalib-0.3.0b0/src/MuonDataLib/data/loader/load_nxs2.py` & `muondatalib-0.5.0b0/src/MuonDataLib/data/loader/load_nxs2.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/tools/conda_dict_to_yml.py` & `muondatalib-0.5.0b0/tools/conda_dict_to_yml.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/tools/create_conda_yml.py` & `muondatalib-0.5.0b0/tools/create_conda_yml.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
     default_yml['name'] = 'MuonDataLib-dev'
     default_yml['channels'] = 'conda-forge'
     default_yml['dependencies'] = {'python': '=' + version + '.*',
                                    'numpy': '',
                                    'pytest': '',
                                    'pre-commit': '>=2.15',
-                                   'Cython': '',
                                    'pip': pip_dict}
     return default_yml
 
 
 if __name__ == "__main__":
     try:
         version = get_input()
```

### Comparing `muondatalib-0.3.0b0/tools/setup_helper.py` & `muondatalib-0.5.0b0/tools/setup_helper.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.3.0b0/tools/version.py` & `muondatalib-0.5.0b0/tools/version.py`

 * *Files identical despite different names*


# Comparing `tmp/dcmqi-0.1.0.tar.gz` & `tmp/dcmqi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcmqi-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "dcmqi-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `dcmqi-0.1.0.tar` & `dcmqi-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.gitattributes
--rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1676 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.gitignore
--rw-r--r--   0        0        0     2591 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dcmqi-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 dcmqi-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 dcmqi-0.1.0/LICENSE
--rw-r--r--   0        0        0     2311 2022-11-09 12:37:21.000000 dcmqi-0.1.0/README.md
--rw-r--r--   0        0        0     1304 2022-11-09 12:37:21.000000 dcmqi-0.1.0/dcmqiUrls.cmake
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 dcmqi-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 dcmqi-0.1.0/docs/index.md
--rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 dcmqi-0.1.0/noxfile.py
--rw-r--r--   0        0        0     4549 2022-11-09 12:37:21.000000 dcmqi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 dcmqi-0.1.0/src/dcmqi/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 dcmqi-0.1.0/src/dcmqi/_version.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 dcmqi-0.1.0/src/dcmqi/_version.pyi
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dcmqi-0.1.0/src/dcmqi/py.typed
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 dcmqi-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 dcmqi-0.1.0/tests/test_executable.py
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 dcmqi-0.1.0/tests/test_package.py
--rw-r--r--   0        0        0     5441 2022-11-09 12:37:21.000000 dcmqi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.gitattributes
+-rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3296 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2591 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 dcmqi-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 dcmqi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2323 2022-11-09 12:37:21.000000 dcmqi-0.1.1/README.md
+-rw-r--r--   0        0        0     1304 2022-11-09 12:37:21.000000 dcmqi-0.1.1/dcmqiUrls.cmake
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 dcmqi-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 dcmqi-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 dcmqi-0.1.1/noxfile.py
+-rw-r--r--   0        0        0     4549 2022-11-09 12:37:21.000000 dcmqi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/_version.py
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/_version.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/py.typed
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 dcmqi-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 dcmqi-0.1.1/tests/test_executable.py
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 dcmqi-0.1.1/tests/test_package.py
+-rw-r--r--   0        0        0     5453 2022-11-09 12:37:21.000000 dcmqi-0.1.1/PKG-INFO
```

### Comparing `dcmqi-0.1.0/.github/CONTRIBUTING.md` & `dcmqi-0.1.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/.github/matchers/pylint.json` & `dcmqi-0.1.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/.github/workflows/cd.yml` & `dcmqi-0.1.1/.github/workflows/cd.yml`

 * *Files 14% similar despite different names*

```diff
@@ -76,31 +76,48 @@
       - uses: actions/download-artifact@v4
         with:
           path: all
 
       - run: pipx run twine check --strict all/*/*
 
   build_wheels:
-    name: Wheel on ${{ matrix.os }}
+    name: Wheel on ${{ matrix.os }} (${{ matrix.arch }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
+        arch: ["auto"]
+        include:
+          - os: ubuntu-latest
+            skip: "*musllinux*"
+            arch: "x86_64"
+
+          - os: windows-latest
+            arch: "ARM64"
+            test-skip: "*-win_arm64"
+
+          - os: macos-14
+            arch: "arm64"
+
+        exclude:
+          - os: ubuntu-latest
+            arch: "auto"
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_ARCHS_LINUX: "x86_64"
           CIBW_BUILD: "cp312-*"
-          CIBW_SKIP: "*musllinux*"
+          CIBW_ARCHS: "${{ matrix.arch }}"
+          CIBW_TEST_SKIP: "${{ matrix.test-skip }}"
+          CIBW_SKIP: ${{ matrix.skip }}
 
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: wheelhouse/*.whl
```

### Comparing `dcmqi-0.1.0/.github/workflows/ci.yml` & `dcmqi-0.1.1/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -43,14 +43,21 @@
         python-version: ["3.8", "3.12"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
           - python-version: pypy-3.10
             runs-on: ubuntu-latest
 
+          - python-version: "3.10"
+            runs-on: macos-latest
+
+        exclude:
+          - python-version: "3.8"
+            runs-on: macos-latest
+
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v5
         with:
@@ -65,7 +72,38 @@
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       # - name: Upload coverage report
       #   uses: codecov/codecov-action@v4.1.0
       #   with:
       #     token: ${{ secrets.CODECOV_TOKEN }}
+
+  checks-cibw:
+    name: >
+      Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
+      (${{matrix.arch }})
+    runs-on: ${{ matrix.runs-on }}
+    needs: [pre-commit]
+    strategy:
+      fail-fast: false
+      matrix:
+        include:
+          - runs-on: macos-14
+            python-version: cp312
+            arch: "arm64"
+
+          - runs-on: windows-latest
+            python-version: cp312
+            arch: "ARM64"
+            test-skip: "*-win_arm64"
+
+    steps:
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - uses: pypa/cibuildwheel@v2.16.5
+        env:
+          CIBW_BUILD: "${{ matrix.python-version }}-*"
+          CIBW_ARCHS: "${{ matrix.arch }}"
+          CIBW_TEST_SKIP: "${{ matrix.test-skip }}"
+          CIBW_SKIP: "*musllinux*"
```

### Comparing `dcmqi-0.1.0/.gitignore` & `dcmqi-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/.pre-commit-config.yaml` & `dcmqi-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/CMakeLists.txt` & `dcmqi-0.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/LICENSE` & `dcmqi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/README.md` & `dcmqi-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 created during installation by pip, leveraging the `[project.scripts]`
 configuration defined in the `pyproject.toml` file.
 
 ## Platforms
 
 The following platforms are supported by the binary wheels:
 
-| OS           | Arch             |
-| ------------ | ---------------- |
-| Windows      | 64-bit           |
-| Linux Intel  | manylinux 64-bit |
-| macOS 10.10+ | Intel            |
-| macOS 11+    | Apple Silicon    |
+| OS           | Arch               |
+| ------------ | ------------------ |
+| Windows      | 64-bit <br/> ARM64 |
+| Linux Intel  | manylinux 64-bit   |
+| macOS 10.10+ | Intel              |
+| macOS 11+    | Apple Silicon      |
 
 ## License
 
 This project is maintained by Leonard Nürnberg, Mass General Brigham. It is
 covered by the OSI-approved MIT License.
 
 `dcmqi` is distributed under the OSI-approved MIT License. For further details
```

### Comparing `dcmqi-0.1.0/dcmqiUrls.cmake` & `dcmqi-0.1.1/dcmqiUrls.cmake`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/docs/conf.py` & `dcmqi-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/noxfile.py` & `dcmqi-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/pyproject.toml` & `dcmqi-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/src/dcmqi/__init__.py` & `dcmqi-0.1.1/src/dcmqi/__init__.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/tests/test_executable.py` & `dcmqi-0.1.1/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.0/PKG-INFO` & `dcmqi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcmqi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python distribution of the DCMQI library collection.
 Author-Email: =?utf-8?q?Leonard_N=C3=BCrnberg?= <lnuernberg@bwh.harvard.edu>
 License: Copyright 2024 Leonard Nürnberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -88,20 +88,20 @@
 created during installation by pip, leveraging the `[project.scripts]`
 configuration defined in the `pyproject.toml` file.
 
 ## Platforms
 
 The following platforms are supported by the binary wheels:
 
-| OS           | Arch             |
-| ------------ | ---------------- |
-| Windows      | 64-bit           |
-| Linux Intel  | manylinux 64-bit |
-| macOS 10.10+ | Intel            |
-| macOS 11+    | Apple Silicon    |
+| OS           | Arch               |
+| ------------ | ------------------ |
+| Windows      | 64-bit <br/> ARM64 |
+| Linux Intel  | manylinux 64-bit   |
+| macOS 10.10+ | Intel              |
+| macOS 11+    | Apple Silicon      |
 
 ## License
 
 This project is maintained by Leonard Nürnberg, Mass General Brigham. It is
 covered by the OSI-approved MIT License.
 
 `dcmqi` is distributed under the OSI-approved MIT License. For further details
```


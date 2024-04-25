# Comparing `tmp/bitwarden_import_msecure-1.4.1.tar.gz` & `tmp/bitwarden_import_msecure-1.5.0.tar.gz`

## Comparing `bitwarden_import_msecure-1.4.1.tar` & `bitwarden_import_msecure-1.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.mypy.ini
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.pylintrc
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/Makefile
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/activate.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/pytest.ini
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/requirements.dev.in
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/requirements.dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/requirements.in
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/requirements.txt
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.github/workflows/static.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/docs/mkdocs.yml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/docs/src/en/index.md
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/docs/src/ru/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/__init__.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/build.sh
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/compile_requirements.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/upload.sh
--rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/scripts/verup.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/__about__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/bitwarden_csv.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/bitwarden_json.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/main.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/msecure.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/test_bitwarden_import_msecure.py
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/test_e2e.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_export.csv
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_export.json
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_notes_export.csv
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_notes_export.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/tests/resources/mSecure Export File.csv
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.mypy.ini
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.pylintrc
+-rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/pytest.ini
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.dev.in
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.in
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/requirements.txt
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tasks.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/docs/src/en/index.md
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2525 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/scripts/verup.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/__about__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_csv.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_json.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/main.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/msecure.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/test_bitwarden_import_msecure.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/test_e2e.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.csv
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.json
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.csv
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/tests/resources/mSecure Export File.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/README.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 bitwarden_import_msecure-1.5.0/PKG-INFO
```

### Comparing `bitwarden_import_msecure-1.4.1/.pre-commit-config.yaml` & `bitwarden_import_msecure-1.5.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 exclude: |
     (?x)(
         tests/|
         site/|
         docs/|
         pyproject.toml|
+        tasks.py|
         __about__.py
     )
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.3.4
+    rev: v0.3.5
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
 
@@ -27,15 +28,17 @@
           --install-types
           --non-interactive
           --strict
           --implicit-reexport
           --warn-unused-ignores
           --cache-fine-grained
           --no-namespace-packages
+        exclude: tasks.py
         files: \.py$
         language: python
 
       - id: pylint
         name: Pylint
         entry: pylint --max-line-length=99 --ignore-imports=yes
         files: \.py$
+        exclude: tasks.py
         language: python
```

### Comparing `bitwarden_import_msecure-1.4.1/activate.sh` & `bitwarden_import_msecure-1.5.0/activate.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/requirements.dev.txt` & `bitwarden_import_msecure-1.5.0/requirements.dev.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile requirements.dev.in --output-file=requirements.dev.txt
 -e .
+allure-pytest==2.13.5
+allure-python-commons==2.13.5
+    # via allure-pytest
 astroid==3.0.2
     # via pylint
+attrs==23.2.0
+    # via allure-python-commons
 babel==2.14.0
     # via mkdocs-material
 bracex==2.4
     # via wcmatch
 certifi==2023.11.17
     # via requests
 cfgv==3.4.0
@@ -35,14 +40,15 @@
 hatchling==1.20.0
 identify==2.5.33
     # via pre-commit
 idna==3.6
     # via requests
 iniconfig==2.0.0
     # via pytest
+invoke==2.2.0
 isort==5.13.2
     # via pylint
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
 markdown==3.5.1
@@ -91,27 +97,30 @@
 platformdirs==4.1.0
     # via
     #   mkdocs
     #   pylint
     #   virtualenv
 pluggy==1.3.0
     # via
+    #   allure-python-commons
     #   hatchling
     #   pytest
 pre-commit==3.6.0
 pydocstyle==6.3.0
 pygments==2.17.2
     # via
     #   mkdocs-material
     #   rich
 pylint==3.0.3
 pymdown-extensions==10.5
     # via mkdocs-material
 pytest==7.4.3
-    # via pytest-cov
+    # via
+    #   allure-pytest
+    #   pytest-cov
 pytest-cov==4.1.0
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0.1
     # via
     #   mkdocs
     #   pre-commit
```

### Comparing `bitwarden_import_msecure-1.4.1/.github/workflows/ci.yml` & `bitwarden_import_msecure-1.5.0/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 #
 name: CI
 
+env:
+  PRIMARY_PYTHON_VERSION: '3.12'
+  PRIMARY_PLATFORM: 'ubuntu-latest'
+  PYTEST_CMD: >-
+    python -m pytest 
+    --junitxml=pytest.xml 
+    --cov-report=term-missing:skip-covered 
+    --cov=src
+    tests/
+
 on:
   push:
     branches: [ master, main ]
   pull_request:
     branches: [ master, main ]
 
+permissions:
+  pull-requests: write
+  contents: write
+
 jobs:
-  build:
+  # Test compatibility with the matrix of Python versions and platforms
+  matrix-build:
     strategy:
       matrix:
-        python-version: [3.9, "3.10", 3.11, 3.12]
+        python-version: ["3.10", 3.11, 3.12]
         platform: [ubuntu-latest, macos-latest, windows-latest]
-    env:
-      PRIMARY_PYTHON_VERSION: '3.12'
-      PRIMARY_PLATFORM: 'ubuntu-latest'
-      PYTEST_CMD: >
-        python -m pytest 
-        --junitxml=pytest.xml 
-        --cov-report=term-missing:skip-covered 
-        --cov=src 
-        tests/
     runs-on: ${{ matrix.platform }}
-    permissions:
-      # Gives the action the necessary permissions for publishing new
-      # comments in pull requests.
-      pull-requests: write
-      # Gives the action the necessary permissions for pushing data to the
-      # python-coverage-comment-action branch, and for editing existing
-      # comments (to avoid publishing multiple comments in the same PR)
-      contents: write
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
@@ -47,31 +45,71 @@
       uses: andgineer/uv-venv@v1
     - name: Install dependencies
       run: uv pip install -r requirements.dev.txt
 
     - name: Test with pytest
       run: ${{ env.PYTEST_CMD }}
 
+# Build with publishing Allure report, coverage report
+  primary-build:
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v4
+
+    - name: Set up Python ${{ env.PRIMARY_PYTHON_VERSION }}
+      uses: actions/setup-python@v5
+      with:
+        python-version: ${{ env.PRIMARY_PYTHON_VERSION }}
+
+    - name: Install uv environment
+      uses: andgineer/uv-venv@v1
+    - name: Install dependencies
+      run: uv pip install -r requirements.dev.txt
+    - name: Test with pytest and Allure report
+      run: "${{ env.PYTEST_CMD }} --alluredir=./allure-results"
+
+    - name: Load Allure test report history
+      uses: actions/checkout@v4
+      if: always()
+      with:
+        ref: gh-pages
+        path: gh-pages-dir
+
+    - name: Generate Allure test report
+      uses: andgineer/allure-report@v3
+      id: allure-report
+      if: always()
+      with:
+        allure-results: allure-results
+        website: gh-pages-dir
+        reports-site-path: builds/tests
+
+    - name: Publish Allure test report
+      uses: peaceiris/actions-gh-pages@v3
+      if: ${{ always() && (steps.allure-report.outcome == 'success') }}
+      with:
+        github_token: ${{ secrets.GITHUB_TOKEN }}
+        publish_branch: gh-pages
+        publish_dir: ${{ steps.allure-report.outputs.reports-site }}
+        destination_dir: ${{ steps.allure-report.outputs.reports-site-path }}
+
     - name: Coverage comment
       id: coverage_comment
-      if: ${{ matrix.python-version == env.PRIMARY_PYTHON_VERSION && matrix.platform == env.PRIMARY_PLATFORM }}
+      if: always()
       uses: py-cov-action/python-coverage-comment-action@v3
       with:
         GITHUB_TOKEN: ${{ github.token }}
         MINIMUM_GREEN: 85
         MINIMUM_ORANGE: 70
 
     - name: Store Pull Request comment to be posted
       uses: actions/upload-artifact@v3
       if: steps.coverage_comment.outputs.COMMENT_FILE_WRITTEN == 'true'
       with:
         name: python-coverage-comment-action
         path: python-coverage-comment-action.txt
 
     - name: Upload coverage data to coveralls.io
-      if: ${{ matrix.python-version == env.PRIMARY_PYTHON_VERSION && matrix.platform == env.PRIMARY_PLATFORM }}
+      if: always()
       uses: coverallsapp/github-action@v2
 
-    - name: Upload Coverage to Codecov
-      if: ${{ matrix.python-version == env.PRIMARY_PYTHON_VERSION && matrix.platform == env.PRIMARY_PLATFORM }}
-      uses: codecov/codecov-action@v3
-
```

### Comparing `bitwarden_import_msecure-1.4.1/.github/workflows/docs.yml` & `bitwarden_import_msecure-1.5.0/.github/workflows/static.yml`

 * *Files 15% similar despite different names*

```diff
@@ -3,33 +3,27 @@
 # publish them as github pages
 #
 #note for myself
 #
 # Do not forget to set git branch `gh-pages` as source for github pages.
 # This branch auto-updated by `mkdocs gh-deploy`
 #
-name: docs
+name: static source code checks
 on:
   push:
     branches:
       - main
       - master
-
-permissions:
-  contents: write
-
 jobs:
   deploy:
     env:
       PRIMARY_PYTHON_VERSION: '3.12'
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PRIMARY_PYTHON_VERSION  }}
+      - uses: andgineer/uv-venv@v1
       - run: |
-          pip install uv
-          uv pip install ghp-import -r requirements.dev.txt --python=${{ env.PRIMARY_PYTHON_VERSION }}
-      - run: ./scripts/build-docs.sh
-      - run: |
-          ghp-import --no-jekyll --push --force site
+          uv pip install pip -r requirements.dev.txt
+          pre-commit run --verbose --all-files
```

### Comparing `bitwarden_import_msecure-1.4.1/.github/workflows/pip_publish.yml` & `bitwarden_import_msecure-1.5.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/docs/mkdocs.yml` & `bitwarden_import_msecure-1.5.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/docs/src/en/index.md` & `bitwarden_import_msecure-1.5.0/docs/src/en/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Instead, it organizes secrets into meaningful folders and offers several options to customize the import process.
 
 Additionally, this simple Python script can be easily modified to meet your specific needs.
 
 ## Installation
 
 ### Installing pipx
+
 [`pipx`](https://pypa.github.io/pipx/) creates isolated environments to avoid conflicts with existing system packages.
 
 === "MacOS"
     In the terminal, execute:
     ```bash
     brew install pipx
     pipx ensurepath
@@ -33,14 +34,15 @@
 
     In the command prompt, type (if Python was installed from the Microsoft Store, use `python3` instead of `python`):
     ```bash
     python -m pip install --user pipx
     ```
 
 ### Installing `bitwarden-import-msecure`:
+
 In the terminal (command prompt), execute:
 
 ```bash
 pipx install bitwarden-import-msecure
 ```
 
 ## Usage
```

### Comparing `bitwarden_import_msecure-1.4.1/docs/src/ru/index.md` & `bitwarden_import_msecure-1.5.0/docs/src/ru/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Вместо этого он организует секреты в папки по смыслу и предлагает несколько опций для настройки процесса импорта.
 
 Кроме того, этот простой скрипт на Python может быть легко изменен для удовлетворения ваших конкретных потребностей.
 
 ## Установка
 
 ## Установка pipx
+
 [`pipx`](https://pypa.github.io/pipx/) создает изолированные среды, чтобы избежать конфликтов с 
 существующими системными пакетами.
 
 === "MacOS"
     В терминале выполните:
 
     ```bash
```

### Comparing `bitwarden_import_msecure-1.4.1/scripts/include_pyproject_requirements.py` & `bitwarden_import_msecure-1.5.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/scripts/verup.sh` & `bitwarden_import_msecure-1.5.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/bitwarden_csv.py` & `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_csv.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/bitwarden_json.py` & `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/bitwarden_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,26 +64,31 @@
             "notes": data["notes"],
             "favorite": False,
             "collectionIds": None,
         }
         if data["type"] == "login":
             item["login"] = {
                 "fido2Credentials": [],
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": data["login_uri"],
+                    }
+                ],
                 "username": data["login_username"],
                 "password": data["login_password"],
                 "totp": None,
             }
         if data["type"] == "card":
             exp_month, exp_year = (
                 data["fields"].pop("Expiration Date", "").split("/") + ["", ""]
             )[:2]
-            cardholder_name = data["fields"].pop("Name on Card", "")
-            if not cardholder_name:
-                cardholder_name = data["fields"].pop("Name", "")
+            cardholder_name = data["fields"].pop("Name on Card", "") or data["fields"].pop(
+                "Name", ""
+            )
             item["card"] = {
                 "cardholderName": cardholder_name,
                 "brand": "",
                 "number": data["login_username"],
                 "expMonth": exp_month,
                 "expYear": exp_year,
                 "code": data["login_password"],
```

### Comparing `bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/main.py` & `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/main.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/src/bitwarden_import_msecure/msecure.py` & `bitwarden_import_msecure-1.5.0/src/bitwarden_import_msecure/msecure.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import rich_click as click
 
 
 BANK_FOLDER = "bank"
 
 
 def import_msecure_row(row: List[str], extra_fields_to_notes: bool) -> Dict[str, Any]:
-    """Extract data from mSecure row."""
+    """Extract data from mSecure CSV row."""
     name = row[0].split("|")[0]
     if len(row[0].split("|")) > 2:
         print(f"Warning: name has more than one '|' character :`{row[0]}`.")
     record_type = "login"
     if row[1].strip() not in ["Login", "Credit Card", "Email Account"]:
         print(f"Warning: record type is not 'Login' :`{row[1]}`.")
     tag = row[2].strip()
```

### Comparing `bitwarden_import_msecure-1.4.1/tests/conftest.py` & `bitwarden_import_msecure-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/tests/test_e2e.py` & `bitwarden_import_msecure-1.5.0/tests/test_e2e.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from click.testing import CliRunner
 
 from bitwarden_import_msecure.main import bitwarden_import_msecure
 
 
+UPDATE_EXPECTED_OUTPUT = False  # (!) Regenerate expected output files, but be sure to check the changes
+
+
 def assert_files_context_is_equal(file_path1, file_path2):
     """Compare the content of two files, abstracting away platform differences in newline characters."""
     with open(file_path1, 'r', newline=None, encoding='utf-8') as f1, open(file_path2, 'r', newline=None,
                                                                            encoding='utf-8') as f2:
         lines1 = f1.readlines()
         lines2 = f2.readlines()
 
@@ -21,29 +24,31 @@
 
     runner = CliRunner()
     result = runner.invoke(bitwarden_import_msecure, [str(input_file)])
     assert result.exit_code == 0
 
     output_file = tmpdir.join("bitwarden.json")
 
-    # bitwarden_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
+    if UPDATE_EXPECTED_OUTPUT:
+        bitwarden_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
     assert_files_context_is_equal(output_file, bitwarden_file)
 
 
 def test_bitwarden_import_msecure_note_mode_default_output(tmpdir, msecure_export, bitwarden_notes_file):
     input_file = tmpdir.join("input.csv")
     input_file.write(msecure_export)
 
     runner = CliRunner()
     result = runner.invoke(bitwarden_import_msecure, [str(input_file), "--extra-fields", "notes"])
     assert result.exit_code == 0
 
     output_file = tmpdir.join("bitwarden.json")
 
-    # bitwarden_notes_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
+    if UPDATE_EXPECTED_OUTPUT:
+        bitwarden_notes_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
     assert_files_context_is_equal(output_file, bitwarden_notes_file)
 
 
 def test_bitwarden_import_msecure_existing_output_file(tmpdir, msecure_export, bitwarden_file):
     input_file = tmpdir.join("input.txt")
     input_file.write(msecure_export)
 
@@ -66,38 +71,41 @@
     output_file = tmpdir.join("output.txt")
     output_file.write("existing data")
 
     runner = CliRunner()
     result = runner.invoke(bitwarden_import_msecure, [str(input_file), str(output_file), "--force"])
     assert result.exit_code == 0
 
-    # bitwarden_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
+    if UPDATE_EXPECTED_OUTPUT:
+        bitwarden_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
     assert_files_context_is_equal(output_file, bitwarden_file)
     assert input_file.read() == msecure_export  # Ensure input file remains unchanged
 
 
 def test_bitwarden_import_msecure_default_csv_output(tmpdir, msecure_export, bitwarden_csv_file):
     input_file = tmpdir.join("input.csv")
     input_file.write(msecure_export)
 
     runner = CliRunner()
     result = runner.invoke(bitwarden_import_msecure, [str(input_file), "--format", "csv"])
     assert result.exit_code == 0
 
     output_file = tmpdir.join("bitwarden.csv")
 
-    # bitwarden_csv_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
+    if UPDATE_EXPECTED_OUTPUT:
+        bitwarden_csv_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
     assert_files_context_is_equal(output_file, bitwarden_csv_file)
 
 
 def test_bitwarden_import_msecure_note_mode_default_csv_output(tmpdir, msecure_export, bitwarden_notes_csv_file):
     input_file = tmpdir.join("input.csv")
     input_file.write(msecure_export)
 
     runner = CliRunner()
     result = runner.invoke(bitwarden_import_msecure, [str(input_file), "--extra-fields", "notes", "--format", "csv"])
     assert result.exit_code == 0
 
     output_file = tmpdir.join("bitwarden.csv")
 
-    # bitwarden_notes_csv_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
+    if UPDATE_EXPECTED_OUTPUT:
+        bitwarden_notes_csv_file.write_text(output_file.read_text(encoding="utf8"))  # uncomment to refresh the expected output
     assert_files_context_is_equal(output_file, bitwarden_notes_csv_file)
```

### Comparing `bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_export.csv` & `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_export.json` & `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981666666666666%*

 * *Differences: {"'items'": "{0: {'login': {'uris': [OrderedDict([('match', 'null'), ('uri', "*

 * *            "'https://www.openstreetmap.org')])]}}, 1: {'login': {'uris': [OrderedDict([('match', "*

 * *            "'null'), ('uri', 'vk.com')])]}}, 2: {'login': {'uris': [OrderedDict([('match', "*

 * *            "'null'), ('uri', 'https://airtable.com/')])]}}, 3: {'notes': '+1 555 555 "*

 * *            '5555\\n11111, London, Baker Street 221B.\\nExpiration Date: 12/2099\\nName on Card: '*

 * *            "Sherlock Holmes', 'card': {'cardholderN […]*

```diff
@@ -15,15 +15,20 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "https://www.openstreetmap.org"
+                    }
+                ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": " OpenStreetMap",
             "notes": "",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
@@ -38,15 +43,20 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "vk.com"
+                    }
+                ],
                 "username": "+1 555 555 5555"
             },
             "name": " VK",
             "notes": "",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
@@ -61,32 +71,37 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "https://airtable.com/"
+                    }
+                ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": "(deleted) airtable sheets",
             "notes": "",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
             "revisionDate": "2024-03-29T09:49:23.836557+01:00",
             "type": 1
         },
         {
             "card": {
                 "brand": "",
-                "cardholderName": "Sherlock Holmes",
+                "cardholderName": "",
                 "code": "123",
-                "expMonth": "12",
-                "expYear": "2099",
+                "expMonth": "",
+                "expYear": "",
                 "number": "1234 5678 9012 3456"
             },
             "collectionIds": null,
             "creationDate": "2024-03-29T09:49:23.836557+01:00",
             "deletedDate": null,
             "favorite": false,
             "fields": [
@@ -96,15 +111,15 @@
                     "type": 1,
                     "value": "1234"
                 }
             ],
             "folderId": "12345678-1234-5678-1234-567812345678",
             "id": "12345678-1234-5678-1234-567812345678",
             "name": "My VISA",
-            "notes": "+1 555 555 5555\n11111, London, Baker Street 221B.",
+            "notes": "+1 555 555 5555\n11111, London, Baker Street 221B.\nExpiration Date: 12/2099\nName on Card: Sherlock Holmes",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
             "revisionDate": "2024-03-29T09:49:23.836557+01:00",
             "type": 3
         },
         {
@@ -115,15 +130,20 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "hub.docker.com"
+                    }
+                ],
                 "username": "sorokin.engineer"
             },
             "name": "Docker hub",
             "notes": "andrey@sorokin.engineer\nBefore 20190429 my-cool-password",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
```

### Comparing `bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_notes_export.csv` & `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_notes_export.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/tests/resources/bitwarden_notes_export.json` & `bitwarden_import_msecure-1.5.0/tests/resources/bitwarden_export.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981666666666666%*

 * *Differences: {"'items'": "{0: {'login': {'uris': [OrderedDict([('match', 'null'), ('uri', "*

 * *            "'https://www.openstreetmap.org')])]}}, 1: {'login': {'uris': [OrderedDict([('match', "*

 * *            "'null'), ('uri', 'vk.com')])]}}, 2: {'login': {'uris': [OrderedDict([('match', "*

 * *            "'null'), ('uri', 'https://airtable.com/')])]}}, 3: {'notes': '+1 555 555 "*

 * *            "5555\\n11111, London, Baker Street 221B.', 'card': {'cardholderName': 'Sherlock "*

 * *            "Holmes', 'expMonth': '12', 'expYear': '2099 […]*

```diff
@@ -15,15 +15,20 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "https://www.openstreetmap.org"
+                    }
+                ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": " OpenStreetMap",
             "notes": "",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
@@ -38,15 +43,20 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "vk.com"
+                    }
+                ],
                 "username": "+1 555 555 5555"
             },
             "name": " VK",
             "notes": "",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
@@ -61,32 +71,37 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "https://airtable.com/"
+                    }
+                ],
                 "username": "andrey@sorokin.engineer"
             },
             "name": "(deleted) airtable sheets",
             "notes": "",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
             "revisionDate": "2024-03-29T09:49:23.836557+01:00",
             "type": 1
         },
         {
             "card": {
                 "brand": "",
-                "cardholderName": "",
+                "cardholderName": "Sherlock Holmes",
                 "code": "123",
-                "expMonth": "",
-                "expYear": "",
+                "expMonth": "12",
+                "expYear": "2099",
                 "number": "1234 5678 9012 3456"
             },
             "collectionIds": null,
             "creationDate": "2024-03-29T09:49:23.836557+01:00",
             "deletedDate": null,
             "favorite": false,
             "fields": [
@@ -96,15 +111,15 @@
                     "type": 1,
                     "value": "1234"
                 }
             ],
             "folderId": "12345678-1234-5678-1234-567812345678",
             "id": "12345678-1234-5678-1234-567812345678",
             "name": "My VISA",
-            "notes": "+1 555 555 5555\n11111, London, Baker Street 221B.\nExpiration Date: 12/2099\nName on Card: Sherlock Holmes",
+            "notes": "+1 555 555 5555\n11111, London, Baker Street 221B.",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
             "revisionDate": "2024-03-29T09:49:23.836557+01:00",
             "type": 3
         },
         {
@@ -115,15 +130,20 @@
             "fields": [],
             "folderId": null,
             "id": "12345678-1234-5678-1234-567812345678",
             "login": {
                 "fido2Credentials": [],
                 "password": "my-cool-password",
                 "totp": null,
-                "uris": [],
+                "uris": [
+                    {
+                        "match": "null",
+                        "uri": "hub.docker.com"
+                    }
+                ],
                 "username": "sorokin.engineer"
             },
             "name": "Docker hub",
             "notes": "andrey@sorokin.engineer\nBefore 20190429 my-cool-password",
             "organizationId": null,
             "passwordHistory": null,
             "reprompt": 0,
```

### Comparing `bitwarden_import_msecure-1.4.1/tests/resources/mSecure Export File.csv` & `bitwarden_import_msecure-1.5.0/tests/resources/mSecure Export File.csv`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/LICENSE.txt` & `bitwarden_import_msecure-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/pyproject.toml` & `bitwarden_import_msecure-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitwarden_import_msecure-1.4.1/PKG-INFO` & `bitwarden_import_msecure-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 6269 7477  : 2.3.Name: bitw
 00000020: 6172 6465 6e2d 696d 706f 7274 2d6d 7365  arden-import-mse
 00000030: 6375 7265 0a56 6572 7369 6f6e 3a20 312e  cure.Version: 1.
-00000040: 342e 310a 5375 6d6d 6172 793a 204d 6967  4.1.Summary: Mig
+00000040: 352e 300a 5375 6d6d 6172 793a 204d 6967  5.0.Summary: Mig
 00000050: 7261 7469 6f6e 2066 726f 6d20 6d53 6563  ration from mSec
 00000060: 7572 6520 746f 2042 6974 7761 7264 656e  ure to Bitwarden
 00000070: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
 00000080: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
 00000090: 616e 6467 696e 6565 722e 6769 7468 7562  andgineer.github
 000000a0: 2e69 6f2f 6269 7477 6172 6465 6e2d 696d  .io/bitwarden-im
 000000b0: 706f 7274 2d6d 7365 6375 7265 2f0a 5072  port-msecure/.Pr
@@ -145,39 +145,58 @@
 00000900: 7079 7468 6f6e 2d63 6f76 6572 6167 652d  python-coverage-
 00000910: 636f 6d6d 656e 742d 6163 7469 6f6e 2d64  comment-action-d
 00000920: 6174 612f 6874 6d6c 636f 762f 696e 6465  ata/htmlcov/inde
 00000930: 782e 6874 6d6c 290a 2320 6269 7477 6172  x.html).# bitwar
 00000940: 6465 6e2d 696d 706f 7274 2d6d 7365 6375  den-import-msecu
 00000950: 7265 0a0a 4d69 6772 6174 696f 6e20 6672  re..Migration fr
 00000960: 6f6d 206d 5365 6375 7265 2074 6f20 4269  om mSecure to Bi
-00000970: 7477 6172 6465 6e20 0a0a 2320 446f 6375  twarden ..# Docu
-00000980: 6d65 6e74 6174 696f 6e0a 0a5b 4269 7477  mentation..[Bitw
-00000990: 6172 6465 6e20 496d 706f 7274 206d 5365  arden Import mSe
-000009a0: 6375 7265 5d28 6874 7470 733a 2f2f 616e  cure](https://an
-000009b0: 6467 696e 6565 722e 6769 7468 7562 2e69  dgineer.github.i
-000009c0: 6f2f 6269 7477 6172 6465 6e2d 696d 706f  o/bitwarden-impo
-000009d0: 7274 2d6d 7365 6375 7265 2f29 0a0a 2320  rt-msecure/)..# 
-000009e0: 4465 7665 6c6f 7065 7273 0a0a 446f 206e  Developers..Do n
-000009f0: 6f74 2066 6f72 6765 7420 746f 2072 756e  ot forget to run
-00000a00: 2060 2e20 2e2f 6163 7469 7661 7465 2e73   `. ./activate.s
-00000a10: 6860 2e0a 0a23 2053 6372 6970 7473 0a20  h`...# Scripts. 
-00000a20: 2020 206d 616b 6520 6865 6c70 0a0a 2323     make help..##
-00000a30: 2043 6f76 6572 6167 6520 7265 706f 7274   Coverage report
-00000a40: 0a2a 205b 436f 6465 636f 765d 2868 7474  .* [Codecov](htt
-00000a50: 7073 3a2f 2f61 7070 2e63 6f64 6563 6f76  ps://app.codecov
-00000a60: 2e69 6f2f 6768 2f61 6e64 6769 6e65 6572  .io/gh/andgineer
-00000a70: 2f62 6974 7761 7264 656e 2d69 6d70 6f72  /bitwarden-impor
-00000a80: 742d 6d73 6563 7572 652f 7472 6565 2f6d  t-msecure/tree/m
-00000a90: 6169 6e2f 7372 6325 3246 6269 7477 6172  ain/src%2Fbitwar
-00000aa0: 6465 6e5f 696d 706f 7274 5f6d 7365 6375  den_import_msecu
-00000ab0: 7265 290a 2a20 5b43 6f76 6572 616c 6c73  re).* [Coveralls
-00000ac0: 5d28 6874 7470 733a 2f2f 636f 7665 7261  ](https://covera
-00000ad0: 6c6c 732e 696f 2f67 6974 6875 622f 616e  lls.io/github/an
-00000ae0: 6467 696e 6565 722f 6269 7477 6172 6465  dgineer/bitwarde
-00000af0: 6e2d 696d 706f 7274 2d6d 7365 6375 7265  n-import-msecure
-00000b00: 290a 0a3e 2043 7265 6174 6564 2077 6974  )..> Created wit
-00000b10: 6820 636f 6f6b 6965 6375 7474 6572 2075  h cookiecutter u
-00000b20: 7369 6e67 205b 7465 6d70 6c61 7465 5d28  sing [template](
-00000b30: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000b40: 6f6d 2f61 6e64 6769 6e65 6572 2f63 6f6f  om/andgineer/coo
-00000b50: 6b69 6563 7574 7465 722d 7079 7468 6f6e  kiecutter-python
-00000b60: 2d70 6163 6b61 6765 29                   -package)
+00000970: 7477 6172 6465 6e2e 0a0a 4d6f 7265 2066  twarden...More f
+00000980: 6c65 7869 626c 6520 7468 616e 2074 6865  lexible than the
+00000990: 2062 7569 6c74 2d69 6e20 4269 7477 6172   built-in Bitwar
+000009a0: 6465 6e20 696d 706f 7274 2074 6f6f 6c2e  den import tool.
+000009b0: 0a0a 2320 446f 6375 6d65 6e74 6174 696f  ..# Documentatio
+000009c0: 6e0a 0a5b 4269 7477 6172 6465 6e20 496d  n..[Bitwarden Im
+000009d0: 706f 7274 206d 5365 6375 7265 5d28 6874  port mSecure](ht
+000009e0: 7470 733a 2f2f 616e 6467 696e 6565 722e  tps://andgineer.
+000009f0: 6769 7468 7562 2e69 6f2f 6269 7477 6172  github.io/bitwar
+00000a00: 6465 6e2d 696d 706f 7274 2d6d 7365 6375  den-import-msecu
+00000a10: 7265 2f29 0a0a 2320 4465 7665 6c6f 7065  re/)..# Develope
+00000a20: 7273 0a0a 446f 206e 6f74 2066 6f72 6765  rs..Do not forge
+00000a30: 7420 746f 2072 756e 2060 2e20 2e2f 6163  t to run `. ./ac
+00000a40: 7469 7661 7465 2e73 6860 2e0a 0a23 2053  tivate.sh`...# S
+00000a50: 6372 6970 7473 0a49 6e73 7461 6c6c 205b  cripts.Install [
+00000a60: 696e 766f 6b65 5d28 6874 7470 733a 2f2f  invoke](https://
+00000a70: 646f 6373 2e70 7969 6e76 6f6b 652e 6f72  docs.pyinvoke.or
+00000a80: 672f 656e 2f73 7461 626c 652f 2920 7072  g/en/stable/) pr
+00000a90: 6566 6572 6162 6c79 2077 6974 6820 5b70  eferably with [p
+00000aa0: 6970 785d 2868 7474 7073 3a2f 2f70 7970  ipx](https://pyp
+00000ab0: 612e 6769 7468 7562 2e69 6f2f 7069 7078  a.github.io/pipx
+00000ac0: 2f29 3a0a 0a20 2020 2070 6970 7820 696e  /):..    pipx in
+00000ad0: 7374 616c 6c20 696e 766f 6b65 0a0a 466f  stall invoke..Fo
+00000ae0: 7220 6120 6c69 7374 206f 6620 6176 6169  r a list of avai
+00000af0: 6c61 626c 6520 7363 7269 7074 7320 7275  lable scripts ru
+00000b00: 6e3a 0a0a 2020 2020 696e 766f 6b65 202d  n:..    invoke -
+00000b10: 2d6c 6973 740a 0a46 6f72 206d 6f72 6520  -list..For more 
+00000b20: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00000b30: 7420 6120 7363 7269 7074 2072 756e 3a0a  t a script run:.
+00000b40: 0a20 2020 2069 6e76 6f6b 6520 3c73 6372  .    invoke <scr
+00000b50: 6970 743e 202d 2d68 656c 700a 0a23 2320  ipt> --help..## 
+00000b60: 416c 6c75 7265 2074 6573 7420 7265 706f  Allure test repo
+00000b70: 7274 0a0a 2a20 5b41 6c6c 7572 6520 7265  rt..* [Allure re
+00000b80: 706f 7274 5d28 6874 7470 733a 2f2f 616e  port](https://an
+00000b90: 6467 696e 6565 722e 6769 7468 7562 2e69  dgineer.github.i
+00000ba0: 6f2f 6269 7477 6172 6465 6e2d 696d 706f  o/bitwarden-impo
+00000bb0: 7274 2d6d 7365 6375 7265 2f62 7569 6c64  rt-msecure/build
+00000bc0: 732f 7465 7374 732f 290a 0a23 2320 436f  s/tests/)..## Co
+00000bd0: 7665 7261 6765 2072 6570 6f72 740a 2a20  verage report.* 
+00000be0: 5b43 6f76 6572 616c 6c73 5d28 6874 7470  [Coveralls](http
+00000bf0: 733a 2f2f 636f 7665 7261 6c6c 732e 696f  s://coveralls.io
+00000c00: 2f67 6974 6875 622f 616e 6467 696e 6565  /github/andginee
+00000c10: 722f 6269 7477 6172 6465 6e2d 696d 706f  r/bitwarden-impo
+00000c20: 7274 2d6d 7365 6375 7265 290a 0a3e 2043  rt-msecure)..> C
+00000c30: 7265 6174 6564 2077 6974 6820 636f 6f6b  reated with cook
+00000c40: 6965 6375 7474 6572 2075 7369 6e67 205b  iecutter using [
+00000c50: 7465 6d70 6c61 7465 5d28 6874 7470 733a  template](https:
+00000c60: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6e64  //github.com/and
+00000c70: 6769 6e65 6572 2f63 6f6f 6b69 6563 7574  gineer/cookiecut
+00000c80: 7465 722d 7079 7468 6f6e 2d70 6163 6b61  ter-python-packa
+00000c90: 6765 29                                  ge)
```


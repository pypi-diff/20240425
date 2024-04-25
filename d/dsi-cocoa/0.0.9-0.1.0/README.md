# Comparing `tmp/dsi-cocoa-0.0.9.tar.gz` & `tmp/dsi_cocoa-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi-cocoa-0.0.9.tar", last modified: Tue Dec 12 20:57:04 2023, max compression
+gzip compressed data, was "dsi_cocoa-0.1.0.tar", last modified: Thu Apr 25 18:53:21 2024, max compression
```

## Comparing `dsi-cocoa-0.0.9.tar` & `dsi_cocoa-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 20:57:04.198476 dsi-cocoa-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 20:57:04.194476 dsi-cocoa-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 20:57:04.198476 dsi-cocoa-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-12 20:57:04.198476 dsi-cocoa-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-12 20:57:04.198476 dsi-cocoa-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 20:57:04.194476 dsi-cocoa-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 20:57:04.198476 dsi-cocoa-0.0.9/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/src/cocoa/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-12 20:56:56.000000 dsi-cocoa-0.0.9/src/cocoa/notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 20:57:04.198476 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-12 20:57:04.000000 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-12 20:57:04.000000 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 20:57:04.000000 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-12 20:57:04.000000 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-12 20:57:04.000000 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-12 20:57:04.000000 dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:21.971950 dsi_cocoa-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:21.967949 dsi_cocoa-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:21.967949 dsi_cocoa-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-25 18:53:21.971950 dsi_cocoa-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-25 18:53:21.971950 dsi_cocoa-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:21.967949 dsi_cocoa-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:21.971950 dsi_cocoa-0.1.0/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 18:53:17.000000 dsi_cocoa-0.1.0/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:21.971950 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-25 18:53:21.000000 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-25 18:53:21.000000 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:53:21.000000 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 18:53:21.000000 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 18:53:21.000000 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 18:53:21.000000 dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi-cocoa-0.0.9/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.1.0/.github/workflows/main.workflow.yml`

 * *Files 13% similar despite different names*

```diff
@@ -27,41 +27,41 @@
         uses: pre-commit/action@v2.0.3
       - name: Install Dependencies
         run: |
           python -m pip install --upgrade pip
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Lint with pre-commit
         uses: pre-commit/action@v3.0.0
-      - name: Run Pytest
-        run: |
-          # coverage run on pytest. If pytest fails, workflow exits in failure
-          coverage run -m pytest --doctest-modules
-          coverage json
-          export TOTAL=$(python -c "import json;print(json.load(open('coverage.json'))['totals']['percent_covered_display'])")
-          echo "total=$TOTAL" >> $GITHUB_ENV
-          coverage report -m --format=markdown >> temp.md
-          # https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#multiline-strings
-          {
-            echo 'REPORT<<EOF'
-            cat temp.md
-            echo EOF
-          } >> "$GITHUB_ENV"
-          echo "report=$REPORT" >> $GITHUB_ENV
-      - name: Report Coverage
-        uses: actions/github-script@v7
-        env:
-          min_coverage: 50
-        with:
-          script: |
-            github.rest.issues.createComment({
-              issue_number: context.issue.number,
-              owner: context.repo.owner,
-              repo: context.repo.repo,
-              body: `${{ env.REPORT }}`
-            })
-            if ( ${{ env.total }} <= ${{ env.min_coverage }} ) { 
-              console.log(
-                "Coverage test failed as code coverage is ${{ env.total }}% and the minimum is ${{ env.min_coverage}}%"
-              )
-              process.exitCode = 1 
-            }
+      # - name: Run Pytest
+      #   run: |
+      #     # coverage run on pytest. If pytest fails, workflow exits in failure
+      #     coverage run -m pytest --doctest-modules
+      #     coverage json
+      #     export TOTAL=$(python -c "import json;print(json.load(open('coverage.json'))['totals']['percent_covered_display'])")
+      #     echo "total=$TOTAL" >> $GITHUB_ENV
+      #     coverage report -m --format=markdown >> temp.md
+      #     # https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#multiline-strings
+      #     {
+      #       echo 'REPORT<<EOF'
+      #       cat temp.md
+      #       echo EOF
+      #     } >> "$GITHUB_ENV"
+      #     echo "report=$REPORT" >> $GITHUB_ENV
+      # - name: Report Coverage
+      #   uses: actions/github-script@v7
+      #   env:
+      #     min_coverage: 50
+      #   with:
+      #     script: |
+      #       github.rest.issues.createComment({
+      #         issue_number: context.issue.number,
+      #         owner: context.repo.owner,
+      #         repo: context.repo.repo,
+      #         body: `${{ env.REPORT }}`
+      #       })
+      #       if ( ${{ env.total }} <= ${{ env.min_coverage }} ) { 
+      #         console.log(
+      #           "Coverage test failed as code coverage is ${{ env.total }}% and the minimum is ${{ env.min_coverage}}%"
+      #         )
+      #         process.exitCode = 1 
+      #       }
```

### Comparing `dsi-cocoa-0.0.9/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.1.0/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi-cocoa-0.0.9/.gitignore` & `dsi_cocoa-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi-cocoa-0.0.9/.pre-commit-config.yaml` & `dsi_cocoa-0.1.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 exclude: "(^docs/|(.*)tsv|(.*)csv)"
 default_stages: [commit]
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
         types: [python]
       - id: end-of-file-fixer
         types: [python]         
       - id: check-yaml
       - id: check-added-large-files
         args: ['--maxkb=25000']
 
   - repo: https://github.com/psf/black
-    rev: 23.11.0
+    rev: 24.4.0
     hooks:
       - id: black
         args: ["--line-length=80"]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         args: ["--settings-path=setup.cfg"]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
       - id: flake8
         args: ["--config=setup.cfg"]
         additional_dependencies: 
           - flake8-isort
           - flake8-bugbear~=23.11
```

### Comparing `dsi-cocoa-0.0.9/pyproject.toml` & `dsi_cocoa-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi-cocoa-0.0.9/src/cocoa/notebooks.py` & `dsi_cocoa-0.1.0/src/cocoa/notebooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities for evaluating the status and structure of Jupyter Notebooks
 """
+
 import json
 
 
 def count_functions(cell):
     """Count the number of functions defined in a Jupyter Notebook cell."""
     code = cell["source"]
     return len([1 for line in code if line.strip().startswith("def ")])
```

### Comparing `dsi-cocoa-0.0.9/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.1.0/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 requirements.txt
 setup.cfg
 .github/workflows/main.workflow.yml
 .github/workflows/publish.workflow.yml
 src/cocoa/__init__.py
 src/cocoa/constants.py
 src/cocoa/evaluate_repo.py
-src/cocoa/git.py
 src/cocoa/linting.py
 src/cocoa/notebooks.py
+src/cocoa/repo.py
+src/cocoa/spring2024.py
 src/dsi_cocoa.egg-info/PKG-INFO
 src/dsi_cocoa.egg-info/SOURCES.txt
 src/dsi_cocoa.egg-info/dependency_links.txt
 src/dsi_cocoa.egg-info/entry_points.txt
 src/dsi_cocoa.egg-info/requires.txt
 src/dsi_cocoa.egg-info/top_level.txt
```

